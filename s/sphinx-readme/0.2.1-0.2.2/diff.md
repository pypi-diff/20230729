# Comparing `tmp/sphinx-readme-0.2.1.tar.gz` & `tmp/sphinx-readme-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-readme-0.2.1.tar", last modified: Sun Jul 23 20:18:05 2023, max compression
+gzip compressed data, was "sphinx-readme-0.2.2.tar", last modified: Sat Jul 29 16:09:09 2023, max compression
```

## Comparing `sphinx-readme-0.2.1.tar` & `sphinx-readme-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 20:18:05.523091 sphinx-readme-0.2.1/
--rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     9427 2023-07-23 20:18:05.523091 sphinx-readme-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     8638 2023-07-23 20:17:32.000000 sphinx-readme-0.2.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-23 20:18:05.523091 sphinx-readme-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 20:18:05.507501 sphinx-readme-0.2.1/sphinx_readme/
--rw-rw-rw-   0        0        0     1768 2023-07-23 20:14:04.000000 sphinx-readme-0.2.1/sphinx_readme/__init__.py
--rw-rw-rw-   0        0        0    12014 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/sphinx_readme/config.py
--rw-rw-rw-   0        0        0    24826 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/sphinx_readme/parser.py
-drwxrwxrwx   0        0        0        0 2023-07-23 20:18:05.523091 sphinx-readme-0.2.1/sphinx_readme/utils/
--rw-rw-rw-   0        0        0        0 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/sphinx_readme/utils/__init__.py
--rw-rw-rw-   0        0        0      603 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/sphinx_readme/utils/docutils.py
--rw-rw-rw-   0        0        0     4643 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/sphinx_readme/utils/git.py
--rw-rw-rw-   0        0        0     3727 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/sphinx_readme/utils/linkcode.py
--rw-rw-rw-   0        0        0     7578 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/sphinx_readme/utils/rst.py
--rw-rw-rw-   0        0        0      810 2023-07-23 19:42:27.000000 sphinx-readme-0.2.1/sphinx_readme/utils/sphinx.py
-drwxrwxrwx   0        0        0        0 2023-07-23 20:18:05.507501 sphinx-readme-0.2.1/sphinx_readme.egg-info/
--rw-rw-rw-   0        0        0     9427 2023-07-23 20:18:05.000000 sphinx-readme-0.2.1/sphinx_readme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-07-23 20:18:05.000000 sphinx-readme-0.2.1/sphinx_readme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 20:18:05.000000 sphinx-readme-0.2.1/sphinx_readme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-23 20:18:05.000000 sphinx-readme-0.2.1/sphinx_readme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-23 20:18:05.000000 sphinx-readme-0.2.1/sphinx_readme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:09.919418 sphinx-readme-0.2.2/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     9551 2023-07-29 16:09:09.919418 sphinx-readme-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8762 2023-07-29 16:07:41.000000 sphinx-readme-0.2.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-29 16:09:09.919418 sphinx-readme-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-07-26 07:43:44.000000 sphinx-readme-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:09.881698 sphinx-readme-0.2.2/sphinx_readme/
+-rw-rw-rw-   0        0        0     1768 2023-07-29 16:06:08.000000 sphinx-readme-0.2.2/sphinx_readme/__init__.py
+-rw-rw-rw-   0        0        0    12043 2023-07-29 10:52:41.000000 sphinx-readme-0.2.2/sphinx_readme/config.py
+-rw-rw-rw-   0        0        0    25759 2023-07-29 15:15:35.000000 sphinx-readme-0.2.2/sphinx_readme/parser.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:09.903797 sphinx-readme-0.2.2/sphinx_readme/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 07:43:44.000000 sphinx-readme-0.2.2/sphinx_readme/utils/__init__.py
+-rw-rw-rw-   0        0        0      603 2023-07-26 07:43:44.000000 sphinx-readme-0.2.2/sphinx_readme/utils/docutils.py
+-rw-rw-rw-   0        0        0     4643 2023-07-26 07:43:44.000000 sphinx-readme-0.2.2/sphinx_readme/utils/git.py
+-rw-rw-rw-   0        0        0     3727 2023-07-26 07:43:44.000000 sphinx-readme-0.2.2/sphinx_readme/utils/linkcode.py
+-rw-rw-rw-   0        0        0     7578 2023-07-26 07:43:44.000000 sphinx-readme-0.2.2/sphinx_readme/utils/rst.py
+-rw-rw-rw-   0        0        0      810 2023-07-26 07:43:44.000000 sphinx-readme-0.2.2/sphinx_readme/utils/sphinx.py
+drwxrwxrwx   0        0        0        0 2023-07-29 16:09:09.898654 sphinx-readme-0.2.2/sphinx_readme.egg-info/
+-rw-rw-rw-   0        0        0     9551 2023-07-29 16:09:09.000000 sphinx-readme-0.2.2/sphinx_readme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-07-29 16:09:09.000000 sphinx-readme-0.2.2/sphinx_readme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-29 16:09:09.000000 sphinx-readme-0.2.2/sphinx_readme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-29 16:09:09.000000 sphinx-readme-0.2.2/sphinx_readme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-29 16:09:09.000000 sphinx-readme-0.2.2/sphinx_readme.egg-info/top_level.txt
```

### Comparing `sphinx-readme-0.2.1/LICENSE` & `sphinx-readme-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.2.1/PKG-INFO` & `sphinx-readme-0.2.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,13 @@
-Metadata-Version: 2.1
-Name: sphinx-readme
-Version: 0.2.1
-Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
-Home-page: https://github.com/tdkorn/sphinx-readme
-Author: Adam Korn
-Author-email: hello@dailykitten.net
-License: MIT License
-Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
-Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
-Platform: UNKNOWN
-Classifier: Framework :: Sphinx :: Extension
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE
-
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_baseurl
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_context
 .. |.`~.parse_intersphinx_nodes`| replace:: ``parse_intersphinx_nodes()``
-.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.2.1/sphinx_readme/parser.py#L213-L237
+.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.2.2/sphinx_readme/parser.py#L216-L240
 .. |readme_docs_url_type| replace:: ``readme_docs_url_type``
 .. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
 .. |readme_inline_markup| replace:: ``readme_inline_markup``
 .. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
 .. |readme_raw_directive| replace:: ``readme_raw_directive``
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 .. |readme_replace_attrs| replace:: ``readme_replace_attrs``
@@ -43,15 +25,15 @@
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.1/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.2/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 
 
 
@@ -94,31 +76,32 @@
 
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
-.. csv-table::
-   :header: 📚 What's Sphinx README?
-
-   "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
-   to generate ``rst`` files that render beautifully on
-   GitHub, PyPi, GitLab, and BitBucket."
+.. list-table::
+   :header-rows: 1
+   
+   * - 📚 What's Sphinx README?
+   * - ``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
+       to generate ``rst`` files that render beautifully on
+       GitHub, PyPi, GitLab, and BitBucket.
 
 
 
 **With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.1/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.2/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 📋 Features
 ~~~~~~~~~~~~
 
@@ -191,18 +174,19 @@
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
-.. csv-table::
-   :header: 📢 Important
-
-   "Filepaths should be specified relative to the source directory"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📢 Important
+   * - Filepaths should be specified relative to the source directory
 
 
 |
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
@@ -216,21 +200,22 @@
 
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
    **Example**: |parse_intersphinx_nodes_html|_
 
 
-.. csv-table::
-   :header: 📝 Note
-
-   "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
-
-   * Instead, they'll be replaced with ``inline literals`` or left as is
-   * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📝 Note
+   * - If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
+    
+       * Instead, they'll be replaced with ``inline literals`` or left as is
+       * Please see |readme_replace_attrs|_ and |readme_inline_markup|_
 
 
 
 .. |parse_intersphinx_nodes_html| replace:: ``parse_intersphinx_nodes()``
 .. _parse_intersphinx_nodes_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_nodes
 
 
@@ -254,30 +239,29 @@
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
 
 
-.. csv-table::
-   :header: 📢 Important
-
-   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
-   be sure to disable |readme_raw_directive|_:
-
-   .. code-block:: python
-
-      readme_raw_directive = False"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📢 Important
+   * - For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
+       be sure to disable |readme_raw_directive|_:
+    
+       .. code-block:: python
+    
+          readme_raw_directive = False
 
 
 
 
 📚 Documentation
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
 .. _docs: https://sphinx-readme.readthedocs.io/en/latest
-
-
```

### Comparing `sphinx-readme-0.2.1/README.rst` & `sphinx-readme-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,31 @@
+Metadata-Version: 2.1
+Name: sphinx-readme
+Version: 0.2.2
+Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
+Home-page: https://github.com/tdkorn/sphinx-readme
+Author: Adam Korn
+Author-email: hello@dailykitten.net
+License: MIT License
+Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
+Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
+Platform: UNKNOWN
+Classifier: Framework :: Sphinx :: Extension
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE
+
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_baseurl
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_context
 .. |.`~.parse_intersphinx_nodes`| replace:: ``parse_intersphinx_nodes()``
-.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.2.1/sphinx_readme/parser.py#L213-L237
+.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.2.2/sphinx_readme/parser.py#L216-L240
 .. |readme_docs_url_type| replace:: ``readme_docs_url_type``
 .. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
 .. |readme_inline_markup| replace:: ``readme_inline_markup``
 .. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
 .. |readme_raw_directive| replace:: ``readme_raw_directive``
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 .. |readme_replace_attrs| replace:: ``readme_replace_attrs``
@@ -25,15 +43,15 @@
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.1/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.2/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 
 
 
@@ -76,31 +94,32 @@
 
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
-.. csv-table::
-   :header: 📚 What's Sphinx README?
-
-   "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
-   to generate ``rst`` files that render beautifully on
-   GitHub, PyPi, GitLab, and BitBucket."
+.. list-table::
+   :header-rows: 1
+   
+   * - 📚 What's Sphinx README?
+   * - ``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
+       to generate ``rst`` files that render beautifully on
+       GitHub, PyPi, GitLab, and BitBucket.
 
 
 
 **With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.1/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.2/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 📋 Features
 ~~~~~~~~~~~~
 
@@ -173,18 +192,19 @@
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
-.. csv-table::
-   :header: 📢 Important
-
-   "Filepaths should be specified relative to the source directory"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📢 Important
+   * - Filepaths should be specified relative to the source directory
 
 
 |
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
@@ -198,21 +218,22 @@
 
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
    **Example**: |parse_intersphinx_nodes_html|_
 
 
-.. csv-table::
-   :header: 📝 Note
-
-   "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
-
-   * Instead, they'll be replaced with ``inline literals`` or left as is
-   * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📝 Note
+   * - If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
+    
+       * Instead, they'll be replaced with ``inline literals`` or left as is
+       * Please see |readme_replace_attrs|_ and |readme_inline_markup|_
 
 
 
 .. |parse_intersphinx_nodes_html| replace:: ``parse_intersphinx_nodes()``
 .. _parse_intersphinx_nodes_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_nodes
 
 
@@ -236,28 +257,31 @@
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
 
 
-.. csv-table::
-   :header: 📢 Important
-
-   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
-   be sure to disable |readme_raw_directive|_:
-
-   .. code-block:: python
-
-      readme_raw_directive = False"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📢 Important
+   * - For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
+       be sure to disable |readme_raw_directive|_:
+    
+       .. code-block:: python
+    
+          readme_raw_directive = False
 
 
 
 
 📚 Documentation
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
 .. _docs: https://sphinx-readme.readthedocs.io/en/latest
+
+
```

### Comparing `sphinx-readme-0.2.1/setup.py` & `sphinx-readme-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.2.1/sphinx_readme/__init__.py` & `sphinx-readme-0.2.2/sphinx_readme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sphinx.environment import BuildEnvironment
 
 from sphinx_readme.utils.sphinx import get_conf_val, set_conf_val
 from sphinx_readme.utils.git import get_repo_dir
 from sphinx_readme.parser import READMEParser
 
 
-__version__ = "v0.2.1"
+__version__ = "v0.2.2"
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     # Avoid setting up extension if building on ReadTheDocs
     if os.environ.get("READTHEDOCS") == "True":
         return {}
```

### Comparing `sphinx-readme-0.2.1/sphinx_readme/config.py` & `sphinx-readme-0.2.2/sphinx_readme/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,12 +313,13 @@
 .. raw:: html
 
    </td></tr>
    </table>
 '''
         else:
             return r'''
-.. csv-table::
-   :header: {icon} {title}
-
-   "\1"
+\1.. list-table::
+\1   :header-rows: 1
+   
+\1   * - {icon} {title}
+\1   * - \2
 '''
```

### Comparing `sphinx-readme-0.2.1/sphinx_readme/parser.py` & `sphinx-readme-0.2.2/sphinx_readme/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         self.ref_map: Dict[str, Union[List, Dict]] = {}
         #: Mapping of source files to their content
         self.sources: Dict[str, str] = self.config.sources
         #: Mapping of source files to their toctree data
         self.toctrees: Dict[str, List[Dict]] = defaultdict(list)
         #: Mapping of source files to their admonition data
         self.admonitions: Dict[str, Dict[str, List[Dict]]] = {}
+        #: Mapping of source files to their rubric data
+        self.rubrics: Dict[str, List[str]] = {}
         #: Mapping of docnames to their parsed titles
         self.titles: Dict[str, str] = {}
         #: Mapping of cross-reference targets to their substitution definitions
         self.substitutions: Dict[str, List[str]] = {}
         #: Standard cross-reference roles
         self.roles: Set[str] = {"doc", "ref"}
 
@@ -172,14 +174,15 @@
 
     def parse_doctree(self, app: Sphinx, doctree: nodes.document, docname: str) -> None:
         """Parses cross-reference, admonition, and toctree data from a resolved doctree"""
         if doctree.get('source') in self.sources:
             self.parse_admonitions(app, doctree, docname)
             self.parse_intersphinx_nodes(doctree)
             self.parse_toctrees(doctree)
+            self.parse_rubrics(doctree)
 
     def parse_admonitions(self, app: Sphinx, doctree: nodes.document, docname: str) -> None:
         """Parses data from generic and specific admonitions
 
         :param doctree: the doctree from one of the :attr:`~.src_files`
         """
         admonitions = {'generic': [], 'specific': []}
@@ -252,25 +255,35 @@
             for _, entry in toctree.get('entries', []):
                 toc['entries'].append({
                     'entry': entry,
                     'title': self.titles.get(entry),
                 })
             self.toctrees[source].append(toc)
 
+    def parse_rubrics(self, doctree: nodes.document) -> None:
+        """Parses the content from :rst:dir:`rubric` directives"""
+        source = doctree.get('source')
+        rubrics = []
+
+        for rubric in doctree.findall(nodes.rubric):
+            rubrics.append(rubric.rawsource)
+
+        self.rubrics[source] = rubrics
+
     def resolve(self) -> None:
         """Uses parsed data from to replace cross-references and directives in the :attr:`~.src_files`
 
         Once resolved, files are written to the :attr:`~.out_dir`.
         """
         for src, rst in self.sources.items():
             # Replace everything using parsed data
             rst = self.replace_admonitions(src, rst)
             rst = self.replace_rst_images(src, rst)
             rst = self.replace_toctrees(src, rst)
-            rst = self.replace_rst_rubrics(rst)
+            rst = self.replace_rubrics(src, rst)
             rst = self.replace_py_xrefs(rst)
 
             for role in self.roles:
                 rst = self.replace_std_xrefs(role, rst)
 
             # Prepend substitution definitions for cross-reference
             header_vals = [
@@ -305,30 +318,41 @@
         for _type in ('generic', 'specific'):
             for admonition in admonitions[_type]:
                 if pattern := self.get_admonition_regex(admonition, _type):
                     icon = self.get_admonition_icon(admonition)
                     if not self.config.raw_directive:
                         rst = re.sub(
                             pattern=pattern,
-                            repl=self.config.admonition_template.format(
-                                title=admonition['title'],
-                                icon=icon),
-                            string=rst
+                            repl=lambda match: self._replace_admonition(
+                                match, admonition, icon),
+                            string=rst,
                         )
                     else:
                         rst = re.sub(
                             pattern=pattern,
                             repl=self.config.admonition_template.format(
                                 title=admonition['title'],
                                 text=admonition['body'],
                                 icon=icon),
                             string=rst
                         )
         return rst
 
+    def _replace_admonition(self, match, admonition: dict, icon: str) -> str:
+        """Helper function for formatting ``list-table`` admonitions"""
+        template = self.config.admonition_template.format(
+            title=admonition['title'],
+            icon=icon
+        ).replace(
+            r'\2', match.group(2).replace('\n', '\n    ')
+        ).replace(
+            r'\1', match.group(1)
+        )
+        return template
+
     def replace_toctrees(self, rst_src: str, rst: str) -> str:
         """Replaces :rst:dir:`toctree` directives with hyperlinked bullet lists
 
         .. note:: Entries will link to HTML documentation regardless of the
            value of :confval:`readme_docs_url_type`
 
         :param rst_src: absolute path of the source file
@@ -402,15 +426,15 @@
             rst = re.sub(
                 pattern=rf"\.\. image:: {img_path}",
                 repl=fr".. image:: {self.config.image_baseurl}/{path_to_img}",
                 string=rst
             )
         return rst
 
-    def replace_rst_rubrics(self, rst: str) -> str:
+    def replace_rubrics(self, rst_src: str, rst: str) -> str:
         """Replaces :rst:dir:`rubric` directives with the section heading
         character specified by :confval:`readme_rubric_heading`
 
         If :confval:`readme_rubric_heading` is not specified, the rubric
         will be replaced with bold text instead
 
         ...
@@ -425,31 +449,36 @@
               **This is a** ``rubric`` **directive**
 
         * Replacement if :code:`readme_rubric_heading = "^"`::
 
               This is a ``rubric`` directive
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+        :param rst_src: absolute path of the source file
         :param rst: content of the source file
         """
+        rubric_pattern = r'\.\. rubric:: ({body})(?=\n?$(?:\n+?^\s*$|\Z))'
         heading_chars = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
-        rubric_pattern = r'\.\. rubric:: (.+?)(?=\n)'
 
         if heading := self.config.rubric_heading:
-            if heading in heading_chars:
-                return re.sub(
-                    pattern=rubric_pattern,
-                    repl=lambda m: f"{m.group(1)}\n{heading * len(m.group(1))}",
-                    string=rst
-                )
-        return re.sub(
-            pattern=rubric_pattern,
-            repl=lambda m: format_rst("bold", m.group(1)),
-            string=rst
-        )
+            if heading not in heading_chars:
+                heading = None
+
+        for rubric in self.rubrics[rst_src]:
+            pattern = rubric_pattern.format(body=rubric.replace("\n", r"\n[ ]+"))
+            text = ' '.join(line.strip() for line in rubric.split('\n'))
+
+            if heading:
+                repl = text + "\n" + (len(text) * heading)
+            else:
+                repl = format_rst("bold", text)
+
+            rst = re.sub(pattern, repl, rst, flags=re.M)
+
+        return rst
 
     def replace_std_xrefs(self, ref_role: str, rst: str) -> str:
         """Replaces cross-references from the |std_domain|
 
         .. hint::
 
            This includes cross-references using the :rst:role:`doc`
@@ -570,21 +599,17 @@
 
     def get_admonition_regex(self, admonition: Dict[str, str], admonition_type: str) -> str:
         """Returns the regex to match a specific admonition directive
 
         :param admonition: a dict containing admonition data
         :param admonition_type: ``"generic"`` or ``"specific"``
         """
-        body = escape_rst(admonition['body'])
+        body = escape_rst(admonition['body']).replace('\n', r'\n\s*')
         title = escape_rst(admonition['title'])
 
-        # Account for arbitrary whitespace before each line of directive content
-        lines = (line.replace('\n', '\n\s+') for line in body.split('\n\n'))
-        body = '\n\n\s+'.join(lines)
-
         if admonition_type == 'specific':
             # For example, .. note:: This is a note
             pattern = fr"\.\. {admonition['class']}::\n*?\s+"
 
         else:
             # Generic admonition directives with/without class option
             pattern = rf"\.\. admonition::\s+{title}" + r"\n"
@@ -593,20 +618,20 @@
                 if 'admonition-' not in cls:
                     pattern += rf"\s+:class: {cls}" + r"\n"
 
             pattern += r"\n*?\s+"
 
         if not self.config.raw_directive:
             # csv-table template body uses match group
-            pattern += rf"({body})"
+            pattern = rf"([ ]*){pattern}({body})"
         else:
             # raw html template body uses string formatting
             pattern += rf"{body}"
 
-        pattern += r"(?=[\n\S]+?)"
+        pattern += r"(?=\n*(?:\S+|\Z))"
         return pattern
 
     def get_admonition_icon(self, admonition: dict) -> str:
         """Returns the icon to use for an admonition
 
         :param admonition: a dict of admonition data
         """
```

### Comparing `sphinx-readme-0.2.1/sphinx_readme/utils/docutils.py` & `sphinx-readme-0.2.2/sphinx_readme/utils/docutils.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.2.1/sphinx_readme/utils/git.py` & `sphinx-readme-0.2.2/sphinx_readme/utils/git.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.2.1/sphinx_readme/utils/linkcode.py` & `sphinx-readme-0.2.2/sphinx_readme/utils/linkcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.2.1/sphinx_readme/utils/rst.py` & `sphinx-readme-0.2.2/sphinx_readme/utils/rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.2.1/sphinx_readme/utils/sphinx.py` & `sphinx-readme-0.2.2/sphinx_readme/utils/sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.2.1/sphinx_readme.egg-info/PKG-INFO` & `sphinx-readme-0.2.2/sphinx_readme.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -17,15 +17,15 @@
 License-File: LICENSE
 
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_baseurl
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-html_context
 .. |.`~.parse_intersphinx_nodes`| replace:: ``parse_intersphinx_nodes()``
-.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.2.1/sphinx_readme/parser.py#L213-L237
+.. _.`~.parse_intersphinx_nodes`: https://github.com/TDKorn/sphinx-readme/blob/v0.2.2/sphinx_readme/parser.py#L216-L240
 .. |readme_docs_url_type| replace:: ``readme_docs_url_type``
 .. _readme_docs_url_type: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_docs_url_type
 .. |readme_inline_markup| replace:: ``readme_inline_markup``
 .. _readme_inline_markup: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_inline_markup
 .. |readme_raw_directive| replace:: ``readme_raw_directive``
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 .. |readme_replace_attrs| replace:: ``readme_replace_attrs``
@@ -43,15 +43,15 @@
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.1/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.2/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 
 
 
@@ -94,31 +94,32 @@
 
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
-.. csv-table::
-   :header: 📚 What's Sphinx README?
-
-   "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
-   to generate ``rst`` files that render beautifully on
-   GitHub, PyPi, GitLab, and BitBucket."
+.. list-table::
+   :header-rows: 1
+   
+   * - 📚 What's Sphinx README?
+   * - ``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
+       to generate ``rst`` files that render beautifully on
+       GitHub, PyPi, GitLab, and BitBucket.
 
 
 
 **With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.1/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.2.2/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 📋 Features
 ~~~~~~~~~~~~
 
@@ -191,18 +192,19 @@
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
-.. csv-table::
-   :header: 📢 Important
-
-   "Filepaths should be specified relative to the source directory"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📢 Important
+   * - Filepaths should be specified relative to the source directory
 
 
 |
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
@@ -216,21 +218,22 @@
 
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
    **Example**: |parse_intersphinx_nodes_html|_
 
 
-.. csv-table::
-   :header: 📝 Note
-
-   "If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
-
-   * Instead, they'll be replaced with ``inline literals`` or left as is
-   * Please see |readme_replace_attrs|_ and |readme_inline_markup|_"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📝 Note
+   * - If set to ``code``, then :code:`:attr:` cross-references will not be replaced with links
+    
+       * Instead, they'll be replaced with ``inline literals`` or left as is
+       * Please see |readme_replace_attrs|_ and |readme_inline_markup|_
 
 
 
 .. |parse_intersphinx_nodes_html| replace:: ``parse_intersphinx_nodes()``
 .. _parse_intersphinx_nodes_html: http://sphinx-readme.readthedocs.io/en/latest/parser.html#sphinx_readme.parser.READMEParser.parse_intersphinx_nodes
 
 
@@ -254,23 +257,24 @@
    readme_src_files = "README.rst"
 
    readme_docs_url_type = "code"
 
 
 
 
-.. csv-table::
-   :header: 📢 Important
-
-   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
-   be sure to disable |readme_raw_directive|_:
-
-   .. code-block:: python
-
-      readme_raw_directive = False"
+.. list-table::
+   :header-rows: 1
+   
+   * - 📢 Important
+   * - For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
+       be sure to disable |readme_raw_directive|_:
+    
+       .. code-block:: python
+    
+          readme_raw_directive = False
 
 
 
 
 📚 Documentation
 ~~~~~~~~~~~~~~~~
```

