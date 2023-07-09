# Comparing `tmp/ncm-clp-dl-0.0.1.tar.gz` & `tmp/ncm-clp-dl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ncm-clp-dl-0.0.1.tar", last modified: Sun Jul  9 03:29:22 2023, max compression
+gzip compressed data, was "dist\ncm-clp-dl-0.0.2.tar", last modified: Sun Jul  9 03:41:00 2023, max compression
```

## Comparing `ncm-clp-dl-0.0.1.tar` & `ncm-clp-dl-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 03:29:22.783974 ncm-clp-dl-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-07-09 03:08:50.000000 ncm-clp-dl-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       24 2023-07-09 03:16:57.000000 ncm-clp-dl-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      426 2023-07-09 03:29:22.782974 ncm-clp-dl-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      128 2023-07-09 03:26:20.000000 ncm-clp-dl-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 03:29:22.781972 ncm-clp-dl-0.0.1/ncm_clp_dl.egg-info/
--rw-rw-rw-   0        0        0      426 2023-07-09 03:29:21.000000 ncm-clp-dl-0.0.1/ncm_clp_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-09 03:29:21.000000 ncm-clp-dl-0.0.1/ncm_clp_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 03:29:21.000000 ncm-clp-dl-0.0.1/ncm_clp_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-09 03:29:21.000000 ncm-clp-dl-0.0.1/ncm_clp_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-07-09 03:29:21.000000 ncm-clp-dl-0.0.1/ncm_clp_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 03:29:21.000000 ncm-clp-dl-0.0.1/ncm_clp_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      724 2023-07-09 03:23:29.000000 ncm-clp-dl-0.0.1/ncm_clp_dl.py
--rw-rw-rw-   0        0        0       34 2023-07-09 03:08:58.000000 ncm-clp-dl-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 03:29:22.783974 ncm-clp-dl-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      765 2023-07-09 03:22:02.000000 ncm-clp-dl-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 03:41:00.814169 ncm-clp-dl-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-07-09 03:08:50.000000 ncm-clp-dl-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-07-09 03:16:57.000000 ncm-clp-dl-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      426 2023-07-09 03:41:00.814169 ncm-clp-dl-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      128 2023-07-09 03:26:20.000000 ncm-clp-dl-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 03:41:00.730615 ncm-clp-dl-0.0.2/ncm_clp_dl/
+-rw-rw-rw-   0        0        0        0 2023-07-09 03:35:20.000000 ncm-clp-dl-0.0.2/ncm_clp_dl/__init__.py
+-rw-rw-rw-   0        0        0      738 2023-07-09 03:38:32.000000 ncm-clp-dl-0.0.2/ncm_clp_dl/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 03:41:00.812168 ncm-clp-dl-0.0.2/ncm_clp_dl.egg-info/
+-rw-rw-rw-   0        0        0      426 2023-07-09 03:41:00.000000 ncm-clp-dl-0.0.2/ncm_clp_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-09 03:41:00.000000 ncm-clp-dl-0.0.2/ncm_clp_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 03:41:00.000000 ncm-clp-dl-0.0.2/ncm_clp_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-09 03:41:00.000000 ncm-clp-dl-0.0.2/ncm_clp_dl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-09 03:41:00.000000 ncm-clp-dl-0.0.2/ncm_clp_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-09 03:41:00.000000 ncm-clp-dl-0.0.2/ncm_clp_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       34 2023-07-09 03:08:58.000000 ncm-clp-dl-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 03:41:00.815169 ncm-clp-dl-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-07-09 03:40:20.000000 ncm-clp-dl-0.0.2/setup.py
```

### Comparing `ncm-clp-dl-0.0.1/LICENSE` & `ncm-clp-dl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-clp-dl-0.0.1/ncm_clp_dl.py` & `ncm-clp-dl-0.0.2/ncm_clp_dl/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import pyperclip
 
 
 def main():
     current_clipboard = pyperclip.paste()
 
     # 网易云音乐格式匹配
-    _re_s = re.compile(r"^https://music\.163\.com/song\?id=\d+&userid=\d+$")
+    _re_s = re.compile(r"^\s*https://music\.163\.com/song\?id=\d+&userid=\d+\s*$")
 
     while True:
         if pyperclip.paste() != current_clipboard:
             # 剪切板内容已变化
             current_clipboard = pyperclip.paste()
             print('剪贴板内容已更改:', current_clipboard)
 
             # 判断是否是网易云音乐连接格式
             if _re_s.match(current_clipboard):
-                os.system('pyncm --no-overwrite "{}"'.format(current_clipboard))
+                os.system('pyncm --no-overwrite "{}"'.format(current_clipboard.strip()))
 
             time.sleep(0.1)
 
 
 if __name__ == "__main__":
     main()
```

