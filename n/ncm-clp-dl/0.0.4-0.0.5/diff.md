# Comparing `tmp/ncm_clp_dl-0.0.4-py3-none-any.whl.zip` & `tmp/ncm_clp_dl-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3552 bytes, number of entries: 8
+Zip file size: 3596 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-09 03:35 ncm_clp_dl/__init__.py
--rw-rw-rw-  2.0 fat     1887 b- defN 23-Jul-09 07:47 ncm_clp_dl/__main__.py
--rw-rw-rw-  2.0 fat     1085 b- defN 23-Jul-09 07:54 ncm_clp_dl-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      491 b- defN 23-Jul-09 07:54 ncm_clp_dl-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 07:54 ncm_clp_dl-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       57 b- defN 23-Jul-09 07:54 ncm_clp_dl-0.0.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-09 07:54 ncm_clp_dl-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      653 b- defN 23-Jul-09 07:54 ncm_clp_dl-0.0.4.dist-info/RECORD
-8 files, 4276 bytes uncompressed, 2400 bytes compressed:  43.9%
+-rw-rw-rw-  2.0 fat     1976 b- defN 23-Jul-09 08:56 ncm_clp_dl/__main__.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Jul-09 08:59 ncm_clp_dl-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-09 08:59 ncm_clp_dl-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-09 08:59 ncm_clp_dl-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-Jul-09 08:59 ncm_clp_dl-0.0.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-09 08:59 ncm_clp_dl-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      653 b- defN 23-Jul-09 08:59 ncm_clp_dl-0.0.5.dist-info/RECORD
+8 files, 4355 bytes uncompressed, 2444 bytes compressed:  43.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ncm_clp_dl/__init__.py
 Comment: 
 
 Filename: ncm_clp_dl/__main__.py
 Comment: 
 
-Filename: ncm_clp_dl-0.0.4.dist-info/LICENSE
+Filename: ncm_clp_dl-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: ncm_clp_dl-0.0.4.dist-info/METADATA
+Filename: ncm_clp_dl-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: ncm_clp_dl-0.0.4.dist-info/WHEEL
+Filename: ncm_clp_dl-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: ncm_clp_dl-0.0.4.dist-info/entry_points.txt
+Filename: ncm_clp_dl-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ncm_clp_dl-0.0.4.dist-info/top_level.txt
+Filename: ncm_clp_dl-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ncm_clp_dl-0.0.4.dist-info/RECORD
+Filename: ncm_clp_dl-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ncm_clp_dl/__main__.py

```diff
@@ -53,21 +53,29 @@
         current_clp = pyperclip.waitForNewPaste()
 
         # 判断是否是网易云音乐连接格式
         if _re_s.match(current_clp):
             # 加入到队列
             song_queue.put(current_clp)
 
+            # 清空剪切板
             pyperclip.copy("")
-    # os.system('pyncm --no-overwrite "{}"'.format(last_clipboard.strip()))
 
 
 def main():
+    dl = DL()
+
+    # 随主线程退出
+    dl.setDaemon(True)
+
     # 开启下载线程
-    DL().start()
+    dl.start()
 
-    # 监控剪切板
-    watch_clp()
+    try:
+        # 监控剪切板
+        watch_clp()
+    except KeyboardInterrupt as e:
+        pass
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `ncm_clp_dl-0.0.4.dist-info/LICENSE` & `ncm_clp_dl-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

