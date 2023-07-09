# Comparing `tmp/pydelorean-1.1.0.tar.gz` & `tmp/pydelorean-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-1.1.0.tar", last modified: Thu Jul  6 11:16:54 2023, max compression
+gzip compressed data, was "pydelorean-1.3.4.tar", last modified: Sun Jul  9 03:07:34 2023, max compression
```

## Comparing `pydelorean-1.1.0.tar` & `pydelorean-1.3.4.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 pydelorean-1.1.0/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2551 2023-07-06 11:16:54.113550 pydelorean-1.1.0/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2108 2023-06-12 11:33:27.000000 pydelorean-1.1.0/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1947 2023-07-03 11:53:35.000000 pydelorean-1.1.0/pydelorean/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3897 2023-07-03 11:53:12.000000 pydelorean-1.1.0/pydelorean/delorean.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-12 11:33:27.000000 pydelorean-1.1.0/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1672 2023-07-03 11:09:36.000000 pydelorean-1.1.0/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6017 2023-07-06 10:23:48.000000 pydelorean-1.1.0/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean/tools/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2602 2023-07-06 11:15:07.000000 pydelorean-1.1.0/pydelorean/tools/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       42 2023-07-04 11:20:36.000000 pydelorean-1.1.0/pydelorean/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1509 2023-07-04 11:22:10.000000 pydelorean-1.1.0/pydelorean/tree/forest.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1916 2023-07-03 11:09:58.000000 pydelorean-1.1.0/pydelorean/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      245 2023-06-21 00:15:53.000000 pydelorean-1.1.0/pydelorean/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2551 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      455 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-06 11:16:54.113550 pydelorean-1.1.0/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      971 2023-07-06 11:16:39.000000 pydelorean-1.1.0/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.465197 pydelorean-1.3.4/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-1.3.4/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2340 2023-07-09 03:07:34.465197 pydelorean-1.3.4/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1916 2023-07-09 02:55:02.000000 pydelorean-1.3.4/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.462197 pydelorean-1.3.4/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1572 2023-07-09 03:00:29.000000 pydelorean-1.3.4/pydelorean/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4186 2023-07-09 02:52:51.000000 pydelorean-1.3.4/pydelorean/delorean.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.464197 pydelorean-1.3.4/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-10 12:14:10.000000 pydelorean-1.3.4/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1647 2023-07-09 02:54:21.000000 pydelorean-1.3.4/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6011 2023-07-09 02:53:43.000000 pydelorean-1.3.4/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.464197 pydelorean-1.3.4/pydelorean/tools/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2533 2023-07-09 02:44:26.000000 pydelorean-1.3.4/pydelorean/tools/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.465197 pydelorean-1.3.4/pydelorean/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-09 02:51:08.000000 pydelorean-1.3.4/pydelorean/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1495 2023-07-09 02:52:16.000000 pydelorean-1.3.4/pydelorean/tree/forest.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1917 2023-07-09 02:43:36.000000 pydelorean-1.3.4/pydelorean/tree/node.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      329 2023-07-09 02:43:36.000000 pydelorean-1.3.4/pydelorean/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.463197 pydelorean-1.3.4/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2340 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      475 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-09 03:07:34.000000 pydelorean-1.3.4/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-09 03:07:34.465197 pydelorean-1.3.4/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      971 2023-07-09 03:07:27.000000 pydelorean-1.3.4/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-09 03:07:34.465197 pydelorean-1.3.4/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1198 2023-06-11 13:13:52.000000 pydelorean-1.3.4/tests/test_mdtree.py
```

### Comparing `pydelorean-1.1.0/LICENSE` & `pydelorean-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-1.1.0/PKG-INFO` & `pydelorean-1.3.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.1.0
+Version: 1.3.4
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.3.4.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.1.0.zip
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -34,18 +33,15 @@
    pip install pydelorean
 
 You can find the library page here `here <nil>`__
 
 Quick Usage Guide
 -----------------
 
-delorean offers only one function ``treeify``, which generates a
-Python object from markup text. The object is a [treelib](https://github.com/caesar0301/treelib) Tree structure.
-
-Take, for example, the following markdown file.
+Check back later for this section.
 
 [[ chikin.md ]]
 
 .. code:: markdown
 
    # Chikin Tales
 
@@ -102,8 +98,7 @@
 3. Traverse and edit the Python data structure.
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
-
```

### Comparing `pydelorean-1.1.0/README.rst` & `pydelorean-1.3.4/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -21,18 +21,15 @@
    pip install pydelorean
 
 You can find the library page here `here <nil>`__
 
 Quick Usage Guide
 -----------------
 
-delorean offers only one function ``treeify``, which generates a
-Python object from markup text. The object is a [treelib](https://github.com/caesar0301/treelib) Tree structure.
-
-Take, for example, the following markdown file.
+Check back later for this section.
 
 [[ chikin.md ]]
 
 .. code:: markdown
 
    # Chikin Tales
```

### Comparing `pydelorean-1.1.0/pydelorean/__init__.py` & `pydelorean-1.3.4/pydelorean/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,13 @@
 from bs4 import BeautifulSoup
 from .delorean import mdtreeify, findMetadata
-from .tree.forest import MarkdownForest
+from .tree import Forest
 import re
 
-def treeify(name:str, md:str, *args, **kwargs) -> MarkdownForest:
-    """Converts a markdown document into a MarkdownForest object.
-
-    Args:
-        name (str, optional): Name of the document.
-        md (str, optional): Contents of the document.
-
-    Returns:
-        MarkdownForest: A forest representation of the markdown document.
-    """
+def treeify(name:str, md:str, *args, **kwargs) -> Forest:
     
     return mdtreeify(name, md, *args, **kwargs)
 
 # def markdownify(tree:MarkdownForest, *args, **kwargs) -> str:
 #     """_summary_
 
 #     Args:
@@ -25,17 +16,14 @@
 #     Returns:
 #         str: _description_
 #     """
     
 #     return mdtextify(tree, *args, **kwargs)
 
 def clean_markdown(md:str) -> str:
-    """
-    Cleans markdown file of bold and italics formatting.
-    """
         
     # Remove the metadata
     _, markdown_text = findMetadata(md)
     
      # Create a BeautifulSoup object with the input markdown text
     soup = BeautifulSoup(markdown_text, 'html.parser')
```

### Comparing `pydelorean-1.1.0/pydelorean/parser/parser.py` & `pydelorean-1.3.4/pydelorean/parser/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-from treelib import Tree
 from .utils import *
 
 class Parser:
     
     def __init__(self, document_name:str, text:str):
         self.document_name = document_name
         self.text = text
         
-    def parse(self) -> Tree:
+    def parse(self) -> Node:
         pass
 
    
 class MarkdownParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
-    def parse(self) -> Tree:
+    def parse(self) -> Node:
         HEADER_PATTERN = r"^(#+\s+)(.*)"
         
         tree = buildTree(self.text, self.document_name, header_pattern=HEADER_PATTERN)
         return tree
         
 
 class RestructuredParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
-    def parse(self) -> Tree:
+    def parse(self) -> Node:
         HEADER_PATTERN = r'^(\S.*)\n[=~`\'^"-]+$'
         
         tree = buildTree(self.text, self.document_name, header_pattern=HEADER_PATTERN)
         return tree
         
 
 class TextParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
-    def parse(self) -> Tree:
+    def parse(self) -> Node:
         pass
 
 
 class YAMLParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
-    def parse(self) -> Tree:
+    def parse(self) -> Node:
         pass
 
 
 class JSONParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
-    def parse(self) -> Tree:
+    def parse(self) -> Node:
         pass
     
 
 class XMLParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
-    def parse(self) -> Tree:
+    def parse(self) -> Node:
         pass
```

### Comparing `pydelorean-1.1.0/pydelorean/parser/utils.py` & `pydelorean-1.3.4/pydelorean/parser/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from pydelorean.tree import TextNode, HeaderNode
 from bigtree import Node, print_tree
 
-def buildTree(inputText:str, *args, **kwargs) -> HeaderNode:
+def buildTree(inputText:str, *args, **kwargs) -> Node:
     """ Function to build the provides tree varaible from the inputText. 
     Works for Github Flavored Markdown (GFM). 
 
     Args:
         inputText (str): Input text to be parsed
         name (Str): Name of the document
```

### Comparing `pydelorean-1.1.0/pydelorean/tools/__init__.py` & `pydelorean-1.3.4/pydelorean/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from bigtree import Node
-from pydelorean.tree.types import HeaderNode, TextNode
-from pydelorean import treeify
+from pydelorean.tree.node import TextNode
 
 def get_progressive_expansion(node, **kwargs) -> list:
     
     # BASE CASE: TextNode
     if isinstance(node, TextNode):
         return [(node.text, "")]
```

### Comparing `pydelorean-1.1.0/pydelorean/tree/forest.py` & `pydelorean-1.3.4/pydelorean/tree/forest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-from .types import HeaderNode
+from .node import HeaderNode
 
 
 class Forest:
     
     def __init__(self, root:HeaderNode, documentName:str="[document]", metadata:dict=None):
         self.documentName = documentName
         self.metadata = metadata
         self.root = root
-        self.treeCount = len(root.children('root'))
-        self.backlinks = []
-        self.tags = []
         
     # TODO: Implement __str__ and __len__ methods
     # FIGUREOUT: What other methods should this base class have ?
 
 
 class MarkdownForest:
     
@@ -53,7 +50,18 @@
         return self.tags
     
 
 # FIGUREOUT: Do we really need a forest for each of the supported formats ?
 class RestructuredForest:
     pass
 
+
+class AsciidocForest:
+    pass
+
+
+class YamlForest:
+    pass
+
+
+class JSONForest:
+    pass
```

### Comparing `pydelorean-1.1.0/pydelorean/tree/types.py` & `pydelorean-1.3.4/pydelorean/tree/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     def text(self):
         return self._text
     
     @text.setter
     def text(self, text:str):
         self._text = text
 
+
 class HeaderNode(Node):
     """_summary_
 
     Args:
         Node (_type_): _description_
     """
```

### Comparing `pydelorean-1.1.0/pydelorean.egg-info/PKG-INFO` & `pydelorean-1.3.4/pydelorean.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.1.0
+Version: 1.3.4
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.3.4.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.1.0.zip
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -34,18 +33,15 @@
    pip install pydelorean
 
 You can find the library page here `here <nil>`__
 
 Quick Usage Guide
 -----------------
 
-delorean offers only one function ``treeify``, which generates a
-Python object from markup text. The object is a [treelib](https://github.com/caesar0301/treelib) Tree structure.
-
-Take, for example, the following markdown file.
+Check back later for this section.
 
 [[ chikin.md ]]
 
 .. code:: markdown
 
    # Chikin Tales
 
@@ -102,8 +98,7 @@
 3. Traverse and edit the Python data structure.
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
-
```

### Comparing `pydelorean-1.1.0/setup.py` & `pydelorean-1.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.1.0'
+VERSION = '1.3.4'
 DESCRIPTION = 'A package to convert between markup language documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
```

