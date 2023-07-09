# Comparing `tmp/url_for_int-2.2.4.tar.gz` & `tmp/url_for_int-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\url_for_int-2.2.4.tar", last modified: Sun Aug 21 10:19:14 2022, max compression
+gzip compressed data, was "url_for_int-2.3.0.tar", last modified: Sun Jul  9 11:10:40 2023, max compression
```

## Comparing `url_for_int-2.2.4.tar` & `url_for_int-2.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-08-21 10:19:13.996431 url_for_int-2.2.4/
--rw-rw-rw-   0        0        0     2495 2022-08-21 10:19:13.996431 url_for_int-2.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1629 2022-08-21 10:16:50.000000 url_for_int-2.2.4/README.md
--rw-rw-rw-   0        0        0       42 2022-08-21 10:19:13.996431 url_for_int-2.2.4/setup.cfg
--rw-rw-rw-   0        0        0      694 2022-08-21 10:19:09.000000 url_for_int-2.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-21 10:19:13.965231 url_for_int-2.2.4/url_for_int/
--rw-rw-rw-   0        0        0      600 2022-08-21 09:16:43.000000 url_for_int-2.2.4/url_for_int/__init__.py
--rw-rw-rw-   0        0        0     4475 2022-08-21 09:48:21.000000 url_for_int-2.2.4/url_for_int/int_gui.py
--rw-rw-rw-   0        0        0     1705 2022-08-21 10:13:23.000000 url_for_int-2.2.4/url_for_int/interpreter.py
-drwxrwxrwx   0        0        0        0 2022-08-21 10:19:13.996431 url_for_int-2.2.4/url_for_int.egg-info/
--rw-rw-rw-   0        0        0     2495 2022-08-21 10:19:13.000000 url_for_int-2.2.4/url_for_int.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2022-08-21 10:19:13.000000 url_for_int-2.2.4/url_for_int.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-21 10:19:13.000000 url_for_int-2.2.4/url_for_int.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-08-21 10:19:13.000000 url_for_int-2.2.4/url_for_int.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 11:10:40.360878 url_for_int-2.3.0/
+-rw-rw-rw-   0        0        0     1068 2023-07-09 05:50:06.000000 url_for_int-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2355 2023-07-09 11:10:40.359968 url_for_int-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1855 2023-07-09 10:52:44.000000 url_for_int-2.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 11:10:40.360878 url_for_int-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-07-09 11:10:09.000000 url_for_int-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:10:40.350612 url_for_int-2.3.0/url_for_int/
+-rw-rw-rw-   0        0        0      600 2023-07-09 05:50:06.000000 url_for_int-2.3.0/url_for_int/__init__.py
+-rw-rw-rw-   0        0        0     5934 2023-07-09 06:26:28.000000 url_for_int-2.3.0/url_for_int/int_gui.py
+-rw-rw-rw-   0        0        0     1853 2023-07-09 07:24:59.000000 url_for_int-2.3.0/url_for_int/interpreter.py
+drwxrwxrwx   0        0        0        0 2023-07-09 11:10:40.358511 url_for_int-2.3.0/url_for_int.egg-info/
+-rw-rw-rw-   0        0        0     2355 2023-07-09 11:10:40.000000 url_for_int-2.3.0/url_for_int.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-09 11:10:40.000000 url_for_int-2.3.0/url_for_int.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 11:10:40.000000 url_for_int-2.3.0/url_for_int.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 11:10:40.000000 url_for_int-2.3.0/url_for_int.egg-info/top_level.txt
```

### Comparing `url_for_int-2.2.4/README.md` & `url_for_int-2.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# url_for_Int *v2.2.4*
+# url_for_Int *v2.3.0*
 
 ### 简介
 - 这是 url-for Interpreter 的开源使用版，遵循 MIT 协议。<br>
 开发者：Hifive
 - Github: https://github.com/Hifive55555/url_for_Int <br>
 Pypi: https://pypi.org/project/url-for-int
 - 它总共分为两个部分：GUI 和 API，使用方法见下
 ### 新版内容
-2.2.4 修复ui数组bug，增加逆转函数omit_int
+- 2.2.4 修复 ui 数组 bug，增加逆转函数 omit_int  
+- 2.3.0 修复 omit_int 函数 bug，完善逆转义功能并添加到GUI上
 
 ---
 
 # 使用方法
 ## API
 ### 函数及类
 - #### int_main 主函数
@@ -33,12 +34,15 @@
 - 启用GUI界面：`start_gui()` 或直接运行 \_\_init__.py 文件
 - 转义一个文件
   - 转录到当前文件夹：`file_catcher("test.html")`
   - 转录到指定文件夹：`file_catcher("test.html", "D:/test")`
   - 转录并覆盖原文件：`file_catcher("test.html", prefix="")`
   - 转录并指定前缀：`file_catcher("test.html", prefix="xxx-")`
   - 转录并增加pre_folder：`file_catcher("test.html", "D:/test", if_pre=True)`
-- 转义一串字符
+- 逆转录一个文件
+  - 同上理，不过要加入参数 `if_omit=True`
+- 转义/逆转录一串字符
   ```python
   content = "xxx"
-  after = int_main(content)
-  ```
+  after_1 = int_main(content) # 转义
+  after_2 = omit_int(content) # 逆转义
+  ```
```

### Comparing `url_for_int-2.2.4/setup.py` & `url_for_int-2.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open("D:\\Projects\\url_for_Int\\README.md", "r", encoding='utf-8') as fh:
+with open("F:\\Code\\url_for_Int\\README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="url_for_int",
-    version="2.2.4",
+    version="2.3.0",
     author="Hifive",
     author_email="2019912635@qq.com",
     description="帮助flask框架中将普通HTML文档转义为url-for的文档",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Hifive55555/url_for_Int",
     packages=setuptools.find_packages(),
```

### Comparing `url_for_int-2.2.4/url_for_int/__init__.py` & `url_for_int-2.3.0/url_for_int/__init__.py`

 * *Files identical despite different names*

### Comparing `url_for_int-2.2.4/url_for_int/int_gui.py` & `url_for_int-2.3.0/url_for_int/int_gui.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,16 +29,18 @@
         tk.Label(self, text="\t\t前缀：").grid(row=3, column=0, pady=10)
         self.entry_text = tk.StringVar(self, value="int_")
         tk.Entry(self, textvariable=self.entry_text).grid(row=3, column=1, pady=10)
 
         self.check_path = tk.IntVar(self, value=1)
         c1 = tk.Checkbutton(self, text="使用原文件路径", variable=self.check_path, onvalue=1, offvalue=0)
         c1.grid(row=4, column=0, pady=10)
-        tk.Button(self, text="--> 转义", command=self.trans, width=30, height=2).grid(
+        tk.Button(self, text="--> 转义", command=self.trans, width=15, height=2).grid(
             row=4, column=1, columnspan=2, pady=10)
+        tk.Button(self, text="--> 逆转义", command=self.omit_trans, width=10, height=2).grid(
+            row=4, column=2, columnspan=2, pady=10)
 
         self.text = tk.Text(height=10)
         self.text.grid(row=5, column=0, columnspan=3, padx=5, pady=5)
         self.text.insert("end", "=============== 转义日志 ===============")
         self.text.config(state="disabled")
 
     def delete(self):
@@ -108,7 +110,40 @@
                 state = file_catcher(ori, save_path, prefix, if_pre=True)
                 write_text()
 
         success_file.reverse()
         for i in success_file:
             del self.paths[i]
         self.text.config(state="disabled")
+
+    def omit_trans(self):
+        state, success_file = None, []
+        prefix = self.entry_text.get()
+        self.text.config(state="normal")
+        self.text.insert("end", "\n>> 执行逆转义\n")
+
+        def write_text():
+            if state:
+                self.text.insert("end", f"{ori}  逆转义成功\n")
+                success_file.append(self.paths.index(ori))
+                self.listbox.delete(0)
+            else:
+                self.text.insert("end", f"！ {ori}逆转义失败\n")
+
+        if self.check_path.get() == 1:
+            if self.entry_text.get() == "" and self.paths != []:
+                check = tkinter.messagebox.askokcancel("提示", "这会覆盖原文件，要执行此操作吗")
+                if not check:
+                    return False
+            for ori in self.paths:
+                state = file_catcher(ori, prefix=prefix, if_omit=True)
+                write_text()
+        else:
+            save_path = filedialog.askdirectory(title="选择保存的文件夹")
+            for ori in self.paths:
+                state = file_catcher(ori, save_path, prefix, if_pre=True, if_omit=True)
+                write_text()
+
+        success_file.reverse()
+        for i in success_file:
+            del self.paths[i]
+        self.text.config(state="disabled")
```

### Comparing `url_for_int-2.2.4/url_for_int/interpreter.py` & `url_for_int-2.3.0/url_for_int/interpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,46 +17,50 @@
     x = re.sub(r"/?(\w[\u4E00-\u9FA5\w_-]+/)+([\u4E00-\u9FA5\w_-]+\.)+\w+\b", add, y)
 
     return x
 
 
 def omit_int(origin_text):
     def omit(match) -> str:
-            address = match.group(2)
-            return address
+        address = match.group(2)
+        return address
 
-    y = re.sub(r"({{ *url_for)(.*)(?=}})", omit, origin_text)
+    y = re.sub(r"({{ *url_for *\( *[\'\"]static[\'\"] *, *filename *= *[\'\"] *)(.*)([\'\"] *\) *}})", omit, origin_text)
+    print(y)
     return y
 
 
-def file_catcher(origin_file, to_path=None, prefix="int_", if_pre=False):
+def file_catcher(origin_file, to_path=None, prefix="int_", if_pre=False, if_omit=False):
     file_name, origin_path, pre_folder = decompose(origin_file)
     if not to_path:
         to_path = origin_path
     if if_pre:
         to_path = os.path.join(to_path, pre_folder)
     to_file = os.path.join(to_path, prefix + file_name)
     # 获取文件
 
-
     with open(origin_file, mode="r", encoding="utf-8") as f:
         origin_text = f.read()
 
     if not os.path.exists(to_path):
         os.makedirs(to_path)
         print("创建新的文件夹")
 
-    x = int_main(origin_text)
+    if not if_omit:
+        x = int_main(origin_text)
+    else:
+        x = omit_int(origin_text)
 
     with open(to_file, mode="w", encoding="utf-8") as f:
         f.write(x)
         print(f"{origin_file}  转义至  {to_file} 成功\n")
         return True
     return False
 
+
 def decompose(content: str):
     """ 将文件路径拆解 """
     file, path = "", ""
     content = content.split("\\")
     file = content[-1]
     pre_folder = content[-2]
     del content[-1]
```

