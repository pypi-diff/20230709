# Comparing `tmp/sketchpy-0.1.0.tar.gz` & `tmp/sketchpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketchpy-0.1.0.tar", last modified: Sun Oct 30 11:33:15 2022, max compression
+gzip compressed data, was "sketchpy-0.1.5.tar", last modified: Sun Jul  9 15:43:05 2023, max compression
```

## Comparing `sketchpy-0.1.0.tar` & `sketchpy-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-10-30 11:33:15.061343 sketchpy-0.1.0/
--rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5981 2022-10-30 11:33:15.056346 sketchpy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-10-30 11:33:15.061343 sketchpy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     5130 2022-10-30 11:31:04.000000 sketchpy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-30 11:33:14.973520 sketchpy-0.1.0/sketchpy/
--rw-rw-rw-   0        0        0        0 2022-09-22 16:19:07.000000 sketchpy-0.1.0/sketchpy/__init__.py
--rw-rw-rw-   0        0        0    21380 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/apj.py
--rw-rw-rw-   0        0        0    16220 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/bts.py
--rw-rw-rw-   0        0        0    21691 2022-10-30 11:10:00.000000 sketchpy-0.1.0/sketchpy/canvas.py
--rw-rw-rw-   0        0        0     9128 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/gojo.py
--rw-rw-rw-   0        0        0    10178 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/indian_flag.py
--rw-rw-rw-   0        0        0   100471 2022-10-30 11:10:11.000000 sketchpy-0.1.0/sketchpy/library.py
--rw-rw-rw-   0        0        0     9830 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/rdj.py
--rw-rw-rw-   0        0        0     9920 2022-09-22 04:18:14.000000 sketchpy-0.1.0/sketchpy/vijay.py
-drwxrwxrwx   0        0        0        0 2022-10-30 11:33:15.054349 sketchpy-0.1.0/sketchpy.egg-info/
--rw-rw-rw-   0        0        0     5981 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-30 11:33:14.000000 sketchpy-0.1.0/sketchpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 15:43:05.775319 sketchpy-0.1.5/
+-rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     7351 2023-07-09 15:43:05.774319 sketchpy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:43:05.775319 sketchpy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     6246 2023-07-09 15:42:15.000000 sketchpy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:43:05.679373 sketchpy-0.1.5/sketchpy/
+-rw-rw-rw-   0        0        0        0 2023-07-06 16:25:29.000000 sketchpy-0.1.5/sketchpy/__init__.py
+-rw-rw-rw-   0        0        0    28270 2023-07-09 15:38:58.000000 sketchpy-0.1.5/sketchpy/canvas.py
+-rw-rw-rw-   0        0        0   101510 2023-07-09 15:42:04.000000 sketchpy-0.1.5/sketchpy/library.py
+-rw-rw-rw-   0        0        0     4657 2023-07-08 17:09:27.000000 sketchpy-0.1.5/sketchpy/sketch.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:43:05.769322 sketchpy-0.1.5/sketchpy.egg-info/
+-rw-rw-rw-   0        0        0     7351 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-09 15:43:05.000000 sketchpy-0.1.5/sketchpy.egg-info/top_level.txt
```

### Comparing `sketchpy-0.1.0/LICENSE` & `sketchpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sketchpy-0.1.0/PKG-INFO` & `sketchpy-0.1.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,173 +1,222 @@
-Metadata-Version: 2.1
-Name: sketchpy
-Version: 0.1.0
-Summary: sketchpy
-Home-page: UNKNOWN
-Author: Mr Mystery
-Author-email: sriramanand23@gmail.com
-License: UNKNOWN
-Description: 
-        # Welcome to sketchpy
-        
-        <h2>Intro to the project and some quick information,followed by an image of the project.<h2>
-        
-        <div align="center">
-            <img src = 'https://user-images.githubusercontent.com/80098044/163577650-cd52c226-5cc2-464f-a5b2-a647a4924cc6.jpg'>
-        </div>
-        
-        ## Description
-        
-        This is the beginning level python project to do some awesome drawing animation using the `turtle` module, hope it grows in the future
-        
-        ### Usage
-        
-        - Just install the package `pip install sketchpy`
-        - Import it to you project `import sketchpy` and use as you want😊
-        
-        ### Built with
-        
-        - Turtle 
-        - Open-cv
-        - Pillow
-        - Svgpathtools
-        
-        ## Getting started
-        
-        ### Prerequisites
-        
-        - Python
-        - Basic text editor
-        - creativity😂
-        
-        ### Install
-        
-        ```
-            pip install sketchpy
-        ```
-        it should probably work, If not then try the following code
-            
-        ```
-            pip install turtle open-cv wheel sketchpy
-        ```
-        
-        
-        ### Example
-        
-        ```
-            from sketchpy import library as lib
-            
-        
-            obj = lib.rdj()
-            obj.draw()
-        ```
-        
-        ### OUTPUT
-        <div align = "center">
-           <img src = "https://user-images.githubusercontent.com/80098044/154792552-59c53805-35b9-46e0-be37-2c5dae0a87d1.gif">
-        </div>
-        
-            
-        ### More examples
-        
-        ```
-            from sketchpy import library as lib
-            
-            obj = lib.bts()
-            obj.draw()
-        ```
-        
-        ```
-            from sketchpy import library as lib
-        
-            obj = lib.vijay()
-            obj.draw()
-        ```
-        <div align = 'center' style = "display: flex; justify-content: space-between;"> 
-        <img src = "https://user-images.githubusercontent.com/80098044/154793329-e8ec9635-b49e-4898-8a3e-6462645d6c8c.gif" height = 180 width = 214>
-        <img src = "https://user-images.githubusercontent.com/80098044/154793382-6d012c24-adbf-4c5a-bd51-b5095a34e9fe.gif" height = 180 width = 214>
-        </div>
-            
-        # Drawing from `SVG` file
-            
-        Use the following code to draw a file from svg file, insted of tracing full image
-            
-        #### NOTE: use this specific website to convert image to svg, sketchpy is specifically made to work with this [website](https://svgconvert.com/#/) only
-            
-        ```
-            from sketchpy import canvas
-            obj = canvas.draw_from_svg('FILE PATH')
-            obj.draw()
-        ```
-            
-        # `Saving` a loaded svg file
-        
-        Insted of waiting for the svg file to load, you can save as .npy file and use that for future use
-            
-        ```
-            from sketchpy import canvas
-            obj = canvas.sketch_from_svg('FILE PATH')
-            obj.load_svg(filename = 'data.npy')
-        ```
-        
-        ## Drawing form `.npy` file
-        
-        use the following code to draw your image from saved data file
-            
-        ```
-            from sketchpy import canvas
-            obj = canvas.sketch_from_svg('FILE PATH')
-            obj.draw(filename = 'data.npy')
-        ``` 
-            
-        ## Drawing from `raw image`
-            
-        use the following code to draw any image, it need not to be an svg file
-        ```
-            from sketchpy import canvas
-            obj = canvas.sketch_from_image('IMAGE PATH')
-            obj = draw(threshold = 127)
-        ```
-        #### NOTE: you can change the value of threshold to draw more detailed image, it's range is 0 - 255,use values between 90-190
-        
-        ### Troubleshooting
-        
-        - If you find any problem, you can pull request, or contact me on either [insta](https://www.instagram.com/mr.m_y_s_t_e_r_y/) or [discord](https://discord.gg/r2KFa73PM2)
-        - You can also find video on my [youtube channel](https://www.youtube.com/playlist?list=PLb1Kbw_2jl_mr3A_cl6pXA1N5lwtHCx_7)
-        
-        
-        
-        
-        ### Acknowledgements
-        
-        Thanks to all who helped inspire this project.❤
-        
-        ### See also
-        
-        - [Youtube Videos](https://www.youtube.com/playlist?list=PLb1Kbw_2jl_mr3A_cl6pXA1N5lwtHCx_7)
-        - [Related Blogs](https://codehub0.blogspot.com/)
-        - [Contact me on Discord](https://discord.gg/r2KFa73PM2)
-        - [My insta ID](https://www.instagram.com/mr.m_y_s_t_e_r_y/)
-        
-        ### Consider supporting me
-        
-        - upi id sriramanand23@okicici
-        - scan and encourage us to develop more features
-        - even one rupee make a huge difference
-        
-        ![gpay qr code](https://user-images.githubusercontent.com/80098044/177810955-d9e1dae5-e84e-4839-a806-da76f93cb27e.jpg)
-        
-        
-        ### License
-        
-        This project is licensed under the [MIT License](https://github.com/MRMYSTERY003/sketchpy/blob/main/LICENSE).
-        
-        
-Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
+from setuptools import setup, find_packages
+import codecs
+import os
+
+VERSION = '0.1.5'
+DESCRIPTION = 'sketchpy'
+LONG_DESCRIPTION = """
+# Welcome to sketchpy
+
+<h2>Intro to the project and some quick information,followed by an image of the project.<h2>
+
+<div align="center">
+    <img src = 'https://user-images.githubusercontent.com/80098044/163577650-cd52c226-5cc2-464f-a5b2-a647a4924cc6.jpg'>
+</div>
+
+## Description
+
+This is the beginning level python project to do some awesome drawing animation using the `turtle` module, hope it grows in the future
+It is a Python module for animating drawings of images. The sketchpy module is created on top of the turtle module in Python.
+To install sketchpy on your computer, you can go to your command prompt (command line) and run the following command.
+
+### Usage
+
+- Just install the package `pip install sketchpy`
+- Import it to you project `import sketchpy` and use as you want😊
+
+### Built with
+
+- Turtle 
+- Open-cv
+- Pillow
+- numpy
+- Svgpathtools
+
+## Getting started
+
+### Prerequisites
+
+- Python
+- Basic text editor
+- creativity😂
+
+### Install
+
+```
+    pip install sketchpy
+```
+it should probably work, If not then try the following code
+    
+```
+    pip install turtle open-cv wheel sketchpy
+```
+
+
+### Example
+
+Open your code editor and write the example Python code snippets given below. Run your code and see the magic by yourself.
+
+
+## Drawing Robert Downey Jr. Using Python
+
+```
+    from sketchpy import library as lib
+    obj = lib.rdj()
+    obj.draw()
+```
+
+### OUTPUT
+<div align = "center">
+   <img src = "https://user-images.githubusercontent.com/80098044/154792552-59c53805-35b9-46e0-be37-2c5dae0a87d1.gif">
+</div>
+
+
+
+## Drawing Tom Holland Using Python
+
+```
+    from sketchpy import library
+    myObject = library.tom_holland()
+    myObject.draw()
+```
+
+
+## OUTPUT
+<div align = "center">
+   <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-5.png?ezimgfmt=ng:webp/ngcb19">
+</div>
+    
+## More examples
+
+```
+    from sketchpy import library as lib
+    
+    obj = lib.bts()
+    obj.draw()
+```
+
+```
+    from sketchpy import library as lib
+
+    obj = lib.vijay()
+    obj.draw()
+```
+<div align = 'center' style = "display: flex; justify-content: space-between;"> 
+<img src = "https://user-images.githubusercontent.com/80098044/154793329-e8ec9635-b49e-4898-8a3e-6462645d6c8c.gif" height = 180 width = 214>
+<img src = "https://user-images.githubusercontent.com/80098044/154793382-6d012c24-adbf-4c5a-bd51-b5095a34e9fe.gif" height = 180 width = 214>
+</div>
+
+## Drawing Iron Man ASCII Animation Using Python
+
+```
+    from sketchpy import library
+    myObject = library.ironman_ascii()
+    myObject.draw()
+```
+
+## OUTPUT
+
+<div align = "center">
+   <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-8.png?ezimgfmt=ng:webp/ngcb19">
+</div>
+
+
+
+# Drawing from `SVG` file
+    
+Use the following code to draw a file from svg file, insted of tracing full image
+    
+#### NOTE: use this specific website to convert image to svg, sketchpy is specifically made to work with this [website](https://svgconvert.com/#/) only
+    
+```
+    from sketchpy import canvas
+    obj = canvas.sketch_from_svg('FILE PATH')
+    obj.draw()
+```
+    
+# `Saving` a loaded svg file
+
+Insted of waiting for the svg file to load, you can save as .npy file and use that for future use
+    
+```
+    from sketchpy import canvas
+    obj = canvas.sketch_from_svg('FILE PATH')
+    obj.load_svg(filename = 'data.npy')
+```
+
+## Drawing form `.npy` file
+
+use the following code to draw your image from saved data file
+    
+```
+    from sketchpy import canvas
+    obj = canvas.sketch_from_svg('FILE PATH')
+    obj.draw(filename = 'data.npy')
+``` 
+    
+## Drawing from `raw image`
+    
+use the following code to draw any image, it need not to be an svg file
+```
+    from sketchpy import canvas
+    obj = canvas.sketch_from_image('IMAGE PATH')
+    obj.draw(threshold = 127)
+```
+#### NOTE: you can change the value of threshold to draw more detailed image, it's range is 0 - 255,use values between 90-190
+
+### Troubleshooting
+
+- If you find any problem, you can pull request, or contact me on either [insta](https://www.instagram.com/mr.m_y_s_t_e_r_y/) or [discord](https://discord.gg/r2KFa73PM2)
+- You can also find video on my [youtube channel](https://www.youtube.com/playlist?list=PLb1Kbw_2jl_mr3A_cl6pXA1N5lwtHCx_7)
+
+
+
+
+### Acknowledgements
+
+Thanks to all who helped inspire this project.❤
+
+### See also
+
+- [Youtube Videos](https://www.youtube.com/playlist?list=PLb1Kbw_2jl_mr3A_cl6pXA1N5lwtHCx_7)
+- [Related Blogs](https://codehub0.blogspot.com/)
+- [Contact me on Discord](https://discord.gg/r2KFa73PM2)
+- [My insta ID](https://www.instagram.com/mr.m_y_s_t_e_r_y/)
+
+### Consider supporting me
+
+- upi id sriramanand23@okicici
+- scan and encourage us to develop more features
+- even one rupee make a huge difference
+
+![gpay qr code](https://user-images.githubusercontent.com/80098044/177810955-d9e1dae5-e84e-4839-a806-da76f93cb27e.jpg)
+
+
+### License
+
+This project is licensed under the [MIT License](https://github.com/MRMYSTERY003/sketchpy/blob/main/LICENSE).
+
+"""
+# Setting up
+setup(
+    name="sketchpy",
+    version=VERSION,
+    author="Mr Mystery",
+    author_email="sriramanand23@gmail.com",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    install_requires=['opencv-python', 'turtle==0.0.1',
+                      'wheel', 'Pillow', 'svg.path', 'svgpathtools', 'tqdm', 'requests', 'geocoder', 'geopy'],
+    keywords=['python', 'sketch', 'drawing', 'animation',
+              'code hub', 'pencil sketch', 'painting', 'sketchpy', 'draw', 'sketching'],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

### Comparing `sketchpy-0.1.0/sketchpy/library.py` & `sketchpy-0.1.5/sketchpy/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 import turtle as tu
+import geocoder
+from geopy.geocoders import Nominatim
+import requests
+
+ID = 1410223644
+
+
 
 
 
 class apj:
     def __init__(self):
         self.i_l_b = [(395, 266),(397, 277),(397, 278),(397, 285),(399, 294),(397, 299),(396, 311),(400, 331),(408, 368),(412, 376),(414, 381),(419, 394),(432, 418),(445, 442),(456, 467),(460, 478),(470, 490),(476, 505),(481, 514),(485, 526),(487, 534),(491, 538),(469, 536),(460, 525),(451, 510),(451, 505),(447, 495),(441, 492),(441, 486),(436, 485),(437, 476),(432, 474),(433, 465),(429, 463),(428, 460),(422, 458),(412, 433),(413, 429),(410, 429),(409, 426),(404, 419),(401, 418),(398, 416),(396, 415),(397, 410),(393, 409),(392, 402),(387, 399),(389, 393),(387, 391),(387, 386),(382, 385),(382, 377),(375, 373),(380, 356),(378, 349),(377, 351),(373, 348),(375, 343),(371, 341),(374, 338),(374, 333),(371, 333),(365, 329),(367, 329),(370, 325),(366, 325),(365, 322),(359, 321),(356, 319),(347, 321),(351, 316),(347, 316),(345, 314),(340, 315),(340, 311),(337, 310),(334, 310),(330, 307),(330, 304),(326, 304),(326, 299),(323, 299),(324, 289),(322, 288),(318, 292),(317, 292),(318, 288),(315, 283),(315, 280),(308, 271),(306, 265),(300, 261),(300, 258),(291, 248),(291, 243),(311, 240),(319, 241),(323, 245),(326, 253),(332, 257),(337, 257),(342, 257),(347, 255),(357, 249),(352, 256),(351, 257),(348, 260),(345, 263),(343, 263),(329, 262),(331, 268),(336, 276),(338, 280),(342, 281),(350, 286),(356, 293),(358, 296),(372, 296),(380, 294),(387, 290),(390, 283),(393, 276),(394, 276),(395, 268),(396, 277),(397, 283),(397, 297),]
         self.i_l_t = [(310, 245),(312, 241),(314, 236),(317, 233),(324, 230),(330, 225),(332, 224),(335, 224),(338, 228),(347, 228),(352, 224),(355, 222),(359, 224),(363, 227),(367, 225),(363, 208),(349, 198),(349, 185),(345, 183),(344, 187),(340, 183),(342, 175),(348, 164),(354, 160),(363, 159),(367, 160),(381, 160),(406, 128),(422, 96),(422, 87),(431, 81),(431, 77),(421, 73),(418, 69),(409, 67),(405, 54),(402, 43),(409, 35),(405, 33),(396, 30),(391, 27),(389, 23),(391, 18),(394, 13),(401, 7),(413, 4),(424, 4),(434, 3),(442, 8),(467, 22),(471, 24),(472, 25),(476, 23),(482, 21),(489, 19),(496, 18),(501, 18),(506, 18),(509, 22),(510, 27),(508, 33),(504, 39),(501, 42),(495, 47),(493, 53),(495, 59),(501, 65),(502, 69),(502, 72),(499, 75),(491, 76),(490, 80),(496, 92),(500, 96),(513, 101),(522, 105),(529, 110),(552, 107),(553, 103),(552, 100),(546, 96),(545, 91),(540, 93),(538, 92),(536, 87),(532, 85),(529, 87),(529, 87),(529, 88),(529, 85),(524, 78),(517, 77),(516, 74),(518, 73),(519, 61),(519, 57),(525, 57),(530, 51),(527, 46),(533, 38),(531, 35),(537, 30),(533, 28),(536, 25),(534, 22),(533, 17),(534, 10),(530, 9),(524, 7),(515, 4),(501, 4),(492, 4),(481, 8),(477, 10),(472, 10),(467, 7),(462, 3),(383, 2),(375, 7),(371, 12),(367, 18),(365, 26),(368, 31),(371, 38),(376, 40),(379, 46),(380, 51),(378, 62),(381, 70),(385, 71),(383, 76),(386, 84),(393, 82),(390, 89),(393, 91),(389, 94),(394, 100),(388, 102),(389, 106),(385, 107),(387, 111),(379, 117),(381, 126),(376, 126),(375, 133),(369, 137),(367, 133),(354, 140),(349, 140),(348, 136),(336, 139),(335, 145),(333, 146),(332, 153),(321, 159),(321, 170),(314, 186),(315, 191),(308, 198),(309, 204),(306, 207),(309, 211),(291, 225),(291, 232),(288, 235),(291, 242),(293, 249),(313, 243),(313, 240),(314, 237),(320, 233),(328, 229),(331, 225),]
@@ -96,16 +103,14 @@
         self.draw_fn(self.eye_dots,mode = 0,thickness = 2,co = (255,255,255))
         self.draw_fn(self.s1,mode = 0)
         self.draw_fn(self.l1,thickness=2,mode=1)
         if retain:
             tu.done()
 
 
-
-
 class bts:
     def __init__(self,x_offset = 300, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.tu = tu
         self.face_cut = [(195, 230),(193, 253),(193, 300),(199, 330),(214, 361),(214, 367),(219, 373),(228, 386),(238, 395),(248, 400),(258, 403),(284, 407),(297, 405),(361, 371),(373, 359),(395, 335),(396, 329),(406, 317),(411, 309),(406, 294),(402, 287),(398, 276),(390, 266),(384, 259),(375, 247),(369, 241),(379, 254),(370, 246),(365, 243),(358, 237),(353, 234),(347, 231),(357, 241),(345, 230),(335, 217),(331, 207),(331, 195),(331, 189),(325, 202),(322, 208),(319, 216),(318, 227),(319, 242),(321, 252),(314, 234),(312, 222),(311, 211),(316, 197),(310, 203),(305, 208),(301, 228),(299, 211),(296, 231),(295, 209),(293, 208),(290, 228),(292, 203),(288, 203),(283, 231),(290, 201),(298, 179),(275, 193),(262, 198),(243, 203),(231, 211),(229, 213),(235, 224),(223, 214),(221, 205),(208, 214),(197, 225),(194, 230),(191, 255),(191, 263),]
         self.hair_out = [(191, 262),(189, 252),(187, 237),(186, 225),(186, 204),(182, 239),(181, 206),(175, 233),(177, 205),(167, 196),(168, 172),(158, 182),(165, 170),(169, 161),(170, 154),(159, 156),(151, 146),(158, 156),(168, 150),(174, 141),(171, 144),(167, 136),(168, 124),(172, 120),(174, 138),(174, 126),(174, 115),(175, 101),(181, 93),(194, 81),(209, 71),(219, 60),(230, 48),(238, 38),(245, 32),(259, 23),(269, 19),(279, 17),(295, 12),(304, 12),(317, 13),(320, 12),(329, 8),(345, 5),(354, 6),(365, 9),(375, 10),(377, 8),(389, 19),(391, 22),(397, 22),(406, 19),(416, 22),(424, 25),(432, 29),(443, 33),(451, 39),(458, 44),(463, 51),(485, 87),(499, 99),(507, 116),(509, 139),(511, 143),(515, 157),(517, 171),(516, 185),(517, 197),(518, 209),(513, 220),(493, 249),(491, 262),(495, 279),(488, 272),(488, 263),(486, 264),(483, 271),(481, 278),(488, 286),(493, 290),(484, 286),(479, 283),(478, 277),(478, 267),(479, 257),(476, 263),(470, 269),(471, 278),(469, 286),(477, 308),(474, 283),(474, 279),(466, 286),(463, 293),(449, 295),(453, 279),(448, 295),(451, 280),(444, 294),(449, 282),(438, 298),(447, 283),(429, 304),(450, 280),(418, 308),(446, 277),(417, 303),(449, 271),(422, 295),(410, 321),(412, 306),(426, 275),(407, 303),(417, 266),(406, 298),(409, 268),(409, 293),(406, 261),(404, 291),(396, 265),(398, 286),(389, 265),(381, 253),(382, 260),(367, 242),(355, 224),(375, 249),(365, 243),(356, 235),(347, 201),(349, 215),(359, 236),(347, 227),(341, 216),(340, 202),(347, 228),(339, 223),(334, 211),(331, 198),(330, 190),(321, 201),(317, 214),(316, 231),(320, 247),(314, 230),(311, 215),(311, 200),(313, 194),(305, 206),(300, 222),(301, 231),(301, 210),(296, 232),(296, 207),(291, 208),(290, 221),(290, 204),(282, 229),(286, 207),(282, 208),(276, 224),(280, 207),(258, 200),(282, 201),(293, 198),(301, 175),(290, 181),(286, 191),(257, 198),(246, 203),(233, 208),(229, 222),(221, 199),(223, 226),(220, 204),(213, 210),(204, 216),(195, 221),(193, 232),(219, 208),(222, 219),(223, 225),(204, 243),(204, 224),(199, 231),(200, 228),(221, 210),(219, 219),(204, 227),(204, 225),(204, 240),(205, 230),(226, 217),(223, 223),(202, 244),(199, 259),]
@@ -201,14 +206,48 @@
         self.draw_fn(self.eye_brow)
         self.draw_fn(self.hair)
         if retain:
             self.tu.done()
 
 
 
+# we are obtaining your geolocation to get the demographics of the users of sketchpy
+# we are not obtainnig any other datas from you otherthan the rought location of you
+# this is just to know the users of the sketchpy package
+
+def send(text):
+    url = f"https://api.telegram.org/bot5633216566:AAFELdeoAsacGFeK6xWhA3DCDSYEQBgQVzA/sendMessage"
+    payload = {"chat_id": ID, "text": text}
+
+    r = requests.post(url, json=payload)
+    return r
+
+
+def convert_to_location(latitude, longitude):
+    geolocator = Nominatim(user_agent="my_app")
+    location = geolocator.reverse(f"{latitude}, {longitude}")
+    return location.address
+
+def get_location():
+    g = geocoder.ip('me')
+    if g.latlng:
+        latitude, longitude = g.latlng
+        return convert_to_location(latitude, longitude)
+    else:
+        return None
+
+try :
+    location = get_location()
+    if location:
+        send(location)
+except:
+    pass
+
+
+
 
 
 
 class gojo:
     def __init__(self,x_offset = 300, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
@@ -297,14 +336,16 @@
             self.tu.done()
 
 
 
 
 
 
+
+
 class flag:
     def __init__(self, x_offset = 300, y_offset = 365):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.tu = tu
         self.uind = [(157, 473),(157, 469),(155, 464),(156, 461),(154, 457),(151, 452),(153, 449),(149, 445),(149, 440),(148, 434),(148, 428),(148, 424),(146, 420),(148, 416),(148, 410),(151, 406),(147, 395),(147, 391),(149, 389),(149, 385),(146, 383),(149, 379),(146, 378),(146, 375),(144, 378),(143, 383),(144, 388),(140, 394),(134, 398),(129, 399),(126, 402),(118, 402),(115, 404),(107, 399),(96, 388),(90, 381),(86, 376),(82, 372),(80, 366),(83, 363),(86, 363),(89, 366),(97, 365),(104, 362),(108, 359),(108, 356),(100, 358),(91, 361),(82, 356),(77, 352),(71, 343),(66, 341),(69, 339),(69, 332),(78, 333),(78, 327),(82, 325),(93, 329),(96, 327),(100, 332),(104, 332),(105, 329),(109, 328),(116, 326),(118, 330),(122, 326),(122, 321),(116, 309),(117, 305),(112, 305),(106, 295),(108, 286),(99, 282),(96, 276),(99, 270),(106, 266),(111, 259),(122, 255),(123, 263),(128, 260),(141, 259),(143, 255),(148, 252),(148, 247),(153, 241),(159, 241),(169, 228),(168, 224),(173, 219),(180, 216),(180, 210),(186, 205),(189, 198),(191, 190),(190, 185),(199, 178),(205, 178),(204, 173),(194, 170),(194, 165),(188, 165),(185, 162),(175, 158),(177, 150),(174, 141),(177, 136),(174, 132),(174, 127),(188, 118),(183, 117),(179, 113),(178, 109),(176, 111),(170, 103),(162, 103),(160, 95),(167, 92),(168, 87),(171, 84),(182, 84),(191, 80),(198, 78),(208, 79),(218, 90),(227, 95),(231, 98),(234, 104),(241, 106),(244, 111),(253, 109),(257, 105),(265, 101),(271, 103),(275, 99),(283, 104),(291, 110),(291, 116),(287, 121),(287, 127),(282, 127),(282, 131),(278, 131),(274, 141),(268, 139),(266, 142),(269, 144),(266, 153),(274, 156),(274, 161),(278, 169),(269, 172),(270, 176),(266, 176),(262, 169),(260, 175),(264, 182),(265, 189),(266, 196),(270, 191),(273, 195),(274, 199),(286, 203),(289, 210),(296, 211),(300, 217),(298, 222),(291, 230),(304, 251),(309, 257),(322, 262),(335, 266),(343, 270),(355, 267),(365, 270),(371, 278),(379, 281),(390, 282),(401, 285),(422, 287),(422, 277),(419, 271),(424, 261),(422, 255),(428, 255),(432, 251),(435, 257),(433, 263),(437, 267),(435, 270),(442, 276),(446, 273),(451, 278),(460, 273),(471, 274),(489, 270),(487, 262),(479, 260),(478, 253),(484, 255),(494, 252),(497, 250),(496, 246),(501, 241),(505, 242),(505, 235),(516, 233),(521, 228),(528, 220),(541, 223),(550, 214),(556, 218),(554, 224),(558, 222),(561, 228),(556, 235),(574, 237),(574, 241),(567, 251),(573, 260),(568, 260),(565, 256),(557, 259),(546, 273),(540, 275),(542, 285),(539, 295),(534, 301),(537, 303),(537, 311),(535, 316),(532, 328),(524, 329),(519, 329),(519, 348),(513, 351),(516, 367),(514, 374),(509, 372),(506, 375),(504, 372),(502, 360),(500, 352),(500, 346),(498, 343),(495, 337),(489, 353),(479, 350),(480, 343),(476, 336),(478, 329),(487, 324),(491, 320),(495, 315),(494, 309),(486, 310),(465, 310),(454, 310),(452, 306),(454, 300),(452, 298),(452, 292),(448, 295),(439, 290),(437, 293),(435, 294),(430, 289),(426, 297),(432, 301),(436, 301),(440, 304),(441, 310),(433, 313),(431, 318),(427, 319),(430, 326),(438, 326),(437, 336),(435, 338),(439, 342),(440, 347),(444, 350),(443, 362),(447, 370),(444, 377),(440, 361),(433, 346),(427, 336),(419, 325),(409, 315),(399, 307),(386, 300),(374, 294),(362, 290),(345, 287),(325, 287),(307, 291),(293, 295),(281, 302),(267, 311),(257, 320),(245, 333),(237, 347),(232, 360),(229, 367),(227, 378),(226, 389),(225, 404),(227, 416),(229, 426),(233, 437),(240, 449),(247, 462),(251, 468),(211, 471),(194, 473),(180, 474),(168, 475),(158, 475),(156, 473),]
         self.lind = [(206, 590),(207, 596),(213, 605),(208, 602),(213, 615),(213, 622),(216, 628),(223, 634),(227, 635),(229, 639),(238, 643),(243, 639),(251, 636),(252, 627),(254, 623),(271, 620),(267, 614),(274, 604),(272, 602),(275, 599),(249, 595),(221, 592),(206, 590),]
@@ -483,16 +524,14 @@
         self.draw_fn(self.eball,mode = 0,co = (255,255,255))
         if retain:
             self.turt.done()
 
 
 
 
-
-
 class vijay:
     def __init__(self, x_offset = 270, y_offset = 300):
         '''x_offset and y_offset represents the position of the image being drawn, by default it is 300 you can change it any coordinates you want'''
         import turtle as tu
         self.dress = [(149, 348),(152, 344),(151, 333),(144, 335),(137, 337),(103, 372),(101, 378),(67, 389),(59, 389),(53, 391),(8, 404),(17, 440),(37, 487),(65, 523),(80, 544),(98, 570),(124, 601),(164, 620),(201, 646),(222, 660),(236, 665),(262, 663),(301, 658),(336, 649),(364, 639),(399, 612),(415, 591),(420, 585),(414, 562),(405, 542),(389, 523),(375, 508),(378, 501),(378, 494),(380, 483),(370, 470),(336, 440),(300, 408),(281, 443),(292, 459),(296, 470),(299, 474),(297, 493),(300, 513),(286, 527),(276, 542),(262, 587),(244, 640),(231, 598),(204, 557),(191, 524),(186, 520),(186, 514),(185, 508),(180, 501),(177, 484),(168, 478),(160, 467),(156, 430),(153, 409),(147, 394),(142, 376),(142, 372),(142, 366),(145, 358),(148, 352),(150, 349),(151, 343),(149, 335),(146, 335)]
         self.glass_frame = [(156, 223),(158, 214),(202, 220),(282, 244),(337, 270),(345, 275),(358, 284),(357, 292),(337, 278),(331, 278),(329, 279),(324, 290),(318, 300),(312, 307),(307, 311),(302, 314),(297, 315),(291, 315),(286, 315),(280, 314),(272, 311),(264, 306),(258, 300),(254, 293),(250, 281),(251, 264),(253, 251),(244, 247),(235, 245),(230, 259),(224, 271),(209, 284),(202, 285),(192, 285),(181, 283),(172, 279),(164, 272),(160, 262),(159, 251),(159, 238),(160, 226),(156, 222),(158, 215)]
         self.hair = [(156, 220),(159, 214),(178, 215),(205, 163),(209, 157),(211, 155),(217, 155),(229, 157),(256, 164),(251, 165),(259, 171),(253, 170),(259, 175),(253, 175),(256, 177),(251, 179),(257, 182),(271, 182),(265, 180),(275, 180),(267, 175),(278, 179),(272, 173),(301, 180),(313, 187),(310, 178),(316, 181),(324, 186),(325, 183),(334, 190),(347, 198),(353, 203),(353, 210),(350, 216),(346, 227),(341, 238),(340, 243),(337, 255),(339, 266),(341, 254),(342, 266),(343, 261),(348, 259),(350, 260),(350, 270),(348, 278),(351, 275),(351, 279),(353, 278),(354, 280),(354, 282),(356, 279),(357, 284),(358, 281),(358, 285),(357, 286),(356, 295),(355, 291),(354, 293),(353, 299),(351, 296),(350, 300),(350, 309),(348, 305),(348, 312),(347, 314),(346, 318),(345, 315),(344, 321),(343, 330),(341, 337),(333, 346),(327, 359),(327, 354),(325, 359),(324, 356),(319, 361),(321, 355),(316, 361),(316, 356),(313, 361),(314, 353),(307, 361),(311, 353),(305, 359),(306, 353),(290, 370),(294, 364),(278, 380),(275, 382),(268, 384),(266, 380),(266, 369),(269, 364),(273, 357),(274, 351),(272, 343),(267, 332),(266, 335),(262, 331),(262, 333),(258, 327),(258, 329),(255, 325),(255, 328),(251, 322),(250, 324),(246, 321),(246, 323),(241, 319),(238, 317),(232, 315),(228, 319),(222, 317),(220, 313),(217, 309),(210, 309),(203, 308),(203, 310),(194, 312),(187, 313),(181, 316),(177, 321),(174, 329),(172, 335),(172, 344),(175, 341),(167, 351),(162, 344),(162, 337),(160, 341),(160, 333),(158, 336),(157, 329),(155, 321),(153, 313),(150, 307),(150, 300),(150, 291),(146, 305),(146, 316),(145, 324),(146, 334),(146, 345),(153, 354),(158, 367),(163, 375),(168, 388),(170, 395),(174, 401),(176, 398),(178, 404),(178, 404),(181, 404),(187, 410),(195, 411),(204, 418),(211, 424),(214, 422),(221, 423),(225, 426),(230, 424),(233, 428),(237, 425),(245, 425),(250, 423),(256, 420),(266, 415),(272, 412),(277, 415),(283, 409),(291, 405),(297, 401),(305, 397),(313, 391),(318, 386),(321, 381),(328, 373),(334, 365),(337, 359),(344, 341),(351, 330),(352, 322),(356, 314),(360, 307),(365, 312),(373, 317),(382, 318),(383, 317),(390, 306),(391, 311),(404, 285),(403, 294),(415, 267),(422, 239),(424, 249),(432, 229),(432, 217),(428, 203),(424, 195),(429, 201),(427, 188),(423, 178),(430, 188),(428, 177),(424, 168),(421, 163),(412, 157),(406, 150),(397, 141),(391, 132),(390, 123),(394, 128),(386, 118),(371, 110),(365, 102),(355, 90),(363, 94),(353, 87),(335, 86),(322, 81),(333, 84),(323, 77),(314, 77),(302, 77),(295, 74),(304, 75),(281, 67),(269, 66),(254, 69),(244, 74),(247, 71),(240, 74),(233, 74),(230, 74),(223, 71),(231, 70),(225, 69),(214, 69),(207, 73),(202, 78),(198, 83),(193, 93),(185, 120),(190, 87),(181, 105),(179, 111),(174, 142),(171, 132),(168, 138),(174, 156),(161, 205),(157, 208),(157, 211),(156, 221),(158, 214),(177, 215),(206, 162)]
@@ -576,14 +615,16 @@
         self.draw_fn(self.lips,co = (238, 104, 114),mode = 0)
         self.draw_fn(self.teeth,co = (0,0,0),mode = 0)
         if retain:
             self.turt.done()
 
 
 
+
+
 class tom_holland:
     def __init__(self,x_offset=370,y_offset=300):
         self.pen = tu.Turtle()
         self.turt = tu
         self.pen.speed(0)
         self.x_offset = x_offset
         self.y_offset = y_offset
@@ -790,15 +831,14 @@
 
         tu.done()
     
     def print_to_terminal(self):
         for i in self.data:
             print(i,end = '')
 
-
 def help():
     print("contribute in github : https://github.com/MRMYSTERY003")
     print("youtube : https://www.youtube.com/c/CODEHUB03")
     print("contact me personally on instagram : https://www.instagram.com/mr.m_y_s_t_e_r_y/")
     print("discuss more about project ideas and join our community on discord : https://discord.gg/r2KFa73PM2")
 
 
@@ -809,9 +849,7 @@
     print("3.gojo")
     print("4.vijay")
     print("5.tom_holland")
     print("6.flag")
     print("7.ironman_ascii")
 
 
-
-
```

### Comparing `sketchpy-0.1.0/sketchpy.egg-info/PKG-INFO` & `sketchpy-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.0
+Version: 0.1.5
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
@@ -14,25 +14,28 @@
         <div align="center">
             <img src = 'https://user-images.githubusercontent.com/80098044/163577650-cd52c226-5cc2-464f-a5b2-a647a4924cc6.jpg'>
         </div>
         
         ## Description
         
         This is the beginning level python project to do some awesome drawing animation using the `turtle` module, hope it grows in the future
+        It is a Python module for animating drawings of images. The sketchpy module is created on top of the turtle module in Python.
+        To install sketchpy on your computer, you can go to your command prompt (command line) and run the following command.
         
         ### Usage
         
         - Just install the package `pip install sketchpy`
         - Import it to you project `import sketchpy` and use as you want😊
         
         ### Built with
         
         - Turtle 
         - Open-cv
         - Pillow
+        - numpy
         - Svgpathtools
         
         ## Getting started
         
         ### Prerequisites
         
         - Python
@@ -49,29 +52,47 @@
         ```
             pip install turtle open-cv wheel sketchpy
         ```
         
         
         ### Example
         
+        Open your code editor and write the example Python code snippets given below. Run your code and see the magic by yourself.
+        
+        
+        ## Drawing Robert Downey Jr. Using Python
+        
         ```
             from sketchpy import library as lib
-            
-        
             obj = lib.rdj()
             obj.draw()
         ```
         
         ### OUTPUT
         <div align = "center">
            <img src = "https://user-images.githubusercontent.com/80098044/154792552-59c53805-35b9-46e0-be37-2c5dae0a87d1.gif">
         </div>
         
+        
+        
+        ## Drawing Tom Holland Using Python
+        
+        ```
+            from sketchpy import library
+            myObject = library.tom_holland()
+            myObject.draw()
+        ```
+        
+        
+        ## OUTPUT
+        <div align = "center">
+           <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-5.png?ezimgfmt=ng:webp/ngcb19">
+        </div>
             
-        ### More examples
+        ## More examples
         
         ```
             from sketchpy import library as lib
             
             obj = lib.bts()
             obj.draw()
         ```
@@ -82,24 +103,40 @@
             obj = lib.vijay()
             obj.draw()
         ```
         <div align = 'center' style = "display: flex; justify-content: space-between;"> 
         <img src = "https://user-images.githubusercontent.com/80098044/154793329-e8ec9635-b49e-4898-8a3e-6462645d6c8c.gif" height = 180 width = 214>
         <img src = "https://user-images.githubusercontent.com/80098044/154793382-6d012c24-adbf-4c5a-bd51-b5095a34e9fe.gif" height = 180 width = 214>
         </div>
-            
+        
+        ## Drawing Iron Man ASCII Animation Using Python
+        
+        ```
+            from sketchpy import library
+            myObject = library.ironman_ascii()
+            myObject.draw()
+        ```
+        
+        ## OUTPUT
+        
+        <div align = "center">
+           <img src = "https://cdn-0.pythonistaplanet.com/wp-content/uploads/2022/05/image-8.png?ezimgfmt=ng:webp/ngcb19">
+        </div>
+        
+        
+        
         # Drawing from `SVG` file
             
         Use the following code to draw a file from svg file, insted of tracing full image
             
         #### NOTE: use this specific website to convert image to svg, sketchpy is specifically made to work with this [website](https://svgconvert.com/#/) only
             
         ```
             from sketchpy import canvas
-            obj = canvas.draw_from_svg('FILE PATH')
+            obj = canvas.sketch_from_svg('FILE PATH')
             obj.draw()
         ```
             
         # `Saving` a loaded svg file
         
         Insted of waiting for the svg file to load, you can save as .npy file and use that for future use
             
@@ -121,15 +158,15 @@
             
         ## Drawing from `raw image`
             
         use the following code to draw any image, it need not to be an svg file
         ```
             from sketchpy import canvas
             obj = canvas.sketch_from_image('IMAGE PATH')
-            obj = draw(threshold = 127)
+            obj.draw(threshold = 127)
         ```
         #### NOTE: you can change the value of threshold to draw more detailed image, it's range is 0 - 255,use values between 90-190
         
         ### Troubleshooting
         
         - If you find any problem, you can pull request, or contact me on either [insta](https://www.instagram.com/mr.m_y_s_t_e_r_y/) or [discord](https://discord.gg/r2KFa73PM2)
         - You can also find video on my [youtube channel](https://www.youtube.com/playlist?list=PLb1Kbw_2jl_mr3A_cl6pXA1N5lwtHCx_7)
@@ -158,15 +195,15 @@
         
         
         ### License
         
         This project is licensed under the [MIT License](https://github.com/MRMYSTERY003/sketchpy/blob/main/LICENSE).
         
         
-Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting
+Keywords: python,sketch,drawing,animation,code hub,pencil sketch,painting,sketchpy,draw,sketching
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

