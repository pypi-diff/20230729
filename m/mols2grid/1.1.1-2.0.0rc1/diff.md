# Comparing `tmp/mols2grid-1.1.1.tar.gz` & `tmp/mols2grid-2.0.0rc1.tar.gz`

## Comparing `mols2grid-1.1.1.tar` & `mols2grid-2.0.0rc1.tar`

### file list

```diff
@@ -1,90 +1,93 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mols2grid-1.1.1/.npmignore
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mols2grid-1.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0    12470 2020-02-02 00:00:00.000000 mols2grid-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mols2grid-1.1.1/CITATION.cff
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 mols2grid-1.1.1/babel.config.js
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mols2grid-1.1.1/codecov.yml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mols2grid-1.1.1/environment.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mols2grid-1.1.1/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid.json
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mols2grid-1.1.1/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mols2grid-1.1.1/setup.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tsconfig.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 mols2grid-1.1.1/webpack.config.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mols2grid-1.1.1/css/widget.css
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/Makefile
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/conf.py
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/contents.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/environment.yml
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/make.bat
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/_static/custom.css
--rw-r--r--   0        0        0    84010 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/_static/demo.png
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/_static/mols2grid_logo.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/api/callbacks.rst
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/api/molgrid.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/api/simple.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/api/utils.rst
--rw-r--r--   0        0        0    10827 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/notebooks/callbacks.ipynb
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/notebooks/customization.ipynb
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/notebooks/filtering.ipynb
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 mols2grid-1.1.1/docs/notebooks/quickstart.ipynb
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/_version.py
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/callbacks.py
--rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/dispatch.py
--rw-r--r--   0        0        0    36580 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/molgrid.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/select.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/utils.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/labextension/package.json
--rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/labextension/static/480.b793e9ee0cf0bcedd405.js
--rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/labextension/static/568.dfe2d319c495ee9c8bd8.js
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/labextension/static/remoteEntry.a2b2bff7fec77dbdfc67.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/nbextension/extension.js
--rw-r--r--   0        0        0     8983 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/nbextension/index.js
--rw-r--r--   0        0        0    24408 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/__init__.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/pages.html
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/table.html
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/css/pages.css
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/css/table.css
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/html/checkbox_dropdown.html
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/html/common_header.html
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/html/iframe.html
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/html/pages_header.html
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/callback.js
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/draw_mol.js
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/filter.js
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/kernel.js
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/molstorage.js
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/pages.js
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/popup.js
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/search.js
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/selection_actions.js
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/sort.js
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/callbacks/external_link.js
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/templates/js/callbacks/show_3d.js
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/widget/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/widget/_frontend.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 mols2grid-1.1.1/mols2grid/widget/widget.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 mols2grid-1.1.1/src/extension.ts
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 mols2grid-1.1.1/src/index.ts
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 mols2grid-1.1.1/src/plugin.ts
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 mols2grid-1.1.1/src/version.ts
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 mols2grid-1.1.1/src/widget.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/pytest.ini
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/test_callbacks.py
--rw-r--r--   0        0        0    29542 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/test_interface.py
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/test_molgrid.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/test_select.py
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/test_utils.py
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 mols2grid-1.1.1/tests/webdriver_utils.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 mols2grid-1.1.1/.gitignore
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 mols2grid-1.1.1/LICENSE
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 mols2grid-1.1.1/README.md
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 mols2grid-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    16602 2020-02-02 00:00:00.000000 mols2grid-1.1.1/PKG-INFO
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

### Comparing `mols2grid-1.1.1/CHANGELOG.md` & `mols2grid-2.0.0rc1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,67 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 ---
 
+## [2.0.0] - ????/??/??
+
+This release is a major change on the UI contributed by @themoenen, refer to
+[PR#55](https://github.com/cbouy/mols2grid/pull/55) for the full list of changes:
+
+### Added
+- `background_color="white"` parameter added to `display` and `save` to control the background
+  color of each cell.
+- Property values displayed via subset or tooltip can now be copied by clicking them.
+
+### Changed
+- Responsiveness: the grid as well as all UI components are now fully responsive, up until around
+  ~415px wide. Smaller usage seems unlikely.
+- `n_items_per_page` replaces the `n_rows` and `n_cols` parameters. The responsive CSS assumes
+  results to be a multiple of 12, otherwise a gap is displayed at the end of the grid.
+- Hover tooltips: now displayed when hovering the *`i`* icon, and anchored by clicking this icon.
+- Save CVS: When exporting as CSV we now use a semicolon `;` as delineator instead of a tab, this
+  way CSVs are properly previewed on Mac.
+- Templates: the `pages`/`table` templates and corresponding functions have been renamed to
+  `interactive`/`static` for clarity.
+- Parameters `width` and `height` have been renamed to `iframe_width` and `iframe_height` to be more
+  descriptive.
+- Improved the sorting UI to be more intuitive.
+- You can now toggle between text/SMARTS search instead of having to click a dropdown.
+- The checkbox menu icon was replaced with a more standard triple dot menu.
+- The mols2grid-id is now permanently displayed next to the checkbox in the corner.
+- SVGs are now rendered with a transparent background.
+- The entire cell is now clickable, instead of just the tiny checkbox.
+- Implemented some basic keyboard navigation: ENTER / ESC for selecting / unselecting, arrows and
+  TAB for navigation.
+- Copy to clipboard: this will now record a tab delineated text which is ready to be pasted into a
+  spreadsheet, instead of the less useful dictionary format.
+- The `tooltip_trigger` parameter has been removed since callback and hover functionalities don't
+  overlap anymore.
+- We're now automatically adding `"img"` to the subset instead of throwing an error.
+- A smaller default font size (12px) makes the experience out of the box a bit more practical.
+
+### Fixed
+- Docstring now mention default values and some inconsistencies have been fixed.
+- All UI elements are now neatly aligned and displayed on top so they're accessible without
+  scrolling.
+- Longer property values are now only truncated in the interactive grid, and broken into multiple
+  lines by default in the static grid, as it is mostly meant for printing. A new parameter
+  `truncate` lets you override the default truncating behavior.
+- The tooltip display zone (around which the tooltip is displayed) is now the entire cell instead
+  of only the image, so it never overlaps with any of the cell's data or functionality.
+- When you download a CSV or SMILES file without any cells selected, you will now download data for
+  all cells instead of an empty document.
+- Parameter `gap` in static template didn't work.
+- We no longer resize the iframe if a custom `iframe_height` is set by the display function.
+
+---
+
 ## [1.1.1] - 2023/03/18
 
 ### Added
 - Support for `pathlib.Path` objects as input for `display`, `save`, `MolGrid.from_sdf`
   and `sdf_to_dataframe`.
 
 ### Changed
```

### Comparing `mols2grid-1.1.1/package.json` & `mols2grid-2.0.0rc1/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9670758928571429%*

 * *Differences: {"'devDependencies'": "{'eslint-config-prettier': '^8.8.0', 'eslint-plugin-prettier': '^4.2.1', "*

 * *                      "'prettier': '^2.8.8'}",*

 * * "'version'": "'2.0.0-rc1'"}*

```diff
@@ -19,22 +19,22 @@
         "@types/jest": "^26.0.0",
         "@types/webpack-env": "^1.13.6",
         "@typescript-eslint/eslint-plugin": "^3.6.0",
         "@typescript-eslint/parser": "^3.6.0",
         "acorn": "^7.2.0",
         "css-loader": "^3.2.0",
         "eslint": "^7.4.0",
-        "eslint-config-prettier": "^6.11.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^4.2.1",
         "fs-extra": "^7.0.0",
         "identity-obj-proxy": "^3.0.0",
         "jest": "^26.0.0",
         "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
-        "prettier": "^2.0.5",
+        "prettier": "^2.8.8",
         "rimraf": "^2.6.2",
         "source-map-loader": "^1.1.3",
         "style-loader": "^1.0.0",
         "ts-jest": "^26.0.0",
         "ts-loader": "^8.0.0",
         "typescript": "~4.1.3",
         "webpack": "^5.61.0",
@@ -86,9 +86,9 @@
         "prepack": "yarn run build:lib",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.1.1"
+    "version": "2.0.0-rc1"
 }
```

### Comparing `mols2grid-1.1.1/tsconfig.json` & `mols2grid-2.0.0rc1/tsconfig.json`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-00000000: 7b0a 2020 2263 6f6d 7069 6c65 724f 7074  {.  "compilerOpt
-00000010: 696f 6e73 223a 207b 0a20 2020 2022 6465  ions": {.    "de
-00000020: 636c 6172 6174 696f 6e22 3a20 7472 7565  claration": true
-00000030: 2c0a 2020 2020 2265 734d 6f64 756c 6549  ,.    "esModuleI
-00000040: 6e74 6572 6f70 223a 7472 7565 2c0a 2020  nterop":true,.  
-00000050: 2020 226c 6962 223a 205b 2265 7332 3031    "lib": ["es201
-00000060: 3622 2c20 2264 6f6d 225d 2c0a 2020 2020  6", "dom"],.    
-00000070: 226d 6f64 756c 6522 3a20 2263 6f6d 6d6f  "module": "commo
-00000080: 6e6a 7322 2c0a 2020 2020 226d 6f64 756c  njs",.    "modul
-00000090: 6552 6573 6f6c 7574 696f 6e22 3a20 226e  eResolution": "n
-000000a0: 6f64 6522 2c0a 2020 2020 226e 6f45 6d69  ode",.    "noEmi
-000000b0: 744f 6e45 7272 6f72 223a 2074 7275 652c  tOnError": true,
-000000c0: 0a20 2020 2022 6e6f 556e 7573 6564 4c6f  .    "noUnusedLo
-000000d0: 6361 6c73 223a 2074 7275 652c 0a20 2020  cals": true,.   
-000000e0: 2022 6f75 7444 6972 223a 2022 6c69 6222   "outDir": "lib"
-000000f0: 2c0a 2020 2020 2272 6573 6f6c 7665 4a73  ,.    "resolveJs
-00000100: 6f6e 4d6f 6475 6c65 223a 2074 7275 652c  onModule": true,
-00000110: 0a20 2020 2022 726f 6f74 4469 7222 3a20  .    "rootDir": 
-00000120: 2273 7263 222c 0a20 2020 2022 736b 6970  "src",.    "skip
-00000130: 4c69 6243 6865 636b 223a 2074 7275 652c  LibCheck": true,
-00000140: 0a20 2020 2022 736f 7572 6365 4d61 7022  .    "sourceMap"
-00000150: 3a20 7472 7565 2c0a 2020 2020 2273 7472  : true,.    "str
-00000160: 6963 7422 3a20 7472 7565 2c0a 2020 2020  ict": true,.    
-00000170: 2273 7472 6963 7450 726f 7065 7274 7949  "strictPropertyI
-00000180: 6e69 7469 616c 697a 6174 696f 6e22 3a20  nitialization": 
-00000190: 6661 6c73 652c 0a20 2020 2022 7461 7267  false,.    "targ
-000001a0: 6574 223a 2022 6573 3230 3136 222c 0a20  et": "es2016",. 
-000001b0: 2020 2022 7479 7065 7322 3a20 5b5d 0a20     "types": []. 
-000001c0: 207d 2c0a 2020 2269 6e63 6c75 6465 223a   },.  "include":
-000001d0: 205b 0a20 2020 2022 7372 632f 2a2a 2f2a   [.    "src/**/*
-000001e0: 2e74 7322 2c0a 2020 2020 2273 7263 2f2a  .ts",.    "src/*
-000001f0: 2a2f 2a2e 7473 7822 2c0a 2020 5d0a 7d0a  */*.tsx",.  ].}.
+00000000: 7b0a 2020 2020 2263 6f6d 7069 6c65 724f  {.    "compilerO
+00000010: 7074 696f 6e73 223a 207b 0a20 2020 2020  ptions": {.     
+00000020: 2020 2022 6465 636c 6172 6174 696f 6e22     "declaration"
+00000030: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
+00000040: 2265 734d 6f64 756c 6549 6e74 6572 6f70  "esModuleInterop
+00000050: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00000060: 2022 6c69 6222 3a20 5b22 6573 3230 3136   "lib": ["es2016
+00000070: 222c 2022 646f 6d22 5d2c 0a20 2020 2020  ", "dom"],.     
+00000080: 2020 2022 6d6f 6475 6c65 223a 2022 636f     "module": "co
+00000090: 6d6d 6f6e 6a73 222c 0a20 2020 2020 2020  mmonjs",.       
+000000a0: 2022 6d6f 6475 6c65 5265 736f 6c75 7469   "moduleResoluti
+000000b0: 6f6e 223a 2022 6e6f 6465 222c 0a20 2020  on": "node",.   
+000000c0: 2020 2020 2022 6e6f 456d 6974 4f6e 4572       "noEmitOnEr
+000000d0: 726f 7222 3a20 7472 7565 2c0a 2020 2020  ror": true,.    
+000000e0: 2020 2020 226e 6f55 6e75 7365 644c 6f63      "noUnusedLoc
+000000f0: 616c 7322 3a20 7472 7565 2c0a 2020 2020  als": true,.    
+00000100: 2020 2020 226f 7574 4469 7222 3a20 226c      "outDir": "l
+00000110: 6962 222c 0a20 2020 2020 2020 2022 7265  ib",.        "re
+00000120: 736f 6c76 654a 736f 6e4d 6f64 756c 6522  solveJsonModule"
+00000130: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
+00000140: 2272 6f6f 7444 6972 223a 2022 7372 6322  "rootDir": "src"
+00000150: 2c0a 2020 2020 2020 2020 2273 6b69 704c  ,.        "skipL
+00000160: 6962 4368 6563 6b22 3a20 7472 7565 2c0a  ibCheck": true,.
+00000170: 2020 2020 2020 2020 2273 6f75 7263 654d          "sourceM
+00000180: 6170 223a 2074 7275 652c 0a20 2020 2020  ap": true,.     
+00000190: 2020 2022 7374 7269 6374 223a 2074 7275     "strict": tru
+000001a0: 652c 0a20 2020 2020 2020 2022 7374 7269  e,.        "stri
+000001b0: 6374 5072 6f70 6572 7479 496e 6974 6961  ctPropertyInitia
+000001c0: 6c69 7a61 7469 6f6e 223a 2066 616c 7365  lization": false
+000001d0: 2c0a 2020 2020 2020 2020 2274 6172 6765  ,.        "targe
+000001e0: 7422 3a20 2265 7332 3031 3622 2c0a 2020  t": "es2016",.  
+000001f0: 2020 2020 2020 2274 7970 6573 223a 205b        "types": [
+00000200: 5d0a 2020 2020 7d2c 0a20 2020 2022 696e  ].    },.    "in
+00000210: 636c 7564 6522 3a20 5b22 7372 632f 2a2a  clude": ["src/**
+00000220: 2f2a 2e74 7322 2c20 2273 7263 2f2a 2a2f  /*.ts", "src/**/
+00000230: 2a2e 7473 7822 5d0a 7d0a                 *.tsx"].}.
```

### Comparing `mols2grid-1.1.1/webpack.config.js` & `mols2grid-2.0.0rc1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/docs/Makefile` & `mols2grid-2.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/docs/conf.py` & `mols2grid-2.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/docs/contents.md` & `mols2grid-2.0.0rc1/docs/contents.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 * [Viewing clustered chemical structures](https://practicalcheminformatics.blogspot.com/2021/07/viewing-clustered-chemical-structures.html) and [Exploratory data analysis](https://practicalcheminformatics.blogspot.com/2021/10/exploratory-data-analysis-with.html) by Pat Walters
 * [Advanced notebook (RDKit UGM 2021)](https://colab.research.google.com/github/rdkit/UGM_2021/blob/main/Notebooks/Bouysset_mols2grid.ipynb)
 
 Feel free to open a pull request if you'd like your snippets to be added to this list!
 
 # 👏 Acknowledgments
 ---
+* [@themoenen](https://github.com/themoenen) (contributor)
 * [@fredrikw](https://github.com/fredrikw) (contributor)
 * [@JustinChavez](https://github.com/JustinChavez) (contributor)
 * [@hadim](https://github.com/hadim) (conda feedstock maintainer)
 
 # 🎓 Citing
 ---
 You can refer to mols2grid in your research by using the following DOI:
```

#### html2text {}

```diff
@@ -58,23 +58,24 @@
 watch?v=0rqIwSeUImo) by Data Professor * [Viewing clustered chemical
 structures](https://practicalcheminformatics.blogspot.com/2021/07/viewing-
 clustered-chemical-structures.html) and [Exploratory data analysis](https://
 practicalcheminformatics.blogspot.com/2021/10/exploratory-data-analysis-
 with.html) by Pat Walters * [Advanced notebook (RDKit UGM 2021)](https://
 colab.research.google.com/github/rdkit/UGM_2021/blob/main/Notebooks/
 Bouysset_mols2grid.ipynb) Feel free to open a pull request if you'd like your
-snippets to be added to this list! # ð Acknowledgments --- * [@fredrikw]
-(https://github.com/fredrikw) (contributor) * [@JustinChavez](https://
-github.com/JustinChavez) (contributor) * [@hadim](https://github.com/hadim)
-(conda feedstock maintainer) # ð Citing --- You can refer to mols2grid in
-your research by using the following DOI: [![DOI:10.5281/zenodo.6591473](https:
-//zenodo.org/badge/348814588.svg)](https://zenodo.org/badge/latestdoi/
-348814588) # â License --- Unless otherwise noted, all files in this
-directory and all subdirectories are distributed under the Apache License,
-Version 2.0: ```text Copyright 2021-2022 CÃ©dric BOUYSSET Licensed under the
-Apache License, Version 2.0 (the "License"); you may not use this file except
-in compliance with the License. You may obtain a copy of the License at http://
-www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
-to in writing, software distributed under the License is distributed on an "AS
-IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-implied. See the License for the specific language governing permissions and
-limitations under the License. ```
+snippets to be added to this list! # ð Acknowledgments --- * [@themoenen]
+(https://github.com/themoenen) (contributor) * [@fredrikw](https://github.com/
+fredrikw) (contributor) * [@JustinChavez](https://github.com/JustinChavez)
+(contributor) * [@hadim](https://github.com/hadim) (conda feedstock maintainer)
+# ð Citing --- You can refer to mols2grid in your research by using the
+following DOI: [![DOI:10.5281/zenodo.6591473](https://zenodo.org/badge/
+348814588.svg)](https://zenodo.org/badge/latestdoi/348814588) # â License --
+- Unless otherwise noted, all files in this directory and all subdirectories
+are distributed under the Apache License, Version 2.0: ```text Copyright 2021-
+2022 CÃ©dric BOUYSSET Licensed under the Apache License, Version 2.0 (the
+"License"); you may not use this file except in compliance with the License.
+You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-
+2.0 Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+License for the specific language governing permissions and limitations under
+the License. ```
```

### Comparing `mols2grid-1.1.1/docs/index.rst` & `mols2grid-2.0.0rc1/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 .. toctree::
    :maxdepth: 2
    :caption: API Reference
 
    api/simple
    api/molgrid
+   api/callbacks
    api/utils
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `mols2grid-1.1.1/docs/make.bat` & `mols2grid-2.0.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/docs/_static/mols2grid_logo.png` & `mols2grid-2.0.0rc1/docs/_static/mols2grid_logo.png`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/docs/notebooks/callbacks.ipynb` & `mols2grid-2.0.0rc1/docs/notebooks/callbacks.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992137419871795%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(4, "Callbacks are **functions that are executed when you '*

 * *            "click on a cell's callback button**. They can be written in *JavaScript* or "*

 * *            '*Python*.\\n")], delete: [4]}}, 10: {\'source\': {insert: [(2, \'    '*

 * *            'subtitle="${data[\\\'SMILES\\\']}",\\n\'), (3, \'    svg="${svg}",\\n\'), (12, '*

 * *            "'        <b>Molecular weight</b>: ${desc.exactmw}<br/>\\n'), (13, '        <b>HBond "*

 * *            "Acceptors</b>: ${desc.NumHBA}<b […]*

```diff
@@ -4,15 +4,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Callbacks\n",
                 "\n",
                 "[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cbouy/mols2grid/blob/master/docs/notebooks/callbacks.ipynb)\n",
                 "\n",
-                "Callbacks are **functions that are executed when you click on a molecule's image**. They can be written in *JavaScript* or *Python*.\n",
+                "Callbacks are **functions that are executed when you click on a cell's callback button**. They can be written in *JavaScript* or *Python*.\n",
                 "\n",
                 "This functionality can be used to display some additional information on the molecule or run some more complex code such as database queries, docking or machine-learning predictions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -201,34 +201,33 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "js_callback = mols2grid.make_popup_callback(\n",
                 "    title=\"${data['NAME']}\",\n",
+                "    subtitle=\"${data['SMILES']}\",\n",
+                "    svg=\"${svg}\",\n",
                 "    js=\"\"\"\n",
                 "        var mol = RDKit.get_mol(data[\"SMILES\"]);\n",
                 "        var svg = mol.get_svg(400, 300);\n",
                 "        var desc = JSON.parse(mol.get_descriptors());\n",
                 "        var inchikey = RDKit.get_inchikey_for_inchi(mol.get_inchi());\n",
                 "        mol.delete();\n",
                 "    \"\"\",\n",
                 "    html=\"\"\"\n",
-                "        <div class=\"row\">\n",
-                "          <div class=\"col\">${svg}</div>\n",
-                "          <div class=\"col\">\n",
-                "            <b>Molecular weight</b>: ${desc.amw}<br/>\n",
-                "            <b>HBond Acceptors</b>: ${desc.NumHBA}<br/>\n",
-                "            <b>HBond Donors</b>: ${desc.NumHBD}<br/>\n",
-                "            <b>ClogP</b>: ${desc.CrippenClogP}<br/>\n",
-                "            <br/>\n",
-                "            <b>InChIKey</b>: ${inchikey}\n",
-                "          </div>\n",
-                "        </div>\"\"\",\n",
-                "    style=\"max-width: 80%;\",\n",
+                "        <b>Molecular weight</b>: ${desc.exactmw}<br/>\n",
+                "        <b>HBond Acceptors</b>: ${desc.NumHBA}<br/>\n",
+                "        <b>HBond Donors</b>: ${desc.NumHBD}<br/>\n",
+                "        <b>TPSA</b>: ${desc.tpsa}<br/>\n",
+                "        <b>ClogP</b>: ${desc.CrippenClogP}<br/>\n",
+                "        <hr>\n",
+                "        <b>InChIKey</b>: ${inchikey}\n",
+                "    \"\"\",\n",
+                "    style=\"border-radius: 10px\",\n",
                 ")\n",
                 "\n",
                 "mols2grid.display(\n",
                 "    df,\n",
                 "    callback=js_callback,\n",
                 ")"
             ]
```

### Comparing `mols2grid-1.1.1/docs/notebooks/customization.ipynb` & `mols2grid-2.0.0rc1/docs/notebooks/customization.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9512167366946779%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 3: {'attachments': OrderedDict()}, 5: "*

 * *            '{\'attachments\': OrderedDict()}, 6: {\'source\': {insert: [(1, "# use .m2g-cell to '*

 * *            'select each grid\'s cell\\n"), (6, \'.m2g-cell {\\n\'), (12, \'.m2g-cell:hover '*

 * *            "{\\n'), (49, '    size=(130, 80),\\n'), (50, '    # number of results per page\\n'), "*

 * *            "(51, '    n_items_per_page=20,\\n'), (55, '    gap=3,\\n')], delete: [57, 53, 52, 51, "*

 * *            '50, 39, 12, 6, 1 […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Customization\n",
                 "\n",
                 "[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cbouy/mols2grid/blob/master/docs/notebooks/customization.ipynb)\n",
                 "\n",
@@ -39,14 +40,15 @@
                 "    f\"{RDConfig.RDDocsDir}/Book/data/solubility.test.sdf\"\n",
                 "    if Path(RDConfig.RDDocsDir).is_dir()\n",
                 "    else \"solubility.test.sdf\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To display all the arguments available, type `help(mols2grid.display)`"
             ]
         },
         {
@@ -75,14 +77,15 @@
                 "    # molecule drawing parameters\n",
                 "    fixedBondLength=25,\n",
                 "    clearBackground=False,\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "See [rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions](https://www.rdkit.org/docs/source/rdkit.Chem.Draw.rdMolDraw2D.html#rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions) for the molecule drawing options available.\n",
                 "\n",
                 "The grid's look can also be customized to an even greater extent:"
             ]
@@ -90,26 +93,26 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# some unnecessarily complicated CSS stylesheet \ud83c\udf08\n",
-                "# use .cell to select each grid's cell\n",
+                "# use .m2g-cell to select each grid's cell\n",
                 "# or .data for every data field\n",
                 "# or .data-<field> for a specific field\n",
                 "css_style = \"\"\"\n",
                 "/* rainbow background */\n",
-                ".cell {\n",
+                ".m2g-cell {\n",
                 "    background: linear-gradient(124deg, #ff2400, #e81d1d, #e8b71d, #e3e81d, #1de840, #1ddde8, #2b1de8, #dd00f3, #dd00f3);\n",
                 "    background-size: 500% 500%;\n",
                 "    -webkit-animation: rainbow 10s ease infinite;\n",
                 "    animation: rainbow 10s ease infinite;\n",
                 "}\n",
-                ".cell:hover {\n",
+                ".m2g-cell:hover {\n",
                 "    border-color: red !important;\n",
                 "}\n",
                 "/* rainbow font color */\n",
                 ".data {\n",
                 "    font-weight: bold;\n",
                 "    -webkit-text-stroke: 1px black;\n",
                 "    background: linear-gradient(to right, #ef5350, #f48fb1, #7e57c2, #2196f3, #26c6da, #43a047, #eeff41, #f9a825, #ff5722);\n",
@@ -128,58 +131,55 @@
                 "    100% {background-position: 0% 50%}\n",
                 "}\n",
                 "\"\"\"\n",
                 "\n",
                 "mols2grid.display(\n",
                 "    SDF_FILE,\n",
                 "    # RDKit drawing options\n",
-                "    clearBackground=False,\n",
                 "    comicMode=True,\n",
                 "    fixedBondLength=20,\n",
                 "    bondLineWidth=1,\n",
                 "    # custom atom colour palette (all white)\n",
                 "    atomColourPalette={z: (1, 1, 1) for z in range(1, 295)},\n",
                 "    # mols2grid options\n",
                 "    subset=[\"NAME\", \"img\"],\n",
                 "    custom_css=css_style,\n",
                 "    fontfamily='\"Comic Sans MS\", \"Comic Sans\", cursive;',\n",
                 "    # image size\n",
-                "    size=(120, 90),\n",
-                "    # number of rows and columns per page\n",
-                "    n_cols=6,\n",
-                "    n_rows=3,\n",
+                "    size=(130, 80),\n",
+                "    # number of results per page\n",
+                "    n_items_per_page=20,\n",
                 "    # border around each cell\n",
                 "    border=\"5px ridge cyan\",\n",
                 "    # gap between cells\n",
-                "    gap=1,\n",
+                "    gap=3,\n",
                 "    # disable selection\n",
                 "    selection=False,\n",
                 ")"
             ]
         }
     ],
     "metadata": {
         "interpreter": {
             "hash": "634da3a3bbf8fbf1ddb65b0056d578c92f3c569db0da492ea274ae9d304e5b24"
         },
         "kernelspec": {
-            "display_name": "Python 3.8.6 ('molgrid')",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.12"
-        },
-        "orig_nbformat": 4
+            "version": "3.9.13"
+        }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `mols2grid-1.1.1/docs/notebooks/filtering.ipynb` & `mols2grid-2.0.0rc1/docs/notebooks/filtering.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998397435897436%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(5, 'view = grid.display(n_items_per_page=12)\\n')], delete: "*

 * *            '[5]}}}'}*

```diff
@@ -74,15 +74,15 @@
             "outputs": [],
             "source": [
                 "grid = mols2grid.MolGrid(\n",
                 "    df,\n",
                 "    size=(120, 100),\n",
                 "    name=\"filters\",\n",
                 ")\n",
-                "view = grid.display(n_rows=2)\n",
+                "view = grid.display(n_items_per_page=12)\n",
                 "\n",
                 "\n",
                 "@interact(\n",
                 "    MolWt=widgets.IntRangeSlider(value=[0, 600], min=0, max=600, step=10),\n",
                 "    LogP=widgets.IntRangeSlider(value=[-10, 10], min=-10, max=10, step=1),\n",
                 "    NumHDonors=widgets.IntRangeSlider(value=[0, 20], min=0, max=20, step=1),\n",
                 "    NumHAcceptors=widgets.IntRangeSlider(value=[0, 20], min=0, max=20, step=1),\n",
```

### Comparing `mols2grid-1.1.1/docs/notebooks/quickstart.ipynb` & `mols2grid-2.0.0rc1/docs/notebooks/quickstart.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977988591269842%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(2, '- Make simple text searches using the searchbar on the "*

 * *            "top right.\\n'), (3, '- Make substructure queries by clicking on `SMARTS` instead of "*

 * *            "`Text` and typing in the searchbar.\\n'), (4, '- Sort molecules by clicking on `Sort` "*

 * *            'and selecting a field (click the arrows on the right side of the `Sort` dropdown to '*

 * *            "reverse the order).\\n'), (5, '- View metadata by hovering your mouse over the *`i`* "*

 * *             […]*

```diff
@@ -60,18 +60,20 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "From this interface, you can:\n",
                 "\n",
-                "- Make simple text searches using the searchbar on the bottom right\n",
-                "- Make substructure queries by clicking on \ud83d\udd0e > SMARTS and typing in the searchbar\n",
-                "- Sort molecules by clicking on `Sort by` and selecting a field (click again to reverse the order)\n",
-                "- Select a couple of molecules (click on the checkbox) and then export the selection to a SMILES or CSV file, or directly to the clipboard (this last functionality might be blocked depending on how you are running the notebook)"
+                "- Make simple text searches using the searchbar on the top right.\n",
+                "- Make substructure queries by clicking on `SMARTS` instead of `Text` and typing in the searchbar.\n",
+                "- Sort molecules by clicking on `Sort` and selecting a field (click the arrows on the right side of the `Sort` dropdown to reverse the order).\n",
+                "- View metadata by hovering your mouse over the *`i`* button of a cell, you can also press that button to anchor the information.\n",
+                "- Select a couple of molecules (click on a cell or on a checkbox, or navigate using your keyboard arrows and press the `ENTER` key).\n",
+                "- Export the selection to a SMILES or CSV file, or directly to the clipboard (this last functionality might be blocked depending on how you are running the notebook). If no selection was made, the entire grid is exported."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can also use a pandas DataFrame as input, containing a column of RDKit molecules (specified using `mol_col=...`) or SMILES strings (specified using `smiles_col=...`):"
@@ -169,14 +171,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.12"
+            "version": "3.8.17"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `mols2grid-1.1.1/mols2grid/callbacks.py` & `mols2grid-2.0.0rc1/mols2grid/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,26 @@
     the optional ``library_src`` as a ``<script>`` tag.
     """
 
     code: str
     library_src: Optional[str] = None
 
 
-def make_popup_callback(title, html, js="", style=""):
+def make_popup_callback(title=None, subtitle=None, svg=None, html="", js="", style=""):
     """Creates a JavaScript callback that displays a popup window
 
     Parameters
     ----------
     title : str
         Title of the popup. Use ``title='${data["Name"]}'`` to use the value
         of the column "Name" as a title
+    subtitle : str
+        Secondary title which works the same as title.
+    svg : str
+        SVG depiction of the molecule
     html : str
         Content of the popup window
     js : str
         JavaScript code executed before making the content of the popup window.
         This allows you to create variables and reuse them later in the `html`
         content of the popup, using the ``${my_variable}`` syntax
     style : str
@@ -32,75 +36,81 @@
 
     Returns
     -------
     js_callback : str
         JavaScript code that allows to display a popup window
     """
     return env.get_template("js/popup.js").render(
-        js=js, html=html, title=title, style=style
+        title=title, subtitle=subtitle, html=html, svg=svg, js=js, style=style
     )
 
 
 def _get_title_field(title):
     return "${data['" + title + "']}" if title else None
 
 
-def info(title="SMILES", img_size=(400, 300), style="max-width: 80%;") -> _JSCallback:
+def info(title="SMILES", subtitle=None, img_size=(400, 300), style="") -> _JSCallback:
     """Displays a bigger image of the molecule, alongside some useful descriptors:
     molecular weight, number of Hydrogen bond donors and acceptors, TPSA, Crippen ClogP
     and InChIKey.
 
     Parameters
     ----------
-    title : str or None
-        Data field used to set the title of the modal window. If ``None``, no title is
-        displayed.
+    title : str
+        Title of the popup. Use ``title='${data["Name"]}'`` to use the value
+        of the column "Name" as a title
+    subtitle : str
+        Secondary title which works the same as title.
     img_size : tuple
         Width and height of the molecule depiction.
     style : str
         CSS style applied to the modal window.
     """
     code = make_popup_callback(
         title=_get_title_field(title),
+        subtitle=_get_title_field(subtitle),
+        svg="${svg}",
         js=f"""
             let mol = RDKit.get_mol(data["SMILES"]);
             let svg = mol.get_svg({img_size[0]}, {img_size[1]});
             let desc = JSON.parse(mol.get_descriptors());
             let inchikey = RDKit.get_inchikey_for_inchi(mol.get_inchi());
             mol.delete();
         """,
         html="""
-            <div class="row">
-            <div class="col">${svg}</div>
-            <div class="col">
-                <b>Molecular weight</b>: ${desc.exactmw}<br/>
-                <b>HBond Acceptors</b>: ${desc.NumHBA}<br/>
-                <b>HBond Donors</b>: ${desc.NumHBD}<br/>
-                <b>TPSA</b>: ${desc.tpsa}<br/>
-                <b>ClogP</b>: ${desc.CrippenClogP}<br/>
-                <br/>
-                <b>InChIKey</b>: ${inchikey}
-            </div>
-            </div>""",
+            <b>Molecular weight</b>: ${desc.exactmw}<br/>
+            <b>HBond Acceptors</b>: ${desc.NumHBA}<br/>
+            <b>HBond Donors</b>: ${desc.NumHBD}<br/>
+            <b>TPSA</b>: ${desc.tpsa}<br/>
+            <b>ClogP</b>: ${desc.CrippenClogP}<br/>
+            <hr>
+            <b>InChIKey</b>: ${inchikey}
+            """,
         style=style,
     )
     return _JSCallback(code=code)
 
 
 def show_3d(
-    title="SMILES", query=["pubchem", "cactus"], height="350px", style="max-width: 80%"
+    title="SMILES",
+    subtitle=None,
+    query=["pubchem", "cactus"],
+    height="100%",
+    style="width:100%;height:100%",
 ) -> _JSCallback:
     """Queries the API(s) listed in ``query`` using the SMILES of the structure, to
     fetch the 3D structure and display it with ``3Dmol.js``
 
     Parameters
     ----------
-    title : str or None
-        Data field used to set the title of the modal window. If ``None``, no title is
-        displayed.
+    title : str
+        Title of the popup. Use ``title='${data["Name"]}'`` to use the value
+        of the column "Name" as a title
+    subtitle : str
+        Secondary title which works the same as title.
     query : list or dict
         List of APIs used to fetch the 3D structure from (by order of priority). To use
         a custom API, use a dict with the following format::
 
             {
                 "url": "https://pubchem.ncbi.nlm.nih.gov/rest/pug/compound/smiles/{}/SDF?record_type=3d",
                 "format": "sdf",
@@ -115,16 +125,17 @@
         Height of the 3Dmol.js viewer in the modal.
     style : str
         CSS style applied to the modal window.
     """
     js_script = env.get_template("js/callbacks/show_3d.js").render(query=query)
     code = make_popup_callback(
         title=_get_title_field(title),
-        js=js_script,
+        subtitle=_get_title_field(subtitle),
         html=f'<div id="molviewer" style="width: 100%; height: {height};"></div>',
+        js=js_script,
         style=style,
     )
     library = """<script src="https://cdnjs.cloudflare.com/ajax/libs/3Dmol/1.8.0/3Dmol-nojquery-min.js" integrity="sha512-9iiTgstim185ZZPL/nZ+t+MLMmIbZEMfoZ1swSBUhxt4AukOPY34yyO2217X1dN5ziVMKi+YLmp/JBj+KyEaUQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>"""
     return _JSCallback(code=code, library_src=library)
 
 
 def external_link(
```

### Comparing `mols2grid-1.1.1/mols2grid/dispatch.py` & `mols2grid-2.0.0rc1/mols2grid/dispatch.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from pandas import DataFrame, Series
 
 from .molgrid import MolGrid
 
 _SIGNATURE = {
     method: dict(inspect.signature(getattr(MolGrid, method)).parameters.items())
-    for method in ["render", "to_pages", "to_table", "display"]
+    for method in ["render", "to_interactive", "to_static", "display"]
 }
-for method in ["render", "to_pages", "to_table", "display"]:
+for method in ["render", "to_interactive", "to_static", "display"]:
     _SIGNATURE[method].pop("self")
     if method in ["render", "display"]:
         _SIGNATURE[method].pop("kwargs")
 
 
 def _prepare_kwargs(kwargs, kind):
     """Separate kwargs for the init and render methods of MolGrid"""
@@ -31,89 +31,146 @@
             }
         )
     return template, kwargs, render_kwargs
 
 
 @singledispatch
 def display(arg, **kwargs):
-    """Display molecules on an interactive grid
+    """Display molecules on an interactive grid.
 
-    Parameters
-    ----------
+    Parameters: Data
+    ----------------
     arg : pandas.DataFrame, SDF file or list of molecules
-        The input containing your molecules
+        The input containing your molecules.
     smiles_col : str or None, default="SMILES"
-        If a pandas DataFrame is used, name of the column with SMILES
+        If a pandas dataframe is used, name of the column with SMILES.
     mol_col : str or None, default=None
-        If a pandas DataFrame is used, name of the column with RDKit molecules
+        If a pandas dataframe is used, name of the column with RDKit molecules.
+        If available, coordinates and atom/bonds annotations from this will be
+        used for depiction.
+
+    Parameters: Display
+    -------------------
+    template : str, default="interactive"
+        Either ``"interactive"`` or ``"static"``. See ``render()`` for more details.
+    size : tuple, default=(130, 90)
+        The size of the drawing canvas. The cell minimum width is set to the
+        width of the image, so if the cell padding is increased, the image will
+        be displayed smaller.
     useSVG : bool, default=True
-        Use SVG images or PNG
-    coordGen : bool, default=True
-        Use the coordGen library instead of the RDKit one to depict the
-        molecules in 2D
-    use_coords : bool, default=False
-        Use the coordinates of the molecules (only relevant when an SDF file, a
-        list of molecules or a DataFrame of RDKit molecules were used as input)
-    removeHs : bool, default=False
-        Remove hydrogen atoms from the drawings
-    size : tuple, default=(160, 120)
-        Size of each image
+        Use SVG images instead of PNG.
     prerender : bool, default=False
-        Prerender images for the entire dataset, or generate them on-the-fly
-        when needed
-    substruct_highlight : bool, default=None
-        Highlight substructure when using the SMARTS search. Active by default
-        when ``prerender=False``.
-    single_highlight : bool, default=False
-        Highlight only the first match of the substructure query
-    MolDrawOptions : rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions or None, default=None
-        Drawing options. Useful for making highly customized drawings
-    rename : dict or None, default=None
-        Rename the properties in the final document
-    name : str, default="default"
-        Name of the grid. Used when retrieving selections from multiple grids
-        at the same time
-    template : str, default="pages"
-        Either ``"pages"`` or ``"table"``
-    width : str, default="100%
-        Width of the frame displayed in the notebook
-    height : int or None, default=None
-        Height of the frame displayed in the notebook. Use ``None`` for an
-        automatic guess
+        Prerender images for the entire dataset, or generate them on-the-fly.
+        Prerendering is slow and memory-hungry, but required when ``template="static"``
+        or ``useSVG=False``.
     subset: list or None, default=None
-        Columns to be displayed in each cell of the grid. Each column's value
-        will be displayed from top to bottom in the same order given here.
-        Use ``"img"`` for the image of the molecule, and ``"mols2grid-id"`` for
-        the molecule's index in your input file.
+        Columns to be displayed in each cell of the grid. Each column's
+        value will be displayed from top to bottom in the order provided.
+        The ``"img"`` and ``"mols2grid-id"`` columns are displayed by default,
+        however you can still add the ``"img"`` column if you wish to change
+        the display order.
     tooltip : list, None or False, default=None
-        Columns to be displayed as a tooltip when hovering/clicking on the
-        image of a cell. Use ``False`` for no tooltip.
+        Columns to be displayed inside the tooltip. When no subset is set,
+        all columns will be listed in the tooltip by default. Use ``False``
+        to hide the tooltip.
     tooltip_fmt : str, default="<strong>{key}</strong>: {value}"
-        Format string of each key/value pair in the tooltip
-    tooltip_trigger : str, default="click hover"
+        Format string of each key/value pair in the tooltip.
+    tooltip_trigger : str, default="focus"
+        Only available for the "static" template.
         Sequence of triggers for the tooltip: ``click``, ``hover`` or ``focus``
     tooltip_placement : str, default="auto"
         Position of the tooltip: ``auto``, ``top``, ``bottom``, ``left`` or
         ``right``
+    transform : dict or None, default=None
+        Functions applied to specific items in all cells. The dict must follow
+        a ``key: function`` structure where the key must correspond to one of
+        the columns in ``subset`` or ``tooltip``. The function takes the item's
+        value as input and transforms it, for example::
+
+            transform={
+                "Solubility": lambda x: f"{x:.2f}",
+                "Melting point": lambda x: f"MP: {5/9*(x-32):.1f}°C"
+            }
+
+        These transformations only affect columns in ``subset`` and
+        ``tooltip``, and do not interfere with ``style``.
+    sort_by : str or None, default=None
+        Sort the grid according to the following field (which must be
+        present in ``subset`` or ``tooltip``).
+    truncate: bool, default=True/False
+        Whether to truncate the text in each cell if it's too long.
+        Defaults to ``True`` for interactive grids, ``False`` for static grid.
+    n_items_per_page, default=24
+        Only available for the "interactive" template.
+        Number of items to display per page. A multiple of 12 is recommended
+        for optimal display.
     n_cols : int, default=5
-        Number of columns per page
-    n_rows` : int, default=3
-        Only available for the "pages" template. Number of rows per page
+        Only available for the "static" template.
+        Number of columns in the table.
+    selection : bool, default=True
+        Only available for the "interactive" template.
+        Enables the selection of molecules and displays a checkbox at the
+        top of each cell. In the context of a Jupyter Notebook, this gives
+        you access to your selection (index and SMILES) through
+        :func:`mols2grid.get_selection()` or :meth:`MolGrid.get_selection()`.
+        In all cases, you can export your selection by clicking on the triple-dot menu.
+    cache_selection : bool, default=False
+        Only available for the "interactive" template.
+        Restores the selection from a previous grid with the same name.
+    use_iframe : bool, default=False
+        Whether to use an iframe to display the grid. When the grid is displayed
+        inside a Jupyter Notebook or JupyterLab, this will default to ``True``.
+    iframe_width : str, default="100%
+        Width of the iframe
+    iframe_height : int or None, default=None
+        Height of the frame. When set to ``None``, the height is set dynamically
+        based on the content.
+
+    Parameters: Mols
+    ----------------
+    removeHs : bool, default=False
+        Remove hydrogen atoms from the drawings.
+    use_coords : bool, default=False
+        Use the coordinates of the molecules (only relevant when an SDF file, a
+        list of molecules or a DataFrame of RDKit molecules were used as input.)
+    coordGen : bool, default=True
+        Use the CoordGen library instead of the RDKit one to depict the
+        molecules in 2D.
+    MolDrawOptions : rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions or None, default=None
+        Drawing options. Useful for making highly customized drawings.
+    substruct_highlight : bool or None, default=None
+        Highlight substructure when using the SMARTS search. Active by default
+        when ``prerender=False``.
+    single_highlight : bool, default=False
+        Highlight only the first match of the substructure query.
+
+    Parameters: CSS
+    ---------------
     border : str, default="1px solid #cccccc"
-        Styling of the border around each cell (CSS)
+        Styling of the border around each cell.
     gap : int, default=0
-        Size of the margin around each cell in px
-    fontsize : str, default="12pt"
-        Font size of the text displayed in each cell (CSS)
+        Size in pixels of the gap between cells.
+    pad : int, default=10
+        Size in pixels of the cell padding.
+    fontsize : str, default="12px"
+        Font size of the text displayed in each cell.
     fontfamily : str, default="'DejaVu', sans-serif"
-        Font used for the text in each cell (CSS)
+        Font used for the text in each cell.
     textalign : str, default="center"
-        Alignment of the text in each cell (CSS)
-    hover_color : str, default="#e7e7e7"
-        Background color when hovering a cell (CSS)
+        Alignment of the text in each cell.
+    background_color : str, default="white"
+        Only available for the "interactive" template.
+        Background color of a cell.
+    hover_color : str, default="rgba(0,0,0,0.05)"
+        Only available for the "interactive" template.
+        Background color when hovering a cell
+    custom_css : str or None, default=None
+        Custom CSS properties applied to the generated HTML. Please note that
+        the CSS will apply to the entire page if no iframe is used (see
+        ``use_iframe`` for more details).
     style : dict or None, default=None
         CSS styling applied to each item in a cell. The dict must follow a
         ``key: function`` structure where the key must correspond to one of the
         columns in ``subset`` or ``tooltip``. The function takes the item's
         value as input, and outputs a valid CSS styling. For example, if you
         want to color the text corresponding to the "Solubility" column in your
         dataframe::
@@ -121,50 +178,32 @@
             style={"Solubility": lambda x: "color: red" if x < -5 else ""}
 
         You can also style a whole cell using the ``__all__`` key, the
         corresponding function then has access to all values for each cell::
 
             style={"__all__": lambda x: "color: red" if x["Solubility"] < -5 else ""}
 
-    selection : bool, default=True
-        Only available for the "pages" template. Enables the selection of
-        molecules and displays a checkbox at the top of each cell. To access
-        your selection (index and SMILES), use :func:`mols2grid.get_selection()`
-        or the export options in the bottom checkbox dropdown menu.
-    cache_selection : bool, default=False
-        Restores the selection from a previous grid with the same name
-    transform : dict or None, default=None
-        Functions applied to specific items in all cells. The dict must follow
-        a ``key: function`` structure where the key must correspond to one of
-        the columns in ``subset`` or ``tooltip``. The function takes the item's
-        value as input and transforms it, for example::
-
-            transform={"Solubility": lambda x: f"{x:.2f}",
-                       "Melting point": lambda x: f"MP: {5/9*(x-32):.1f}°C"}
-
-        These transformations only affect columns in ``subset`` and
-        ``tooltip``, and do not interfere with ``style``.
-    custom_css : str or None, default=None
-        Only available for the "pages" template. Custom CSS properties applied
-        to the content of the HTML document.
+    Parameters: Customization
+    -------------------------
+    name : str, default="default"
+        Name of the grid. Used when retrieving selections from multiple grids
+        at the same time
+    rename : dict or None, default=None
+        Rename the properties in the final document.
     custom_header : str or None, default=None
-        Custom libraries to be loaded in the header of the document
-    callback : str or None, default=None
-        Only available for the "pages" template. JavaScript or Python
-        callback to be executed when clicking on an image. A dictionnary
-        containing the data for the full cell is directly available as
-        ``data`` in JS. For Python, the callback function must have
-        ``data`` as the first argument to the function. All the values in
-        the ``data`` dict are parsed as strings, except "mols2grid-id"
-        which is always an integer. Note that fields containing spaces in
-        their name will be replaced by hyphens, i.e. "mol weight" becomes
-        available as ``data["mol-weight"]``.
-    sort_by : str or None, default=None
-        Sort the grid according to the following field (which must be present
-        in ``subset`` or ``tooltip``).
+        Custom libraries to be loaded in the header of the document.
+    callback : str, callable or None, default=None
+        Only available for the "interactive" template.
+        JavaScript or Python callback to be executed when clicking on an image.
+        A dictionnary containing the data for the full cell is directly available
+        as ``data`` in JS. For Python, the callback function must have ``data``
+        as the first argument to the function. All the values in the ``data`` dict
+        are parsed as strings, except "mols2grid-id" which is always an integer.
+        Note that fields containing spaces in their name will be replaced by
+        hyphens, i.e. "mol weight" becomes available as ``data["mol-weight"]``.
 
     Returns
     -------
     view : IPython.core.display.HTML
 
     Notes
     -----
@@ -175,15 +214,15 @@
 
     .. versionadded:: 0.1.0
         Added ``sort_by``, ``custom_css``, ``custom_header`` and ``callback``
         arguments. Added the ability to style an entire cell with
         ``style={"__all__": <function>}``.
 
     .. versionadded:: 0.2.0
-        Added ``substruct_highlight`` argument
+        Added ``substruct_highlight`` argument.
 
     .. versionchanged:: 0.2.2
         If both ``subset`` and ``tooltip`` are ``None``, the index and image
         will be directly displayed on the grid while the remaining fields will
         be in the tooltip.
 
     .. versionchanged:: 1.0.0
@@ -215,26 +254,26 @@
 def _(mols, **kwargs):
     template, kwargs, render_kwargs = _prepare_kwargs(kwargs, "display")
     return MolGrid.from_mols(mols, **kwargs).display(template=template, **render_kwargs)
 
 
 @singledispatch
 def save(arg, **kwargs):
-    """Generate an interactive grid of molecules and save it
+    """Generate an interactive grid of molecules and save it.
 
     Parameters
     ----------
     arg : pandas.DataFrame, SDF file or list of molecules
-        The input containing your molecules
+        The input containing your molecules.
     output : str
-        Name and path of the output document
+        Name and path of the output document.
 
     Notes
     -----
-    See :func:`display` for the full list of arguments
+    See :func:`display` for the full list of arguments.
     """
     raise TypeError(f"No save method registered for type {type(arg)!r}")
 
 
 @save.register(DataFrame)
 def _(df, **kwargs):
     template, kwargs, render_kwargs = _prepare_kwargs(kwargs, "save")
@@ -250,14 +289,14 @@
     return MolGrid.from_sdf(sdf, **kwargs).save(
         output, template=template, **render_kwargs
     )
 
 
 @save.register(Series)
 @save.register(list)
-@display.register(tuple)
+@save.register(tuple)
 def _(mols, **kwargs):
     template, kwargs, render_kwargs = _prepare_kwargs(kwargs, "save")
     output = kwargs.pop("output")
     return MolGrid.from_mols(mols, **kwargs).save(
         output, template=template, **render_kwargs
     )
```

### Comparing `mols2grid-1.1.1/mols2grid/molgrid.py` & `mols2grid-2.0.0rc1/mols2grid/molgrid.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,92 +26,117 @@
 from .widget import MolGridWidget
 
 try:
     from IPython.display import HTML, Javascript, display
 except ModuleNotFoundError:
     pass
 else:
-    warnings.filterwarnings("ignore", "Consider using IPython.display.IFrame instead")
+    warnings.filterwarnings("ignore", "Consider using IPython.display.IFrame instead.")
+
+
+# Detect if mols2grid is running inside a Jupyter Notebook/Lab.
+# If it is, we wrap the HTML in an iframe.
+try:
+    get_ipython()  # This is callable only in Jupyter Notebook.
+    is_jupyter = True
+except NameError:
+    is_jupyter = False
 
 
 class MolGrid:
     """Class that handles drawing molecules, rendering the HTML document and
-    saving or displaying it in a notebook
+    saving or displaying it in a Jupyter Notebook.
 
-    Parameters
-    ----------
-    df : pandas.DataFrame, dict or list
+    Parameters: Data
+    ----------------
+    df : pandas.DataFrame, dict or list, required
         Dataframe containing a SMILES or mol column, or dictionary containing a
-        list of SMILES, or list of dictionnaries containing a SMILES field
-    smiles_col : str or None
-        Name of the SMILES column in the dataframe, if available
-    mol_col : str or None
+        list of SMILES, or list of dictionnaries containing a SMILES field.
+    smiles_col : str or None, default="SMILES"
+        Name of the SMILES column in the dataframe, if available.
+    mol_col : str or None, default=None
         Name of an RDKit molecule column. If available, coordinates and
-        atom/bonds annotations from this will be used for depiction
-    removeHs : bool
-        Remove hydrogen atoms from the drawings
-    use_coords : bool
-        Use the existing coordinates of the molecule
-    coordGen : bool
-        Sets whether or not the CoordGen library should be preferred to the
-        RDKit depiction library
-    useSVG : bool
-        Use SVG instead of PNG
-    size : tuple
-        The size of the drawing canvas
-    MolDrawOptions : rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions or None
-        Drawing options. Useful for making highly customized drawings
-    rename : dict or None
-        Rename the properties/fields stored in the molecule
-    name : str
+        atom/bonds annotations from this will be used for depiction.
+
+    Parameters: Display
+    -------------------
+    size : tuple, default=(130, 90)
+        The size of the drawing canvas. The cell minimum width is set to the
+        width of the image, so if the cell padding is increased, the image will
+        be displayed smaller.
+    useSVG : bool, default=True
+        Use SVG images instead of PNG.
+    prerender : bool, default=False
+        Prerender images for the entire dataset, or generate them on-the-fly.
+        Prerendering is slow and memory-hungry, but required when ``template="static"``
+        or ``useSVG=False``.
+    cache_selection : bool, default=False
+        Restores the selection from a previous grid with the same name.
+
+    Parameters: Mols
+    ----------------
+    removeHs : bool, default=False
+        Remove hydrogen atoms from the drawings.
+    use_coords : bool, default=False
+        Use the coordinates of the molecules (only relevant when an SDF file, a
+        list of molecules or a DataFrame of RDKit molecules were used as input.)
+    coordGen : bool, default=True
+        Use the CoordGen library instead of the RDKit one to depict the
+        molecules in 2D.
+    MolDrawOptions : rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions or None, default=None
+        Drawing options. Useful for making highly customized drawings.
+
+    Parameters: Customization
+    -------------------------
+    name : str, default="default"
         Name of the grid. Used when retrieving selections from multiple grids
-        at the same time
-    cache_selection : bool
-        Restores the selection from a previous grid with the same name
-    prerender : bool
-        Prerender images for the entire dataset, or generate them on-the-fly
-        when needed
+        at the same time.
+    rename : dict or None, default=None
+        Rename the properties in the final document.
     kwargs : object
         :class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions` attributes, and
-        the additional ``atomColourPalette``
+        the additional ``atomColourPalette``.
 
     Notes
     -----
     On-the-fly rendering of images does not read the atom colour palette
     from the :class:`~rdkit.Chem.Draw.rdMolDraw2D.MolDrawOptions` parameter.
     If this is needed, use the following::
 
         MolGrid(df, atomColourPalette={1: (.8, 0, 1)})
 
     .. versionchanged:: 0.1.0
-        Added ``rename`` parameter to replace ``mapping``
+        Added ``rename`` parameter to replace ``mapping``.
 
     .. versionadded:: 0.2.0
-        Added ``prerender`` and ``cache_selection`` parameters
+        Added ``prerender`` and ``cache_selection`` parameters.
 
     .. versionchanged:: 0.2.0
         Images are now generated on-the-fly. ``use_coords`` is now ``False`` by
-        default to avoid a systematic error when using ``MolGrid.from_sdf``
+        default to avoid a systematic error when using ``MolGrid.from_sdf``.
     """
 
     def __init__(
         self,
         df,
         smiles_col="SMILES",
         mol_col=None,
+        #
+        size=(130, 90),
+        useSVG=True,
+        prerender=False,
+        cache_selection=False,
+        #
         removeHs=False,
         use_coords=False,
         coordGen=True,
-        useSVG=True,
-        size=(160, 120),
         MolDrawOptions=None,
-        rename=None,
+        #
         name="default",
-        prerender=False,
-        cache_selection=False,
+        rename=None,
         **kwargs,
     ):
         if not (smiles_col or mol_col):
             raise ValueError("One of `smiles_col` or `mol_col` must be set")
         if not isinstance(name, str):
             raise TypeError(
                 f"`name` must be a string. Currently of type {type(name).__name__}"
@@ -128,22 +153,22 @@
         self.img_size = size
         self.prerender = prerender
         self.smiles_col = smiles_col
         self.mol_col = mol_col
         if isinstance(df, pd.DataFrame):
             dataframe = df.copy()
         else:
-            # list of dicts or other input formats for dataframes
+            # List of dicts or other input formats for dataframes.
             dataframe = pd.DataFrame(df)
         if rename:
             dataframe.rename(columns=rename, inplace=True)
         self._extra_columns = ["img", "mols2grid-id"]
-        # add index
+        # Add index.
         dataframe["mols2grid-id"] = list(range(len(dataframe)))
-        # generate drawing options
+        # Generate drawing options.
         if prerender:
             Draw.rdDepictor.SetPreferCoordGen(coordGen)
             opts = MolDrawOptions or Draw.MolDrawOptions()
             for key, value in kwargs.items():
                 setattr(opts, key, value)
             self.MolDrawOptions = opts
             self._MolDraw2D = Draw.MolDraw2DSVG if useSVG else Draw.MolDraw2DCairo
@@ -157,56 +182,57 @@
                         or callable(value)
                         or value.__class__.__module__ != "builtins"
                     ):
                         opts[key] = value
             opts.update(kwargs)
             opts.update({"width": self.img_size[0], "height": self.img_size[1]})
             self.json_draw_opts = json.dumps(opts)
-        # prepare smiles and images
+        # Prepare smiles and images.
         self._prepare_dataframe(dataframe)
         self.dataframe = dataframe
-        # register instance
+        # Register instance.
         self._grid_id = name
         if cache_selection:
             try:
                 self._cached_selection = register.get_selection(name)
             except KeyError:
                 self._cached_selection = {}
                 register._init_grid(name)
             else:
                 register._update_current_grid(name)
         else:
             self._cached_selection = {}
             register._init_grid(name)
-        # create widget
+        # Create widget.
         widget = MolGridWidget(grid_id=name, selection=str(self._cached_selection))
         selection_handler = partial(register.selection_updated, name)
         widget.observe(selection_handler, names=["selection"])
+        # Register widget JS-side.
         display(widget)
         self.widget = widget
 
     @classmethod
     def from_mols(cls, mols, **kwargs):
         """Set up the dataframe used by mols2grid directly from a list of RDKit
-        molecules
+        molecules.
 
         Parameters
         ----------
         mols : list
             List of RDKit molecules
         kwargs : object
             Other arguments passed on initialization
         """
         mol_col = kwargs.pop("mol_col", "mol")
         df = pd.DataFrame([mol_to_record(mol, mol_col=mol_col) for mol in mols])
         return cls(df, mol_col=mol_col, **kwargs)
 
     @classmethod
     def from_sdf(cls, sdf_file, **kwargs):
-        """Set up the dataframe used by mols2grid directly from an SDFile
+        """Set up the dataframe used by mols2grid directly from an SDFile.
 
         Parameters
         ----------
         sdf_file : str, pathlib.Path
             Path to the SDF file (.sdf or .sdf.gz)
         kwargs : object
             Other arguments passed on initialization
@@ -219,236 +245,264 @@
         df = sdf_to_dataframe(sdf_file, mol_col=mol_col)
         return cls(df, mol_col=mol_col, **kwargs)
 
     @property
     def template(self):
         """Kind of grid displayed, one of:
 
-        * pages
-        * table
+        * interactive
+        * static
         """
         return self._template
 
     @template.setter
     def template(self, value):
-        if value not in ["pages", "table"]:
+        if value not in ["interactive", "static"]:
             raise ValueError(
-                f"template={value!r} not supported. " "Use one of 'pages' or 'table'"
+                f"template={value!r} not supported. "
+                "Use either 'interactive' or 'static'."
             )
         self._template = value
 
     def draw_mol(self, mol):
-        """Draw a molecule"""
+        """Draw a molecule."""
         d2d = self._MolDraw2D(*self.img_size)
         d2d.SetDrawOptions(self.MolDrawOptions)
         hl_atoms = getattr(mol, "__sssAtoms", [])
         d2d.DrawMolecule(mol, highlightAtoms=hl_atoms)
         d2d.FinishDrawing()
         return d2d.GetDrawingText()
 
     def mol_to_img(self, mol):
-        """Convert an RDKit mol to an HTML image containing a drawing of the
-        molecule"""
+        """Convert an RDKit mol to an inline PNG image containing a drawing of the
+        molecule."""
         img = self.draw_mol(mol)
         if self.useSVG:
             return img
         data = b64encode(img).decode()
         return f'<img src="data:image/png;base64,{data}">'
 
     def _prepare_dataframe(self, dataframe):
         """Prepares the dataframe with SMILES and images depending on user input. The
         dataframe is modified inplace."""
         if self.prerender:
             if self.mol_col:
                 keep_mols = True
             else:
-                # make temporary mol column if not present
+                # Make temporary mol column if not present.
                 self.mol_col = "mol"
                 keep_mols = False
                 dataframe[self.mol_col] = dataframe[self.smiles_col].apply(
                     Chem.MolFromSmiles
                 )
-            # drop empty mols
+            # Drop empty mols.
             dataframe.dropna(axis=0, subset=[self.mol_col], inplace=True)
-            # modify mol according to user pref
+            # Modify mol according to user pref.
             if not self.use_coords:
                 dataframe[self.mol_col] = dataframe[self.mol_col].apply(
                     remove_coordinates
                 )
             if self.removeHs:
                 dataframe[self.mol_col] = dataframe[self.mol_col].apply(Chem.RemoveHs)
-            # render
+            # Render.
             dataframe["img"] = dataframe[self.mol_col].apply(self.mol_to_img)
-            # cleanup
+            # Cleanup.
             if not keep_mols:
                 dataframe.drop(columns=self.mol_col, inplace=True)
                 self.mol_col = None
         else:
             dataframe["img"] = None
-        # generate smiles col if not present or needs to be updated
+        # Generate smiles col if not present or needs to be updated.
         if self.mol_col and self.smiles_col not in dataframe.columns:
             dataframe[self.smiles_col] = dataframe[self.mol_col].apply(mol_to_smiles)
 
-    def render(self, template="pages", **kwargs):
-        """Returns the HTML document corresponding to the "pages" or "table"
-        template. See :meth:`to_pages` and :meth:`to_table` for the full list
-        of arguments
+    def render(self, template="interactive", **kwargs):
+        """Returns the HTML document corresponding to the "interactive" or "static"
+        template. See :meth:`to_interactive` and :meth:`to_static` for the full list
+        of arguments.
 
         Parameters
         ----------
         template : str
-            Kind of grid to draw:
+            What kind of grid to draw:
 
-            * table
-                A very simple table where all molecules are displayed on the
-                document, similarly to RDKit's :func:`~rdkit.Chem.Draw.rdMolDraw2D.MolsToGridImage`.
+            * interactive
+                An interactive grid that layouts the original set of
+                molecules on several pages, allowing for selecting molecules and
+                filtering them using text or substructure queries.
+            * static
+                A simple table with all molecules displayed at once, similarly
+                to RDKit's :func:`~rdkit.Chem.Draw.rdMolDraw2D.MolsToGridImage`.
                 This template is mainly used for printing on paper or in a PDF
                 file. Most of the interactive actions aren't available.
-            * pages
-                A more interactive version that layouts the original set of
-                molecules on several pages, allows for selecting molecules and
-                filtering them using text or substructure queries.
         """
         self.template = template
         return getattr(self, f"to_{self.template}")(**kwargs)
 
-    def to_pages(
+    def to_interactive(
         self,
+        # Display
         subset=None,
         tooltip=None,
-        n_cols=5,
-        n_rows=3,
+        tooltip_fmt="<strong>{key}</strong>: {value}",
+        tooltip_placement="auto",
+        transform=None,
+        sort_by=None,
+        use_iframe=False,
+        truncate=True,
+        n_items_per_page=24,
+        selection=True,
+        # Mols
+        substruct_highlight=None,
+        single_highlight=False,
+        # CSS
         border="1px solid #cccccc",
         gap=0,
-        fontsize="12pt",
+        pad=10,
+        fontsize="12px",
         fontfamily="'DejaVu', sans-serif",
         textalign="center",
-        tooltip_fmt="<strong>{key}</strong>: {value}",
-        tooltip_trigger="click hover",
-        tooltip_placement="auto",
-        hover_color="#e7e7e7",
-        style=None,
-        selection=True,
-        transform=None,
+        background_color="white",
+        hover_color="rgba(0,0,0,0.05)",
         custom_css=None,
+        style=None,
+        # Customization
         custom_header=None,
         callback=None,
-        sort_by=None,
-        substruct_highlight=None,
-        single_highlight=False,
+        **kwargs,
     ):
-        """Returns the HTML document for the "pages" template
+        """Returns the HTML document for the "interactive" template.
 
-        Parameters
-        ----------
-        subset : list or None
+        Parameters: Display
+        -------------------
+        subset: list or None, default=None
             Columns to be displayed in each cell of the grid. Each column's
-            value will be displayed from top to bottom in the same order given
-            here. Use ``"img"`` for the image of the molecule, and
-            ``"mols2grid-id"`` for the molecule's index in your input file.
-        tooltip : list or None
-            Columns to be displayed as a tooltip when hovering/clicking on the
-            image of a cell.
-        tooltip_fmt : str
-            Format string of each key/value pair in the tooltip
-        tooltip_trigger : str
-            Sequence of triggers for the tooltip: ``click``, ``hover`` or
-            ``focus``
-        tooltip_placement : str
-            Position of the tooltip: ``auto``, ``top``, ``bottom``, ``left``
-            or ``right``
-        n_cols : int
-            Number of columns per page
-        n_rows : int
-            Number of rows per page
-        border : str
-            Styling of the border around each cell (CSS)
-        gap : int
-            Size of the margin around each cell in px
-        fontsize : str
-            Font size of the text displayed in each cell (CSS)
-        fontfamily : str
-            Font used for the text in each cell (CSS)
-        textalign : str
-            Alignment of the text in each cell (CSS)
-        hover_color : str
-            Background color when hovering a cell (CSS)
-        style : dict or None
+            value will be displayed from top to bottom in the order provided.
+            The ``"img"`` and ``"mols2grid-id"`` columns are displayed by default,
+            however you can still add the ``"img"`` column if you wish to change
+            the display order.
+        tooltip : list, None or False, default=None
+            Columns to be displayed inside the tooltip. When no subset is set,
+            all columns will be listed in the tooltip by default. Use ``False``
+            to hide the tooltip.
+        tooltip_fmt : str, default="<strong>{key}</strong>: {value}"
+            Format string of each key/value pair in the tooltip.
+        tooltip_placement : str, default="auto"
+            Position of the tooltip: ``auto``, ``top``, ``bottom``, ``left`` or
+            ``right``.
+        transform : dict or None, default=None
+            Functions applied to specific items in all cells. The dict must follow
+            a ``key: function`` structure where the key must correspond to one of
+            the columns in ``subset`` or ``tooltip``. The function takes the item's
+            value as input and transforms it, for example::
+
+                transform={
+                    "Solubility": lambda x: f"{x:.2f}",
+                    "Melting point": lambda x: f"MP: {5/9*(x-32):.1f}°C"
+                }
+
+            These transformations only affect columns in ``subset`` and
+            ``tooltip``, and do not interfere with ``style``.
+        sort_by : str or None, default=None
+            Sort the grid according to the following field (which must be
+            present in ``subset`` or ``tooltip``).
+        use_iframe : bool, default=False
+            Whether to use an iframe to display the grid. When the grid is displayed
+            inside a Jupyter Notebook or JupyterLab, this will default to ``True``.
+        truncate: bool, default=True/False
+            Whether to truncate the text in each cell if it's too long.
+            Defaults to ``True`` for interactive grids, ``False`` for static grid.
+        n_items_per_page, default=24
+            Number of items to display per page. A multiple of 12 is recommended
+            for optimal display.
+        selection : bool, default=True
+            Enables the selection of molecules and displays a checkbox at the
+            top of each cell. In the context of a Jupyter Notebook, this gives
+            you access to your selection (index and SMILES) through
+            :func:`mols2grid.get_selection()` or :meth:`MolGrid.get_selection()`.
+            In all cases, you can export your selection by clicking on the triple-dot menu.
+
+        Parameters: Mols
+        ----------------
+        substruct_highlight : bool or None, default=None
+            Highlight substructure when using the SMARTS search. Active by default
+            when ``prerender=False``.
+        single_highlight : bool, default=False
+            Highlight only the first match of the substructure query.
+
+        Parameters: CSS
+        ---------------
+        border : str, default="1px solid #cccccc"
+            Styling of the border around each cell.
+        gap : int, default=0
+            Size in pixels of the gap between cells.
+        pad : int, default=10
+            Size in pixels of the cell padding.
+        fontsize : str, default="12px"
+            Font size of the text displayed in each cell.
+        fontfamily : str, default="'DejaVu', sans-serif"
+            Font used for the text in each cell.
+        textalign : str, default="center"
+            Alignment of the text in each cell.
+        background_color : str, default="white"
+            Background color of a cell.
+        hover_color : str, default="rgba(0,0,0,0.05)"
+            Background color when hovering a cell.
+        custom_css : str or None, default=None
+            Custom CSS properties applied to the generated HTML. Please note that
+            the CSS will apply to the entire page if no iframe is used (see
+            ``use_iframe`` for more details).
+        style : dict or None, default=None
             CSS styling applied to each item in a cell. The dict must follow a
             ``key: function`` structure where the key must correspond to one of the
             columns in ``subset`` or ``tooltip``. The function takes the item's
             value as input, and outputs a valid CSS styling. For example, if you
             want to color the text corresponding to the "Solubility" column in your
             dataframe::
 
                 style={"Solubility": lambda x: "color: red" if x < -5 else ""}
 
             You can also style a whole cell using the ``__all__`` key, the
             corresponding function then has access to all values for each cell::
 
                 style={"__all__": lambda x: "color: red" if x["Solubility"] < -5 else ""}
 
-        selection : bool
-            Enables the selection of molecules and displays a checkbox at the
-            top of each cell. In the context of a Jupyter notebook, this gives
-            you access to your selection (index and SMILES) through :func:`mols2grid.get_selection()`
-            or :meth:`MolGrid.get_selection()`. In all cases, you can export your
-            selection by clicking on the ☑ icon.
-        transform : dict or None
-            Functions applied to specific items in all cells. The dict must follow
-            a ``key: function`` structure where the key must correspond to one of
-            the columns in ``subset`` or ``tooltip``. The function takes the item's
-            value as input and transforms it, for example::
-
-                transform={"Solubility": lambda x: f"{x:.2f}",
-                           "Melting point": lambda x: f"MP: {5/9*(x-32):.1f}°C"}
-
-            These transformations only affect columns in ``subset`` and
-            ``tooltip``, and do not interfere with ``style``.
-        custom_css : str or None
-            Custom CSS properties applied to the content of the HTML document
-        custom_header : str or None
-            Custom libraries to be loaded in the header of the document
-        callback : str or callable
-            Only available for the "pages" template. JavaScript or Python
-            callback to be executed when clicking on an image. A dictionnary
-            containing the data for the full cell is directly available as
-            ``data`` in JS. For Python, the callback function must have
-            ``data`` as the first argument to the function. All the values in
-            the ``data`` dict are parsed as strings, except "mols2grid-id"
-            which is always an integer. Note that fields containing spaces in
-            their name will be replaced by hyphens, i.e. "mol weight" becomes
-            available as ``data["mol-weight"]``.
-        sort_by : str or None
-            Sort the grid according to the following field (which must be
-            present in ``subset`` or ``tooltip``).
-        substruct_highlight : bool or None
-            Highlight substructure when using the SMARTS search. Only available
-            when ``prerender=False``
-        single_highlight : bool
-            Highlight only the first match of the substructure query
+            Parameters: Customization
+            -------------------------
+            custom_header : str or None, default=None
+                Custom libraries to be loaded in the header of the document.
+            callback : str, callable or None, default=None
+                JavaScript or Python callback to be executed when clicking on an image.
+                A dictionnary containing the data for the full cell is directly available
+                as ``data`` in JS. For Python, the callback function must have ``data``
+                as the first argument to the function. All the values in the ``data`` dict
+                are parsed as strings, except "mols2grid-id" which is always an integer.
+                Note that fields containing spaces in their name will be replaced by
+                hyphens, i.e. "mol weight" becomes available as ``data["mol-weight"]``.
 
         Returns
         -------
         html_document : str
 
         Notes
         -----
         If ``subset=None, tooltip=None``, the index and image will be directly
         displayed on the grid while the remaining fields will be in the
         tooltip.
 
+        The cell width is defined by the size[0] parameter.
+
         .. versionadded:: 0.1.0
             Added ``sort_by``, ``custom_css``, ``custom_header`` and
             ``callback`` arguments.
             Added the ability to style an entire cell with
             ``style={"__all__": <function>}``.
 
         .. versionadded:: 0.2.0
-            Added ``substruct_highlight`` argument
+            Added ``substruct_highlight`` argument.
 
         .. versionchanged:: 0.2.2
             If both ``subset`` and ``tooltip`` are ``None``, the index and
             image will be directly displayed on the grid while the remaining
             fields will be in the tooltip.
 
         .. versionchanged:: 1.0.0
@@ -463,212 +517,251 @@
             raise ValueError(
                 "Cannot highlight substructure search with prerendered images"
             )
         if self.mol_col:
             df = self.dataframe.drop(columns=self.mol_col).copy()
         else:
             df = self.dataframe.copy()
-        cell_width = self.img_size[0]
         smiles = self.smiles_col
-        content = []
+        content = []  # Gets filled with the HTML content of each cell.
         column_map = {}
-        width = n_cols * (cell_width + 2 * (gap + 2))
 
         if subset is None:
             if tooltip is None:
                 subset = ["mols2grid-id", "img"]
                 tooltip = [x for x in df.columns.tolist() if x not in subset]
             else:
+                # When no subset is defined, all columns are displayed.
                 subset = df.columns.tolist()
-                subset = [subset.pop(subset.index("img"))] + subset
+        else:
+            # work on a copy
+            subset = subset[:]
 
+        if "mols2grid-id" not in subset:
+            subset.insert(0, "mols2grid-id")
         if "img" not in subset:
-            raise KeyError("Please add the 'img' field in the `subset` parameter")
+            subset.insert(0, "img")
+
+        # Always make sure the image comes first.
+        # subset = [subset.pop(subset.index("img"))] + subset
+        #
+        # This was removed at Cedric's request, so you can choose
+        # to have certain properties displayed above the image.
 
-        # define fields that are searchable and sortable
+        # Define fields that are searchable and sortable.
         search_cols = [f"data-{col}" for col in subset if col != "img"]
         if tooltip:
             search_cols.extend([f"data-{col}" for col in tooltip])
             for col in tooltip:
                 if col not in subset:
                     s = f'<div class="data data-{slugify(col)}" style="display: none;"></div>'
                     content.append(s)
                     column_map[col] = f"data-{col}"
         else:
             tooltip = []
         sort_cols = search_cols[:]
-        sort_cols = ["mols2grid-id"] + sort_cols
-        # get unique list but keep order
+        sort_cols = ["data-mols2grid-id"] + sort_cols
+
+        # Get unique list but keep order.
         sort_cols = list(dict.fromkeys(sort_cols))
         if style is None:
             style = {}
         if transform is None:
             transform = {}
         value_names = list(set(subset + [smiles] + tooltip))
         value_names = [f"data-{col}" for col in value_names]
 
-        # force id, SMILES, and tooltip values to be present in the data
+        # Force id, SMILES, and tooltip values to be present in the data.
         final_columns = subset[:]
         final_columns.extend(["mols2grid-id", smiles])
         if tooltip:
             final_columns.extend(tooltip)
         final_columns = list(set(final_columns))
 
-        # make a copy if id shown explicitely
-        if "mols2grid-id" in subset:
-            id_name = "mols2grid-id-copy"
-            df[id_name] = df["mols2grid-id"]
-            value_names.append(f"data-{id_name}")
-            final_columns.append(id_name)
-            subset = [id_name if x == "mols2grid-id" else x for x in subset]
-        # organize data
+        # Make a copy of id shown explicitly.
+        id_name = "mols2grid-id-display"
+        df[id_name] = df["mols2grid-id"]
+        value_names.append(f"data-{id_name}")
+        final_columns.append(id_name)
+        subset = [id_name if x == "mols2grid-id" else x for x in subset]
+        id_display_html = f'<div class="data-{id_name}"></div>'
+
+        # Organize data.
         temp = []
         for col in subset:
-            if col == "img" and tooltip:
-                s = (
-                    f'<a tabindex="0" class="data data-{col} mols2grid-tooltip" '
-                    'data-toggle="popover" data-content="."></a>'
-                )
+            if col == "mols2grid-id-display":
+                s = ""  # Avoid an empty div to be created for the display id.
+            elif col == "img" and tooltip:
+                s = f'<a class="data data-{col}"></a>'
             else:
                 if style.get(col):
                     s = (
-                        f'<div class="data data-{slugify(col)} style-{slugify(col)}" '
+                        f'<div class="data data-{slugify(col)} copy-me style-{slugify(col)}" '
                         'style=""></div>'
                     )
                 else:
-                    s = f'<div class="data data-{slugify(col)}"></div>'
+                    s = f'<div class="data data-{slugify(col)} copy-me"></div>'
             temp.append(s)
             column_map[col] = f"data-{col}"
         content = temp + content
-        # add but hide SMILES div if not present
+
+        # Add but hide SMILES div if not present.
         if smiles not in (subset + tooltip):
-            s = f'<div class="data data-{slugify(smiles)}" style="display: none;"></div>'
+            s = f'<div class="data data-{slugify(smiles)} copy-me" style="display: none;"></div>'
             content.append(s)
             column_map[smiles] = f"data-{smiles}"
-        # set mapping for list.js
+
+        # Set mapping for list.js.
         if "__all__" in style.keys():
             whole_cell_style = True
             x = "[{data: ['mols2grid-id', 'cellstyle']}, "
         else:
             whole_cell_style = False
             x = "[{data: ['mols2grid-id']}, "
         value_names = [slugify(c) for c in value_names]
         value_names = x + str(value_names)[1:]
 
-        # apply CSS styles
+        # Apply CSS styles.
         for col, func in style.items():
             if col == "__all__":
                 name = "cellstyle"
                 df[name] = df.apply(func, axis=1)
             else:
                 name = f"style-{slugify(col)}"
                 df[name] = df[col].apply(func)
             final_columns.append(name)
             value_names = value_names[:-1] + f", {{ attr: 'style', name: {name!r} }}]"
 
+        # Create tooltip.
         if tooltip:
-            df["mols2grid-tooltip"] = df.apply(
+            df["m2g-tooltip"] = df.apply(
                 tooltip_formatter, axis=1, args=(tooltip, tooltip_fmt, style, transform)
             )
-            final_columns += ["mols2grid-tooltip"]
+            final_columns += ["m2g-tooltip"]
             value_names = (
-                value_names[:-1]
-                + ", {attr: 'data-content', name: 'mols2grid-tooltip'}]"
+                value_names[:-1] + ", {attr: 'data-content', name: 'm2g-tooltip'}]"
             )
+            info_btn_html = '<div class="m2g-info">i</div>'
+        else:
+            info_btn_html = ""
 
-        # apply custom user function
+        # Apply custom user function.
         for col, func in transform.items():
             df[col] = df[col].apply(func)
 
+        # Add checkboxes.
         if selection:
             if self._cached_selection:
                 df["cached_checkbox"] = False
                 df.loc[
                     df["mols2grid-id"].isin(self._cached_selection.keys()),
                     "cached_checkbox",
                 ] = True
                 final_columns += ["cached_checkbox"]
                 value_names = (
                     value_names[:-1] + ", {attr: 'checked', name: 'cached_checkbox'}]"
                 )
-            checkbox = (
-                '<input type="checkbox" '
+            checkbox_html = (
+                '<input type="checkbox" tabindex="-1" '
                 'class="position-relative float-left cached_checkbox">'
             )
         else:
-            checkbox = ""
-        if whole_cell_style:
-            item = (
-                '<div class="cell" data-mols2grid-id="0" '
-                'data-cellstyle="0">{checkbox}{content}</div>'
-            )
+            checkbox_html = ""
+
+        # Add callback button.
+        if callback:
+            callback_btn_html = '<div class="m2g-callback"></div>'
         else:
-            item = (
-                '<div class="cell" data-mols2grid-id="0">' "{checkbox}{content}</div>"
-            )
-        item = item.format(checkbox=checkbox, content="".join(content))
+            callback_btn_html = ""
 
-        # callback
-        if callback and "click" in tooltip_trigger and len(tooltip_trigger.split()) > 1:
-            # remove click from triggers if callback is present
-            tooltip_trigger = tooltip_trigger.replace("click", "")
+        # Generate cell HTML.
+        item = (
+            '<div class="m2g-cell" data-mols2grid-id="0" tabindex="0">'
+            '<div class="m2g-cb-wrap">{checkbox_html}<div class="m2g-cb"></div>{id_display_html}</div>'
+            '<div class="m2g-cell-actions">{info_btn_html}{callback_btn_html}</div>'
+            "{content}"
+            "{tooltip_html}"
+            "</div>"
+        )
+
+        item = item.format(
+            checkbox_html=checkbox_html,
+            id_display_html=id_display_html,
+            info_btn_html=info_btn_html,
+            callback_btn_html=callback_btn_html,
+            content="".join(content),
+            tooltip_html='<div class="m2g-tooltip" data-toggle="popover" data-content="."></div>'
+            if tooltip
+            else "",
+        )
+
+        # Callback
         if isinstance(callback, _JSCallback):
             if custom_header and callback.library_src:
                 custom_header = callback.library_src + custom_header
             else:
                 custom_header = callback.library_src
             callback = callback.code
         if callable(callback):
             callback_type = "python"
             cb_handler = partial(callback_handler, callback)
             self.widget.observe(cb_handler, names=["callback_kwargs"])
         else:
             callback_type = "js"
 
+        # Sort
         if sort_by and sort_by != "mols2grid-id":
             if sort_by in (subset + tooltip):
                 sort_by = f"data-{slugify(sort_by)}"
             else:
                 raise ValueError(
                     f"{sort_by!r} is not an available field in " "`subset` or `tooltip`"
                 )
         else:
             sort_by = "mols2grid-id"
 
-        # slugify remaining vars
+        # Slugify remaining vars.
         column_map = {k: slugify(v) for k, v in column_map.items()}
         sort_cols = [slugify(c) for c in sort_cols]
         search_cols = [slugify(c) for c in search_cols]
         smiles = slugify(smiles)
         df = df[final_columns].rename(columns=column_map).sort_values(sort_by)
 
-        template = env.get_template("pages.html")
+        template = env.get_template("interactive.html")
         template_kwargs = dict(
-            padding=18,
-            width=width,
-            height=self.img_size[1],
+            tooltip=tooltip,
+            tooltip_placement=repr(tooltip_placement),
+            n_items_per_page=n_items_per_page,
+            selection=selection,
+            truncate=truncate,
+            sort_by=sort_by,
+            use_iframe=use_iframe,
+            #
             border=border,
-            textalign=textalign,
-            cell_width=cell_width,
-            fontfamily=fontfamily,
+            gap=gap,
+            gap_px="-1px -1px 0 0" if gap == 0 else f"{gap}px",
+            pad=pad,
             fontsize=fontsize,
-            gap=f"{gap}px",
+            fontfamily=fontfamily,
+            textalign=textalign,
+            background_color=background_color,
             hover_color=hover_color,
+            #
+            iframe_padding=18,
+            cell_width=self.img_size[0],
+            image_width=self.img_size[0],
+            image_height=self.img_size[1],
+            #
             item=item,
             item_repr=repr(item),
             value_names=value_names,
-            tooltip=tooltip,
-            tooltip_trigger=repr(tooltip_trigger),
-            tooltip_placement=repr(tooltip_placement),
-            n_items_per_page=n_rows * n_cols,
             search_cols=search_cols,
             data=json.dumps(
                 df.to_dict("records"), indent=None, default=lambda x: "🤷‍♂️"
             ),
-            selection=selection,
             cached_selection=(
                 [
                     list(self._cached_selection.keys()),
                     list(self._cached_selection.values()),
                 ]
                 if self._cached_selection
                 else False
@@ -677,38 +770,37 @@
             sort_cols=sort_cols,
             grid_id=self._grid_id,
             whole_cell_style=whole_cell_style,
             custom_css=custom_css or "",
             custom_header=custom_header or "",
             callback=callback,
             callback_type=callback_type,
-            sort_by=sort_by,
             removeHs=self.removeHs,
             prefer_coordGen=self.prefer_coordGen,
             onthefly=not self.prerender,
             substruct_highlight=substruct_highlight,
             json_draw_opts=getattr(self, "json_draw_opts", ""),
             single_highlight=single_highlight,
         )
         return template.render(**template_kwargs)
 
     def get_selection(self):
-        """Retrieve the dataframe subset corresponding to your selection
+        """Retrieve the dataframe subset corresponding to your selection.
 
         Returns
         -------
         pandas.DataFrame
         """
         sel = list(register.get_selection(self._grid_id).keys())
         return self.dataframe.loc[self.dataframe["mols2grid-id"].isin(sel)].drop(
             columns=self._extra_columns
         )
 
     def filter(self, mask):
-        """Filters the grid using a mask (boolean array)
+        """Filters the grid using a mask (boolean array).
 
         Parameters
         ----------
         mask : list, pandas.Series or numpy.ndarray
             Boolean array: ``True`` when the item should be displayed,
             ``False`` if it should be filtered out.
         """
@@ -719,106 +811,128 @@
                 grid_id=self._grid_id, mask=json.dumps(mask)
             )
             return Javascript(filtering_script)
         else:
             self.widget.filter_mask = mask
 
     def filter_by_index(self, indices):
-        """Filters the grid using the dataframe's index"""
+        """Filters the grid using the dataframe's index."""
+
         # convert index to mask
         mask = self.dataframe.index.isin(indices)
         return self.filter(mask)
 
-    def to_table(
+    def to_static(
         self,
+        # Display
         subset=None,
         tooltip=None,
+        tooltip_fmt="<strong>{key}</strong>: {value}",
+        tooltip_trigger="focus",
+        tooltip_placement="auto",
+        transform=None,
+        sort_by=None,
+        use_iframe=False,
+        truncate=False,
         n_cols=5,
-        cell_width=160,
+        # CSS Styling
         border="1px solid #cccccc",
         gap=0,
-        fontsize="12pt",
+        pad=10,
+        fontsize="12px",
         fontfamily="'DejaVu', sans-serif",
         textalign="center",
-        tooltip_fmt="<strong>{key}</strong>: {value}",
-        tooltip_trigger="click hover",
-        tooltip_placement="auto",
-        hover_color="#e7e7e7",
-        style=None,
-        transform=None,
         custom_css=None,
+        style=None,
+        # Customization
         custom_header=None,
-        sort_by=None,
+        **kwargs,
     ):
-        """Returns the HTML document for the "table" template
+        """Returns the HTML document for the "static" template
 
-        Parameters
-        ----------
-        subset : list or None
+        Parameters: Display
+        -------------------
+        subset: list or None, default=None
             Columns to be displayed in each cell of the grid. Each column's
-            value will be displayed from top to bottom in the same order given
-            here. Use ``"img"`` for the image of the molecule, and
-            ``"mols2grid-id"`` for the molecule's index in your input file.
-        tooltip : list or None
-            Columns to be displayed as a tooltip when hovering/clicking on the
-            image of a cell.
-        tooltip_fmt : str
-            Format string of each key/value pair in the tooltip
-        tooltip_trigger : str
-            Sequence of triggers for the tooltip: ``click``, ``hover`` or
-            ``focus``
-        tooltip_placement : str
-            Position of the tooltip: ``auto``, ``top``, ``bottom``, ``left``
-            or ``right``
-        n_cols : int
-            Number of columns in the table
-        border : str
-            Styling of the border around each cell (CSS)
-        gap : int or str
-            Size of the margin around each cell (CSS)
-        fontsize : str
-            Font size of the text displayed in each cell (CSS)
-        fontfamily : str
-            Font used for the text in each cell (CSS)
-        textalign : str
-            Alignment of the text in each cell (CSS)
-        hover_color : str
-            Background color when hovering a cell (CSS)
-        style : dict or None
+            value will be displayed from top to bottom in the order provided.
+            The ``"img"`` and ``"mols2grid-id"`` columns are displayed by default,
+            however you can still add the ``"img"`` column if you wish to change
+            the display order.
+        tooltip : list, None or False, default=None
+            Columns to be displayed inside the tooltip. When no subset is set,
+            all columns will be listed in the tooltip by default. Use ``False``
+            to hide the tooltip.
+        tooltip_fmt : str, default="<strong>{key}</strong>: {value}"
+            Format string of each key/value pair in the tooltip.
+        tooltip_trigger : str, default="focus"
+            Sequence of triggers for the tooltip: ``click``, ``hover`` or ``focus``
+        tooltip_placement : str, default="auto"
+            Position of the tooltip: ``auto``, ``top``, ``bottom``, ``left`` or
+            ``right``.
+        transform : dict or None, default=None
+            Functions applied to specific items in all cells. The dict must follow
+            a ``key: function`` structure where the key must correspond to one of
+            the columns in ``subset`` or ``tooltip``. The function takes the item's
+            value as input and transforms it, for example::
+
+                transform={
+                    "Solubility": lambda x: f"{x:.2f}",
+                    "Melting point": lambda x: f"MP: {5/9*(x-32):.1f}°C"
+                }
+
+            These transformations only affect columns in ``subset`` and
+            ``tooltip``, and do not interfere with ``style``.
+        sort_by : str or None, default=None
+            Sort the grid according to the following field (which must be
+            present in ``subset`` or ``tooltip``).
+        use_iframe : bool, default=False
+            Whether to use an iframe to display the grid. When the grid is displayed
+            inside a Jupyter Notebook or JupyterLab, this will default to ``True``.
+        truncate: bool, default=False
+            Whether to truncate the text in each cell if it's too long.
+        n_cols : int, default=5
+            Number of columns in the table.
+
+        Parameters: CSS
+        --------------
+        border : str, default="1px solid #cccccc"
+            Styling of the border around each cell.
+        gap : int, default=0
+            Size in pixels of the gap between cells.
+        pad: int, default=10
+            Size in pixels of the cell padding.
+        fontsize : str, default="12pt"
+            Font size of the text displayed in each cell.
+        fontfamily : str, default="'DejaVu', sans-serif"
+            Font used for the text in each cell.
+        textalign : str, default="center"
+            Alignment of the text in each cell.
+        custom_css : str or None, default=None
+            Custom CSS properties applied to the generated HTML. Please note that
+            the CSS will apply to the entire page if no iframe is used (see
+            ``use_iframe`` for more details).
+        style : dict or None, default=None
             CSS styling applied to each item in a cell. The dict must follow a
             ``key: function`` structure where the key must correspond to one of the
             columns in ``subset`` or ``tooltip``. The function takes the item's
             value as input, and outputs a valid CSS styling. For example, if you
             want to color the text corresponding to the "Solubility" column in your
             dataframe::
 
                 style={"Solubility": lambda x: "color: red" if x < -5 else ""}
 
             You can also style a whole cell using the ``__all__`` key, the
             corresponding function then has access to all values for each cell::
 
                 style={"__all__": lambda x: "color: red" if x["Solubility"] < -5 else ""}
 
-        transform : dict or None
-            Functions applied to specific items in all cells. The dict must follow
-            a ``key: function`` structure where the key must correspond to one of
-            the columns in ``subset`` or ``tooltip``. The function takes the item's
-            value as input and transforms it, for example::
-
-                transform={"Solubility": lambda x: f"{x:.2f}",
-                           "Melting point": lambda x: f"MP: {5/9*(x-32):.1f}°C"}
-
-            These transformations only affect columns in ``subset`` and
-            ``tooltip``, and do not interfere with ``style``.
-        custom_css : str or None
-            Custom CSS properties applied to the content of the HTML document
+        Parameters: Customization
+        -----------------------
         custom_header : str or None
             Custom libraries to be loaded in the header of the document
-        sort_by : str or None
-            Sort the table according to the following field
 
         Returns
         -------
         html_document : str
 
         Notes
         -----
@@ -836,63 +950,70 @@
         .. versionchanged:: 0.2.2
             If both ``subset`` and ``tooltip`` are ``None``, the index and
             image will be directly displayed on the grid while the remaining
             fields will be in the tooltip.
         """
         if not self.prerender:
             raise ValueError(
-                "Please set `prerender=True` when using the 'table' template"
+                "Please set `prerender=True` when using the 'static' template"
             )
         tr = []
         data = []
         sort_by = sort_by or "mols2grid-id"
         df = self.dataframe.sort_values(sort_by).reset_index(drop=True)
-        cell_width = self.img_size[0]
 
         if subset is None:
             if tooltip is None:
                 subset = ["mols2grid-id", "img"]
                 tooltip = [x for x in df.columns.tolist() if x not in subset]
             else:
+                # When no subset is defined, all columns are displayed.
                 subset = df.columns.tolist()
-                subset = [subset.pop(subset.index("img"))] + subset
+        else:
+            # work on a copy
+            subset = subset[:]
+
+        if "mols2grid-id" not in subset:
+            subset.insert(0, "mols2grid-id")
+        if "img" not in subset:
+            subset.insert(0, "img")
+
+        # Always make surer the image comes first.
+        subset = [subset.pop(subset.index("img"))] + subset
+
         if style is None:
             style = {}
         if transform is None:
             transform = {}
         if not tooltip:
             tooltip = []
 
         for i, row in df.iterrows():
             ncell = i + 1
             nrow, ncol = divmod(i, n_cols)
-            td = [f'<td class="col-{ncol}">']
+            popover = tooltip_formatter(row, tooltip, tooltip_fmt, style, transform)
+            td = [
+                f'<td class="col-{ncol} m2g-tooltip" tabindex="0" data-toggle="popover" data-content="{escape(popover)}">'
+            ]
             if "__all__" in style.keys():
                 s = style["__all__"](row)
-                div = [f'<div class="cell-{i}" style="{s}">']
+                div = [f'<div class="m2g-cell-{i}" style="{s}">']
             else:
-                div = [f'<div class="cell-{i}">']
+                div = [f'<div class="m2g-cell-{i}">']
             for col in subset:
                 v = row[col]
                 if col == "img" and tooltip:
-                    popover = tooltip_formatter(
-                        row, tooltip, tooltip_fmt, style, transform
-                    )
-                    item = (
-                        f'<div class="data data-img mols2grid-tooltip" '
-                        f'data-toggle="popover" data-content="{escape(popover)}">'
-                        f"{v}</div>"
-                    )
+                    item = f'<div class="data data-img">' f"{v}</div>"
                 else:
                     func = style.get(col)
                     slug_col = slugify(col)
                     if func:
-                        item = f'<div class="data data-{slug_col}" style="{func(v)}">'
+                        item = f'<div class="data copy-me data-{slug_col}" style="{func(v)}">'
                     else:
-                        item = f'<div class="data data-{slug_col}">'
+                        item = f'<div class="data copy-me data-{slug_col}">'
                     func = transform.get(col)
                     v = func(v) if func else v
                     item += f"{v}</div>"
                 div.append(item)
             div.append("</div>")
             td.append("\n".join(div))
             td.append("</td>")
@@ -901,55 +1022,67 @@
             if (ncell % n_cols == 0) or (ncell == len(df)):
                 cell = [f'<tr class="row-{nrow}">']
                 cell.append("\n".join(tr))
                 cell.append("</tr>")
                 data.append("\n".join(cell))
                 tr = []
 
-        template = env.get_template("table.html")
+        template = env.get_template("static.html")
         template_kwargs = dict(
-            padding=18,
-            border=border,
-            textalign=textalign,
-            cell_width=cell_width,
-            fontfamily=fontfamily,
-            fontsize=fontsize,
-            gap=gap,
-            hover_color=hover_color,
             tooltip=tooltip,
             tooltip_trigger=repr(tooltip_trigger),
             tooltip_placement=repr(tooltip_placement),
+            use_iframe=use_iframe,
+            truncate=truncate,
+            #
+            border=border,
+            gap=gap,
+            pad=pad,
+            textalign=textalign,
+            fontsize=fontsize,
+            fontfamily=fontfamily,
+            #
+            iframe_padding=18,
+            cell_width=self.img_size[0],
+            #
             custom_css=custom_css or "",
             custom_header=custom_header or "",
             data="\n".join(data),
         )
         return template.render(**template_kwargs)
 
     @requires("IPython.display")
     def display(
         self,
-        width="100%",
-        height=None,
+        use_iframe=False,
+        iframe_width="100%",
+        iframe_height=None,
         iframe_allow="clipboard-write",
         iframe_sandbox="allow-scripts allow-same-origin allow-downloads allow-popups allow-modals",
         **kwargs,
     ):
-        """Render and display the grid in a Jupyter notebook
+        """Render and display the grid in a Jupyter notebook.
 
         Returns
         -------
         view : IPython.core.display.HTML
         """
-        doc = self.render(**kwargs)
-        iframe = env.get_template("html/iframe.html").render(
-            width=width,
-            height=height,
-            allow=iframe_allow,
-            sandbox=iframe_sandbox,
-            doc=escape(doc),
-        )
-        return HTML(iframe)
+        use_iframe = is_jupyter or use_iframe
+        doc = self.render(**kwargs, use_iframe=use_iframe)
+        if use_iframe:
+            # Render HTML in iframe.
+            iframe = env.get_template("html/iframe.html").render(
+                width=iframe_width,
+                height=iframe_height,
+                allow=iframe_allow,
+                sandbox=iframe_sandbox,
+                doc=escape(doc),
+            )
+            return HTML(iframe)
+        else:
+            # Render HTML regularly.
+            return HTML(doc)
 
     def save(self, output, **kwargs):
-        """Render and save the grid in an HTML document"""
+        """Render and save the grid in an HTML document."""
         with open(output, "w", encoding="utf-8") as f:
             f.write(self.render(**kwargs))
```

### Comparing `mols2grid-1.1.1/mols2grid/select.py` & `mols2grid-2.0.0rc1/mols2grid/select.py`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/mols2grid/utils.py` & `mols2grid-2.0.0rc1/mols2grid/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,20 +46,20 @@
     transform : dict
         Functions applied to each value before rendering
     """
     items = []
     for k, v in s[subset].to_dict().items():
         displayed = transform[k](v) if transform.get(k) else v
         v = (
-            f'<span style="{style[k](v)}">{displayed}</span>'
+            f'<span class="copy-me" style="{style[k](v)}">{displayed}</span>'
             if style.get(k)
-            else displayed
+            else f'<span class="copy-me">{displayed}</span>'
         )
         items.append(fmt.format(key=k, value=v))
-    return "<br>".join(items)
+    return '<br>'.join(items)
 
 
 def mol_to_smiles(mol):
     """Returns a SMILES from an RDKit molecule, or None if not an RDKit mol"""
     return Chem.MolToSmiles(mol) if mol else None
 
 
@@ -85,15 +85,16 @@
     """
     if str(sdf_path).endswith(".gz"):
         read_file = gzip.open
     else:
         read_file = partial(open, mode="rb")
     with read_file(sdf_path) as f:
         return pd.DataFrame(
-            [mol_to_record(mol, mol_col) for mol in Chem.ForwardSDMolSupplier(f)]
+            [mol_to_record(mol, mol_col)
+             for mol in Chem.ForwardSDMolSupplier(f)]
         )
 
 
 def remove_coordinates(mol):
     """Removes the existing coordinates from the molecule. The molecule is
     modified inplace"""
     mol.RemoveAllConformers()
```

### Comparing `mols2grid-1.1.1/mols2grid/labextension/package.json` & `mols2grid-2.0.0rc1/mols2grid/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9660993303571429%*

 * *Differences: {"'devDependencies'": "{'eslint-config-prettier': '^8.8.0', 'eslint-plugin-prettier': '^4.2.1', "*

 * *                      "'prettier': '^2.8.8'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.791f11d71f83b76ea703.js'}}",*

 * * "'version'": "'2.0.0-rc1'"}*

```diff
@@ -19,22 +19,22 @@
         "@types/jest": "^26.0.0",
         "@types/webpack-env": "^1.13.6",
         "@typescript-eslint/eslint-plugin": "^3.6.0",
         "@typescript-eslint/parser": "^3.6.0",
         "acorn": "^7.2.0",
         "css-loader": "^3.2.0",
         "eslint": "^7.4.0",
-        "eslint-config-prettier": "^6.11.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^4.2.1",
         "fs-extra": "^7.0.0",
         "identity-obj-proxy": "^3.0.0",
         "jest": "^26.0.0",
         "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
-        "prettier": "^2.0.5",
+        "prettier": "^2.8.8",
         "rimraf": "^2.6.2",
         "source-map-loader": "^1.1.3",
         "style-loader": "^1.0.0",
         "ts-jest": "^26.0.0",
         "ts-loader": "^8.0.0",
         "typescript": "~4.1.3",
         "webpack": "^5.61.0",
@@ -48,15 +48,15 @@
         "dist/*.map",
         "css/*.css"
     ],
     "homepage": "https://github.com/cbouy/mols2grid",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a2b2bff7fec77dbdfc67.js"
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
-    "version": "1.1.1"
+    "version": "2.0.0-rc1"
 }
```

### Comparing `mols2grid-1.1.1/mols2grid/labextension/static/480.b793e9ee0cf0bcedd405.js` & `mols2grid-2.0.0rc1/mols2grid/labextension/static/480.a99394933b0f23a624ab.js`

 * *Files 2% similar despite different names*

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
-            e.exports = JSON.parse('{"name":"mols2grid","version":"1.1.1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0-rc1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `mols2grid-1.1.1/mols2grid/labextension/static/568.dfe2d319c495ee9c8bd8.js` & `mols2grid-2.0.0rc1/mols2grid/labextension/static/568.d44a1a2f4790f58ec0e3.js`

 * *Files 2% similar despite different names*

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
-            e.exports = JSON.parse('{"name":"mols2grid","version":"1.1.1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0-rc1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `mols2grid-1.1.1/mols2grid/labextension/static/remoteEntry.a2b2bff7fec77dbdfc67.js` & `mols2grid-2.0.0rc1/mols2grid/labextension/static/remoteEntry.791f11d71f83b76ea703.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, l, s, u, f, d, c, p, h, v = {
+    var e, r, t, n, o, i, a, l, s, u, f, d, c, p, h, v, g = {
             53: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(829), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(829), t.e(480)]).then((() => () => t(480)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -20,103 +20,104 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => i
                 })
             }
         },
-        g = {};
+        m = {};
 
-    function m(e) {
-        var r = g[e];
+    function b(e) {
+        var r = m[e];
         if (void 0 !== r) return r.exports;
-        var t = g[e] = {
+        var t = m[e] = {
             id: e,
             exports: {}
         };
-        return v[e].call(t.exports, t, t.exports, m), t.exports
+        return g[e].call(t.exports, t, t.exports, b), t.exports
     }
-    m.m = v, m.c = g, m.d = (e, r) => {
-        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
+    b.m = g, b.c = m, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        480: "b793e9ee0cf0bcedd405",
-        568: "dfe2d319c495ee9c8bd8",
-        829: "a7028e64d0c8c91f54e1"
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
+        480: "a99394933b0f23a624ab",
+        568: "d44a1a2f4790f58ec0e3",
+        829: "d620f53947100b9acdd6"
     } [e] + ".js?v=" + {
-        480: "b793e9ee0cf0bcedd405",
-        568: "dfe2d319c495ee9c8bd8",
-        829: "a7028e64d0c8c91f54e1"
-    } [e], m.g = function() {
+        480: "a99394933b0f23a624ab",
+        568: "d44a1a2f4790f58ec0e3",
+        829: "d620f53947100b9acdd6"
+    } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "mols2grid:", m.l = (t, n, o, i) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "mols2grid:", b.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
             var a, l;
             if (void 0 !== o)
                 for (var s = document.getElementsByTagName("script"), u = 0; u < s.length; u++) {
                     var f = s[u];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         a = f;
                         break
                     }
                 }
-            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, b.nc && a.setAttribute("nonce", b.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var d = (r, n) => {
                     a.onerror = a.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, (() => {
-        m.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        m.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                m.o(m.S, t) || (m.S[t] = {});
-                var i = m.S[t],
+                b.o(b.S, t) || (b.S[t] = {});
+                var i = b.S[t],
                     a = "mols2grid",
                     l = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = i[e] = i[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (o[r] = {
-                        get: () => Promise.all([m.e(829), m.e(568)]).then((() => () => m(568))),
+                        get: () => Promise.all([b.e(829), b.e(568)]).then((() => () => b(568))),
                         from: a,
                         eager: !1
                     })
-                })("mols2grid", "1.1.1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("mols2grid", "2.0.0-rc1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        m.g.importScripts && (e = m.g.location + "");
-        var r = m.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
-            t.length && (e = t[t.length - 1].src)
+            if (t.length)
+                for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -182,86 +183,88 @@
             p = c.pop.bind(c);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
         return !!p()
     }, a = (e, r) => {
-        var t = m.S[e];
-        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", u = (e, r, t, n) => {
         var o = l(e, t);
-        return i(n, o) || "undefined" != typeof console && console.warn && console.warn(s(e, t, o, n)), f(e[t][o])
-    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
-        var i = m.I(r);
-        return i && i.then ? i.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), c = {}, p = {
-        829: () => d("default", "@jupyter-widgets/base", [, [1, 6],
+        return i(n, o) || f(s(e, t, o, n)), d(e[t][o])
+    }, f = e => {
+        "undefined" != typeof console && console.warn && console.warn(e)
+    }, d = e => (e.loaded = 1, e.get()), c = (e => function(r, t, n, o) {
+        var i = b.I(r);
+        return i && i.then ? i.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), p = {}, h = {
+        829: () => c("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
         ])
-    }, h = {
+    }, v = {
         829: [829]
-    }, m.f.consumes = (e, r) => {
-        m.o(h, e) && h[e].forEach((e => {
-            if (m.o(c, e)) return r.push(c[e]);
+    }, b.f.consumes = (e, r) => {
+        b.o(v, e) && v[e].forEach((e => {
+            if (b.o(p, e)) return r.push(p[e]);
             var t = r => {
-                    c[e] = 0, m.m[e] = t => {
-                        delete m.c[e], t.exports = r()
+                    p[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], m.m[e] = t => {
-                        throw delete m.c[e], r
+                    delete p[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
-                var o = p[e]();
-                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                var o = h[e]();
+                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             848: 0
         };
-        m.f.j = (r, t) => {
-            var n = m.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (829 != r) {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
-                var i = m.p + m.u(r),
+                var i = b.p + b.u(r),
                     a = new Error;
-                m.l(i, (t => {
-                    if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                b.l(i, (t => {
+                    if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
                             i = t && t.target && t.target.src;
                         a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
                 var n, o, [i, a, l] = t,
                     s = 0;
                 if (i.some((r => 0 !== e[r]))) {
-                    for (n in a) m.o(a, n) && (m.m[n] = a[n]);
-                    l && l(m)
+                    for (n in a) b.o(a, n) && (b.m[n] = a[n]);
+                    l && l(b)
                 }
-                for (r && r(t); s < i.length; s++) o = i[s], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); s < i.length; s++) o = i[s], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkmols2grid = self.webpackChunkmols2grid || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), m.nc = void 0;
-    var b = m(53);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).mols2grid = b
+    })(), b.nc = void 0;
+    var w = b(53);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).mols2grid = w
 })();
```

### Comparing `mols2grid-1.1.1/mols2grid/labextension/static/third-party-licenses.json` & `mols2grid-2.0.0rc1/mols2grid/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/mols2grid/nbextension/index.js` & `mols2grid-2.0.0rc1/mols2grid/nbextension/index.js`

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
-                e.exports = JSON.parse('{"name":"mols2grid","version":"1.1.1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                e.exports = JSON.parse('{"name":"mols2grid","version":"2.0.0-rc1","description":"Custom widget for the Python mols2grid package","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","dist/*.map","css/*.css"],"homepage":"https://github.com/cbouy/mols2grid","bugs":{"url":"https://github.com/cbouy/mols2grid/issues"},"license":"Apache-2.0","author":{"name":"Cedric Bouysset","email":"cedric@bouysset.net"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/cbouy/mols2grid"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf mols2grid/labextension","clean:nbextension":"rimraf mols2grid/nbextension/static/index.js","prepack":"yarn run build:lib","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^8.8.0","eslint-plugin-prettier":"^4.2.1","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.8","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"mols2grid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         n = {};
 
     function i(e) {
         var r = n[e];
         if (void 0 !== r) return r.exports;
```

### Comparing `mols2grid-1.1.1/mols2grid/nbextension/index.js.map` & `mols2grid-2.0.0rc1/mols2grid/nbextension/index.js.map`

 * *Files 1% similar despite different names*

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

### Comparing `mols2grid-1.1.1/mols2grid/templates/js/draw_mol.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/draw_mol.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-// generate images for the currently displayed molecules
+// Generate images for the currently displayed molecules.
 RDKit.prefer_coordgen({
     {
         prefer_coordGen | tojson
     }
 });
 
 function draw_mol(smiles, index, template_mol) {
@@ -21,33 +21,35 @@
         } else {
             var details = json_draw_opts;
         }
         svg = mol.get_svg_with_highlights(details);
     }
     mol.delete();
     if (svg == "") {
-        return '<svg width="{{ cell_width }}" height="{{ height }}" xmlns="http://www.w3.org/2000/svg" version="1.1" viewBox="0 0 {{ cell_width }} {{ height }}"></svg>';
+        return '<svg width="{{ image_width }}" height="{{ image_height }}" xmlns="http://www.w3.org/2000/svg" version="1.1" viewBox="0 0 {{ image_width }} {{ image_height }}"></svg>';
     }
     return svg;
 }
+
+// Update images when the list is updated.
 listObj.on("updated", function(list) {
-    var query = $('#mols2grid #searchbar').val();
+    var query = $('#mols2grid .m2g-searchbar').val();
     var template_mol;
     if (query === "") {
         smarts_matches = {};
         template_mol = null;
     } else {
         template_mol = RDKit.get_qmol(query);
         template_mol.set_new_coords({
             {
                 prefer_coordGen | tojson
             }
         });
     }
-    $('#mols2grid .cell').each(function() {
+    $('#mols2grid .m2g-cell').each(function() {
         var $t = $(this);
         var smiles = $t.children(".data-{{ smiles_col }}").first().text();
         var index = parseInt(this.getAttribute("data-mols2grid-id"));
         var svg = draw_mol(smiles, index, template_mol);
         $t.children(".data-img").html(svg);
     });
     if (template_mol) {
```

### Comparing `mols2grid-1.1.1/mols2grid/templates/js/kernel.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/kernel.js`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/mols2grid/templates/js/molstorage.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/molstorage.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,35 +1,54 @@
 class MolStorage extends Map {
     multi_set(_id, _smiles) {
         for (let i = 0; i < _id.length; i++) {
-            this.set(_id[i], _smiles[i]);
+            this.set(_id[i], _smiles[i])
         }
     }
     multi_del(_id) {
         for (let i = 0; i < _id.length; i++) {
-            this.delete(_id[i]);
-        };
+            this.delete(_id[i])
+        }
     }
     to_dict() {
-        var content = "{";
+        var content = '{'
         for (let [key, value] of this) {
-            content += key + ":" + JSON.stringify(value) + ",";
+            content += key + ':' + JSON.stringify(value) + ','
         }
-        content = content.length > 1 ? content.slice(0, -1) : content;
-        content += "}";
+        content = content.length > 1 ? content.slice(0, -1) : content
+        content += '}'
         return content
     }
-    download_smi(fileName) {
-        var content = "";
-        for (let [key, value] of this) {
-            content += value + " " + key + "\n";
+    to_keys() {
+        var content = []
+        for (let [key] of this) {
+            content.push(key)
+        }
+        return content
+    }
+    download_smi(fileName, allItems) {
+        var content = ''
+
+        if (allItems) {
+            // Gather all smiles
+            for (var item of allItems) {
+                var smiles = item.values()['data-SMILES']
+                var id = item.values()['mols2grid-id']
+                content += smiles + ' ' + id + '\n'
+            }
+        } else {
+            // Gather selected smiles
+            for (let [key, value] of this) {
+                content += value + ' ' + key + '\n'
+            }
         }
-        var a = document.createElement("a");
+
+        var a = document.createElement('a')
         var file = new Blob([content], {
-            type: "text/plain"
-        });
-        a.href = URL.createObjectURL(file);
-        a.download = fileName;
-        a.click();
-        a.remove();
+            type: 'text/plain'
+        })
+        a.href = URL.createObjectURL(file)
+        a.download = fileName
+        a.click()
+        a.remove()
     }
 }
```

### Comparing `mols2grid-1.1.1/mols2grid/templates/js/pages.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/interactive.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,10 @@
 // list.js
 var listObj = new List('mols2grid', {
+    listClass: 'm2g-list',
     valueNames: {
         {
             value_names
         }
     },
     item: {
         {
@@ -12,26 +13,28 @@
     },
     page: {
         {
             n_items_per_page
         }
     },
     pagination: {
-        name: "pagination",
+        paginationClass: "m2g-pagination",
         item: '<li class="page-item"><a class="page page-link" href="#" onclick="event.preventDefault()"></a></li>',
         innerWindow: 1,
         outerWindow: 1,
     },
 });
 listObj.remove("mols2grid-id", "0");
 listObj.add({
     {
         data
     }
 });
+
+
 // filter
 if (window.parent.mols2grid_lists === undefined) {
     window.parent.mols2grid_lists = {};
 }
 window.parent.mols2grid_lists[{
     {
         grid_id | tojson
@@ -72,15 +75,15 @@
     }
 }, {
     {
         cached_selection[1]
     }
 });
 listObj.on("updated", function(list) {
-    $('#mols2grid .cell input[checked="false"]').prop("checked", false);
+    $('#mols2grid .m2g-cell input[checked="false"]').prop("checked", false);
 }); {
     % endif %
 }
 
 // sort
 {
     % include 'js/sort.js' %
@@ -88,15 +91,15 @@
 
 {
     %
     if whole_cell_style %
 }
 // add style for whole cell
 listObj.on("updated", function(list) {
-    $('#mols2grid div.cell').each(function() {
+    $('#mols2grid div.m2g-cell').each(function() {
         var $t = $(this);
         $t.attr({
                 style: $t.attr('data-cellstyle')
             })
             .removeAttr('data-cellstyle');
     });
 }); {
@@ -107,58 +110,37 @@
     %
     if tooltip %
 }
 // tooltips
 $.fn.tooltip.Constructor.Default.whiteList.span = ['style']
 listObj.on("updated", function(list) {
     $(function() {
-        // hide previous popovers
+        // Hide previous popovers.
         $('#mols2grid a.page-link').click(function(e) {
-            $('.mols2grid-tooltip[data-toggle="popover"]').popover('hide')
+            $('.m2g-tooltip[data-toggle="popover"]').popover('hide')
         });
-        // create new popover
-        $('.mols2grid-tooltip[data-toggle="popover"]').popover({
+        // Create new popover.
+        $('.m2g-tooltip[data-toggle="popover"]').popover({
             placement: {
                 {
                     tooltip_placement
                 }
             },
-            trigger: {
-                {
-                    tooltip_trigger
-                }
-            },
+            trigger: 'manual',
             html: true,
             sanitize: false,
         });
     })
 }); {
     % endif %
 }
 
+// grid interactions (select, click, tooltip, key events)
 {
-    %
-    if selection %
-}
-// selection modifyers and export options
-{
-    % include 'js/selection_actions.js' %
-} {
-    % endif %
-}
-
-{
-    %
-    if callback %
-}
-// callback
-{
-    % include 'js/callback.js' %
-} {
-    % endif %
+    % include 'js/grid_interaction.js' %
 }
 
 {
     %
     if onthefly %
 }
 // generate images for the currently displayed molecules
@@ -176,28 +158,27 @@
 window
     .initRDKitModule()
     .then(function(RDKit) {
         console.log('RDKit version: ', RDKit.version());
         window.RDKit = RDKit;
         window.RDKitModule = RDKit;
 
-        // search bar
+        // Searchbar
         {
             % include 'js/search.js' %
         }
 
         {
             %
             if onthefly %
         } {
             % include 'js/draw_mol.js' %
         } {
             % endif %
         }
 
-        // trigger update to activate tooltips, draw images, setup callbacks...
+        // Trigger update to activate tooltips, draw images, setup callbacks...
         listObj.update();
-        // resize iframe to fit content
-        if (window.frameElement) {
-            fit_height(window.frameElement);
-        }
+
+        // Set iframe height to fit content.
+        fitIframe(window.frameElement);
     });
```

### Comparing `mols2grid-1.1.1/mols2grid/templates/js/search.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/search.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 function SmartsSearch(query, columns) {
     var smiles_col = columns[0];
     smarts_matches = {};
-    var query = $('#mols2grid #searchbar').val();
+    var query = $('#mols2grid .m2g-searchbar').val();
     var qmol = RDKit.get_qmol(query);
     if (qmol.is_valid()) {
         listObj.items.forEach(function(item) {
             var smiles = item.values()[smiles_col]
             var mol = RDKit.get_mol(smiles, '{"removeHs": {{ removeHs | tojson }} }');
             if (mol.is_valid()) {
                 var results = mol.get_substruct_matches(qmol);
@@ -63,22 +63,24 @@
                 return ''
             }
             return this
         }
         return _super.apply(this, arguments);
     };
 })(String.prototype.replace);
+
 // Switch search type (Text or SMARTS)
-$('#mols2grid .search-btn').click(function() {
+$('#mols2grid .m2g-search-options .m2g-option').click(function() {
     search_type = $(this).text();
-    $('#mols2grid button.search-btn.active').removeClass("active");
-    $(this).addClass("active");
+    $('#mols2grid .m2g-search-options .m2g-option.sel').removeClass("sel");
+    $(this).addClass("sel");
 });
+
 // Searchbar update event handler
-$('#mols2grid #searchbar').on("keyup", function(e) {
+$('#mols2grid .m2g-searchbar').on("keyup", function(e) {
     var query = e.target.value;
     if (search_type === "Text") {
         smarts_matches = {};
         listObj.search(query, {
             {
                 search_cols
             }
```

### Comparing `mols2grid-1.1.1/mols2grid/templates/js/sort.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/sort.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,64 +1,78 @@
-var sort_field = "{{ sort_by }}";
-var sort_order = "asc";
+var sortField = '{{ sort_by }}'
+var sortOrder = 'asc'
+
+// Sort dropdown
+$('#mols2grid .m2g-sort select').change(sort)
+
+// Sort order
+$('#mols2grid .m2g-order').click(flipSort)
+
+function sort(e) {
+    if (e) {
+        sortField = e.target.value
+        var selectedOption = e.target.options[e.target.selectedIndex]
+        var sortFieldDisplay = selectedOption.text
+    }
+
+    // Sort
+    if (sortField == 'checkbox') {
+        listObj.sort('mols2grid-id', {
+            order: sortOrder,
+            sortFunction: checkboxSort
+        })
+    } else {
+        listObj.sort(sortField, {
+            order: sortOrder,
+            sortFunction: mols2gridSortFunction
+        })
+    }
+
+    // Update UI.
+    $(this).parent().find('.m2g-display').text(sortFieldDisplay)
+}
+
+// prettier-ignore
+function flipSort() {
+    $(this).parent().removeClass('m2d-arrow-' + sortOrder)
+    sortOrder = sortOrder === 'desc' ? 'asc' : 'desc'
+    $(this).parent().addClass('m2d-arrow-' + sortOrder)
+    sort()
+}
 
 function mols2gridSortFunction(itemA, itemB, options) {
-    var x = itemA.values()[options.valueName];
-    var y = itemB.values()[options.valueName];
-    if (typeof x === "number") {
+    var x = itemA.values()[options.valueName]
+    var y = itemB.values()[options.valueName]
+    if (typeof x === 'number') {
         if (isFinite(x - y)) {
-            return x - y;
+            return x - y
         } else {
-            return isFinite(x) ? -1 : 1;
+            return isFinite(x) ? -1 : 1
         }
     } else {
-        x = x.toLowerCase();
-        y = y.toLowerCase();
-        return (x < y) ? -1 : (x > y) ? 1 : 0;
+        x = x ? x.toLowerCase() : x
+        y = y ? y.toLowerCase() : y
+        return x < y ? -1 : x > y ? 1 : 0
     }
 }
 
 function checkboxSort(itemA, itemB, options) {
     if (itemA.elm !== undefined) {
-        var checkedA = itemA.elm.firstChild.checked;
+        var checkedA = itemA.elm.querySelector('input[type=checkbox]').checked
         if (itemB.elm !== undefined) {
-            var checkedB = itemB.elm.firstChild.checked;
+            var checkedB = itemB.elm.querySelector('input[type=checkbox]').checked
             if (checkedA && !checkedB) {
-                return -1;
+                return -1
             } else if (!checkedA && checkedB) {
-                return 1;
+                return 1
             } else {
-                return 0;
+                return 0
             }
         } else {
-            return -1;
+            return -1
         }
     } else if (itemB.elm !== undefined) {
-        return 1;
-    } else {
-        return 0;
-    }
-}
-$('#mols2grid button.sort-btn').click(function(e) {
-    var _field = $(this).attr("data-name");
-    if (_field == sort_field) {
-        $(this).removeClass("arrow-" + sort_order)
-        sort_order = (sort_order === "desc") ? "asc" : "desc";
+        return 1
     } else {
-        $('#mols2grid button.sort-btn.active').removeClass("active arrow-" + sort_order);
-        sort_order = "asc";
-        sort_field = _field;
-        $(this).addClass("active");
-    }
-    $(this).addClass("arrow-" + sort_order)
-    if (sort_field == "checkbox") {
-        listObj.sort("mols2grid-id", {
-            order: sort_order,
-            sortFunction: checkboxSort
-        });
-    } else {
-        listObj.sort(_field, {
-            order: sort_order,
-            sortFunction: mols2gridSortFunction
-        });
+        return 0
     }
-});
+}
```

### Comparing `mols2grid-1.1.1/mols2grid/templates/js/callbacks/show_3d.js` & `mols2grid-2.0.0rc1/mols2grid/templates/js/callbacks/show_3d.js`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/mols2grid/widget/__init__.py` & `mols2grid-2.0.0rc1/mols2grid/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/mols2grid/widget/widget.py` & `mols2grid-2.0.0rc1/mols2grid/widget/widget.py`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/src/extension.ts` & `mols2grid-2.0.0rc1/src/extension.ts`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/src/plugin.ts` & `mols2grid-2.0.0rc1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/src/version.ts` & `mols2grid-2.0.0rc1/src/version.ts`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/src/widget.ts` & `mols2grid-2.0.0rc1/src/widget.ts`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/tests/conftest.py` & `mols2grid-2.0.0rc1/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,13 +34,13 @@
 @pytest.fixture(scope="module")
 def grid_prerendered(df):
     return MolGrid(df, mol_col="mol", prerender=True)
 
 
 @pytest.fixture(scope="module")
 def grid(df):
-    return MolGrid(df, mol_col="mol")
+    return MolGrid(df, mol_col="mol", size=(160, 120))
 
 
 @pytest.fixture(scope="module")
 def mols(small_df):
     return small_df["mol"]
```

### Comparing `mols2grid-1.1.1/tests/test_callbacks.py` & `mols2grid-2.0.0rc1/tests/test_callbacks.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 from mols2grid import callbacks
 
 
 def test_make_popup_callback():
     popup = callbacks.make_popup_callback(
         title="${title}",
+        subtitle="${title}",
+        svg="<svg><rect width='10' height='10'/></svg>",
         html='<span id="foo">${title}</span>',
         js='var title = "FOOBAR";',
         style="max-width: 42%;",
     )
-    assert '<h5 class="modal-title">${title}</h5>' in popup
+    assert '<h2>${title}</h2>' in popup
+    assert '<p>${title}</p>' in popup
     assert '<span id="foo">${title}</span>' in popup
-    assert '// prerequisite JavaScript code\nvar title = "FOOBAR";' in popup
-    assert '<div class="modal-dialog" style="max-width: 42%;">' in popup
+    assert '// Prerequisite JavaScript code.\n// prettier-ignore\nvar title = "FOOBAR";' in popup
+    assert '<div id="m2g-modal" tabindex="-1" style="max-width: 42%;">' in popup
 
 
 @pytest.mark.parametrize(
     "title, expected",
     [
         ("SMILES", "${data['SMILES']}"),
         (None, None),
```

### Comparing `mols2grid-1.1.1/tests/test_interface.py` & `mols2grid-2.0.0rc1/tests/test_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 import json
 import os
+import sys
 from base64 import b64encode
 from datetime import datetime, timezone
 from pathlib import Path
 from types import SimpleNamespace
 
-import geckodriver_autoinstaller
 import imagehash
+import pyautogecko
 import pytest
 from flaky import flaky
 from rdkit import Chem
 from rdkit import __version__ as rdkit_version
 from rdkit.Chem import AllChem
 from selenium import webdriver
-from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions as EC
 
 import mols2grid
 from mols2grid.select import register
 from mols2grid.utils import env
 
 from .webdriver_utils import FirefoxDriver
 
-geckodriver_autoinstaller.install()
-pytestmark = pytest.mark.webdriver
-GITHUB_ACTIONS = os.environ.get("GITHUB_ACTIONS")
+try:
+    from rdkit.Chem.rdDepictor import IsCoordGenSupportAvailable
+except ImportError:
+    COORDGEN_SUPPORT = not sys.platform.startswith("win")
+else:
+    COORDGEN_SUPPORT = IsCoordGenSupportAvailable()
+
+# for local debug, switch headless mode to False
 HEADLESS = True
+
+pytestmark = pytest.mark.webdriver
+GITHUB_ACTIONS = bool(os.environ.get("GITHUB_ACTIONS"))
 PAGE_LOAD_TIMEOUT = 10
+skip_no_coordgen = pytest.mark.skipif(
+    not COORDGEN_SUPPORT,
+    reason="CoordGen library not available in this RDKit build",
+)
+pyautogecko.install()
 
 
 def determine_scope(fixture_name, config):
     if GITHUB_ACTIONS:
         return "function"
     return "module"
 
@@ -57,52 +69,59 @@
     driver.set_page_load_timeout(PAGE_LOAD_TIMEOUT)
     yield driver
     driver.quit()
 
 
 @pytest.fixture(scope="module")
 def html_doc(grid):
-    return get_doc(grid, dict(n_rows=1, subset=["_Name", "img"]))
+    return get_doc(
+        grid,
+        dict(
+            n_items_per_page=5,
+            subset=["_Name", "img"],
+            size=(160, 120),
+        ),
+    )
 
 
 # make sure non-parametrized test is ran first
 @pytest.mark.order(1)
 def test_no_subset_all_visible(driver: FirefoxDriver, grid):
     doc = get_doc(grid, {"tooltip": [], "selection": False})
     driver.get(doc)
-    columns = set(grid.dataframe.columns.drop("mol").to_list())
-    cell = driver.find_by_css_selector("#mols2grid .cell")
-    data_el = cell.find_elements_by_class_name("data")
+    columns = set(grid.dataframe.columns.drop(["mol", "mols2grid-id"]).to_list())
+    cell = driver.find_by_css_selector("#mols2grid .m2g-cell")
+    data_el = cell.find_elements(By.CLASS_NAME, "data")
     classes = [
-        c.replace("data-", "").replace("-copy", "")
+        c.replace("data-", "").replace("-display", "")
         for x in data_el
         for c in x.get_attribute("class").split(" ")
         if c.startswith("data-")
     ]
     classes = set(classes)
     assert classes == columns
 
 
 def test_smiles_hidden(driver: FirefoxDriver, html_doc):
     driver.get(html_doc)
-    el = driver.find_by_css_selector("#mols2grid .cell .data-SMILES")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-SMILES")
     assert not el.is_displayed()
 
 
 @pytest.mark.parametrize("page", [1, 2, 3])
 def test_page_click(driver: FirefoxDriver, grid, page):
-    doc = get_doc(grid, dict(subset=["img", "_Name"], n_cols=3, n_rows=3))
+    doc = get_doc(grid, dict(subset=["img", "_Name"], n_items_per_page=9))
     driver.get(doc)
     for i in range(2, page + 1):
         driver.wait_for_img_load()
         next_page = driver.find_by_css_selector(f'a.page-link[data-i="{i}"]')
         next_page.click()
-    first_cell = driver.find_by_class_name("cell")
+    first_cell = driver.find_by_class_name("m2g-cell")
     mols2grid_id = 9 * (page - 1)
-    name = first_cell.find_element_by_class_name("data-_Name")
+    name = first_cell.find_element(By.CLASS_NAME, "data-_Name")
     ref = grid.dataframe.iloc[mols2grid_id]
     assert name.text == ref["_Name"]
 
 
 @pytest.mark.parametrize(
     ["name", "css_prop", "value", "expected"],
     [
@@ -112,167 +131,177 @@
         ("border", "border-top-color", "1px solid blue", "rgb(0, 0, 255)"),
         ("fontsize", "font-size", "16pt", "21.3333px"),
         ("fontfamily", "font-family", "Consolas", "Consolas"),
         ("textalign", "text-align", "right", "right"),
         (
             "custom_css",
             "background-color",
-            ".cell { background-color: black; }",
+            "#mols2grid .m2g-cell { background-color: black; }",
             "rgb(0, 0, 0)",
         ),
     ],
 )
 def test_css_properties(driver: FirefoxDriver, grid, name, css_prop, value, expected):
     doc = get_doc(grid, {name: value})
     driver.get(doc)
     computed = driver.execute_script(
-        f"return getComputedStyle(document.querySelector('#mols2grid .cell')).getPropertyValue({css_prop!r});"
+        f"""return getComputedStyle(
+            document.querySelector('#mols2grid .m2g-cell')
+        ).getPropertyValue({css_prop!r});
+        """
     )
     assert computed == expected
 
 
 def test_text_search(driver: FirefoxDriver, html_doc):
     driver.get(html_doc)
     driver.wait_for_img_load()
     driver.text_search("iodopropane")
-    el = driver.find_by_css_selector("#mols2grid .cell .data-SMILES")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-SMILES")
     assert el.get_attribute("innerHTML") == "CC(I)C"
 
 
 def test_text_search_regex_chars(driver: FirefoxDriver, html_doc):
     driver.get(html_doc)
     driver.wait_for_img_load()
     driver.text_search("1-pentene")
-    el = driver.find_by_css_selector("#mols2grid .cell .data-SMILES")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-SMILES")
     assert el.get_attribute("innerHTML") == "CCCC=C"
 
 
 @flaky(max_runs=3, min_passes=1)
 def test_smarts_search(driver: FirefoxDriver, html_doc):
     driver.get(html_doc)
     driver.wait_for_img_load()
     driver.substructure_query("CC(I)C")
-    el = driver.find_by_css_selector("#mols2grid .cell .data-_Name")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-_Name")
     assert el.text == "2-iodopropane"
 
 
 def test_selection_click(driver: FirefoxDriver, html_doc):
     driver.get(html_doc)
     driver.wait_for_img_load()
-    driver.find_clickable(By.CSS_SELECTOR, "input[type='checkbox']").click()
-    sel = driver.wait_for_selection(is_empty=False)
+    sel = driver.click_checkbox()
     assert sel == {0: "CCC(C)CC"}
     register._clear()
 
 
 def test_export_csv(driver: FirefoxDriver, html_doc):
+    sep = ";"
     driver.get(html_doc)
     driver.wait_for_img_load()
-    driver.find_clickable(By.CSS_SELECTOR, "input[type='checkbox']").click()
-    driver.wait_for_selection(is_empty=False)
-    driver.find_clickable(By.ID, "sortDropdown").click()
-    driver.find_clickable(
-        By.CSS_SELECTOR, 'button.sort-btn[data-name="data-_Name"]'
-    ).click()
-    driver.wait_for_img_load()
-    driver.find_clickable(By.ID, "chkboxDropdown").click()
+    driver.click_checkbox()
+    driver.sort_grid("_Name")
     now = datetime.now(tz=timezone.utc)
-    driver.find_clickable(By.ID, "btn-chkbox-dlcsv").click()
+    driver.grid_action("save-csv")
     csv_files = sorted(
         (Path.home() / "Downloads").glob("selection*.csv"),
         key=lambda x: x.stat().st_mtime,
     )
     csv_file = csv_files[-1]
     file_mtime = datetime.fromtimestamp(csv_file.stat().st_mtime, tz=timezone.utc)
     assert (file_mtime - now).seconds < 1, "Could not find recent selection file"
     content = csv_file.read_text()
-    assert content == "index\t_Name\tSMILES\n0\t3-methylpentane\tCCC(C)CC\n"
+    expected = (
+        sep.join(("index", "_Name", "SMILES"))
+        + "\n"
+        + sep.join(("0", "3-methylpentane", "CCC(C)CC"))
+        + "\n"
+    )
+    assert content == expected
     csv_file.unlink()
     register._clear()
 
 
 def test_selection_with_cache_check_and_uncheck(driver: FirefoxDriver, df):
     register._init_grid("cached_sel")
     event = SimpleNamespace(new='{0: "CCC(C)CC"}')
     register.selection_updated("cached_sel", event)
     grid = get_grid(df, name="cached_sel", cache_selection=True)
     doc = get_doc(grid, {})
     driver.get(doc)
     driver.wait_for_img_load()
     sel = driver.wait_for_selection(is_empty=False)
     assert sel == {0: "CCC(C)CC"}
-    driver.find_clickable(By.CSS_SELECTOR, "input[type='checkbox']").click()
-    empty_sel = driver.wait_for_selection(is_empty=True)
+    empty_sel = driver.click_checkbox(is_empty=True)
     assert empty_sel is True
     register._clear()
 
 
 def test_selection_check_uncheck_invert(driver: FirefoxDriver, html_doc):
     driver.get(html_doc)
     driver.wait_for_img_load()
     # search
     driver.text_search("iodopropane")
     # check all
-    driver.find_clickable(By.ID, "chkboxDropdown").click()
-    driver.find_clickable(By.ID, "btn-chkbox-all").click()
+    driver.grid_action("select-all")
     sel = driver.wait_for_selection(is_empty=False)
     assert len(sel) == 30
     # uncheck all
-    driver.find_clickable(By.ID, "chkboxDropdown").click()
-    driver.find_clickable(By.ID, "btn-chkbox-none").click()
+    driver.grid_action("unselect-all")
     empty_sel = driver.wait_for_selection(is_empty=True)
     assert empty_sel is True
     # check matching
-    driver.find_clickable(By.ID, "chkboxDropdown").click()
-    driver.find_clickable(By.ID, "btn-chkbox-match").click()
+    driver.grid_action("select-matching")
     sel = driver.wait_for_selection(is_empty=False)
     assert sel == {27: "CC(I)C"}
     # invert
-    driver.find_clickable(By.ID, "chkboxDropdown").click()
-    driver.find_clickable(By.ID, "btn-chkbox-invert").click()
+    driver.grid_action("invert")
     sel = driver.wait_for_selection(is_empty=False)
     assert len(sel) == 29
     register._clear()
 
 
 @pytest.mark.parametrize("prerender", [True, False])
 def test_image_size(driver: FirefoxDriver, df, prerender):
-    grid = get_grid(df, size=(100, 100), prerender=prerender)
+    size = (200, 300)
+    grid = get_grid(df, size=size, prerender=prerender)
     doc = get_doc(
-        grid, {"selection": False, "border": "0", "substruct_highlight": False}
+        grid,
+        {
+            "selection": False,
+            "border": "0",
+            "substruct_highlight": False,
+            "n_items_per_page": 1,
+        },
     )
     driver.get(doc)
     if not prerender:
         driver.wait_for_img_load()
-    img = driver.find_by_css_selector("#mols2grid .cell .data-img *")
-    assert img.size == {"height": 100.0, "width": 100.0}
+    img = driver.find_by_css_selector("#mols2grid .m2g-cell .data-img *")
+    assert img.size == {"width": size[0], "height": size[1]}
 
 
 def test_image_use_coords(driver: FirefoxDriver, df):
     mols = df["mol"][:1]
     AllChem.EmbedMolecule(mols[0], randomSeed=0xF00D)
     grid = mols2grid.MolGrid.from_mols(
-        mols, use_coords=True, prerender=True, useSVG=False
+        mols,
+        use_coords=True,
+        prerender=True,
+        useSVG=False,
+        size=(160, 120),
     )
     doc = get_doc(grid, {"substruct_highlight": False})
     driver.get(doc)
     hash_ = driver.get_png_hash()
     diff = hash_ - imagehash.hex_to_hash(
         "ffffffffff7fff7ffe7ffe7ffe7ffe7ffe7fe07fc33f0fbc3f80ffc7ffffffff"
     )
     assert diff <= 2
 
 
 @pytest.mark.parametrize(
     ["coordGen", "prerender", "expected"],
     [
-        (
+        pytest.param(
             True,
             True,
             "fffffffffffffe7ffe7ffe7ffe7ffe7ffe7f3e7c8811c183e7e7ffffffffffff",
+            marks=skip_no_coordgen,
         ),
         (
             True,
             False,
             "fffffffffffffe7ffe7ffe7ffe7ffe7ffe7f3e7c8811c183e7e7ffffffffffff",
         ),
         (
@@ -286,43 +315,47 @@
             "ffffffff03fcf9fcfdf9fcf9fcfbfe03fe07fcfffcfffdfff9fffbffffffffff",
         ),
     ],
 )
 def test_coordgen(driver: FirefoxDriver, mols, coordGen, prerender, expected):
     useSVG = not prerender
     grid = mols2grid.MolGrid.from_mols(
-        mols, coordGen=coordGen, prerender=prerender, useSVG=useSVG, use_coords=False
+        mols,
+        coordGen=coordGen,
+        prerender=prerender,
+        useSVG=useSVG,
+        size=(160, 120),
+        use_coords=False,
     )
     doc = get_doc(grid, {"substruct_highlight": False})
     driver.get(doc)
     if not prerender:
         driver.wait_for_img_load()
-    if useSVG:
-        hash_ = driver.get_svg_hash()
-    else:
-        hash_ = driver.get_png_hash()
+    hash_ = driver.get_svg_hash() if useSVG else driver.get_png_hash()
     assert str(hash_) == expected
 
 
 @pytest.mark.parametrize(
     ["removeHs", "prerender", "expected"],
     [
-        (
+        pytest.param(
             True,
             True,
             "fffffffffffffe7ffe7ffe7ffe7ffe7ffe7f3e7c8811c183e7e7ffffffffffff",
+            marks=skip_no_coordgen,
         ),
-        (
+        pytest.param(
             False,
             True,
             (
                 "ffffff7fff3fffbff907e02fe13ff80fcbafe33fe033cb07fa4ffa4fff97ffd7"
                 if rdkit_version == "2020.03.1"
                 else "ff7ffe1ff91ffd3ff00ff0cffcbff0bff00ffd3fe1bff887f29ff30fff6fff7f"
             ),
+            marks=skip_no_coordgen,
         ),
         (
             True,
             False,
             "fffffffffffffe7ffe7ffe7ffe7ffe7ffe7f3e7c8811c183e7e7ffffffffffff",
         ),
         (
@@ -334,17 +367,22 @@
 )
 def test_removeHs(driver: FirefoxDriver, df, removeHs, prerender, expected):
     useSVG = not prerender
     mol = df["mol"][0]
     mol.ClearProp("SMILES")
     mols = [Chem.AddHs(mol)]
     grid = mols2grid.MolGrid.from_mols(
-        mols, removeHs=removeHs, prerender=prerender, useSVG=useSVG, use_coords=False
+        mols,
+        removeHs=removeHs,
+        prerender=prerender,
+        useSVG=useSVG,
+        size=(160, 120),
+        use_coords=False,
     )
-    doc = get_doc(grid, {"n_rows": 1, "substruct_highlight": False})
+    doc = get_doc(grid, {"n_items_per_page": 5, "substruct_highlight": False})
     driver.get(doc)
     if not prerender:
         driver.wait_for_img_load()
     if useSVG:
         hash_ = driver.get_svg_hash()
     else:
         hash_ = driver.get_png_hash()
@@ -372,96 +410,72 @@
         (
             dict(legend="foo"),
             "fffffffffffffe7ffe7ffe7ffe7ffe7f3e7c1818c183e7e7fffffffffe7ffe7f",
         ),
     ],
 )
 def test_moldrawoptions(driver: FirefoxDriver, df, kwargs, expected):
-    grid = get_grid(df, **kwargs)
-    doc = get_doc(grid, dict(n_rows=1, n_cols=1, subset=["img"]))
+    grid = get_grid(df, size=(160, 120), **kwargs)
+    doc = get_doc(grid, dict(n_items_per_page=1, subset=["img"]))
     driver.get(doc)
     driver.wait_for_img_load()
     hash_ = driver.get_svg_hash()
     assert str(hash_) == expected
 
 
+@pytest.mark.xfail(GITHUB_ACTIONS, reason="only seem to pass locally")
 def test_hover_color(driver: FirefoxDriver, grid):
-    doc = get_doc(grid, {"hover_color": "red"})
+    doc = get_doc(grid, {"hover_color": "rgba(255, 0, 0, 0.1)"})
     driver.get(doc)
     (
         ActionChains(driver)
-        .move_to_element(driver.find_by_css_selector("#mols2grid .cell"))
+        .move_to_element(driver.find_by_css_selector("#mols2grid .m2g-cell"))
+        .pause(0.2)
         .perform()
     )
     color = driver.execute_script(
-        f"return getComputedStyle(document.querySelector('#mols2grid .cell')).getPropertyValue('background-color');"
+        """
+        return getComputedStyle(
+            document.querySelector('#mols2grid .m2g-cell:hover'), ":after"
+        ).getPropertyValue('background-color');
+        """
     )
-    assert color == "rgb(255, 0, 0)"
+    assert color == "rgba(255, 0, 0, 0.1)"
 
 
 @flaky(max_runs=3, min_passes=1)
 def test_tooltip(driver: FirefoxDriver, grid):
     doc = get_doc(grid, {"tooltip": ["_Name"]})
     driver.get(doc)
     driver.wait_for_img_load()
-    (
-        ActionChains(driver)
-        .move_to_element(driver.find_by_css_selector("#mols2grid .cell .data-img *"))
-        .perform()
-    )
-    tooltip = driver.find_by_css_selector('div.popover[role="tooltip"]')
-    el = tooltip.find_element_by_class_name("popover-body")
-    assert el.get_attribute("innerHTML") == "<strong>_Name</strong>: 3-methylpentane"
-
-
-@flaky(max_runs=3, min_passes=1)
-def test_tooltip_trigger(driver: FirefoxDriver, grid):
-    doc = get_doc(grid, {"tooltip": ["_Name"], "tooltip_trigger": "click"})
-    driver.get(doc)
-    driver.wait_for_img_load()
-    (
-        ActionChains(driver)
-        .move_to_element(driver.find_by_css_selector("#mols2grid .cell .data-img *"))
-        .perform()
+    tooltip = driver.get_tooltip_content()
+    assert (
+        tooltip
+        == '<strong>_Name</strong>: <span class="copy-me">3-methylpentane</span>'
     )
-    with pytest.raises(NoSuchElementException):
-        driver.find_element_by_css_selector('div.popover[role="tooltip"]')
-    driver.find_clickable(By.CSS_SELECTOR, "#mols2grid .cell .data-img *").click()
-    tooltip = driver.find_by_css_selector('div.popover[role="tooltip"]')
-    el = tooltip.find_element_by_class_name("popover-body")
-    assert el.get_attribute("innerHTML") == "<strong>_Name</strong>: 3-methylpentane"
 
 
 @flaky(max_runs=3, min_passes=1)
 def test_tooltip_fmt(driver: FirefoxDriver, grid):
     doc = get_doc(grid, {"tooltip": ["_Name"], "tooltip_fmt": "<em>{value}</em>"})
     driver.get(doc)
     driver.wait_for_img_load()
-    (
-        ActionChains(driver)
-        .move_to_element(driver.find_by_css_selector("#mols2grid .cell .data-img *"))
-        .perform()
-    )
-    tooltip = driver.find_by_css_selector('div.popover[role="tooltip"]')
-    el = tooltip.find_element_by_class_name("popover-body")
-    assert el.get_attribute("innerHTML") == "<em>3-methylpentane</em>"
+    tooltip = driver.get_tooltip_content()
+    assert tooltip == '<em><span class="copy-me">3-methylpentane</span></em>'
 
 
 def test_tooltip_not_in_subset(driver: FirefoxDriver, grid):
     doc = get_doc(grid, {"tooltip": ["_Name"], "subset": ["ID", "img"]})
     driver.get(doc)
     driver.wait_for_img_load()
-    (
-        ActionChains(driver)
-        .move_to_element(driver.find_by_css_selector("#mols2grid .cell .data-img *"))
-        .perform()
+    tooltip = driver.get_tooltip_content()
+    assert (
+        tooltip
+        == '<strong>_Name</strong>: <span class="copy-me">3-methylpentane</span>'
     )
-    tooltip = driver.find_by_css_selector('div.popover[role="tooltip"]')
-    el = tooltip.find_element_by_class_name("popover-body")
-    assert el.get_attribute("innerHTML") == "<strong>_Name</strong>: 3-methylpentane"
 
 
 @flaky(max_runs=3, min_passes=1)
 def test_style(driver: FirefoxDriver, grid):
     doc = get_doc(
         grid,
         {
@@ -470,49 +484,39 @@
                 "__all__": lambda x: "color: red",
                 "_Name": lambda x: "color: blue",
             },
         },
     )
     driver.get(doc)
     driver.wait_for_img_load()
-    el = driver.find_by_css_selector("#mols2grid .cell")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell")
     assert el.value_of_css_property("color") == "rgb(255, 0, 0)"
-    el = driver.find_by_css_selector("#mols2grid .cell .data-_Name")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-_Name")
     assert el.value_of_css_property("color") == "rgb(0, 0, 255)"
-    (
-        ActionChains(driver)
-        .move_to_element(driver.find_by_css_selector("#mols2grid .cell .data-img *"))
-        .perform()
-    )
-    tooltip = driver.find_by_css_selector('div.popover[role="tooltip"]')
-    el = tooltip.find_element_by_class_name("popover-body")
+    tooltip = driver.get_tooltip_content()
     assert (
-        el.get_attribute("innerHTML")
-        == '<strong>_Name</strong>: <span style="color: blue">3-methylpentane</span>'
+        tooltip == '<strong>_Name</strong>: <span class="copy-me" '
+        'style="color: blue">3-methylpentane</span>'
     )
 
 
 @flaky(max_runs=3, min_passes=1)
 def test_transform(driver: FirefoxDriver, grid):
     doc = get_doc(
         grid, {"tooltip": ["_Name"], "transform": {"_Name": lambda x: x.upper()}}
     )
     driver.get(doc)
-    name = driver.find_by_css_selector("#mols2grid .cell .data-_Name")
+    name = driver.find_by_css_selector("#mols2grid .m2g-cell .data-_Name")
     assert name.text == "3-METHYLPENTANE"
     driver.wait_for_img_load()
-    (
-        ActionChains(driver)
-        .move_to_element(driver.find_by_css_selector("#mols2grid .cell .data-img *"))
-        .pause(0.5)
-        .perform()
+    tooltip = driver.get_tooltip_content(pause=0.5)
+    assert (
+        tooltip
+        == '<strong>_Name</strong>: <span class="copy-me">3-METHYLPENTANE</span>'
     )
-    tooltip = driver.find_by_css_selector('div.popover[role="tooltip"]')
-    el = tooltip.find_element_by_class_name("popover-body")
-    assert el.get_attribute("innerHTML") == "<strong>_Name</strong>: 3-METHYLPENTANE"
 
 
 @flaky(max_runs=3, min_passes=1)
 def test_transform_style_tooltip(driver: FirefoxDriver, grid):
     doc = get_doc(
         grid,
         {
@@ -522,109 +526,110 @@
                 "__all__": lambda x: "background-color: red",
                 "_Name": lambda x: "color: green" if x == "foo" else "color: blue",
             },
         },
     )
     driver.get(doc)
     driver.wait_for_img_load()
-    cell = driver.find_by_css_selector("#mols2grid .cell")
+    cell = driver.find_by_css_selector("#mols2grid .m2g-cell")
     assert cell.value_of_css_property("background-color") == "rgb(255, 0, 0)"
-    name = cell.find_element_by_class_name("data-_Name")
+    name = cell.find_element(By.CLASS_NAME, "data-_Name")
     assert name.text == "foo"
-    (
-        ActionChains(driver)
-        .move_to_element(driver.find_by_css_selector("#mols2grid .cell .data-img *"))
-        .pause(0.5)
-        .perform()
-    )
-    tooltip = driver.find_by_css_selector('div.popover[role="tooltip"]')
-    el = tooltip.find_element_by_class_name("popover-body")
+    tooltip = driver.get_tooltip_content(pause=0.5)
     assert (
-        el.get_attribute("innerHTML")
-        == '<strong>_Name</strong>: <span style="color: blue">foo</span>'
+        tooltip == '<strong>_Name</strong>: <span class="copy-me" style="color: blue">'
+        "foo</span>"
     )
 
 
 @pytest.mark.parametrize("selection", [True, False])
 def test_callback_js(driver: FirefoxDriver, grid, selection):
     doc = get_doc(
         grid,
         {
             "subset": ["img", "_Name"],
-            "callback": "$('#mols2grid .cell .data-_Name').html('foo')",
+            "callback": "$('#mols2grid .m2g-cell .data-_Name').html('foo')",
             "selection": selection,
         },
     )
     driver.get(doc)
     driver.wait_for_img_load()
-    driver.find_clickable(By.CSS_SELECTOR, "#mols2grid .cell .data-img").click()
-    el = driver.find_by_css_selector("#mols2grid .cell .data-_Name")
+    driver.trigger_callback()
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-_Name")
     assert el.text == "foo"
 
 
 def test_sort_by(driver: FirefoxDriver, grid):
     doc = get_doc(grid, {"subset": ["img", "_Name"], "sort_by": "_Name"})
     driver.get(doc)
-    el = driver.find_by_css_selector("#mols2grid .cell .data-_Name")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-_Name")
     assert el.text == "1,1,2,2-tetrachloroethane"
 
 
 def test_sort_button(driver: FirefoxDriver, html_doc):
     driver.get(html_doc)
     driver.wait_for_img_load()
-    driver.find_clickable(By.ID, "sortDropdown").click()
-    driver.find_clickable(
-        By.CSS_SELECTOR, 'button.sort-btn[data-name="data-_Name"]'
-    ).click()
-    el = driver.find_by_css_selector("#mols2grid .cell .data-_Name")
+    driver.sort_grid("_Name")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-_Name")
     assert el.text == "1,1,2,2-tetrachloroethane"
-    driver.find_clickable(By.ID, "sortDropdown").click()
-    driver.find_clickable(
-        By.CSS_SELECTOR, 'button.sort-btn[data-name="data-_Name"]'
-    ).click()
-    el = driver.find_by_css_selector("#mols2grid .cell .data-_Name")
+    driver.invert_sort()
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-_Name")
     assert el.text == "tetrachloromethane"
 
 
 @pytest.mark.parametrize(
     ["substruct_highlight", "expected"],
     [
         (True, "fffffe7ffc3ffc3ffe7ffe7ffe7ffe7ffe7ffc3ff81fc003c3c3c7e3c7e3eff7"),
         (False, "fe7ffe7ffe7ffe7ffe7ffe7ffe7ffe7ffe7ffe7ffe7ffc3ff99fe3c7c7e3cff3"),
     ],
 )
 def test_substruct_highlight(
     driver: FirefoxDriver, grid, substruct_highlight, expected
 ):
-    doc = get_doc(grid, {"n_rows": 1, "substruct_highlight": substruct_highlight})
+    doc = get_doc(
+        grid, {"n_items_per_page": 5, "substruct_highlight": substruct_highlight}
+    )
     driver.get(doc)
     driver.wait_for_img_load()
     driver.substructure_query("CC(I)C")
     hash_ = driver.get_svg_hash()
     assert str(hash_) == expected
 
 
 def test_substruct_clear_removes_highlight(driver: FirefoxDriver, grid):
-    doc = get_doc(grid, {"n_rows": 1, "substruct_highlight": True})
+    doc = get_doc(
+        grid,
+        {
+            "n_items_per_page": 5,
+            "substruct_highlight": True,
+            "size": (160, 120),
+        },
+    )
     driver.get(doc)
     driver.wait_for_img_load()
     driver.substructure_query("C")
     hash_hl = driver.get_svg_hash()
-    driver.find_by_id("searchbar").clear()
-    driver.find_by_id("searchbar").send_keys(Keys.BACKSPACE)
-    driver.wait_for_img_load()
+    driver.clear_search()
     hash_ = driver.get_svg_hash()
     assert hash_ != hash_hl
     assert (
         str(hash_) == "fffffffffffffe7ffe7ffe7ffe7ffe7ffe7f3e7c8811c183e7e7ffffffffffff"
     )
 
 
 def test_smarts_to_text_search_removes_highlight(driver: FirefoxDriver, grid):
-    doc = get_doc(grid, {"n_rows": 1, "substruct_highlight": True})
+    doc = get_doc(
+        grid,
+        {
+            "n_items_per_page": 5,
+            "substruct_highlight": True,
+            "size": (160, 120),
+        },
+    )
     driver.get(doc)
     driver.wait_for_img_load()
     driver.substructure_query("I")
     hash_hl = driver.get_svg_hash()
     driver.text_search("odopropane")
     hash_ = driver.get_svg_hash()
     assert hash_ != hash_hl
@@ -643,119 +648,119 @@
     driver.get(doc)
     mask = grid.dataframe["_Name"].str.contains("iodopropane")
     filter_code = env.get_template("js/filter.js").render(
         grid_id=grid._grid_id, mask=json.dumps(mask.tolist())
     )
     driver.wait_for_img_load()
     driver.execute_script(filter_code)
-    el = driver.find_by_css_selector("#mols2grid .cell .data-_Name")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-_Name")
     assert el.text == "2-iodopropane"
 
 
 def test_subset_gives_rows_order(driver: FirefoxDriver, grid):
-    subset = ["_Name", "img", "ID"]
-    doc = get_doc(grid, {"subset": subset, "n_rows": 1})
+    subset = ["_Name", "ID"]
+    doc = get_doc(grid, {"subset": subset, "n_items_per_page": 5})
     driver.get(doc)
     driver.wait_for_img_load()
-    cell = driver.find_by_css_selector("#mols2grid .cell")
-    elements = cell.find_elements_by_class_name("data")
-    for i, el in enumerate(elements):
+    cell = driver.find_by_css_selector("#mols2grid .m2g-cell")
+    elements = cell.find_elements(By.CLASS_NAME, "data")
+    i = 0
+    for el in elements:
         class_list = el.get_attribute("class").split()
         name = [x.replace("data-", "") for x in class_list if x.startswith("data-")][0]
-        if i == len(elements) - 1:
-            assert name == "SMILES"
-            assert el.value_of_css_property("display") == "none"
-        else:
-            assert name == subset[i]
+        if name in {"img", "SMILES"}:
+            continue
+        assert name == subset[i]
+        i += 1
+    # smiles should always be there, and last
+    assert name == "SMILES"
+    assert el.value_of_css_property("display") == "none"
 
 
 def test_colname_with_spaces(driver: FirefoxDriver, df):
     df = df.rename(columns={"SMILES": "Molecule", "_Name": "Molecule name"}).drop(
         columns="mol"
     )
     grid = mols2grid.MolGrid(df, smiles_col="Molecule")
     doc = get_doc(
-        grid, dict(subset=["Molecule name", "img"], tooltip=["Molecule"], n_rows=1)
+        grid,
+        dict(subset=["Molecule name", "img"], tooltip=["Molecule"], n_items_per_page=5),
     )
     driver.get(doc)
     driver.wait_for_img_load()
-    el = driver.find_by_css_selector("#mols2grid .cell .data")
+    el = driver.find_by_css_selector("#mols2grid .m2g-cell .data-Molecule-name")
     assert el.text == "3-methylpentane"
 
 
 @flaky(max_runs=3, min_passes=1)
 def test_custom_header(driver: FirefoxDriver, grid):
     doc = get_doc(
         grid,
         {
             "subset": ["img"],
             "custom_header": '<script src="https://unpkg.com/@rdkit/rdkit@2021.9.2/Code/MinimalLib/dist/RDKit_minimal.js"></script>',
-            "n_rows": 1,
+            "n_items_per_page": 5,
         },
     )
     driver.get(doc)
     driver.wait_for_img_load()
     val = driver.execute_script("return RDKit.version();")
     assert val == "2021.09.2"
 
 
-def test_table_template(driver: FirefoxDriver, sdf_path):
+def test_static_template(driver: FirefoxDriver, sdf_path):
     df = mols2grid.sdf_to_dataframe(sdf_path)[:15]
-    grid = mols2grid.MolGrid(df, mol_col="mol", prerender=True)
+    grid = mols2grid.MolGrid(df, mol_col="mol", prerender=True, size=(160, 120))
     doc = get_doc(
         grid,
         dict(
-            template="table",
+            template="static",
             subset=["mols2grid-id", "img"],
             tooltip=["_Name"],
             sort_by="_Name",
+            tooltip_trigger="hover",
         ),
     )
     driver.get(doc)
     el = driver.find_by_css_selector("#mols2grid td.col-0")
-    assert el.find_element_by_class_name("data-mols2grid-id").text == "8"
-    (
-        ActionChains(driver)
-        .move_to_element(el.find_element_by_css_selector(".data-img *"))
-        .perform()
-    )
-    tooltip = driver.find_by_css_selector('div.popover[role="tooltip"]')
-    el = tooltip.find_element_by_class_name("popover-body")
+    assert el.find_element(By.CLASS_NAME, "data-mols2grid-id").text == "8"
+    tooltip = driver.get_tooltip_content(selector=".m2g-cell-0")
     assert (
-        el.get_attribute("innerHTML")
-        == "<strong>_Name</strong>: 1,3,5-trimethylbenzene"
-    )
-    hash_ = driver.get_svg_hash("#mols2grid td .data-img")
-    diff = hash_ - imagehash.hex_to_hash(
-        "fffffe7ffe7ffe7ffe7ffe7ffc3ff10ff3cff3cff3cff3cff38fe1078c319e79"
+        tooltip
+        == '<strong>_Name</strong>: <span class="copy-me">1,3,5-trimethylbenzene</span>'
     )
-    assert diff <= 1
+    if COORDGEN_SUPPORT:
+        hash_ = driver.get_svg_hash("#mols2grid td .data-img")
+        diff = hash_ - imagehash.hex_to_hash(
+            "fffffe7ffe7ffe7ffe7ffe7ffc3ff10ff3cff3cff3cff3cff38fe1078c319e79"
+        )
+        assert diff <= 1
 
 
 def test_default_subset_tooltip(driver: FirefoxDriver, grid):
-    doc = get_doc(grid, {"n_rows": 1})
+    doc = get_doc(grid, {"n_items_per_page": 5})
     driver.get(doc)
     driver.wait_for_img_load()
-    expected_subset = ["mols2grid-id", "img"]
+    expected_subset = ["img"]
     expected_tooltip = [
         x
-        for x in grid.dataframe.columns.drop("mol").to_list()
+        for x in grid.dataframe.columns.drop(["mol", "mols2grid-id"]).to_list()
         if x not in expected_subset
     ]
-    cell = driver.find_by_css_selector("#mols2grid .cell")
-    data_elements = cell.find_elements_by_class_name("data")
+    cell = driver.find_by_css_selector("#mols2grid .m2g-cell")
+    data_elements = cell.find_elements(By.CLASS_NAME, "data")
     subset = [
-        c.replace("data-", "").replace("-copy", "")
+        c.replace("data-", "").replace("-display", "")
         for x in data_elements
         for c in x.get_attribute("class").split(" ")
         if c.startswith("data-") and not x.get_attribute("style")
     ]
     assert subset == expected_subset
     tooltip = [
-        c.replace("data-", "").replace("-copy", "")
+        c.replace("data-", "").replace("-display", "")
         for x in data_elements
         for c in x.get_attribute("class").split(" ")
         if c.startswith("data-") and x.get_attribute("style") == "display: none;"
     ]
     assert tooltip == expected_tooltip
 
 
@@ -798,70 +803,77 @@
 
 def test_highlight_with_hydrogens(driver: FirefoxDriver, df):
     mols = []
     for mol in df["mol"][25:]:
         m = Chem.AddHs(mol)
         m.ClearProp("SMILES")
         mols.append(m)
-    grid = mols2grid.MolGrid.from_mols(mols, removeHs=False)
+    grid = mols2grid.MolGrid.from_mols(
+        mols,
+        removeHs=False,
+        size=(160, 120),
+    )
     doc = get_doc(grid, dict(substruct_highlight=True, single_highlight=False))
     driver.get(doc)
     driver.wait_for_img_load()
     driver.substructure_query("Cl")
     hash_ = driver.get_svg_hash()
     assert (
         str(hash_) == "fdfffcfff8fffcfffdc7cdc780cf885bd901fb81f3b3f3bfff9fff1fff9fffbf"
     )
 
 
 def test_callbacks_info(driver: FirefoxDriver, grid):
     doc = get_doc(grid, {"callback": mols2grid.callbacks.info()})
     driver.get(doc)
     driver.trigger_callback()
-    modal = driver.find_by_css_selector("div.modal-content")
+    modal = driver.find_by_css_selector("#m2g-modal")
     assert (
-        modal.find_element_by_css_selector(".modal-header .modal-title").get_attribute(
+        modal.find_element(By.CSS_SELECTOR, ".m2g-modal-header h2").get_attribute(
             "innerHTML"
         )
         == "CCC(C)CC"
     )
-    content = modal.find_element_by_css_selector(
-        ".modal-body .row .col:nth-child(2)"
-    ).get_attribute("innerHTML")
+    content = modal.find_element(By.CSS_SELECTOR, ".m2g-modal-body").get_attribute(
+        "innerHTML"
+    )
     assert "PFEOZHBOMNWTJB-UHFFFAOYSA-N" in content
 
 
 def test_callbacks_3D(driver: FirefoxDriver, grid):
     doc = get_doc(grid, {"callback": mols2grid.callbacks.show_3d()})
     driver.get(doc)
-    driver.trigger_callback()
-    modal = driver.find_by_css_selector("div.modal-content")
+    driver.trigger_callback(pause=2.0)
+    modal = driver.find_by_css_selector("#m2g-modal")
     assert (
-        modal.find_element_by_css_selector(".modal-header .modal-title").get_attribute(
+        modal.find_element(By.CSS_SELECTOR, ".m2g-modal-header h2").get_attribute(
             "innerHTML"
         )
         == "CCC(C)CC"
     )
-    content = modal.find_element_by_css_selector(".modal-body").get_attribute(
+    content = modal.find_element(By.CSS_SELECTOR, ".m2g-modal-body").get_attribute(
         "innerHTML"
     )
     assert '<div id="molviewer' in content
-    # cannot test for actual rendering as there's no GL available
-    assert driver.execute_script("return typeof($3Dmol)") != "undefined"
+    if not GITHUB_ACTIONS:
+        # only works when testing locally...
+        assert "<canvas" in content
+        # cannot test for actual rendering as there's no GL available
+        assert driver.execute_script("return typeof($3Dmol)") != "undefined"
 
 
 def test_callbacks_external_link(driver: FirefoxDriver, grid):
     doc = get_doc(grid, {"callback": mols2grid.callbacks.external_link()})
     driver.get(doc)
     driver.trigger_callback()
     # check if new tab was opened
     assert len(driver.window_handles) > 1
     urls = []
     for handle in driver.window_handles[1:]:
-        driver.switch_to_window(handle)
+        driver.switch_to.window(handle)
         driver.wait(EC.url_contains("https://"))
         url = driver.current_url
         if url == "https://leruli.com/search/Q0NDKEMpQ0M=/home":
             break
         urls.append(url)
     else:
         raise AssertionError("Corresponding URL not found", urls)
```

### Comparing `mols2grid-1.1.1/tests/test_molgrid.py` & `mols2grid-2.0.0rc1/tests/test_molgrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from pathlib import Path
-from tempfile import NamedTemporaryFile
 from types import SimpleNamespace
 
 import pytest
 from numpy.testing import assert_equal
 from rdkit import Chem
 from rdkit.Chem import Draw
 from rdkit.Chem.rdDepictor import Compute2DCoords
@@ -190,15 +188,15 @@
         grid = MolGrid.from_sdf(sdf_path, prerender=True, **{param: value})
     else:
         grid = MolGrid.from_sdf(sdf_path, **{param: value})
     assert getattr(grid, attr) == value
 
 
 def test_template(grid_prerendered):
-    grid_prerendered.template = "pages"
+    grid_prerendered.template = "interactive"
     assert grid_prerendered._template is grid_prerendered.template
 
 
 def test_template_setter(grid_prerendered):
     with pytest.raises(ValueError, match="template='foo' not supported"):
         grid_prerendered.template = "foo"
 
@@ -234,52 +232,52 @@
     register.selection_updated("grid", event)
     assert register.current_selection == "grid"
     assert grid.get_selection().equals(small_df.head(1))
     assert other.get_selection().equals(small_df.head(0))  # empty dataframe
     register._clear()
 
 
-def test_save(grid):
-    with NamedTemporaryFile("w", suffix=".html") as f:
-        grid.save(f.name)
-        assert Path(f.name).is_file()
+def test_save(grid, tmp_path):
+    output = tmp_path / "output.html"
+    grid.save(output)
+    assert output.is_file()
 
 
-def test_render_pages(grid):
-    grid.render(template="pages")
+def test_render_interactive(grid):
+    grid.render(template="interactive")
 
 
-def test_render_table(grid_prerendered):
-    grid_prerendered.render(template="table")
+def test_render_static(grid_prerendered):
+    grid_prerendered.render(template="static")
 
 
 def test_render_wrong_template(grid):
     with pytest.raises(ValueError, match="template='foo' not supported"):
         grid.render(template="foo")
 
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         dict(),
         dict(subset=["ID"]),
         dict(tooltip=["ID"]),
-        dict(gap="5px"),
+        dict(gap=5),
         dict(style={"ID": lambda x: "color: red" if x == 1 else ""}),
         dict(transform={"ID": lambda x: f"Id. #{x}"}),
     ],
 )
-def test_integration_table(grid_prerendered, kwargs):
-    grid_prerendered.to_table(**kwargs)
+def test_integration_static(grid_prerendered, kwargs):
+    grid_prerendered.to_static(**kwargs)
 
 
 def test_python_callback(grid):
-    html = grid.to_pages(subset=["img"], callback=lambda data: None)
-    assert "// trigger custom python callback" in html
-    assert "// no kernel detected for callback" in html
+    html = grid.to_interactive(subset=["img"], callback=lambda data: None)
+    assert "// Trigger custom python callback" in html
+    assert "// No kernel detected for callback" in html
 
 
 def test_cache_selection(small_df):
     grid = get_grid(small_df, name="cache")
     event = SimpleNamespace(new='{0: "CCO"}')
     register.selection_updated("cache", event)
     grid = get_grid(small_df, name="cache", cache_selection=True)
@@ -321,29 +319,26 @@
         ValueError, match="Cannot use coordinates with on-the-fly rendering"
     ):
         get_grid(small_df, use_coords=True, prerender=False)
 
 
 def test_sort_by_not_in_subset_or_tooltip(grid):
     with pytest.raises(ValueError, match="'_Name' is not an available field"):
-        grid.to_pages(subset=["ID", "img"], sort_by="_Name")
+        grid.to_interactive(subset=["ID", "img"], sort_by="_Name")
 
 
-def test_subset_without_img_error(grid):
-    with pytest.raises(
-        KeyError, match="Please add the 'img' field in the `subset` parameter"
-    ):
-        grid.display(subset=["_Name"])
+def test_subset_without_img_no_error(grid):
+    grid.display(subset=["_Name"])
 
 
-def test_table_no_prerender_error(grid):
+def test_static_no_prerender_error(grid):
     with pytest.raises(
-        ValueError, match="Please set `prerender=True` when using the 'table' template"
+        ValueError, match="Please set `prerender=True` when using the 'static' template"
     ):
-        grid.display(template="table")
+        grid.display(template="static")
 
 
 def test_replace_non_serializable_from_default_output(small_df):
     grid = get_grid(small_df)
     grid.dataframe["non-serializable"] = grid.dataframe[grid.mol_col]
     html = grid.render()
     assert "\\ud83e\\udd37\\u200d\\u2642\\ufe0f" in html  # 🤷‍♂️
```

### Comparing `mols2grid-1.1.1/tests/test_select.py` & `mols2grid-2.0.0rc1/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/tests/test_utils.py` & `mols2grid-2.0.0rc1/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,31 +26,38 @@
     ["subset", "fmt", "style", "transform", "exp"],
     [
         (
             ["SMILES", "ID"],
             "<strong>{key}</strong>: {value}",
             {},
             {},
-            "<strong>SMILES</strong>: CCO<br><strong>ID</strong>: 0",
+            '<strong>SMILES</strong>: <span class="copy-me">CCO</span><br>'
+            '<strong>ID</strong>: <span class="copy-me">0</span>',
         ),
-        (["ID"], "foo-{value}", {}, {}, "foo-0"),
+        (["ID"], "foo-{value}", {}, {}, 'foo-<span class="copy-me">0</span>'),
         (
             ["ID"],
             "{value}",
             {"ID": lambda x: "color: red"},
             {},
-            '<span style="color: red">0</span>',
+            '<span class="copy-me" style="color: red">0</span>',
+        ),
+        (
+            ["Activity"],
+            "{value}",
+            {},
+            {"Activity": lambda x: f"{x:.2f}"},
+            '<span class="copy-me">42.01</span>',
         ),
-        (["Activity"], "{value}", {}, {"Activity": lambda x: f"{x:.2f}"}, "42.01"),
         (
             ["Activity"],
             "{key}: {value}",
             {"Activity": lambda x: "color: red" if x > 40 else ""},
             {"Activity": lambda x: f"{x:.2f}"},
-            'Activity: <span style="color: red">42.01</span>',
+            'Activity: <span class="copy-me" style="color: red">42.01</span>',
         ),
     ],
 )
 def test_tooltip_formatter(subset, fmt, style, transform, exp):
     row = pd.Series(
         {
             "ID": 0,
```

### Comparing `mols2grid-1.1.1/.gitignore` & `mols2grid-2.0.0rc1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -371,10 +371,9 @@
 
 # ======
 # Custom
 # ======
 
 mols2grid/nbextension/index.*
 mols2grid/labextension
-package-lock.json
 .vscode/
 quickstart-grid.html
```

### Comparing `mols2grid-1.1.1/LICENSE` & `mols2grid-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mols2grid-1.1.1/README.md` & `mols2grid-2.0.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 [![Code coverage](https://codecov.io/gh/cbouy/mols2grid/branch/master/graph/badge.svg?token=QDI1XQSDUC)](https://codecov.io/gh/cbouy/mols2grid)
 
 [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
 [![Knime Hub](https://img.shields.io/badge/Available%20on-KNIME-ffd500.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAABdUExURUxpcf/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAPfHMOMAAAAfdFJOUwCyq6CEYtAEApEspncGDpjxVlAYgDSdiEBHbMrCHtmwXwB/AAAAT3pUWHRSYXcgcHJvZmlsZSB0eXBlIGlwdGMAAHic48osKEnmUgADIwsuYwsTIxNLkxQDEyBEgDTDZAMjs1Qgy9jUyMTMxBzEB8uASKBKLgAolQ7jKiJtHwAAAIxJREFUGNNdjFkSgyAQBYdtYADZVNxz/2NGjSlj+q9fvWqAD1rDk1Ke3nJqH4NnpH7d4iCFvV1XVJ3r7u6URPZiHb8eeFJ25sjDNahlKRDUkq7u5njd32ZC3A433g2+h3bKCuUx9FHOecyV/CzXfi/KSJG9EjJB0lEAS9UxxriINMiOLJim0SfNiYF/3szTBp6mEP9HAAAAAElFTkSuQmCC)](https://hub.knime.com/cbouy/spaces/Public/latest/Interactive%20Grid%20of%20Molecules)
 
 **mols2grid** is an interactive molecule viewer for 2D structures, based on RDKit.
 
+![Demo image](docs/_static/demo.png)
+
 ## [Documentation](https://mols2grid.readthedocs.io/en/latest/contents.html)
 
 Installation, basic usage, links to resources...*etc.*
 
 ## [Notebooks](https://mols2grid.readthedocs.io/en/latest/notebooks/quickstart.html)
 
 Showcases examples of most features, with links to run the notebooks on Google Colab
```

### Comparing `mols2grid-1.1.1/pyproject.toml` & `mols2grid-2.0.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -35,46 +35,54 @@
 ]
 dependencies = [
     "ipywidgets>=7,<8",
     "jinja2>=2.11.0",
     "numpy",
     "pandas",
 ]
-version = "1.1.1"
+dynamic = ["version"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 build = [
     "build",
 ]
 tests = [
     "cairosvg==2.5.2",
-    "codecov==2.1.12",
     "flaky==3.7.0",
-    "geckodriver-autoinstaller==0.1.0",
+    "pyautogecko==0.1.3",
     "imagehash~=4.3",
     "ipython==7.12.0",
     "pytest-cov==2.12.1",
     "pytest==6.2.5",
-    "selenium==3.141.0",
+    "selenium==4.10.0",
+]
+docs = [
+    "mistune<3.0.0",
 ]
 dev = [
     "tbump",
     "mols2grid[build,tests]",
 ]
 
 [project.urls]
 Homepage = "https://github.com/cbouy/mols2grid"
 Documentation = "https://mols2grid.readthedocs.io/en/latest/"
 Discussions = "https://github.com/cbouy/mols2grid/discussions"
 Issues = "https://github.com/cbouy/mols2grid/issues"
 Changelog = "https://github.com/cbouy/mols2grid/blob/master/CHANGELOG.md"
 
+[tool.setuptools.dynamic]
+version = { attr = "mols2grid._version.__version__" }
+
+[tool.hatch.version]
+path = "mols2grid/_version.py"
+
 [tool.hatch.build]
 artifacts = [
     "mols2grid/nbextension/index.*",
     "mols2grid/labextension",
 ]
 
 [tool.hatch.build.targets.wheel.shared-data]
```

### Comparing `mols2grid-1.1.1/PKG-INFO` & `mols2grid-2.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mols2grid
-Version: 1.1.1
+Version: 2.0.0rc1
 Summary: Interactive 2D small molecule viewer
 Project-URL: Homepage, https://github.com/cbouy/mols2grid
 Project-URL: Documentation, https://mols2grid.readthedocs.io/en/latest/
 Project-URL: Discussions, https://github.com/cbouy/mols2grid/discussions
 Project-URL: Issues, https://github.com/cbouy/mols2grid/issues
 Project-URL: Changelog, https://github.com/cbouy/mols2grid/blob/master/CHANGELOG.md
 Author-email: Cédric Bouysset <cedric@bouysset.net>
@@ -203,24 +203,25 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: build
 Requires-Dist: build; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: mols2grid[build,tests]; extra == 'dev'
 Requires-Dist: tbump; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: mistune<3.0.0; extra == 'docs'
 Provides-Extra: tests
 Requires-Dist: cairosvg==2.5.2; extra == 'tests'
-Requires-Dist: codecov==2.1.12; extra == 'tests'
 Requires-Dist: flaky==3.7.0; extra == 'tests'
-Requires-Dist: geckodriver-autoinstaller==0.1.0; extra == 'tests'
 Requires-Dist: imagehash~=4.3; extra == 'tests'
 Requires-Dist: ipython==7.12.0; extra == 'tests'
+Requires-Dist: pyautogecko==0.1.3; extra == 'tests'
 Requires-Dist: pytest-cov==2.12.1; extra == 'tests'
 Requires-Dist: pytest==6.2.5; extra == 'tests'
-Requires-Dist: selenium==3.141.0; extra == 'tests'
+Requires-Dist: selenium==4.10.0; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # ![mols2grid logo](https://user-images.githubusercontent.com/27850535/154588465-43dc5d82-ee2d-4178-a2f3-e06000bc87c9.png) mols2grid
 
 [![Pypi version](https://img.shields.io/pypi/v/mols2grid.svg)](https://pypi.python.org/pypi/mols2grid)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/mols2grid)](https://anaconda.org/conda-forge/mols2grid)
 
@@ -230,14 +231,16 @@
 [![Code coverage](https://codecov.io/gh/cbouy/mols2grid/branch/master/graph/badge.svg?token=QDI1XQSDUC)](https://codecov.io/gh/cbouy/mols2grid)
 
 [![Powered by RDKit](https://img.shields.io/badge/Powered%20by-RDKit-3838ff.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAFVBMVEXc3NwUFP8UPP9kZP+MjP+0tP////9ZXZotAAAAAXRSTlMAQObYZgAAAAFiS0dEBmFmuH0AAAAHdElNRQfmAwsPGi+MyC9RAAAAQElEQVQI12NgQABGQUEBMENISUkRLKBsbGwEEhIyBgJFsICLC0iIUdnExcUZwnANQWfApKCK4doRBsKtQFgKAQC5Ww1JEHSEkAAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMi0wMy0xMVQxNToyNjo0NyswMDowMDzr2J4AAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjItMDMtMTFUMTU6MjY6NDcrMDA6MDBNtmAiAAAAAElFTkSuQmCC)](https://www.rdkit.org/)
 [![Knime Hub](https://img.shields.io/badge/Available%20on-KNIME-ffd500.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAABdUExURUxpcf/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAP/VAPfHMOMAAAAfdFJOUwCyq6CEYtAEApEspncGDpjxVlAYgDSdiEBHbMrCHtmwXwB/AAAAT3pUWHRSYXcgcHJvZmlsZSB0eXBlIGlwdGMAAHic48osKEnmUgADIwsuYwsTIxNLkxQDEyBEgDTDZAMjs1Qgy9jUyMTMxBzEB8uASKBKLgAolQ7jKiJtHwAAAIxJREFUGNNdjFkSgyAQBYdtYADZVNxz/2NGjSlj+q9fvWqAD1rDk1Ke3nJqH4NnpH7d4iCFvV1XVJ3r7u6URPZiHb8eeFJ25sjDNahlKRDUkq7u5njd32ZC3A433g2+h3bKCuUx9FHOecyV/CzXfi/KSJG9EjJB0lEAS9UxxriINMiOLJim0SfNiYF/3szTBp6mEP9HAAAAAElFTkSuQmCC)](https://hub.knime.com/cbouy/spaces/Public/latest/Interactive%20Grid%20of%20Molecules)
 
 **mols2grid** is an interactive molecule viewer for 2D structures, based on RDKit.
 
+![Demo image](docs/_static/demo.png)
+
 ## [Documentation](https://mols2grid.readthedocs.io/en/latest/contents.html)
 
 Installation, basic usage, links to resources...*etc.*
 
 ## [Notebooks](https://mols2grid.readthedocs.io/en/latest/notebooks/quickstart.html)
 
 Showcases examples of most features, with links to run the notebooks on Google Colab
```

