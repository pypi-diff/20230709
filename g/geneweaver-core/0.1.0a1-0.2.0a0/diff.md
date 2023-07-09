# Comparing `tmp/geneweaver_core-0.1.0a1.tar.gz` & `tmp/geneweaver_core-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_core-0.1.0a1.tar", max compression
+gzip compressed data, was "geneweaver_core-0.2.0a0.tar", max compression
```

## Comparing `geneweaver_core-0.1.0a1.tar` & `geneweaver_core-0.2.0a0.tar`

### file list

```diff
@@ -1,19 +1,36 @@
--rw-r--r--   0        0        0     1909 2023-03-22 12:59:10.822034 geneweaver_core-0.1.0a1/README.md
--rw-r--r--   0        0        0      660 2023-03-22 12:59:10.822034 geneweaver_core-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0       52 2023-03-22 12:59:10.822034 geneweaver_core-0.1.0a1/src/geneweaver/core/__init__.py
--rw-r--r--   0        0        0      172 2023-03-22 12:59:10.822034 geneweaver_core-0.1.0a1/src/geneweaver/core/config.py
--rw-r--r--   0        0        0      415 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/config_class.py
--rw-r--r--   0        0        0      702 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/enum.py
--rw-r--r--   0        0        0      189 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/exc.py
--rw-r--r--   0        0        0      302 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/__init__.py
--rw-r--r--   0        0        0      307 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/gene.py
--rw-r--r--   0        0        0     1308 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/geneset.py
--rw-r--r--   0        0        0      365 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/group.py
--rw-r--r--   0        0        0      921 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/legacy_api.py
--rw-r--r--   0        0        0      415 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/ontology.py
--rw-r--r--   0        0        0      231 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/project.py
--rw-r--r--   0        0        0      264 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/publication.py
--rw-r--r--   0        0        0      133 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/stubgenerator.py
--rw-r--r--   0        0        0      776 2023-03-22 12:59:10.826034 geneweaver_core-0.1.0a1/src/geneweaver/core/schema/user.py
--rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 geneweaver_core-0.1.0a1/setup.py
--rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 geneweaver_core-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-07 21:06:27.507278 geneweaver_core-0.2.0a0/LICENSE
+-rw-r--r--   0        0        0     2293 2023-07-09 16:24:42.461328 geneweaver_core-0.2.0a0/README.md
+-rw-r--r--   0        0        0      975 2023-07-09 16:25:03.999905 geneweaver_core-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-07-07 21:06:27.512998 geneweaver_core-0.2.0a0/src/geneweaver/core/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-07 21:06:27.518287 geneweaver_core-0.2.0a0/src/geneweaver/core/config.py
+-rw-r--r--   0        0        0      444 2023-07-07 21:06:27.519010 geneweaver_core-0.2.0a0/src/geneweaver/core/config_class.py
+-rw-r--r--   0        0        0     1119 2023-07-07 21:06:27.519663 geneweaver_core-0.2.0a0/src/geneweaver/core/enum.py
+-rw-r--r--   0        0        0      150 2023-07-07 21:06:27.520361 geneweaver_core-0.2.0a0/src/geneweaver/core/exc.py
+-rw-r--r--   0        0        0       49 2023-03-30 21:52:33.405429 geneweaver_core-0.2.0a0/src/geneweaver/core/fixtures/__init__.py
+-rw-r--r--   0        0        0    16646 2023-03-30 21:52:42.793539 geneweaver_core-0.2.0a0/src/geneweaver/core/fixtures/gene.py
+-rw-r--r--   0        0        0     3395 2023-03-30 21:52:59.273669 geneweaver_core-0.2.0a0/src/geneweaver/core/fixtures/species.py
+-rw-r--r--   0        0        0       53 2023-07-07 21:07:18.421064 geneweaver_core-0.2.0a0/src/geneweaver/core/parse/__init__.py
+-rw-r--r--   0        0        0    18323 2023-07-07 21:07:18.422072 geneweaver_core-0.2.0a0/src/geneweaver/core/parse/batch.py
+-rw-r--r--   0        0        0     5844 2023-07-06 20:48:07.516442 geneweaver_core-0.2.0a0/src/geneweaver/core/parse/csv.py
+-rw-r--r--   0        0        0      304 2023-07-07 21:07:24.176048 geneweaver_core-0.2.0a0/src/geneweaver/core/parse/enum.py
+-rw-r--r--   0        0        0     1455 2023-07-07 21:07:24.176650 geneweaver_core-0.2.0a0/src/geneweaver/core/parse/exceptions.py
+-rw-r--r--   0        0        0     9436 2023-07-07 21:07:18.423871 geneweaver_core-0.2.0a0/src/geneweaver/core/parse/score.py
+-rw-r--r--   0        0        0     1935 2023-07-07 15:50:24.608982 geneweaver_core-0.2.0a0/src/geneweaver/core/parse/utils.py
+-rw-r--r--   0        0        0     7322 2023-07-06 20:47:22.339725 geneweaver_core-0.2.0a0/src/geneweaver/core/parse/xlsx.py
+-rw-r--r--   0        0        0      338 2023-07-07 21:06:27.520894 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/__init__.py
+-rw-r--r--   0        0        0     1744 2023-07-07 21:07:18.425205 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/batch.py
+-rw-r--r--   0        0        0     1041 2023-07-07 21:06:27.521613 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/gene.py
+-rw-r--r--   0        0        0     2213 2023-07-07 21:06:27.522161 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/geneset.py
+-rw-r--r--   0        0        0      461 2023-07-07 21:06:27.522847 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/group.py
+-rw-r--r--   0        0        0     1217 2023-07-07 21:06:27.523472 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/legacy_api.py
+-rw-r--r--   0        0        0      831 2023-07-07 21:07:18.425899 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/messages.py
+-rw-r--r--   0        0        0      504 2023-07-07 21:06:27.524206 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/ontology.py
+-rw-r--r--   0        0        0      329 2023-07-07 21:06:27.525208 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/project.py
+-rw-r--r--   0        0        0      392 2023-07-07 21:06:27.525704 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/publication.py
+-rw-r--r--   0        0        0      465 2023-07-07 21:07:18.426455 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/score.py
+-rw-r--r--   0        0        0      489 2023-03-30 21:56:32.835515 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/species.py
+-rw-r--r--   0        0        0      211 2023-07-07 21:06:27.526193 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/stubgenerator.py
+-rw-r--r--   0        0        0      485 2023-03-30 21:55:58.119130 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/tools.py
+-rw-r--r--   0        0        0      932 2023-07-07 21:06:27.526702 geneweaver_core-0.2.0a0/src/geneweaver/core/schema/user.py
+-rw-r--r--   0        0        0      187 2023-07-06 20:28:04.832362 geneweaver_core-0.2.0a0/src/geneweaver/core/types.py
+-rw-r--r--   0        0        0     3061 1970-01-01 00:00:00.000000 geneweaver_core-0.2.0a0/PKG-INFO
```

### Comparing `geneweaver_core-0.1.0a1/README.md` & `geneweaver_core-0.2.0a0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -32,14 +32,23 @@
 
 
 * `geneweaver.core.exc`: Geneweaver shared exceptions
   * `GeneweaverException`: Base exception class for Geneweaver
   * `GeneweaverError`: Base error class for Geneweaver
   * `GeneweaverWarning`: Base warning class for Geneweaver
 
+* `geneweaver.core.pase`: Geneweaver file parsing functionality
+  * `batch`: Functions for parsing a batch file
+  * `score`: Functions for parsing a score
+  * `csv`: Functions for parsing a CSV file
+  * `xlsx`: Functions for parsing an Excel file
+  * `enum`: Enumerations for file parsing
+  * `exceptions`: Exceptions for file parsing
+  * `utils`: Utility functions for file parsing
+
 #### Planned Functionality
 * `geneweaver.core.logging`: Shared logging management
 * `geneweaver.core.utils`: Shared utility functions
 
 
 ## Acknowledgements
 This project was developed by the Computational Systems and Synthetic Biology Center at the Jackson Laboratory in
```

### Comparing `geneweaver_core-0.1.0a1/src/geneweaver/core/schema/geneset.py` & `geneweaver_core-0.2.0a0/src/geneweaver/core/schema/geneset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+"""Schemas for geneset."""
 import datetime
 from typing import List
-from pydantic import BaseModel, Field
 
-from geneweaver.core.enum import GenesetAccess
+from geneweaver.core.enum import GenesetAccess, GenesetScoreType
 from geneweaver.core.schema.gene import GeneValue
-from geneweaver.core.enum import GenesetScoreType
+from pydantic import BaseModel, Field
 
 
 class Geneset(BaseModel):
+    """Geneset schema."""
+
     name: str
     abbreviation: str
     description: str
     count: int
     threshold_type: int
     threshold: str
     gene_id_type: int
@@ -20,40 +22,85 @@
     updated: datetime.datetime
     status: str
     gsv_qual: str
     attribution: int
     is_edgelist: bool
 
 
+class GenesetGenes(BaseModel):
+    """Geneset genes schema."""
+
+    genes: List[GeneValue]
+
+
 class GenesetUpload(BaseModel):
+    """Geneset upload schema."""
+
     name: str
     label: str
-    score_type: GenesetScoreType = Field(..., alias='score-type')
+    score_type: GenesetScoreType = Field(..., alias="score-type")
     description: str
-    pubmed_id: str = Field(..., alias='pubmed-id')
+    pubmed_id: str = Field(..., alias="pubmed-id")
     access: GenesetAccess
     groups: List[str]
     species: str
-    gene_identifier: str = Field(..., alias='gene-identifier')
-    gene_list: List[GeneValue] = Field(..., alias='gene-list')
+    gene_identifier: str = Field(..., alias="gene-identifier")
+    gene_list: List[GeneValue] = Field(..., alias="gene-list")
 
 
 class BatchUpload(BaseModel):
+    """Batch upload schema."""
+
     batch_file: str
     curation_group: List[str]
 
 
 class GenesetInfo(BaseModel):
-    id: int
+    """Geneset info schema."""
+
+    id: int  # noqa: A003
     page_views: int
     referers: List[str]
     analyses: List[str]
     resource_id: int
     last_sim: str
     last_ann: str
     jac_started: str
     jac_completed: str
 
 
 class SimilarGeneset(Geneset):
+    """Schema for similar geneset relation."""
+
     jax_value: float
     gic_value: float
+
+
+class GenesetRow(BaseModel):
+    """Geneset schema for database row."""
+
+    gs_id: int
+    usr_id: int
+    file_id: int
+    gs_name: str
+    gs_abbreviation: str
+    pub_id: int
+    res_id: int
+    cur_id: int
+    gs_description: str
+    sp_id: int
+    gs_count: int
+    gs_threshold_type: int
+    gs_threshold: str
+    gs_groups: str
+    gs_attribution_old: str
+    gs_uri: str
+    gs_gene_id_type: int
+    gs_created: datetime.date
+    admin_flag: str
+    gs_updated: datetime.datetime
+    gs_status: str
+    gsv_qual: str
+    _comments_author: str
+    _comments_curator: str
+    gs_attribution: int
+    gs_is_edgelist: bool
```

### Comparing `geneweaver_core-0.1.0a1/src/geneweaver/core/schema/user.py` & `geneweaver_core-0.2.0a0/src/geneweaver/core/schema/user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+"""User related schemas."""
 import datetime
 from typing import List, Optional
-from pydantic import BaseModel
 
-from geneweaver.core.schema.stubgenerator import StubGenerator
 from geneweaver.core.enum import AdminLevel
+from geneweaver.core.schema.stubgenerator import StubGenerator
+from pydantic import BaseModel
 
 
 class UserRequiredFields(BaseModel):
-    id: int
+    """User schema for required fields."""
+
+    id: int  # noqa: A003
     email: str
     prefs: str = "{}"
     is_guest: bool = False
 
 
 class User(UserRequiredFields):
+    """User schema."""
+
     first_name: Optional[str] = None
     last_name: Optional[str] = None
     password: Optional[str] = None
     admin: AdminLevel = AdminLevel.NORMAL_USER
     last_seen: Optional[datetime.datetime] = None
     create: Optional[datetime.date] = None
     ip_address: Optional[str] = None
     api_key: Optional[str] = None
     sso_id: Optional[str] = None
 
 
 class UserFull(User):
+    """User schema with full information."""
+
     groups: List[str]
     stubgenerators: List[StubGenerator]
```

### Comparing `geneweaver_core-0.1.0a1/PKG-INFO` & `geneweaver_core-0.2.0a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: geneweaver-core
-Version: 0.1.0a1
+Version: 0.2.0a0
 Summary: The core of the Jax-Geneweaver Python library
+Home-page: https://bergsalex.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax & Baylor Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic[dotenv] (>=1.10.5,<2.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
+Project-URL: Repository, https://bitbucket.org/jacksonlaboratory/geneweaver-core
 Description-Content-Type: text/markdown
 
 # Geneweaver Core
 The Geneweaver Core Python library provides shared foundational functionality for the Geneweaver project. 
 It is a dependency of all other Geneweaver Python libraries, and is not intended to be used directly.
 
 ## Installation
@@ -48,14 +51,23 @@
 
 
 * `geneweaver.core.exc`: Geneweaver shared exceptions
   * `GeneweaverException`: Base exception class for Geneweaver
   * `GeneweaverError`: Base error class for Geneweaver
   * `GeneweaverWarning`: Base warning class for Geneweaver
 
+* `geneweaver.core.pase`: Geneweaver file parsing functionality
+  * `batch`: Functions for parsing a batch file
+  * `score`: Functions for parsing a score
+  * `csv`: Functions for parsing a CSV file
+  * `xlsx`: Functions for parsing an Excel file
+  * `enum`: Enumerations for file parsing
+  * `exceptions`: Exceptions for file parsing
+  * `utils`: Utility functions for file parsing
+
 #### Planned Functionality
 * `geneweaver.core.logging`: Shared logging management
 * `geneweaver.core.utils`: Shared utility functions
 
 
 ## Acknowledgements
 This project was developed by the Computational Systems and Synthetic Biology Center at the Jackson Laboratory in
```

