# Comparing `tmp/omnivoreql-0.1.5.tar.gz` & `tmp/omnivoreql-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivoreql-0.1.5.tar", last modified: Thu Jul  6 07:47:01 2023, max compression
+gzip compressed data, was "omnivoreql-0.1.6.tar", last modified: Sun Jul  9 09:10:35 2023, max compression
```

## Comparing `omnivoreql-0.1.5.tar` & `omnivoreql-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:47:01.258224 omnivoreql-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-06 07:46:57.000000 omnivoreql-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-06 07:46:57.000000 omnivoreql-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-06 07:47:01.258224 omnivoreql-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-06 07:46:57.000000 omnivoreql-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:47:01.258224 omnivoreql-0.1.5/omnivoreql/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 07:46:57.000000 omnivoreql-0.1.5/omnivoreql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-06 07:46:57.000000 omnivoreql-0.1.5/omnivoreql/omnivoreql.py
--rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-06 07:46:57.000000 omnivoreql-0.1.5/omnivoreql/schema.gql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:47:01.258224 omnivoreql-0.1.5/omnivoreql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-06 07:47:01.000000 omnivoreql-0.1.5/omnivoreql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 07:47:01.000000 omnivoreql-0.1.5/omnivoreql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:47:01.000000 omnivoreql-0.1.5/omnivoreql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 07:47:01.000000 omnivoreql-0.1.5/omnivoreql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 07:47:01.000000 omnivoreql-0.1.5/omnivoreql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-06 07:46:57.000000 omnivoreql-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 07:47:01.258224 omnivoreql-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-06 07:46:57.000000 omnivoreql-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:10:35.201529 omnivoreql-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-09 09:10:29.000000 omnivoreql-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-09 09:10:29.000000 omnivoreql-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-09 09:10:35.201529 omnivoreql-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-09 09:10:29.000000 omnivoreql-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:10:35.201529 omnivoreql-0.1.6/omnivoreql/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-09 09:10:29.000000 omnivoreql-0.1.6/omnivoreql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-07-09 09:10:29.000000 omnivoreql-0.1.6/omnivoreql/omnivoreql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-09 09:10:29.000000 omnivoreql-0.1.6/omnivoreql/schema.gql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 09:10:35.201529 omnivoreql-0.1.6/omnivoreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-09 09:10:35.000000 omnivoreql-0.1.6/omnivoreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-09 09:10:35.000000 omnivoreql-0.1.6/omnivoreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 09:10:35.000000 omnivoreql-0.1.6/omnivoreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-09 09:10:35.000000 omnivoreql-0.1.6/omnivoreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 09:10:35.000000 omnivoreql-0.1.6/omnivoreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-09 09:10:29.000000 omnivoreql-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 09:10:35.201529 omnivoreql-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-09 09:10:29.000000 omnivoreql-0.1.6/setup.py
```

### Comparing `omnivoreql-0.1.5/LICENSE` & `omnivoreql-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.5/PKG-INFO` & `omnivoreql-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.1.5
+Version: 0.1.6
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
```

### Comparing `omnivoreql-0.1.5/README.md` & `omnivoreql-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.5/omnivoreql/omnivoreql.py` & `omnivoreql-0.1.6/omnivoreql/omnivoreql.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,19 +109,19 @@
                     }
                 }
                 }
             """
         )
         return self.client.execute(query)
 
-    def search_articles(self, first: int = None, after: int = None, query: str = None):
+    def get_articles(self, limit: int = None, cursor: str = None, format: str = 'markdown', query: str = "in:inbox", include_content: bool = False):
         q = gql(
             """
-            query Search($after: String, $first: Int, $query: String) {
-                search(first: $first, after: $after, query: $query) {
+            query Search($after: String, $first: Int, $query: String, $format: String, $includeContent: Boolean) {
+                search(after: $after, first: $first, query: $query, format: $format, includeContent: $includeContent) {
                     ... on SearchSuccess {
                         edges {
                             cursor
                             node {
                                 id
                                 title
                                 slug
@@ -207,25 +207,23 @@
                     color
                     createdAt
                 }
             }
         """
         )
         return self.client.execute(
-            q, variable_values={"first": first, "after": after, "query": query}
+            q, variable_values={
+                "first": limit, "after": cursor, "query": query, "format": format, "includeContent": include_content}
         )
 
-    def get_articles(self, first: int = None, after: int = None):
-        return self.search_articles(first, after)
-
-    def get_article(self, username: str, slug: str, include_friends_highlights: bool = False):
+    def get_article(self, username: str, slug: str, format: str = None, include_friends_highlights: bool = False):
         query = gql(
             """
-            query GetArticle($username: String!, $slug: String!, $includeFriendsHighlights: Boolean) {
-                article(username: $username, slug: $slug) {
+            query GetArticle($username: String!, $slug: String!, $format: String, $includeFriendsHighlights: Boolean) {
+                article(username: $username, slug: $slug, format: $format) {
                     ... on ArticleSuccess {
                         article {
                             ...ArticleFields
                             content
                             highlights(input: { includeFriends: $includeFriendsHighlights }) {
                                 ...HighlightFields
                             }
@@ -311,10 +309,63 @@
         """
         )
         return self.client.execute(
             query,
             variable_values={
                 "username": username,
                 "slug": slug,
-                "includeFriendsHighlights": include_friends_highlights,
+                "format": format,
             },
         )
+
+    def archive_article(self, article_id: str, toArchive: bool = True):
+        mutation = gql(
+            """
+        mutation SetLinkArchived($input: ArchiveLinkInput!) {
+            setLinkArchived(input: $input) {
+                    ... on ArchiveLinkSuccess {
+                        linkId
+                        message
+                    }
+                    ... on ArchiveLinkError {
+                        errorCodes
+                        message
+                    }
+                }
+            }
+        """)
+        return self.client.execute(
+            mutation,
+            variable_values={
+                "input": {
+                    "linkId": article_id,
+                    "archived": toArchive
+                }
+            }
+        )
+
+    def unarchive_article(self, article_id: str):
+        return self.archive_article(article_id, False)
+
+    def delete_article(self, article_id: str):
+        mutation = gql("""
+            mutation SetBookmarkArticle($input: SetBookmarkArticleInput!) {
+                setBookmarkArticle(input: $input) {
+                    ... on SetBookmarkArticleSuccess {
+                        bookmarkedArticle {
+                            id
+                        }
+                    }
+                    ... on SetBookmarkArticleError {
+                        errorCodes
+                    }
+                }
+            }""")
+        return self.client.execute(
+            mutation,
+            variable_values= {
+                "input": {
+                    "articleID": article_id,
+                    "bookmark": False
+                }
+            }
+        )
```

### Comparing `omnivoreql-0.1.5/omnivoreql/schema.gql` & `omnivoreql-0.1.6/omnivoreql/schema.gql`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.5/omnivoreql.egg-info/PKG-INFO` & `omnivoreql-0.1.6/omnivoreql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.1.5
+Version: 0.1.6
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
```

### Comparing `omnivoreql-0.1.5/setup.py` & `omnivoreql-0.1.6/setup.py`

 * *Files identical despite different names*

