# Comparing `tmp/md2cf-2.1.0.tar.gz` & `tmp/md2cf-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/md2cf-2.1.0.tar", last modified: Mon Mar 13 14:34:00 2023, max compression
+gzip compressed data, was "dist/md2cf-2.2.0.tar", last modified: Sun Jul  9 01:00:17 2023, max compression
```

## Comparing `md2cf-2.1.0.tar` & `md2cf-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:34:00.000000 md2cf-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-03-13 14:34:00.000000 md2cf-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-03-13 14:33:58.000000 md2cf-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:34:00.000000 md2cf-2.1.0/md2cf/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26703 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/confluence_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/ignored_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/tui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-03-13 14:33:58.000000 md2cf-2.1.0/md2cf/upsert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 14:34:00.000000 md2cf-2.1.0/md2cf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-03-13 14:34:00.000000 md2cf-2.1.0/md2cf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-13 14:34:00.000000 md2cf-2.1.0/md2cf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 14:34:00.000000 md2cf-2.1.0/md2cf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-13 14:34:00.000000 md2cf-2.1.0/md2cf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-13 14:34:00.000000 md2cf-2.1.0/md2cf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-13 14:34:00.000000 md2cf-2.1.0/md2cf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 14:34:00.000000 md2cf-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-13 14:33:58.000000 md2cf-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:00:17.000000 md2cf-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-09 01:00:17.000000 md2cf-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-09 01:00:11.000000 md2cf-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27089 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/confluence_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/ignored_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/tui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-09 01:00:11.000000 md2cf-2.2.0/md2cf/upsert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-09 01:00:16.000000 md2cf-2.2.0/md2cf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 01:00:16.000000 md2cf-2.2.0/md2cf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 01:00:17.000000 md2cf-2.2.0/md2cf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 01:00:17.000000 md2cf-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-09 01:00:11.000000 md2cf-2.2.0/setup.py
```

### Comparing `md2cf-2.1.0/PKG-INFO` & `md2cf-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2cf
-Version: 2.1.0
+Version: 2.2.0
 Summary: Convert Markdown documents to Confluence
 Home-page: https://github.com/iamjackg/md2cf
 Author: Jack Gaino
 Author-email: md2cf@jackgaino.com
 License: MIT
 Description: # md2cf
         
@@ -169,14 +169,23 @@
         
         To avoid re-uploading unchanged content and receiving update emails when there are no changes, consider using the `--only-changed` option. Keep in mind that this option will include a hash of the page or attachment contents in the version update message.
         
         ## Linking to other documents (relative links)
         
         By default, support for relative links is disabled. To enable it, pass the `--enable-relative-links` flag. The behavior of relative links is similar to [GitHub relative links](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes#relative-links-and-image-paths-in-readme-files), with the exception that links starting with `/` are **not supported** and will be left unchanged.
         
+        Reference to a section from another file is possible using Markdown fragment link navigation:
+        ` [link](./file.md#section-name) // note the dash!`
+        
+        In file.md:
+        ```
+        ## ...
+        ## section name
+        ```
+        
         > :warning: Enabling this function requires two uploads for every page containing relative links. First, a page must be uploaded to Confluence with all internal links replaced by placeholders. Then, once the final Confluence link is known, the placeholders will be replaced with the appropriate links.
         
         By default, relative links that point to non-existent files (or files that are not being uploaded in the current batch) will result in an error. To ignore these errors and keep the links as they are, use the `--ignore-relative-link-errors` flag.
         
         ## Directory arguments
         
         ### Uploading Folders Recursively
```

### Comparing `md2cf-2.1.0/README.md` & `md2cf-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,23 @@
 
 To avoid re-uploading unchanged content and receiving update emails when there are no changes, consider using the `--only-changed` option. Keep in mind that this option will include a hash of the page or attachment contents in the version update message.
 
 ## Linking to other documents (relative links)
 
 By default, support for relative links is disabled. To enable it, pass the `--enable-relative-links` flag. The behavior of relative links is similar to [GitHub relative links](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes#relative-links-and-image-paths-in-readme-files), with the exception that links starting with `/` are **not supported** and will be left unchanged.
 
+Reference to a section from another file is possible using Markdown fragment link navigation:
+` [link](./file.md#section-name) // note the dash!`
+
+In file.md:
+```
+## ...
+## section name
+```
+
 > :warning: Enabling this function requires two uploads for every page containing relative links. First, a page must be uploaded to Confluence with all internal links replaced by placeholders. Then, once the final Confluence link is known, the placeholders will be replaced with the appropriate links.
 
 By default, relative links that point to non-existent files (or files that are not being uploaded in the current batch) will result in an error. To ignore these errors and keep the links as they are, use the `--ignore-relative-link-errors` flag.
 
 ## Directory arguments
 
 ### Uploading Folders Recursively
```

### Comparing `md2cf-2.1.0/md2cf/__main__.py` & `md2cf-2.2.0/md2cf/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -580,29 +580,33 @@
                 link_absolute_path = (
                     page.file_path.parent / Path(link_data.path)
                 ).resolve()
                 page_on_confluence = path_to_page[link_absolute_path]
             except KeyError:
                 if args.ignore_relative_link_errors:
                     page.body = page.body.replace(
-                        link_data.replacement, link_data.escaped_original
+                        link_data.replacement,
+                        link_data.escaped_original
+                        + (("#" + link_data.fragment) if link_data.fragment else ""),
                     )
                     continue
                 else:
                     error_console.log(
                         f"Page {page.file_path} has a relative link to {link_data.path}"
                         ", which was not uploaded correctly.\n"
                     )
                     break
 
             # in a dry run we don't actually have page URLs since we never upload
             # anything
             if not args.dry_run:
                 page.body = page.body.replace(
-                    link_data.replacement, confluence.get_url(page_on_confluence)
+                    link_data.replacement,
+                    confluence.get_url(page_on_confluence)
+                    + (("#" + link_data.fragment) if link_data.fragment else ""),
                 )
             page_modified = True
 
         if page_modified:
             tui.reset_item_task(page.original_title, total=1)
             tui.set_item_progress_label(page.original_title, "Updating relative links")
             tui.start_item_task(page.original_title)
@@ -702,26 +706,29 @@
 
         if len(pages_to_upload) == 1:
             only_page = pages_to_upload[0]
 
             if args.title:
                 only_page.title = args.title
 
-            # This is implicitly only here if relative link processing is active
+            # This is implicitly only truthy if relative link processing is active
             if only_page.relative_links:
                 # This covers the last edge case where directory processing leaves us
-                # with only one page, which we can't anticipate.
+                # with only one page, which we can't anticipate at startup time.
                 # In this case, we have to restore all the links to their original
                 # values.
                 error_console.log(
                     "Relative links are ignored when there's a single page\n"
                 )
                 for link_data in only_page.relative_links:
                     only_page.body.replace(
-                        link_data.replacement, link_data.escaped_original
+                        link_data.replacement,
+                        link_data.escaped_original
+                        + (("#" + link_data.fragment) if link_data.fragment else ""),
                     )
+                only_page.relative_links = []
 
     return pages_to_upload
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `md2cf-2.1.0/md2cf/api.py` & `md2cf-2.2.0/md2cf/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,26 +220,25 @@
         if existing_attachments.size:
             return existing_attachments.results[0]
 
     def update_attachment(self, confluence_page, fp, existing_attachment, message=""):
         return self._post(
             f"content/{confluence_page.id}/child/attachment/{existing_attachment.id}/"
             f"data",
-            json={"comment": message} if message else None,
             headers={"X-Atlassian-Token": "nocheck"},
-            files={"file": fp},
+            files={"file": fp, "comment": message if message else None},
         )
 
     def create_attachment(self, confluence_page, fp, message=""):
         return self._post(
             f"content/{confluence_page.id}/child/attachment",
             json={"comment": message} if message else None,
             headers={"X-Atlassian-Token": "nocheck"},
             params={"allowDuplicated": "true"},
-            files={"file": fp},
+            files={"file": fp, "comment": message if message else None},
         )
 
     def add_labels(self, page, labels):
         # return self.api.content(page.id).post(
         return self._post(
             f"content/{page.id}/label",
             data=[{"name": label, "type": "global"} for label in labels],
```

### Comparing `md2cf-2.1.0/md2cf/confluence_renderer.py` & `md2cf-2.2.0/md2cf/confluence_renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import urllib.parse as urlparse
 import uuid
 from pathlib import Path
 from typing import List, NamedTuple
+from urllib.parse import unquote, urlparse
 
 import mistune
 
 
 class RelativeLink(NamedTuple):
     path: str
+    fragment: str
     replacement: str
     original: str
     escaped_original: str
 
 
 class ConfluenceTag(object):
     def __init__(self, name, text="", attrib=None, namespace="ac", cdata=False):
@@ -99,26 +100,27 @@
 
     def plain_text_body(self, text):
         body_tag = ConfluenceTag("plain-text-body", cdata=True)
         body_tag.text = text
         return body_tag
 
     def link(self, link, title, text):
-        parsed_link = urlparse.urlparse(link)
+        parsed_link = urlparse(link)
         if self.enable_relative_links and (
-            not parsed_link.scheme
-            and not parsed_link.netloc
-            and not parsed_link.fragment
+            not parsed_link.scheme and not parsed_link.netloc
         ):
             # relative link
             replacement_link = f"md2cf-internal-link-{uuid.uuid4()}"
             self.relative_links.append(
                 RelativeLink(
-                    path=parsed_link.path,
+                    # make sure to unquote the url as relative paths
+                    # might have escape sequences
+                    path=unquote(parsed_link.path),
                     replacement=replacement_link,
+                    fragment=parsed_link.fragment,
                     original=link,
                     escaped_original=mistune.escape_link(link),
                 )
             )
             link = replacement_link
         return super(ConfluenceRenderer, self).link(link, title, text)
 
@@ -139,15 +141,15 @@
 
     def image(self, src, title, text):
         attributes = {"alt": text}
         if title:
             attributes["title"] = title
 
         root_element = ConfluenceTag(name="image", attrib=attributes)
-        parsed_source = urlparse.urlparse(src)
+        parsed_source = urlparse(src)
         if not parsed_source.netloc:
             # Local file, requires upload
             basename = Path(src).name
             url_tag = ConfluenceTag(
                 "attachment", attrib={"filename": basename}, namespace="ri"
             )
             self.attachments.append(src)
```

### Comparing `md2cf-2.1.0/md2cf/document.py` & `md2cf-2.2.0/md2cf/document.py`

 * *Files 10% similar despite different names*

```diff
@@ -107,81 +107,89 @@
       search
     :param enable_relative_links: extract all relative links and replace them with
       placeholders
     :return: A list of paths to the markdown files to upload.
     """
     processed_pages = list()
     base_path = file_path.resolve()
-    parent_page_title = None
     folder_data = dict()
     git_repo = GitRepository(file_path, use_gitignore=use_gitignore)
 
     for current_path, directories, file_names in os.walk(file_path):
         current_path = Path(current_path).resolve()
 
+        if git_repo.is_ignored(current_path):
+            continue
+
         markdown_files = [
             Path(current_path, file_name)
             for file_name in file_names
             if file_name.endswith(".md")
         ]
         # Filter out ignored files
         markdown_files = [
             path for path in markdown_files if not git_repo.is_ignored(path)
         ]
 
-        folder_data[current_path] = {
-            "n_files": len(markdown_files),
-            "title": current_path.name if current_path != base_path else None,
-        }
-
-        if not markdown_files and not directories:
-            continue
+        folder_data[current_path] = {"n_files": len(markdown_files)}
 
-        if not markdown_files and (skip_empty or collapse_empty):
-            continue
+        # we'll capture title and path of the parent folder for this folder:
+        folder_parent_title = None
+        folder_parent_path = None
+
+        # title for this folder's page (as parent of its children):
+        parent_page_title = None
+        # title for the folder (same as above except when collapsing):
+        folder_title = None
 
         if current_path != base_path:
             # TODO: add support for .pages file to read folder title
             if skip_empty or collapse_empty:
                 folder_parent_path = find_non_empty_parent_path(
                     current_path, folder_data, default=file_path
                 )
             else:
                 folder_parent_path = current_path.parent
 
             folder_parent_title = folder_data[folder_parent_path]["title"]
+            parent_page_title = current_path.name
             if len(markdown_files) == 1 and collapse_single_pages:
                 parent_page_title = folder_parent_title
+                folder_title = None
             else:
                 if collapse_empty:
-                    folder_data[current_path]["title"] = str(
+                    parent_page_title = str(
                         current_path.relative_to(folder_parent_path)
                     )
                 if beautify_folders:
-                    folder_data[current_path]["title"] = (
-                        folder_data[current_path]["title"]
-                        .replace("-", " ")
+                    parent_page_title = (
+                        current_path.name.replace("-", " ")
                         .replace("_", " ")
                         .capitalize()
                     )
-                elif use_pages_file and ".pages" in file_names:
-                    with open(current_path.joinpath(".pages")) as pages_fp:
-                        pages_file_contents = yaml.safe_load(pages_fp)
-                    if "title" in pages_file_contents:
-                        folder_data[current_path]["title"] = pages_file_contents[
-                            "title"
-                        ]
-                parent_page_title = folder_data[current_path]["title"]
-                processed_pages.append(
-                    Page(
-                        title=parent_page_title,
-                        parent_title=folder_parent_title,
-                        body="",
-                    )
+                folder_title = parent_page_title
+        if use_pages_file and ".pages" in file_names:
+            with open(current_path.joinpath(".pages")) as pages_fp:
+                pages_file_contents = yaml.safe_load(pages_fp)
+            if "title" in pages_file_contents:
+                parent_page_title = pages_file_contents["title"]
+                folder_title = parent_page_title
+
+        folder_data[current_path]["title"] = folder_title
+
+        if folder_title is not None and (
+            markdown_files or (directories and not skip_empty and not collapse_empty)
+        ):
+            processed_pages.append(
+                Page(
+                    title=folder_title,
+                    parent_title=folder_parent_title,
+                    body="",
                 )
+            )
 
         for markdown_file in markdown_files:
             processed_page = get_page_data_from_file_path(
                 markdown_file,
                 strip_header=strip_header,
                 remove_text_newlines=remove_text_newlines,
                 enable_relative_links=enable_relative_links,
```

### Comparing `md2cf-2.1.0/md2cf/ignored_files.py` & `md2cf-2.2.0/md2cf/ignored_files.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.1.0/md2cf/tui.py` & `md2cf-2.2.0/md2cf/tui.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.1.0/md2cf/upsert.py` & `md2cf-2.2.0/md2cf/upsert.py`

 * *Files identical despite different names*

### Comparing `md2cf-2.1.0/md2cf.egg-info/PKG-INFO` & `md2cf-2.2.0/md2cf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2cf
-Version: 2.1.0
+Version: 2.2.0
 Summary: Convert Markdown documents to Confluence
 Home-page: https://github.com/iamjackg/md2cf
 Author: Jack Gaino
 Author-email: md2cf@jackgaino.com
 License: MIT
 Description: # md2cf
         
@@ -169,14 +169,23 @@
         
         To avoid re-uploading unchanged content and receiving update emails when there are no changes, consider using the `--only-changed` option. Keep in mind that this option will include a hash of the page or attachment contents in the version update message.
         
         ## Linking to other documents (relative links)
         
         By default, support for relative links is disabled. To enable it, pass the `--enable-relative-links` flag. The behavior of relative links is similar to [GitHub relative links](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes#relative-links-and-image-paths-in-readme-files), with the exception that links starting with `/` are **not supported** and will be left unchanged.
         
+        Reference to a section from another file is possible using Markdown fragment link navigation:
+        ` [link](./file.md#section-name) // note the dash!`
+        
+        In file.md:
+        ```
+        ## ...
+        ## section name
+        ```
+        
         > :warning: Enabling this function requires two uploads for every page containing relative links. First, a page must be uploaded to Confluence with all internal links replaced by placeholders. Then, once the final Confluence link is known, the placeholders will be replaced with the appropriate links.
         
         By default, relative links that point to non-existent files (or files that are not being uploaded in the current batch) will result in an error. To ignore these errors and keep the links as they are, use the `--ignore-relative-link-errors` flag.
         
         ## Directory arguments
         
         ### Uploading Folders Recursively
```

### Comparing `md2cf-2.1.0/setup.py` & `md2cf-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="md2cf",
-    version="2.1.0",
+    version="2.2.0",
     packages=["md2cf"],
     url="https://github.com/iamjackg/md2cf",
     license="MIT",
     author="Jack Gaino",
     author_email="md2cf@jackgaino.com",
     description="Convert Markdown documents to Confluence",
     long_description=long_description,
@@ -21,14 +21,14 @@
     ],
     keywords="markdown confluence",
     install_requires=[
         "rich-argparse==1.0.0",
         "rich==13.0.1",
         "mistune==0.8.4",
         "chardet==5.1.0",
-        "requests==2.28.2",
+        "requests==2.31.0",
         "PyYAML==6.0",
         "gitignorefile==1.1.2",
     ],
     python_requires=">=3.7",
     entry_points={"console_scripts": ["md2cf=md2cf.__main__:main"]},
 )
```

