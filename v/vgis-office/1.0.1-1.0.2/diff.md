# Comparing `tmp/vgis_office-1.0.1.tar.gz` & `tmp/vgis_office-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_office-1.0.1.tar", last modified: Tue Jun 27 09:19:39 2023, max compression
+gzip compressed data, was "dist\vgis_office-1.0.2.tar", last modified: Sun Jul  9 04:33:27 2023, max compression
```

## Comparing `vgis_office-1.0.1.tar` & `vgis_office-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 09:19:39.939770 vgis_office-1.0.1/
--rw-rw-rw-   0        0        0     1037 2023-06-27 09:19:39.938844 vgis_office-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-06-27 09:08:40.000000 vgis_office-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 09:19:39.940309 vgis_office-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2198 2023-06-27 09:12:19.000000 vgis_office-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:19:39.917845 vgis_office-1.0.1/vgis_office/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_office-1.0.1/vgis_office/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:19:39.928844 vgis_office-1.0.1/vgis_office/vgis_excel/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_office-1.0.1/vgis_office/vgis_excel/__init__.py
--rw-rw-rw-   0        0        0     4693 2023-06-27 09:16:10.000000 vgis_office-1.0.1/vgis_office/vgis_excel/excelTools.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:19:39.931844 vgis_office-1.0.1/vgis_office/vgis_pdf/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_office-1.0.1/vgis_office/vgis_pdf/__init__.py
--rw-rw-rw-   0        0        0     2120 2023-06-27 09:16:19.000000 vgis_office-1.0.1/vgis_office/vgis_pdf/pdfHelper.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:19:39.933844 vgis_office-1.0.1/vgis_office/vgis_txt/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_office-1.0.1/vgis_office/vgis_txt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:19:39.936844 vgis_office-1.0.1/vgis_office/vgis_word/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_office-1.0.1/vgis_office/vgis_word/__init__.py
--rw-rw-rw-   0        0        0     4915 2023-06-27 08:29:35.000000 vgis_office-1.0.1/vgis_office/vgis_word/worddir2xls.py
-drwxrwxrwx   0        0        0        0 2023-06-27 09:19:39.925845 vgis_office-1.0.1/vgis_office.egg-info/
--rw-rw-rw-   0        0        0     1037 2023-06-27 09:19:39.000000 vgis_office-1.0.1/vgis_office.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-06-27 09:19:39.000000 vgis_office-1.0.1/vgis_office.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 09:19:39.000000 vgis_office-1.0.1/vgis_office.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-27 09:19:39.000000 vgis_office-1.0.1/vgis_office.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-27 09:19:39.000000 vgis_office-1.0.1/vgis_office.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 04:33:27.812434 vgis_office-1.0.2/
+-rw-rw-rw-   0        0        0     1037 2023-07-09 04:33:27.811435 vgis_office-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-07-06 02:41:01.000000 vgis_office-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 04:33:27.813435 vgis_office-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2272 2023-07-09 04:33:08.000000 vgis_office-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 04:33:27.708434 vgis_office-1.0.2/vgis_office/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_office-1.0.2/vgis_office/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 04:33:27.751436 vgis_office-1.0.2/vgis_office/vgis_excel/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_office-1.0.2/vgis_office/vgis_excel/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-07-09 04:21:34.000000 vgis_office-1.0.2/vgis_office/vgis_excel/excelTools.py
+drwxrwxrwx   0        0        0        0 2023-07-09 04:33:27.772434 vgis_office-1.0.2/vgis_office/vgis_pdf/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_office-1.0.2/vgis_office/vgis_pdf/__init__.py
+-rw-rw-rw-   0        0        0     2116 2023-07-09 04:25:33.000000 vgis_office-1.0.2/vgis_office/vgis_pdf/pdfHelper.py
+drwxrwxrwx   0        0        0        0 2023-07-09 04:33:27.782436 vgis_office-1.0.2/vgis_office/vgis_txt/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_office-1.0.2/vgis_office/vgis_txt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 04:33:27.800433 vgis_office-1.0.2/vgis_office/vgis_word/
+-rw-rw-rw-   0        0        0      202 2023-07-06 02:41:01.000000 vgis_office-1.0.2/vgis_office/vgis_word/__init__.py
+-rw-rw-rw-   0        0        0     4915 2023-07-06 02:41:01.000000 vgis_office-1.0.2/vgis_office/vgis_word/worddir2xls.py
+drwxrwxrwx   0        0        0        0 2023-07-09 04:33:27.736437 vgis_office-1.0.2/vgis_office.egg-info/
+-rw-rw-rw-   0        0        0     1037 2023-07-09 04:33:27.000000 vgis_office-1.0.2/vgis_office.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-07-09 04:33:27.000000 vgis_office-1.0.2/vgis_office.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 04:33:27.000000 vgis_office-1.0.2/vgis_office.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-09 04:33:27.000000 vgis_office-1.0.2/vgis_office.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 04:33:27.000000 vgis_office-1.0.2/vgis_office.egg-info/top_level.txt
```

### Comparing `vgis_office-1.0.1/PKG-INFO` & `vgis_office-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_office
-Version: 1.0.1
+Version: 1.0.2
 Summary: A libary for office operator
 Home-page: https://github.com/gisfanmachel/vgisOffice
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis office lib
```

### Comparing `vgis_office-1.0.1/setup.py` & `vgis_office-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_office",  # Required 项目名称
-    version="1.0.1",  # Required 发布版本号
+    version="1.0.2",  # Required 发布版本号
     description="A libary for office operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisOffice",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
@@ -48,10 +48,11 @@
 
     keywords="office,setuptools,development",  # Optional 搜索关键字
 
     packages=find_packages(),  # Required
 
     python_requires=">=3.7, <4",  # python 版本要求
 
-    install_requires=["pandas","vgis-utils","fitz","openpyxl","python-docx"],  # Optional 第三方依赖库
+    install_requires=["pandas", "vgis-utils", "fitz", "openpyxl", "python-docx", "PyMuPDF", "comtypes", "frontend",
+                      "loguru"],  # Optional 第三方依赖库
 
-)
+)
```

### Comparing `vgis_office-1.0.1/vgis_office/vgis_excel/excelTools.py` & `vgis_office-1.0.2/vgis_office/vgis_excel/excelTools.py`

 * *Files 25% similar despite different names*

```diff
@@ -100,28 +100,16 @@
                 # writer.save()
                 # writer.close()
         else:
             # 创建空白excel
             fd = open(result_excel_path, 'w')
             fd.close()
 
-    @staticmethod
-    # 读取excel表内容指定行数据
-    def read_excel_data_values_by_row(row_num, excel_obj):
-        for row_index in range(len(excel_obj)):
-            # excel内容从第二行开始
-            if row_index == row_num-1:
-                result_row_values = excel_obj.values[row_index]
-                return result_row_values
 
-    @staticmethod
-    #  读取excel表字段
-    def read_excel_data_columns(excel_obj):
-        result_row_values = excel_obj.columns
-        return result_row_values
+
 
     @staticmethod
     # 根据Excel列索引值生成列字母名
     def get_column_name(column_index):
         ret = ''
         ci = column_index - 1
         index = ci // 26
```

### Comparing `vgis_office-1.0.1/vgis_office/vgis_pdf/pdfHelper.py` & `vgis_office-1.0.2/vgis_office/vgis_pdf/pdfHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # @Time    :  2023/3/23 19:03
 # @Author  : chenxw
 # @Email   : gisfanmachel@gmail.com
 # @File    : pdfHelper.py
 # @Descr   : pdf操作
 # @Software: PyCharm
 import fitz
-
+import os
+import comtypes.client
 
 # 将pdf转换为img
 def convert_pdf_to_img(pdf_file):
     doc = fitz.open(pdf_file)
     (file_pre_path, temp_filename) = os.path.split(pdf_file)
     (shot_name, file_ext) = os.path.splitext(temp_filename)
     img_path_list = []
@@ -24,17 +25,14 @@
         pm = page.getPixmap(matrix=trans, alpha=False)
         img_path = os.path.join(file_pre_path, shot_name + "_" + str(pg) + ".png")
         img_path_list.append(img_path)
         pm.writePNG(img_path)
     return "&&&".join(img_path_list)
 
 
-import os
-import comtypes.client
-
 
 def get_path():
     path = "E:\\work-维璟\\2 项目实施\\2.1行业应用部\\54保险OCR识别\\原油附件压缩包" # 获取当前运行路径
     filename_list = os.listdir(path)
     wordname_list = [filename for filename in filename_list if filename.endswith((".doc", ".docx"))]
     for wordname in wordname_list:
         # 分离word文件名称和后缀，转化为pdf名称
```

### Comparing `vgis_office-1.0.1/vgis_office/vgis_word/worddir2xls.py` & `vgis_office-1.0.2/vgis_office/vgis_word/worddir2xls.py`

 * *Files identical despite different names*

### Comparing `vgis_office-1.0.1/vgis_office.egg-info/PKG-INFO` & `vgis_office-1.0.2/vgis_office.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-office
-Version: 1.0.1
+Version: 1.0.2
 Summary: A libary for office operator
 Home-page: https://github.com/gisfanmachel/vgisOffice
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis office lib
```

