# Comparing `tmp/py_astrolab-0.1.5.tar.gz` & `tmp/py_astrolab-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.1.5.tar", max compression
+gzip compressed data, was "py_astrolab-0.1.6.tar", max compression
```

## Comparing `py_astrolab-0.1.5.tar` & `py_astrolab-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.1.5/README.md
--rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.1.5/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    16850 2023-06-21 20:38:42.474113 py_astrolab-0.1.5/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.1.5/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    70111 2023-06-17 10:10:20.247410 py_astrolab-0.1.5/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.1.5/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.1.5/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.1.5/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-05-29 18:14:56.449179 py_astrolab-0.1.5/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    26385 2023-06-21 20:10:47.767169 py_astrolab-0.1.5/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.1.5/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.1.5/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2356 2023-06-17 10:10:20.255187 py_astrolab-0.1.5/py_astrolab/report.py
--rwxr-xr-x   0        0        0     5061 2023-05-31 21:03:53.211311 py_astrolab-0.1.5/py_astrolab/types.py
--rwxr-xr-x   0        0        0     5952 2023-06-17 10:10:20.255187 py_astrolab-0.1.5/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      689 2023-06-21 20:48:27.158466 py_astrolab-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.1.6/README.md
+-rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.1.6/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    16850 2023-06-21 20:38:42.474113 py_astrolab-0.1.6/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.1.6/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    72284 2023-07-09 14:33:18.004388 py_astrolab-0.1.6/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.1.6/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.1.6/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    61624 2023-07-09 13:46:32.333795 py_astrolab-0.1.6/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.1.6/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.1.6/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    26385 2023-06-21 20:10:47.767169 py_astrolab-0.1.6/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.1.6/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.1.6/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2356 2023-06-17 10:10:20.255187 py_astrolab-0.1.6/py_astrolab/report.py
+-rwxr-xr-x   0        0        0     5061 2023-05-31 21:03:53.211311 py_astrolab-0.1.6/py_astrolab/types.py
+-rwxr-xr-x   0        0        0     5952 2023-06-17 10:10:20.255187 py_astrolab-0.1.6/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      689 2023-07-09 14:33:08.497846 py_astrolab-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.1.6/PKG-INFO
```

### Comparing `py_astrolab-0.1.5/py_astrolab/__init__.py` & `py_astrolab-0.1.6/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/aspects.py` & `py_astrolab-0.1.6/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.1.6/py_astrolab/charts/charts_svg.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,16 @@
             self.output_directory = Path(new_output_directory)
         else:
             self.output_directory = self.homedir
 
         # Template types:
         if template_type == "basic":
             self.xml_svg = DATADIR / 'templates/basic.xml'
+        elif template_type == 'minimal':
+            self.xml_svg = DATADIR / 'templates/minimal.xml'
         else:
             self.xml_svg = DATADIR / 'templates/extended.xml'
 
         # SVG Width
         self.natal_width = 772.2
         self.full_width = 1200
 
@@ -384,26 +386,56 @@
         elif type == "2":
             out = '%(#1)02d&#176;%(#2)02d&#39;' % {'#1': a, '#2': b_rounded}
         elif type == "1":
             out = '%(#1)02d&#176;' % {'#1': a}
         return str(out)
 
     # draw svg aspects: ring, aspect ring, degreeA degreeB
-    def __drawAspect(self, r, ar, degA, degB, color, label = None):
+    def __drawAspect(self, r, ar, degA, degB, color, orb=None, label=None, isAxis=False):
         offset = (int(self.houses_degree_ut[6]) / -1) + int(degA)
-        x1 = self.__sliceToX(0, ar, offset) + (r-ar)
-        y1 = self.__sliceToY(0, ar, offset) + (r-ar)
+        x1 = self.__sliceToX(0, ar, offset) + (r - ar)
+        y1 = self.__sliceToY(0, ar, offset) + (r - ar)
         offset = (int(self.houses_degree_ut[6]) / -1) + int(degB)
-        x2 = self.__sliceToX(0, ar, offset) + (r-ar)
-        y2 = self.__sliceToY(0, ar, offset) + (r-ar)
-        out = '            <line x1="'+str(x1)+'" y1="'+str(y1)+'" x2="'+str(x2)+'" y2="'+str(
-            y2)+'" style="stroke: '+color+'; stroke-width: 1; stroke-opacity: .9;"/>'
-        if label:
-            out += f'<text x="{x1}" y="{y1-10}" fill="{color}" text-anchor="middle" dominant-baseline="central">{label}</text>'
-        return out
+        x2 = self.__sliceToX(0, ar, offset) + (r - ar)
+        y2 = self.__sliceToY(0, ar, offset) + (r - ar)
+        if isAxis:
+            width = x2 - x1
+            height = y2 - y1
+            start = start = {'x': x1, 'y': y1}
+            end = {'x': x2, 'y': y2}
+            cut_by = 7
+            ratio = width / cut_by
+            firstCut = {'x': start['x'] + ratio, 'y': start['y'] + (height / width) * ratio }
+            lastCut = {'x': start['x'] + (cut_by - 1) * ratio, 'y': start['y'] + (height / width) * (cut_by - 1) * ratio }
+            add_arrow = f'marker-start: url(#arrowhead{label});'
+        else:
+            add_arrow = ''
+        if isAxis:
+            axis_stroke_width = '1.5'
+            axis_stroke_opacity = '1'
+            line = f'''
+                <g style="stroke-width: {axis_stroke_width}; stroke-opacity: {axis_stroke_opacity}; transform: translate(0, 0);" stroke-linecap="round" >
+                    <line x1="{start["x"]}" y1="{start["y"]}" x2="{firstCut["x"]}" y2="{firstCut["y"]}" style="stroke: {color}; {add_arrow}" />
+                    <line x1="{firstCut["x"]}" y1="{firstCut["y"]}" x2="{lastCut["x"]}" y2="{lastCut["y"]}" style="stroke: none; stroke-opacity: 0;" />
+                    <line x1="{lastCut["x"]}" y1="{lastCut["y"]}" x2="{end["x"]}" y2="{end["y"]}" style="stroke: {color};"/>
+                </g>
+            '''
+        else:
+            if orb:
+                width_max = 5
+                width_min = 1
+                max_orb = 5
+                aspect_stroke_width = max(width_min, min(width_max, width_max - (abs(orb) / max_orb) * (width_max - width_min)))
+            else:
+                aspect_stroke_width = '1.5'
+            line = '<line x1="' + str(x1) + '" y1="' + str(y1) + '" x2="' + str(x2) + '" y2="' + str(
+                y2) + '" style="stroke: ' + color + f'; stroke-width: {aspect_stroke_width}; stroke-opacity: 1;" stroke-linecap="round" />'
+        # if label:
+        #     line += f'<text x="{x1-15}" y="{y1-15}" fill="{color}" text-anchor="center" dominant-baseline="central">{label}</text>'
+        return line
 
     def __sliceToX(self, slice, r, offset):
         plus = (math.pi * offset) / 180
         radial = ((math.pi/6) * slice) + plus
         return r * (math.cos(radial)+1)
 
     def __sliceToY(self, slice, r, offset):
@@ -424,67 +456,56 @@
         # symbols
         offset = offset + 15
         # check transit
         if self.chart_type == "Transit" or self.chart_type == "Composite":
             dropin = 54
         else:
             dropin = 18+self.c1
-        sign = '<g transform="translate(-16,-16)"><use x="' + str(dropin + self.__sliceToX(num, r-dropin, offset)) + '" y="' + str(
+        sign = '<g transform="translate(-13,-13)"><use x="' + str(dropin + self.__sliceToX(num, r-dropin, offset)) + '" y="' + str(
             dropin + self.__sliceToY(num, r-dropin, offset)) + '" xlink:href="#' + type + '" /></g>'
         return slice + '' + sign
 
     def __makeZodiac(self, r):
         output = ""
         for i in range(len(self.zodiac)):
             output = output + self.__zodiacSlice(i, r, "fill:" + self.colors_settings["zodiac_bg_%s" % (
-                i)] + "; fill-opacity: 0.5;", self.zodiac[i]) + ''
+                i)] + "; fill-opacity: 1; fill-opacity: 1; stroke:#FFFFFF; stroke-opacity: 1; stroke-width: 2;", self.zodiac[i]) + ''
         return output
 
     def __makeHouses(self, r):
         path = ""
 
         xr = 12
         for i in range(xr):
             # check transit
             if self.chart_type == "Transit" or self.chart_type == "Composite":
                 dropin = 160
                 roff = 72
                 t_roff = 36
             else:
                 dropin = self.c3
-                roff = self.c1
+                roff = self.c2
 
             # offset is negative desc houses_degree_ut[6]
-            offset = (
-                int(self.houses_degree_ut[int(xr/2)]) / -1) + int(self.houses_degree_ut[i])
+            offset = (int(self.houses_degree_ut[int(xr/2)]) / -1) + int(self.houses_degree_ut[i])
             x1 = self.__sliceToX(0, (r-dropin), offset) + dropin
             y1 = self.__sliceToY(0, (r-dropin), offset) + dropin
             x2 = self.__sliceToX(0, r-roff, offset) + roff
             y2 = self.__sliceToY(0, r-roff, offset) + roff
 
             if i < (xr-1):
                 text_offset = offset + \
                     int(self.__degreeDiff(self.houses_degree_ut[(
-                        i+1)], self.houses_degree_ut[i]) / 2)
+                        i+1)], self.houses_degree_ut[i]) / 6)
             else:
                 text_offset = offset + \
                     int(self.__degreeDiff(
-                        self.houses_degree_ut[0], self.houses_degree_ut[(xr-1)]) / 2)
+                        self.houses_degree_ut[0], self.houses_degree_ut[(xr-1)]) / 6)
 
-            # mc, asc, dsc, ic
-            if i == 0:
-                linecolor = self.planets_settings[12]['color']
-            elif i == 9:
-                linecolor = self.planets_settings[13]['color']
-            elif i == 6:
-                linecolor = self.planets_settings[14]['color']
-            elif i == 3:
-                linecolor = self.planets_settings[15]['color']
-            else:
-                linecolor = self.colors_settings['houses_radix_line']
+            linecolor = self.colors_settings['houses_radix_line']
 
             # Transit houses lines.
             if self.chart_type == "Transit" or self.chart_type == "Composite":
 
                 # Degrees for point zero.
 
                 zeropoint = 360 - self.houses_degree_ut[6]
@@ -527,23 +548,34 @@
 
             # if transit
             if self.chart_type == "Transit" or self.chart_type == "Composite":
                 dropin = 84
 
             dropin = 48
 
+            if i+1 == 1:
+                house_number = 'I'
+            elif i+1 == 4:
+                house_number = 'IV'
+            elif i+1 == 7:
+                house_number = 'VII'
+            elif i+1 == 10:
+                house_number = 'X'
+            else:
+                house_number = i+1
+
             xtext = self.__sliceToX(
                 0, (r-dropin), text_offset) + dropin  # was 132
             ytext = self.__sliceToY(
                 0, (r-dropin), text_offset) + dropin  # was 132
             path = path + '<line x1="'+str(x1)+'" y1="'+str(y1)+'" x2="'+str(x2)+'" y2="'+str(
-                y2)+'" style="stroke: '+linecolor+'; stroke-width: 2px; stroke-dasharray:3,2; stroke-opacity:.4;"/>'
-            path = path + '<text style="fill: #f00; fill-opacity: .6; font-size: 14px"><tspan x="' + \
-                str(xtext-3)+'" y="'+str(ytext+3) + \
-                '">'+str(i+1)+'</tspan></text>'
+                y2)+'" style="stroke: '+linecolor+'; stroke-width: 2px; stroke-opacity:.4;"/>'
+            path = path + '<text style="fill: #000000; fill-opacity: .4; font-size: 14px; font-weight: bold"><tspan x="' + \
+                str(xtext-10)+'" y="'+str(ytext+3) + \
+                '">'+str(house_number)+'</tspan></text>'
 
         return path
 
     def __makePlanets(self, r):
 
         planets_degut = {}
 
@@ -1036,15 +1068,15 @@
 
     # Aspect and aspect grid functions for natal type charts.
 
     def __makeAspects(self, r, ar):
         out = ""
         for element in self.aspects_list:
             out += self.__drawAspect(r, ar, element['p1_abs_pos'], element['p2_abs_pos'],
-                                   self.colors_settings[f"aspect_{element['aspect_degrees']}"])
+                                   self.colors_settings[f"aspect_{element['aspect_degrees']}"], element['orbit'])
 
         return out
 
     def __makeAspectGrid(self, r):
 
         out = ""
         style = 'stroke:%s; stroke-width: 1px; stroke-opacity:.6; fill:none' % (
@@ -1167,16 +1199,21 @@
         return out
 
     def __makeAxis(self, r, ar):
         out = ''
         for axis in self.user.axis_list:
             if axis.name in {'Ascendant', 'Midheaven'}:
                 axis_data = next((planet for planet in self.planets_settings if planet['name'] == axis.name), None)
+                arrow_top = f'''
+                    <marker id="arrowhead{axis_data['label_short']}" markerWidth="12" markerHeight="12" refX="6" refY="6" orient="auto-start-reverse">
+                        <polyline points="0,2 6,6 0,10" style="fill: none; stroke: {axis_data['color']};" />
+                    </marker>
+                '''
                 if axis_data:
-                    out += self.__drawAspect(r, ar, axis.abs_pos, (axis.abs_pos + 180) % 360, axis_data['color'], axis_data['label_short'])
+                    out += arrow_top + self.__drawAspect(r, ar, axis.abs_pos, (axis.abs_pos + 180) % 360, axis_data['color'], None, axis_data['label_short'], True)
         return out
 
     def __makePlanetGrid(self):
         out = '<g transform="translate(500,-20)">'
 
         # loop over all planets
         li = 10
@@ -1397,19 +1434,19 @@
             # circles
             td['c1'] = 'cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-36) + '"'
             td['c1style'] = 'fill: none; stroke: %s; stroke-width: 1px; stroke-opacity:.4;' % (
                 self.colors_settings['zodiac_transit_ring_2'])
             td['c2'] = 'cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-72) + '"'
-            td['c2style'] = 'fill: %s; fill-opacity:.4; stroke: %s; stroke-opacity:.4; stroke-width: 1px' % (
+            td['c2style'] = 'fill: %s; fill-opacity: 1; stroke: %s; stroke-opacity:.4; stroke-width: 1px' % (
                 self.colors_settings['paper_1'], self.colors_settings['zodiac_transit_ring_1'])
             td['c3'] = 'cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-160) + '"'
-            td['c3style'] = 'fill: %s; fill-opacity:.8; stroke: %s; stroke-width: 1px' % (
+            td['c3style'] = 'fill: %s; fill-opacity: 1; stroke: %s; stroke-width: 1px' % (
                 self.colors_settings['paper_1'], self.colors_settings['zodiac_transit_ring_0'])
             td['makeAspects'] = self.__makeAspectsTransit(r, (r-160))
             td['makeAspectGrid'] = self.__makeAspectTransitGrid(r)
             td['makePatterns'] = ''
             td['makeAxis'] = ''
             td['chart_width'] = self.full_width
         else:
@@ -1418,22 +1455,22 @@
             # circles
             td['c1'] = 'cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-self.c1) + '"'
             td['c1style'] = 'fill: none; stroke: %s; stroke-width: 1px; ' % (
                 self.colors_settings['zodiac_radix_ring_2'])
             td['c2'] = 'cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-self.c2) + '"'
-            td['c2style'] = 'fill: %s; fill-opacity:.2; stroke: %s; stroke-opacity:.4; stroke-width: 1px' % (
+            td['c2style'] = 'fill: %s; fill-opacity: 1; stroke: %s; stroke-opacity:.4; stroke-width: 1px' % (
                 self.colors_settings['paper_1'], self.colors_settings['zodiac_radix_ring_1'])
             td['c3'] = 'cx="' + str(r) + '" cy="' + \
                 str(r) + '" r="' + str(r-self.c3) + '"'
-            td['c3style'] = 'fill: %s; fill-opacity:.8; stroke: %s; stroke-width: 1px' % (
+            td['c3style'] = 'fill: %s; fill-opacity: 1; stroke: %s; stroke-width: 1px' % (
                 self.colors_settings['paper_1'], self.colors_settings['zodiac_radix_ring_0'])
             td['makeAspects'] = self.__makeAspects(r, (r-self.c3))
-            td['makeAxis'] = self.__makeAxis(r, (r-self.c2))
+            td['makeAxis'] = self.__makeAxis(r, (r-self.c1+20))
             td['makeAspectGrid'] = self.__makeAspectGrid(r)
             td['makePatterns'] = self.__makePatterns()
             td['chart_width'] = self.natal_width
 
         td['circleX'] = str(0)
         td['circleY'] = str(0)
         td['svgWidth'] = str(svgWidth)
```

### Comparing `py_astrolab-0.1.5/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.1.6/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.1.6/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/fetch_geonames.py` & `py_astrolab-0.1.6/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/kr.config.json` & `py_astrolab-0.1.6/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/main.py` & `py_astrolab-0.1.6/py_astrolab/main.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/print_all_data.py` & `py_astrolab-0.1.6/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/relationship_score.py` & `py_astrolab-0.1.6/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/report.py` & `py_astrolab-0.1.6/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/types.py` & `py_astrolab-0.1.6/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/py_astrolab/utilities.py` & `py_astrolab-0.1.6/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.1.5/pyproject.toml` & `py_astrolab-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.1.5/PKG-INFO` & `py_astrolab-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

