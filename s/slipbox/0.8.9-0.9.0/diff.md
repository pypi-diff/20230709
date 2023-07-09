# Comparing `tmp/slipbox-0.8.9.tar.gz` & `tmp/slipbox-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slipbox-0.8.9.tar", last modified: Sun Aug 16 14:06:22 2020, max compression
+gzip compressed data, was "dist/slipbox-0.9.0.tar", last modified: Mon Aug 24 09:11:02 2020, max compression
```

## Comparing `slipbox-0.8.9.tar` & `slipbox-0.9.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-16 14:06:22.337353 slipbox-0.8.9/
--rw-r--r--   0 levi      (1000) levi      (1000)     1994 2020-08-16 14:06:22.337353 slipbox-0.8.9/PKG-INFO
--rw-r--r--   0 levi      (1000) levi      (1000)     1063 2020-08-11 10:52:03.000000 slipbox-0.8.9/README.md
--rw-r--r--   0 levi      (1000) levi      (1000)       38 2020-08-16 14:06:22.337353 slipbox-0.8.9/setup.cfg
--rw-r--r--   0 levi      (1000) levi      (1000)      775 2020-08-16 14:05:55.000000 slipbox-0.8.9/setup.py
-drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-16 14:06:22.334019 slipbox-0.8.9/slipbox/
--rw-r--r--   0 levi      (1000) levi      (1000)        0 2020-07-27 04:23:14.000000 slipbox-0.8.9/slipbox/__init__.py
--rw-r--r--   0 levi      (1000) levi      (1000)     1589 2020-08-11 10:35:31.000000 slipbox-0.8.9/slipbox/__main__.py
--rw-r--r--   0 levi      (1000) levi      (1000)      487 2020-08-11 10:22:14.000000 slipbox-0.8.9/slipbox/config.py
--rw-r--r--   0 levi      (1000) levi      (1000)      758 2020-08-11 09:59:22.000000 slipbox-0.8.9/slipbox/conftest.py
-drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-16 14:06:22.334019 slipbox-0.8.9/slipbox/data/
--rw-r--r--   0 levi      (1000) levi      (1000)    17953 2020-08-16 14:06:01.000000 slipbox-0.8.9/slipbox/data/bundle.js
--rw-r--r--   0 levi      (1000) levi      (1000)     3045 2020-08-10 04:36:21.000000 slipbox-0.8.9/slipbox/data.py
-drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-16 14:06:22.337353 slipbox-0.8.9/slipbox/filters/
--rw-r--r--   0 levi      (1000) levi      (1000)      409 2020-07-27 03:57:42.000000 slipbox-0.8.9/slipbox/filters/base64.lua
--rw-r--r--   0 levi      (1000) levi      (1000)      601 2020-08-09 15:26:02.000000 slipbox-0.8.9/slipbox/filters/csv.lua
--rw-r--r--   0 levi      (1000) levi      (1000)     4884 2020-08-16 13:05:42.000000 slipbox-0.8.9/slipbox/filters/filters.lua
--rw-r--r--   0 levi      (1000) levi      (1000)      519 2020-08-04 13:45:06.000000 slipbox-0.8.9/slipbox/filters/footnotes.lua
--rw-r--r--   0 levi      (1000) levi      (1000)      880 2020-07-27 03:57:42.000000 slipbox-0.8.9/slipbox/filters/images.lua
--rw-r--r--   0 levi      (1000) levi      (1000)      492 2020-08-07 05:41:51.000000 slipbox-0.8.9/slipbox/filters/log.lua
--rw-r--r--   0 levi      (1000) levi      (1000)     1493 2020-08-09 14:08:44.000000 slipbox-0.8.9/slipbox/filters/refs.lua
--rw-r--r--   0 levi      (1000) levi      (1000)     2132 2020-08-16 12:57:11.000000 slipbox-0.8.9/slipbox/filters/scan.lua
--rw-r--r--   0 levi      (1000) levi      (1000)     6905 2020-08-16 13:01:29.000000 slipbox-0.8.9/slipbox/filters/slipbox.lua
--rw-r--r--   0 levi      (1000) levi      (1000)     2401 2020-08-12 03:33:05.000000 slipbox-0.8.9/slipbox/filters/utils.lua
--rw-r--r--   0 levi      (1000) levi      (1000)     5610 2020-08-12 03:33:05.000000 slipbox-0.8.9/slipbox/filters/utils.test.lua
--rw-r--r--   0 levi      (1000) levi      (1000)     1038 2020-08-16 12:36:23.000000 slipbox-0.8.9/slipbox/filters/zk.lua
--rw-r--r--   0 levi      (1000) levi      (1000)     7309 2020-08-16 13:33:09.000000 slipbox-0.8.9/slipbox/page.py
--rw-r--r--   0 levi      (1000) levi      (1000)     4220 2020-08-11 10:27:56.000000 slipbox-0.8.9/slipbox/pandoc.css
--rw-r--r--   0 levi      (1000) levi      (1000)     5656 2020-08-10 13:08:43.000000 slipbox-0.8.9/slipbox/scan.py
--rw-r--r--   0 levi      (1000) levi      (1000)     1830 2020-08-09 11:59:47.000000 slipbox-0.8.9/slipbox/schema.sql
--rw-r--r--   0 levi      (1000) levi      (1000)     4724 2020-08-11 09:53:29.000000 slipbox-0.8.9/slipbox/slipbox.py
--rw-r--r--   0 levi      (1000) levi      (1000)      884 2020-08-04 10:25:10.000000 slipbox-0.8.9/slipbox/templates.py
--rw-r--r--   0 levi      (1000) levi      (1000)      330 2020-08-10 04:15:38.000000 slipbox-0.8.9/slipbox/test_data.py
--rw-r--r--   0 levi      (1000) levi      (1000)     2697 2020-08-04 15:21:01.000000 slipbox-0.8.9/slipbox/test_page.py
--rw-r--r--   0 levi      (1000) levi      (1000)    11724 2020-08-16 13:17:46.000000 slipbox-0.8.9/slipbox/test_scan.py
--rw-r--r--   0 levi      (1000) levi      (1000)     5775 2020-08-12 03:33:05.000000 slipbox-0.8.9/slipbox/test_slipbox.py
--rw-r--r--   0 levi      (1000) levi      (1000)      768 2020-08-04 11:20:44.000000 slipbox-0.8.9/slipbox/test_templates.py
--rw-r--r--   0 levi      (1000) levi      (1000)     1743 2020-08-04 12:52:27.000000 slipbox-0.8.9/slipbox/test_utils.py
--rw-r--r--   0 levi      (1000) levi      (1000)     1449 2020-08-10 12:07:55.000000 slipbox-0.8.9/slipbox/utils.py
-drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-16 14:06:22.334019 slipbox-0.8.9/slipbox.egg-info/
--rw-r--r--   0 levi      (1000) levi      (1000)     1994 2020-08-16 14:06:21.000000 slipbox-0.8.9/slipbox.egg-info/PKG-INFO
--rw-r--r--   0 levi      (1000) levi      (1000)      839 2020-08-16 14:06:21.000000 slipbox-0.8.9/slipbox.egg-info/SOURCES.txt
--rw-r--r--   0 levi      (1000) levi      (1000)        1 2020-08-16 14:06:21.000000 slipbox-0.8.9/slipbox.egg-info/dependency_links.txt
--rw-r--r--   0 levi      (1000) levi      (1000)        8 2020-08-16 14:06:21.000000 slipbox-0.8.9/slipbox.egg-info/top_level.txt
+drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-24 09:11:02.230933 slipbox-0.9.0/
+-rw-r--r--   0 levi      (1000) levi      (1000)     1970 2020-08-24 09:11:02.230933 slipbox-0.9.0/PKG-INFO
+-rw-r--r--   0 levi      (1000) levi      (1000)     1047 2020-08-24 09:09:29.000000 slipbox-0.9.0/README.md
+-rw-r--r--   0 levi      (1000) levi      (1000)       38 2020-08-24 09:11:02.230933 slipbox-0.9.0/setup.cfg
+-rw-r--r--   0 levi      (1000) levi      (1000)      775 2020-08-24 09:09:48.000000 slipbox-0.9.0/setup.py
+drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-24 09:11:02.227600 slipbox-0.9.0/slipbox/
+-rw-r--r--   0 levi      (1000) levi      (1000)        0 2020-07-27 04:23:14.000000 slipbox-0.9.0/slipbox/__init__.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     1580 2020-08-24 08:56:49.000000 slipbox-0.9.0/slipbox/__main__.py
+-rw-r--r--   0 levi      (1000) levi      (1000)      487 2020-08-11 10:22:14.000000 slipbox-0.9.0/slipbox/config.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     1023 2020-08-17 04:15:47.000000 slipbox-0.9.0/slipbox/conftest.py
+drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-24 09:11:02.227600 slipbox-0.9.0/slipbox/data/
+-rw-r--r--   0 levi      (1000) levi      (1000)    17953 2020-08-24 09:10:41.000000 slipbox-0.9.0/slipbox/data/bundle.js
+-rw-r--r--   0 levi      (1000) levi      (1000)     3045 2020-08-10 04:36:21.000000 slipbox-0.9.0/slipbox/data.py
+drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-24 09:11:02.230933 slipbox-0.9.0/slipbox/filters/
+-rw-r--r--   0 levi      (1000) levi      (1000)      409 2020-07-27 03:57:42.000000 slipbox-0.9.0/slipbox/filters/base64.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)      601 2020-08-09 15:26:02.000000 slipbox-0.9.0/slipbox/filters/csv.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)     6390 2020-08-24 08:54:44.000000 slipbox-0.9.0/slipbox/filters/filters.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)      880 2020-08-19 07:39:55.000000 slipbox-0.9.0/slipbox/filters/images.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)      492 2020-08-07 05:41:51.000000 slipbox-0.9.0/slipbox/filters/log.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)     1493 2020-08-09 14:08:44.000000 slipbox-0.9.0/slipbox/filters/refs.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)     6938 2020-08-24 08:56:01.000000 slipbox-0.9.0/slipbox/filters/slipbox.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)     2676 2020-08-24 07:11:59.000000 slipbox-0.9.0/slipbox/filters/utils.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)     5610 2020-08-12 03:33:05.000000 slipbox-0.9.0/slipbox/filters/utils.test.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)      483 2020-08-24 06:40:55.000000 slipbox-0.9.0/slipbox/filters/zk.lua
+-rw-r--r--   0 levi      (1000) levi      (1000)     7309 2020-08-16 13:33:09.000000 slipbox-0.9.0/slipbox/page.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     4220 2020-08-11 10:27:56.000000 slipbox-0.9.0/slipbox/pandoc.css
+-rw-r--r--   0 levi      (1000) levi      (1000)      436 2020-08-24 08:34:43.000000 slipbox-0.9.0/slipbox/preprocess.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     5613 2020-08-24 09:08:55.000000 slipbox-0.9.0/slipbox/scan.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     1830 2020-08-09 11:59:47.000000 slipbox-0.9.0/slipbox/schema.sql
+-rw-r--r--   0 levi      (1000) levi      (1000)     4724 2020-08-11 09:53:29.000000 slipbox-0.9.0/slipbox/slipbox.py
+-rw-r--r--   0 levi      (1000) levi      (1000)      884 2020-08-04 10:25:10.000000 slipbox-0.9.0/slipbox/templates.py
+-rw-r--r--   0 levi      (1000) levi      (1000)      330 2020-08-10 04:15:38.000000 slipbox-0.9.0/slipbox/test_data.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     2697 2020-08-04 15:21:01.000000 slipbox-0.9.0/slipbox/test_page.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     1429 2020-08-24 05:40:34.000000 slipbox-0.9.0/slipbox/test_preprocess.py
+-rw-r--r--   0 levi      (1000) levi      (1000)    12171 2020-08-24 08:58:57.000000 slipbox-0.9.0/slipbox/test_scan.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     5551 2020-08-24 08:56:29.000000 slipbox-0.9.0/slipbox/test_slipbox.py
+-rw-r--r--   0 levi      (1000) levi      (1000)      768 2020-08-04 11:20:44.000000 slipbox-0.9.0/slipbox/test_templates.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     1737 2020-08-24 08:57:31.000000 slipbox-0.9.0/slipbox/test_utils.py
+-rw-r--r--   0 levi      (1000) levi      (1000)     1327 2020-08-24 08:54:14.000000 slipbox-0.9.0/slipbox/utils.py
+drwxr-xr-x   0 levi      (1000) levi      (1000)        0 2020-08-24 09:11:02.227600 slipbox-0.9.0/slipbox.egg-info/
+-rw-r--r--   0 levi      (1000) levi      (1000)     1970 2020-08-24 09:11:01.000000 slipbox-0.9.0/slipbox.egg-info/PKG-INFO
+-rw-r--r--   0 levi      (1000) levi      (1000)      833 2020-08-24 09:11:01.000000 slipbox-0.9.0/slipbox.egg-info/SOURCES.txt
+-rw-r--r--   0 levi      (1000) levi      (1000)        1 2020-08-24 09:11:01.000000 slipbox-0.9.0/slipbox.egg-info/dependency_links.txt
+-rw-r--r--   0 levi      (1000) levi      (1000)        8 2020-08-24 09:11:01.000000 slipbox-0.9.0/slipbox.egg-info/top_level.txt
```

### Comparing `slipbox-0.8.9/PKG-INFO` & `slipbox-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipbox
-Version: 0.8.9
+Version: 0.9.0
 Summary: Static-site generator for Zettelkasten notes
 Home-page: https://github.com/lggruspe/slipbox
 Author: Levi Gruspe
 Author-email: mail.levig@gmail.com
 License: UNKNOWN
 Description: slipbox
         =======
@@ -23,15 +23,14 @@
         
         Requirements
         ------------
         
         - `pandoc`
         - `pandoc-citeproc`
         - `python3`
-        - GNU `grep`
         
         Installation
         ------------
         
         ```bash
         pip install slipbox
         ```
@@ -46,15 +45,15 @@
         This command create an HTML out of your markdown notes in the `notes` directory.
         
         - `notes.db` is the filename of the sqlite database.
         - `notes` is your notes directory, must be visible from the working directory.
         - ` -o notes.html` can be replaced with any pandoc option.
             + Take note of the quotes and the leading space.
         
-        See [docs/](https://lggruspe.github.io/slipbox) and `examples/`.
+        See [docs/](https://lggruspe.github.io/slipbox) for examples.
         
         License
         -------
         
         MIT.
         
         Credits
```

### Comparing `slipbox-0.8.9/README.md` & `slipbox-0.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 Requirements
 ------------
 
 - `pandoc`
 - `pandoc-citeproc`
 - `python3`
-- GNU `grep`
 
 Installation
 ------------
 
 ```bash
 pip install slipbox
 ```
@@ -38,15 +37,15 @@
 This command create an HTML out of your markdown notes in the `notes` directory.
 
 - `notes.db` is the filename of the sqlite database.
 - `notes` is your notes directory, must be visible from the working directory.
 - ` -o notes.html` can be replaced with any pandoc option.
     + Take note of the quotes and the leading space.
 
-See [docs/](https://lggruspe.github.io/slipbox) and `examples/`.
+See [docs/](https://lggruspe.github.io/slipbox) for examples.
 
 License
 -------
 
 MIT.
 
 Credits
```

### Comparing `slipbox-0.8.9/setup.py` & `slipbox-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fp:
     long_description = fp.read()
 
 setuptools.setup(
     name="slipbox",
-    version="0.8.9",
+    version="0.9.0",
     author="Levi Gruspe",
     author_email="mail.levig@gmail.com",
     description="Static-site generator for Zettelkasten notes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lggruspe/slipbox",
     packages=setuptools.find_packages(),
```

### Comparing `slipbox-0.8.9/slipbox/__main__.py` & `slipbox-0.9.0/slipbox/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def main(config_: Config) -> None:
     """Compile notes into static page."""
     with Slipbox(config_) as slipbox:
         slipbox.run()
 
 if __name__ == "__main__":
     if not check_requirements():
-        sys.exit("[ERROR] pandoc and grep not found.")
+        sys.exit("[ERROR] pandoc not found.")
 
     config = Config()
 
     parser = ArgumentParser(
         description="Generate a single-page HTML from your notes.")
     parser.add_argument("-s", "--database", default=config.database, type=Path,
                         help="filename of sqlite3 database")
```

### Comparing `slipbox-0.8.9/slipbox/data/bundle.js` & `slipbox-0.9.0/slipbox/data/bundle.js`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/data.py` & `slipbox-0.9.0/slipbox/data.py`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/filters/csv.lua` & `slipbox-0.9.0/slipbox/filters/csv.lua`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/filters/filters.lua` & `slipbox-0.9.0/slipbox/filters/filters.lua`

 * *Files 23% similar despite different names*

```diff
@@ -2,42 +2,74 @@
 
 local pandoc = require "pandoc"
 pandoc.utils = require "pandoc.utils"
 
 local log = require "filters/log"
 local utils = require "filters/utils"
 
+local function preprocess()
+  -- Create filter that preprocesses headers by setting the filename
+  -- attribute of Headers to the name of the file.
+
+  local function Pandoc(doc)
+    local filename
+    for _, elem in ipairs(doc.blocks) do
+      if elem.tag == "RawBlock" and elem.format == "html" then
+        filename = utils.parse_filename(elem) or filename
+      elseif elem.tag == "Header" and elem.level == 1 then
+        assert(filename)
+        elem.attributes.filename = filename
+      end
+    end
+    return doc
+  end
+
+  return {
+    Pandoc = Pandoc,
+  }
+end
+
 local function init(slipbox)
   -- Create filter that preprocesses headers by splitting the document
   -- into sections.
 
+  local function RawBlock(elem)
+      -- Strip #slipbox-metadata.
+      if elem.format == "html" and utils.parse_filename(elem) then
+        return {}
+      end
+  end
+
   local function Header(elem)
     -- Only scan level 1 headers.
     if elem.level ~= 1 then return end
 
     local content = pandoc.utils.stringify(elem.content)
     local id, title = utils.parse_id_and_title(content)
     if id and title then
-      local err = slipbox:save_note(id, title)
+      local filename = elem.attributes.filename
+      local err = slipbox:save_note(id, title, filename)
       if err then log.warning(err) end
 
       elem.identifier = id
       elem.attributes.title = title
       elem.attributes.level = elem.level  -- Gets added to parent section
+      elem.attributes.filename = nil
       return elem
     end
   end
 
   local function Pandoc(doc)
     doc.blocks = pandoc.utils.make_sections(false, nil, doc.blocks)
     return doc
   end
 
   return {
     Header = Header,
+    RawBlock = RawBlock,
     Pandoc = Pandoc,
   }
 end
 
 local Collector = {}
 function Collector:new(slipbox, div)
   local id = tonumber(div.identifier)
@@ -95,14 +127,15 @@
   local id = tonumber(div.identifier)
   if not id then return end
 
   self.__index = self
   return setmetatable({
     id = id,
     div = div,
+    footnotes = {},
     has_empty_link_target = false,
   }, self)
 end
 
 function Modifier:Link(elem)
   -- Rewrite links with empty targets/text.
   if not elem.target or elem.target == "" then
@@ -119,55 +152,76 @@
         elem.target,
         elem.title),
       pandoc.Str "]",
     }
   end
 end
 
+function Modifier:Note(elem)
+  -- Collect footnotes.
+  table.insert(self.footnotes, pandoc.Div(elem.content))
+  local count = #self.footnotes
+  return pandoc.Superscript(pandoc.Str(tostring(count)))
+end
+
 function Modifier.Str(elem)
   -- Turn #tags into links.
   if utils.hashtag_prefix(elem.text) then
     return pandoc.Link({elem}, '#'..elem.text)
   end
 end
 
 function Modifier:filter()
   return {
     Link = function(elem) return self:Link(elem) end,
+    Note = function(elem) return self:Note(elem) end,
     Str = function(elem) return self.Str(elem) end,
   }
 end
 
 local function modify(slipbox)
   -- Create filter that modifies the document.
   return {
     Div = function(div)
       local mod = Modifier:new(div)
       if mod then
         div = pandoc.walk_block(div, mod:filter())
         if mod.has_empty_link_target then
           slipbox.invalid.has_empty_link_target[mod.id] = true
         end
+        if next(mod.footnotes) then
+          local ol = pandoc.OrderedList{}
+          for _, block in ipairs(mod.footnotes) do
+            table.insert(ol.content, {block})
+          end
+          table.insert(div.content, pandoc.HorizontalRule())
+          table.insert(div.content, ol)
+        end
+
+        if div.attributes.level then
+          if div.attributes.level == "1" then
+            div.attributes.style = "display:none"
+          end
+          div.attributes.level = nil
+        end
+
       end
       return div
     end
   }
 end
 
 local function serialize(slipbox)
   -- Create filter to dump slipbox data into SLIPBOX_TMPDIR.
   return {
     Pandoc = function()
       local tmpdir = os.getenv "SLIPBOX_TMPDIR"
-      local scan_input_list = os.getenv "SCAN_INPUT_LIST"
-      if not tmpdir or tmpdir == "" then return end
-
-      local scan = require "filters/scan"
-      scan.grep_filenames(slipbox, scan_input_list)
-      slipbox:write_data(tmpdir)
+      if tmpdir and tmpdir ~= "" then
+        slipbox:write_data(tmpdir)
+      end
     end
   }
 end
 
 local function check(slipbox)
   -- Create filter that prints warning messages for invalid notes.
   return {
@@ -195,13 +249,14 @@
       end
       log.warning(messages)
     end
   }
 end
 
 return {
+  preprocess = preprocess,
   init = init,
   collect = collect,
   modify = modify,
   serialize = serialize,
   check = check,
 }
```

### Comparing `slipbox-0.8.9/slipbox/filters/images.lua` & `slipbox-0.9.0/slipbox/filters/images.lua`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/filters/refs.lua` & `slipbox-0.9.0/slipbox/filters/refs.lua`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/filters/slipbox.lua` & `slipbox-0.9.0/slipbox/filters/slipbox.lua`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,33 @@
   -- Save citation from note id (number).
   assert(type(id) == "number")
   local citations = self.citations[id] or {}
   citations[citation] = true
   self.citations[id] = citations
 end
 
-function SlipBox:save_note(id, title)
+function SlipBox:save_note(id, title, filename)
   -- Save note into slipbox.
   -- Return list of error messages if a note with the same ID already
   -- exists.
   assert(type(id) == "number")
   assert(type(title) == "string")
+  assert(type(filename) == "string")
   assert(title ~= "")
+  assert(filename ~= "")
 
   local note = self.notes[id]
   if note then
     return {
       string.format("Duplicate ID: %d.", id),
       string.format("Could not insert note '%s'.", title),
       string.format("Note '%s' already uses the ID.", note.title)
     }
   end
-  self.notes[id] = {title = title}
+  self.notes[id] = {title = title, filename = filename}
 end
 
 function SlipBox:save_alias(id, alias, owner)
   -- Save alias record in the slipbox.
   -- Return list of error messages if the alias is already used by a
   -- different note.
   assert(type(id) == "number")
@@ -233,15 +235,14 @@
     return sql
   end
   return ""
 end
 
 function SlipBox:write_data(basedir)
   -- Create sql statements from slipbox contents.
-  -- Must be called only after filenames have been grepped.
   local write = utils.write_text
   write(basedir .. "/files.csv", files_to_csv(self.notes))
   write(basedir .. "/notes.csv", notes_to_csv(self.notes))
   write(basedir .. "/tags.csv", tags_to_csv(self.tags))
   write(basedir .. "/links.csv", links_to_csv(self.links))
   write(basedir .. "/aliases.csv", aliases_to_csv(self.aliases))
   write(basedir .. "/sequences.csv", sequences_to_csv(self.aliases))
```

### Comparing `slipbox-0.8.9/slipbox/filters/utils.lua` & `slipbox-0.9.0/slipbox/filters/utils.lua`

 * *Files 5% similar despite different names*

```diff
@@ -77,16 +77,24 @@
   local file = io.open(filename, 'w')
   if not file then return false end
   file:write(text)
   file:close()
   return true
 end
 
+local function parse_filename(elem)
+  assert(elem.tag == "RawBlock")
+  local pattern = '^<!%-%-#slipbox%-metadata\nfilename: (.-)\n%-%->$'
+  local filename, count = elem.text:gsub(pattern, '%1')
+  if count > 0 then return filename end
+end
+
 return {
   is_valid_alias = is_valid_alias,
   hashtag_prefix = hashtag_prefix,
   get_link = get_link,
   parse_id_and_title = parse_id_and_title,
+  parse_filename = parse_filename,
   alias_parent = alias_parent,
   write_text = write_text,
   append_text = append_text,
 }
```

### Comparing `slipbox-0.8.9/slipbox/filters/utils.test.lua` & `slipbox-0.9.0/slipbox/filters/utils.test.lua`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/page.py` & `slipbox-0.9.0/slipbox/page.py`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/pandoc.css` & `slipbox-0.9.0/slipbox/pandoc.css`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/scan.py` & `slipbox-0.9.0/slipbox/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 import shlex
 from sqlite3 import Connection, IntegrityError
 import sys
 from typing import Iterable, List, Set, Tuple, Union
 
 from . import data, utils
+from .preprocess import concatenate
 
 def initialize_database(conn: Connection) -> None:
     """Initialize database with schema.sql."""
     sql = Path(__file__).with_name("schema.sql").read_text()
     conn.executescript(sql)
     conn.commit()
 
@@ -79,28 +80,27 @@
     """
     def key(filename: Union[str, Path]) -> Tuple[str, str]:
         root, ext = os.path.splitext(filename)
         return (ext, "") if ext else ("", root)
     groups = groupby(sorted(files, key=key), key=key)
     return map(lambda g: g[1], groups)
 
-def build_command(inputs: str, output: str, options: str = "") -> str:
+def build_command(input_: Path, output: str, options: str = "") -> str:
     """Construct a single pandoc command to run on inputs.
 
     inputs is a string of filenames separated by spaces.
     Each filename must be shlex.quoted if needed.
     Return an empty string if there are no input files.
     """
-    if not inputs.strip():
-        return ""
+    assert input_.exists()
     datadir = shlex.quote(str(Path(__file__).parent.resolve()))
     cmd = f"{utils.pandoc()} -Lzk.lua -Fpandoc-citeproc -Lrefs.lua --section-divs " \
             f"--data-dir {datadir} -Mlink-citations:true {options} " \
             "-o {} ".format(shlex.quote(output))
-    return cmd + ' ' + inputs
+    return cmd + ' ' + str(input_)
 
 def store_html_sections(conn: Connection, html: str, sources: List[Path]) -> None:
     """Insert Html and Sections entries for html and sources.
 
     html
     : HTML body text.
     sources
@@ -120,28 +120,31 @@
         cur2.execute(insert, (row[0], lastrowid))
     conn.commit()
 
 def scan(conn: Connection, inputs: List[Path], scan_options: str, self_contained: bool) -> None:
     """Process inputs and store results in database."""
     convert_to_data_url = "1" if self_contained else ""
     for batch in group_by_file_extension(inputs):
-        files = list(batch)
-        scan_input_list = " ".join(shlex.quote(str(p)) for p in files)
-
         with utils.temporary_directory() as tempdir:
             html = tempdir/"temp.html"
-            cmd = build_command(scan_input_list, str(html), scan_options)
+
+            preprocessed_input = tempdir/"input.md"
+            concatenate(preprocessed_input, *batch)
+
+            cmd = build_command(
+                preprocessed_input,
+                str(html),
+                scan_options)
             proc = utils.run_command(cmd, SLIPBOX_TMPDIR=str(tempdir),
-                                     CONVERT_TO_DATA_URL=convert_to_data_url,
-                                     GREP=utils.grep(),
-                                     SCAN_INPUT_LIST=scan_input_list)
+                                     CONVERT_TO_DATA_URL=convert_to_data_url)
             if proc.stdout:
                 print(proc.stdout.decode())
             if proc.stderr:
                 print(proc.stderr.decode(), file=sys.stderr)
             if proc.returncode:
                 print("Scan failed.", file=sys.stderr)
                 continue
+
             data.process_csvs(conn, tempdir)
             execute_script(conn, tempdir/"citations.sql")
             contents = html.read_text()
         store_html_sections(conn, contents, inputs)
```

### Comparing `slipbox-0.8.9/slipbox/schema.sql` & `slipbox-0.9.0/slipbox/schema.sql`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/slipbox.py` & `slipbox-0.9.0/slipbox/slipbox.py`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/templates.py` & `slipbox-0.9.0/slipbox/templates.py`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/test_page.py` & `slipbox-0.9.0/slipbox/test_page.py`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/test_scan.py` & `slipbox-0.9.0/slipbox/test_scan.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,34 +106,42 @@
 def test_group_by_file_extension_on_the_same_type():
     """group_by_file_extension should group files with the same type together."""
     files = [f"{c}.md" for c in "abcdefg"]
     groups = list(map(list, scan.group_by_file_extension(files)))
     assert len(groups) == 1
     assert files in groups
 
-def test_build_command():
+def test_build_command(tmp_path):
     """Sanity check for build_command."""
+    input_file = tmp_path/"input.md"
     output = "output.html"
     options = "--mathjax"
-    assert not scan.build_command("  ", output, options)
-    cmd = scan.build_command("cha1.md cha2.md", output, options)
-    assert "cha1.md cha2.md" in cmd
+    input_file.touch()
+
+    cmd = scan.build_command(input_file, output, options)
+    assert str(input_file) in cmd
     assert f"-o {output}" in cmd
     assert options in cmd
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.xfail
+def test_build_command_when_input_file_does_not_exist(tmp_path):
+    """build_command must fail if input file does not exist."""
+    input_file = tmp_path/"input.md"
+    scan.build_command(input_file, "output.html", "")
+
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan(mock_db, tmp_path):
     """Smoke test for scan."""
     input_file = tmp_path/"input.md"
     input_file.write_text("# 1 Test note\n\nHello, world!\n")
     assert not list(mock_db.execute("SELECT * FROM Html"))
     scan.scan(mock_db, [input_file], "", False)
     assert len(list(mock_db.execute("SELECT * FROM Html"))) == 1
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_empty_file(mock_db, tmp_path):
     """Scanned files that are empty shouldn't have entries in the database."""
     empty = tmp_path/"empty.md"
     empty.touch()
     scan.scan(mock_db, [empty], "", False)
     assert not list(mock_db.execute("SELECT * FROM Files"))
     assert not list(mock_db.execute("SELECT * FROM Notes"))
@@ -142,41 +150,41 @@
     assert not list(mock_db.execute("SELECT * FROM Aliases"))
     assert not list(mock_db.execute("SELECT * FROM Sequences"))
     assert not list(mock_db.execute("SELECT * FROM Html"))
     assert not list(mock_db.execute("SELECT * FROM Sections"))
     assert not list(mock_db.execute("SELECT * FROM Bibliography"))
     assert not list(mock_db.execute("SELECT * FROM Citations"))
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_filenames(mock_db, tmp_path):
-    """Filenames must be grepped from input files only."""
+    """Filenames must be scanned corretly."""
     markdown = tmp_path/"foo.md"
     skip = tmp_path/"bar.md"
     markdown.write_text("# 0 Note\n\nBody.\n")
     skip.write_text("# 0 Note\n\nBody.\n")
     scan.scan(mock_db, [markdown], "", False)
 
     result = list(mock_db.execute("SELECT filename FROM Notes WHERE id = 0"))
     assert len(result) == 1
     assert markdown.samefile(result[0][0])
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_filenames0(mock_db, tmp_path):
-    """Filenames must be grepped from input files only."""
+    """Filenames must be scanned correctly."""
     markdown = tmp_path/"bar.md"
     skip = tmp_path/"foo.md"
     markdown.write_text("# 0 Note\n\nBody.\n")
     skip.write_text("# 0 Note\n\nBody.\n")
     scan.scan(mock_db, [markdown], "", False)
 
     result = list(mock_db.execute("SELECT filename FROM Notes WHERE id = 0"))
     assert len(result) == 1
     assert markdown.samefile(result[0][0])
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_non_level1_headers(mock_db, tmp_path):
     """Only level 1 headers must be considered as note headers."""
     markdown = tmp_path/"test.md"
     markdown.write_text("""# 0 Valid note header
 
 Foo.
 
@@ -185,15 +193,15 @@
 Bar.
 """)
     scan.scan(mock_db, [markdown], "", False)
     result = [nid for nid, in mock_db.execute("SELECT id FROM Notes")]
     assert len(result) == 1
     assert result == [0]
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_with_duplicate_existing_id(mock_db, tmp_path, capsys):
     """scan must show a warning if a new note shares ID of an existing note.
 
     The warning message must show the filenames of both notes.
     """
     file_a = tmp_path/"a.md"
     file_a.write_text("# 0 Existing note\n\nTest.\n")
@@ -217,15 +225,15 @@
 
     stdout, stderr = capsys.readouterr()
     assert not stdout
     assert stderr
     assert str(file_a) in stderr
     assert str(file_b) in stderr
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_with_duplicate_ids_in_a_file(mock_db, tmp_path, capsys):
     """If there are duplicate IDs in a file, only the first one must be saved.
 
     scan must show a warning when this happens.
     """
     markdown = tmp_path/"test.md"
     markdown.write_text("""# 0 First note
@@ -241,15 +249,15 @@
     assert len(result) == 1
     assert result == [(0, "First note")]
 
     stdout, stderr = capsys.readouterr()
     assert not stdout
     assert stderr
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_with_missing_alias(mock_db, tmp_path, capsys):
     """scan must show a warning if there's a gap in an alias sequence."""
     markdown = tmp_path/"test.md"
     markdown.write_text("""# 0 Foo
 
 [Bar](#1 '/a')
 [Baz](#2 '/a1a')
@@ -263,72 +271,81 @@
 Baz.
 """)
     scan.scan(mock_db, [markdown], "", False)
     stdout, stderr = capsys.readouterr()
     assert not stdout
     assert stderr
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
-def test_scan_with_blank_grep(mock_db, tmp_path, capsys, monkeypatch):
-    """scan must ignore GREP="" variable setting."""
-    markdown = tmp_path/"test.md"
-    markdown.write_text("# 0 Test\n\nTest.\n")
-    monkeypatch.setenv("GREP", "")
-    scan.scan(mock_db, [markdown], "", False)
-    stdout, stderr = capsys.readouterr()
-    assert not stdout
-    assert not stderr
-
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_aliases(mock_db, tmp_path):
     """Only slash aliases must be saved."""
     file_a = tmp_path/"a.md"
     file_b = tmp_path/"b.md"
     file_c = tmp_path/"c.md"
     file_a.write_text("""# 0 A
 
-[B](#1 '0a').
-[C](#2 '/b').
+[B](#1 '0a')
+[C](#2 '/b')
 """)
-    file_b.write_text("# 1 B\n\nB.")
-    file_c.write_text("# 2 C\n\nC.")
+    file_b.write_text("# 1 B\n\nB")
+    file_c.write_text("# 2 C\n\nC")
 
     scan.scan(mock_db, [file_a, file_b, file_c], "", False)
     result = list(mock_db.execute("SELECT id, alias, owner FROM Aliases ORDER BY alias"))
     assert len(result) == 2
     assert result == [(0, '0', 0), (2, '0b', 0)]
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_with_empty_link_target(mock_db, tmp_path, capsys):
     """scan must show a warning if there is a link with an empty target."""
     markdown = tmp_path/"test.md"
     markdown.write_text("# 0 Foo\n\n[Empty]().\n")
     scan.scan(mock_db, [markdown], "", False)
     result = list(mock_db.execute("SELECT * FROM Links"))
     assert not result
 
     stdout, stderr = capsys.readouterr()
     assert not stdout
     assert stderr
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_with_id_in_scientific_form(mock_db, tmp_path, capsys):
     """Headers with non-integer IDs should be ignored."""
     markdown = tmp_path/"test.md"
     markdown.write_text("# 1e1 Invalid note ID\n\nTest.\n")
     scan.scan(mock_db, [markdown], "", False)
 
     result = list(mock_db.execute("SELECT * FROM Notes"))
     assert not result
 
     stdout, stderr = capsys.readouterr()
     assert not stdout
     assert not stderr
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
+def test_scan_with_non_text_titles(mock_db, tmp_path, capsys):
+    """Notes with non-text titles in the header must still be recognized."""
+    file_a = tmp_path/"a.md"
+    file_b = tmp_path/"b.md"
+    file_c = tmp_path/"c.md"
+    file_a.write_text("# 0 $1 + 1 = 2$\n\nTest.\n")
+    file_b.write_text("# 1 [Note 0](#0)\n\nTest.\n")
+    file_c.write_text("# 2 `print('Title')`\n\nTest.\n")
+
+    scan.scan(mock_db, [file_a, file_b, file_c], "", False)
+    result = list(mock_db.execute("SELECT id, title FROM Notes ORDER BY id"))
+
+    assert len(result) == 3
+    assert result == [(0, "1 + 1 = 2"), (1, "Note 0"), (2, "print('Title')")]
+
+    stdout, stderr = capsys.readouterr()
+    assert not stdout
+    assert not stderr
+
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
 def test_scan_with_duplicate_aliases(mock_db, tmp_path, capsys):
     """If a note defines duplicate aliases, only the first one must be saved.
 
     scan must show a warning when this happens.
     """
     markdown = tmp_path/"test.md"
     markdown.write_text("""# 0 Foo
```

### Comparing `slipbox-0.8.9/slipbox/test_slipbox.py` & `slipbox-0.9.0/slipbox/test_slipbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -108,20 +108,18 @@
 
     result = slipbox.conn.execute("SELECT filename FROM Files")
     remaining = sorted(filename for filename, in result)
     assert len(remaining) == 2
     for path, filename in zip(paths, remaining):
         assert path.samefile(filename)
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
-def test_suggest_edits_backlinks(tmp_path, sbox):
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
+def test_suggest_edits_backlinks(files_abc, sbox):
     """slipbox.suggest_edits must include backlinks of outdated notes."""
-    file_a = tmp_path/"a.md"
-    file_b = tmp_path/"b.md"
-    file_c = tmp_path/"c.md"
+    file_a, file_b, file_c = files_abc
     file_a.write_text("# 0 A\n\nA.\n[B](#1 '/a').\n")
     file_b.write_text("# 1 B\n\nB.\n[C](#2).\n")
     file_c.write_text("# 2 C\n\nC.\n")
 
     slipbox = sbox
     slipbox.timestamp = time()
 
@@ -129,20 +127,18 @@
 
     file_c.touch()
 
     notes = slipbox.find_notes()
     suggestions = list(slipbox.suggest_edits(notes))
     assert suggestions == [(1, "B", file_b)]
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
-def test_suggest_edits_aliases(tmp_path, sbox):
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
+def test_suggest_edits_aliases(files_abc, sbox):
     """slipbox.suggest_edits must include alias owners of outdated notes."""
-    file_a = tmp_path/"a.md"
-    file_b = tmp_path/"b.md"
-    file_c = tmp_path/"c.md"
+    file_a, file_b, file_c = files_abc
     file_a.write_text("# 0 A\n\nA.\n[B](#1 '/a').\n")
     file_b.write_text("# 1 B\n\nB.\n[C](#2).\n")
     file_c.write_text("# 2 C\n\nC.\n")
 
     slipbox = sbox
     slipbox.timestamp = time()
 
@@ -150,20 +146,18 @@
 
     file_b.touch()
 
     notes = slipbox.find_notes()
     suggestions = list(slipbox.suggest_edits(notes))
     assert suggestions == [(0, "A", file_a)]
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
-def test_suggest_edits_exclude_deleted_notes(tmp_path, sbox):
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
+def test_suggest_edits_exclude_deleted_notes(files_abc, sbox):
     """slipbox.suggest_edits must exclude deleted notes."""
-    file_a = tmp_path/"a.md"
-    file_b = tmp_path/"b.md"
-    file_c = tmp_path/"c.md"
+    file_a, file_b, file_c = files_abc
     file_a.write_text("# 0 A\n\nA.\n[B](#2 '/a').\n")
     file_b.write_text("# 1 B\n\nB.\n[C](#2).\n")
     file_c.write_text("# 2 C\n\nC.\n")
 
     slipbox = sbox
     slipbox.timestamp = time()
 
@@ -173,20 +167,18 @@
     file_a.unlink()
 
     notes = slipbox.find_notes()
     suggestions = list(slipbox.suggest_edits(notes))
     assert suggestions == [(1, "B", file_b)]
 
 
-@pytest.mark.skipif(not check_requirements(), reason="requires grep and pandoc")
-def test_run(tmp_path, capsys, sbox):
+@pytest.mark.skipif(not check_requirements(), reason="requires pandoc")
+def test_run(files_abc, capsys, sbox):
     """There must be no suggestions when running for the first time."""
-    file_a = tmp_path/"a.md"
-    file_b = tmp_path/"b.md"
-    file_c = tmp_path/"c.md"
+    file_a, file_b, file_c = files_abc
     file_a.write_text("# 0 A\n\nA.\n[B](#2 '/a').\n")
     file_b.write_text("# 1 B\n\nB.\n[C](#2).\n")
     file_c.write_text("# 2 C\n\nC.\n")
 
     slipbox = sbox
     slipbox.timestamp = time()
```

### Comparing `slipbox-0.8.9/slipbox/test_templates.py` & `slipbox-0.9.0/slipbox/test_templates.py`

 * *Files identical despite different names*

### Comparing `slipbox-0.8.9/slipbox/test_utils.py` & `slipbox-0.9.0/slipbox/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """temporary_directory gets deleted when the context manager exits."""
     with utils.temporary_directory() as temp:
         path = temp
         assert temp.exists()
         assert temp.is_dir()
     assert not path.exists()
 
-@pytest.mark.skipif(not shutil.which(utils.grep()), reason="requires grep")
+@pytest.mark.skipif(not shutil.which("grep"), reason="requires grep")
 def test_run_command(tmp_path):
     """run_command must return stdout and stderr output."""
     first = tmp_path/"first.txt"
     second = tmp_path/"second.txt"
     first.write_text("first")
     second.write_text("second")
```

### Comparing `slipbox-0.8.9/slipbox/utils.py` & `slipbox-0.9.0/slipbox/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,17 @@
 import tempfile
 from typing import Any, Iterator
 
 def pandoc() -> str:
     """Pandoc location."""
     return os.environ.get("PANDOC", "pandoc")
 
-def grep() -> str:
-    """Grep location."""
-    return os.environ.get("GREP", "grep")
-
 def check_requirements() -> bool:
-    """Check if grep and pandoc are installed."""
-    return bool(shutil.which(pandoc()) and shutil.which(grep()))
+    """Check if pandoc is installed."""
+    return bool(shutil.which(pandoc()))
 
 def sqlite_string(text: str) -> str:
     """Encode python string into sqlite string."""
     return "'{}'".format(text.replace("'", "''"))
 
 @contextlib.contextmanager
 def temporary_directory() -> Iterator[Path]:
```

### Comparing `slipbox-0.8.9/slipbox.egg-info/PKG-INFO` & `slipbox-0.9.0/slipbox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipbox
-Version: 0.8.9
+Version: 0.9.0
 Summary: Static-site generator for Zettelkasten notes
 Home-page: https://github.com/lggruspe/slipbox
 Author: Levi Gruspe
 Author-email: mail.levig@gmail.com
 License: UNKNOWN
 Description: slipbox
         =======
@@ -23,15 +23,14 @@
         
         Requirements
         ------------
         
         - `pandoc`
         - `pandoc-citeproc`
         - `python3`
-        - GNU `grep`
         
         Installation
         ------------
         
         ```bash
         pip install slipbox
         ```
@@ -46,15 +45,15 @@
         This command create an HTML out of your markdown notes in the `notes` directory.
         
         - `notes.db` is the filename of the sqlite database.
         - `notes` is your notes directory, must be visible from the working directory.
         - ` -o notes.html` can be replaced with any pandoc option.
             + Take note of the quotes and the leading space.
         
-        See [docs/](https://lggruspe.github.io/slipbox) and `examples/`.
+        See [docs/](https://lggruspe.github.io/slipbox) for examples.
         
         License
         -------
         
         MIT.
         
         Credits
```

### Comparing `slipbox-0.8.9/slipbox.egg-info/SOURCES.txt` & `slipbox-0.9.0/slipbox.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 slipbox/__init__.py
 slipbox/__main__.py
 slipbox/config.py
 slipbox/conftest.py
 slipbox/data.py
 slipbox/page.py
 slipbox/pandoc.css
+slipbox/preprocess.py
 slipbox/scan.py
 slipbox/schema.sql
 slipbox/slipbox.py
 slipbox/templates.py
 slipbox/test_data.py
 slipbox/test_page.py
+slipbox/test_preprocess.py
 slipbox/test_scan.py
 slipbox/test_slipbox.py
 slipbox/test_templates.py
 slipbox/test_utils.py
 slipbox/utils.py
 slipbox.egg-info/PKG-INFO
 slipbox.egg-info/SOURCES.txt
 slipbox.egg-info/dependency_links.txt
 slipbox.egg-info/top_level.txt
 slipbox/data/bundle.js
 slipbox/filters/base64.lua
 slipbox/filters/csv.lua
 slipbox/filters/filters.lua
-slipbox/filters/footnotes.lua
 slipbox/filters/images.lua
 slipbox/filters/log.lua
 slipbox/filters/refs.lua
-slipbox/filters/scan.lua
 slipbox/filters/slipbox.lua
 slipbox/filters/utils.lua
 slipbox/filters/utils.test.lua
 slipbox/filters/zk.lua
```

