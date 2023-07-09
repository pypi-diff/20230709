# Comparing `tmp/mplfooty-0.0.3.tar.gz` & `tmp/mplfooty-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mplfooty-0.0.3.tar", last modified: Mon Jun 26 23:17:19 2023, max compression
+gzip compressed data, was "mplfooty-0.1.0.tar", last modified: Sun Jul  9 10:58:22 2023, max compression
```

## Comparing `mplfooty-0.0.3.tar` & `mplfooty-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-26 23:17:19.133016 mplfooty-0.0.3/
--rw-r--r--   0 ciaran     (501) staff       (20)     1069 2023-06-20 07:00:35.000000 mplfooty-0.0.3/LICENSE
--rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-06-26 23:17:19.132834 mplfooty-0.0.3/PKG-INFO
--rw-r--r--   0 ciaran     (501) staff       (20)     3228 2023-06-21 07:32:42.000000 mplfooty-0.0.3/README.md
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-26 23:17:19.131240 mplfooty-0.0.3/mplfooty/
--rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-06-20 06:57:42.000000 mplfooty-0.0.3/mplfooty/__init__.py
--rw-r--r--   0 ciaran     (501) staff       (20)     4710 2023-06-26 23:09:13.000000 mplfooty-0.0.3/mplfooty/dimensions.py
--rw-r--r--   0 ciaran     (501) staff       (20)     2762 2023-06-20 06:57:42.000000 mplfooty-0.0.3/mplfooty/pitch.py
--rw-r--r--   0 ciaran     (501) staff       (20)    35636 2023-06-20 06:57:42.000000 mplfooty-0.0.3/mplfooty/pitch_base.py
--rw-r--r--   0 ciaran     (501) staff       (20)    43682 2023-06-20 06:57:42.000000 mplfooty-0.0.3/mplfooty/pitch_plot.py
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-06-26 23:17:19.132524 mplfooty-0.0.3/mplfooty.egg-info/
--rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/PKG-INFO
--rw-r--r--   0 ciaran     (501) staff       (20)      299 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/SOURCES.txt
--rw-r--r--   0 ciaran     (501) staff       (20)        1 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/dependency_links.txt
--rw-r--r--   0 ciaran     (501) staff       (20)      206 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/requires.txt
--rw-r--r--   0 ciaran     (501) staff       (20)        9 2023-06-26 23:17:19.000000 mplfooty-0.0.3/mplfooty.egg-info/top_level.txt
--rw-r--r--   0 ciaran     (501) staff       (20)      774 2023-06-26 23:16:52.000000 mplfooty-0.0.3/pyproject.toml
--rw-r--r--   0 ciaran     (501) staff       (20)       38 2023-06-26 23:17:19.133090 mplfooty-0.0.3/setup.cfg
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-07-09 10:58:22.163712 mplfooty-0.1.0/
+-rw-r--r--   0 ciaran     (501) staff       (20)     1069 2023-06-20 07:00:35.000000 mplfooty-0.1.0/LICENSE
+-rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-07-09 10:58:22.163525 mplfooty-0.1.0/PKG-INFO
+-rw-r--r--   0 ciaran     (501) staff       (20)     3228 2023-06-21 07:32:42.000000 mplfooty-0.1.0/README.md
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-07-09 10:58:22.162172 mplfooty-0.1.0/mplfooty/
+-rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-06-20 06:57:42.000000 mplfooty-0.1.0/mplfooty/__init__.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     4710 2023-06-26 23:09:13.000000 mplfooty-0.1.0/mplfooty/dimensions.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     5756 2023-07-09 10:56:53.000000 mplfooty-0.1.0/mplfooty/pitch.py
+-rw-r--r--   0 ciaran     (501) staff       (20)    36044 2023-07-09 10:56:53.000000 mplfooty-0.1.0/mplfooty/pitch_base.py
+-rw-r--r--   0 ciaran     (501) staff       (20)    46235 2023-07-09 10:56:53.000000 mplfooty-0.1.0/mplfooty/pitch_plot.py
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-07-09 10:58:22.163297 mplfooty-0.1.0/mplfooty.egg-info/
+-rw-r--r--   0 ciaran     (501) staff       (20)     4799 2023-07-09 10:58:22.000000 mplfooty-0.1.0/mplfooty.egg-info/PKG-INFO
+-rw-r--r--   0 ciaran     (501) staff       (20)      299 2023-07-09 10:58:22.000000 mplfooty-0.1.0/mplfooty.egg-info/SOURCES.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)        1 2023-07-09 10:58:22.000000 mplfooty-0.1.0/mplfooty.egg-info/dependency_links.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)      206 2023-07-09 10:58:22.000000 mplfooty-0.1.0/mplfooty.egg-info/requires.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)        9 2023-07-09 10:58:22.000000 mplfooty-0.1.0/mplfooty.egg-info/top_level.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)      774 2023-07-09 10:57:42.000000 mplfooty-0.1.0/pyproject.toml
+-rw-r--r--   0 ciaran     (501) staff       (20)       38 2023-07-09 10:58:22.163754 mplfooty-0.1.0/setup.cfg
```

### Comparing `mplfooty-0.0.3/LICENSE` & `mplfooty-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.3/PKG-INFO` & `mplfooty-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplfooty
-Version: 0.0.3
+Version: 0.1.0
 Summary: AFL pitch plotting using matplotlib
 Author-email: Ciaran Grant <ciaran.grant@hotmail.co.uk>
 License: MIT License
         
         Copyright (c) 2023 ciaran-grant
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mplfooty-0.0.3/README.md` & `mplfooty-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.3/mplfooty/dimensions.py` & `mplfooty-0.1.0/mplfooty/dimensions.py`

 * *Files identical despite different names*

### Comparing `mplfooty-0.0.3/mplfooty/pitch_base.py` & `mplfooty-0.1.0/mplfooty/pitch_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 class BasePitch(ABC):
     """ A class for plotting AFL pitches in Matplotlib
 
     Parameters
     ----------
     half : bool, default False
         Whether to display half of the pitch.
-    pitch_color : any Matplotlib color, default None
-        The background color for each Matplotlib axis.
+    pitch_colour : any Matplotlib colour, default None
+        The background colour for each Matplotlib axis.
          If None, defaults to rcParams["axes.facecolor"].
         To remove the background set to "None" or 'None'.
-    line_color : any Matplotlib color, default None
-        The line color for the pitch markings. If None, defaults to rcParams["grid.color"].
+    line_colour : any Matplotlib colour, default None
+        The line colour for the pitch markings. If None, defaults to rcParams["grid.color"].
     line_alpha : float, default 1
         The transparency of the pitch and the markings.
     linewidth : float, default 2
         The line width for the pitch markings.
     linestyle : str or typle
         Linestyle for the pitch lines:
         {'-', '--', '-.', ':', '', (offset, on-off-seq), ...}
@@ -243,42 +243,52 @@
         ax.grid(grid)
         ax.tick_params(bottom=tick, top=tick, left=tick, right=tick,
                        labelbottom=label, labeltop=label, labelleft=label, labelright=label)
     
     def _draw_ax(self, ax):
         """ Defines the axes and draw AFL pitch markings & goals. """
         self._set_axes(ax)
+        self._set_background(ax)
         self._draw_pitch_markings(ax)
         self._draw_goals(ax)
         
     def _set_axes(self, ax):
         # Set axis on/off, labels, grid, ticks
         self.set_visible(ax, spine_bottom=self.axis, spine_top=self.axis, spine_left=self.axis, spine_right=self.axis,
                          grid=False, tick=self.tick, label=self.label)
         
         # Set limits and aspect
         ax.set_xlim(self.extent[0], self.extent[1])
         ax.set_ylim(self.extent[2], self.extent[3])
         ax.set_aspect(self.dim.aspect)
+        
+    def _set_background(self, ax):
+        ax.set_facecolor(self.pitch_colour)
                
     def _draw_pitch_markings(self, ax):
         """ Draw all lines on the pitch. """
         self._draw_boundary(ax)
         self._draw_centre(ax)
         self._draw_inside_50(ax)
         
     def _draw_boundary(self, ax):
         # Top Pitch Boundary
+        top_theta_start = 0
+        if self.vertical:
+            top_theta_start = 180
+        top_theta_end = top_theta_start + 180
         self._draw_arc(ax, x=0, y=self.dim.behind_top, 
                        width=self.pitch_length, height = self.dim.boundary_width,
-                       theta1=0, theta2=180, **self.arc_properties)
+                       theta1=top_theta_start, theta2=top_theta_end, **self.arc_properties)
         # Bottom Pitch Boundary
+        bottom_theta_start = top_theta_end
+        bottom_theta_end = bottom_theta_start + 180
         self._draw_arc(ax, x=0, y=self.dim.behind_bottom, 
                        width=self.pitch_length, height = self.dim.boundary_width,
-                       theta1=180, theta2=360, **self.arc_properties)
+                       theta1=bottom_theta_start, theta2=bottom_theta_end, **self.arc_properties)
         
     def _draw_inside_50(self, ax):
         # Left Inside 50
         self._draw_arc(ax, 
                        x=self.dim.left, y=0, 
                        width=self.dim.inside_50_radius*2, height = self.dim.inside_50_radius*2,
                        theta1=360-self.dim.inside_50_angle, theta2=self.dim.inside_50_angle, **self.arc_properties)
```

### Comparing `mplfooty-0.0.3/mplfooty/pitch_plot.py` & `mplfooty-0.1.0/mplfooty/pitch_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,27 +131,39 @@
             raise ValueError("x and y must be the same size.")
         
         x, y = self._reverse_if_vertical(x, y)
                         
         kde = sns.kdeplot(x=x, y=y, ax=ax, **kwargs)
         
         # Clip to pitch boundary
-        top_boundary_arc = Arc((0, self.dim.behind_top), 
+        top_theta_start = 0
+        top_boundary_y = self.dim.behind_top
+        bottom_boundary_y = self.dim.behind_bottom
+        if self.vertical:
+            top_theta_start = 180
+            top_boundary_y = self.dim.behind_bottom
+            bottom_boundary_y = self.dim.behind_top
+        top_theta_end = top_theta_start + 180
+        top_boundary_arc = Arc((0, top_boundary_y), 
                                         width = self.dim.pitch_length, 
                                         height = self.dim.boundary_width, 
-                                        theta1=0, theta2=180
+                                        theta1=top_theta_start, theta2=top_theta_end
                                         )
+        top_vertices = self._reverse_vertices_if_vertical(top_boundary_arc.get_verts()[:-1])
 
-        bottom_boundary_arc = Arc((0, self.dim.behind_bottom), 
+        bottom_theta_start = top_theta_end
+        bottom_theta_end = bottom_theta_start + 180
+        bottom_boundary_arc = Arc((0, bottom_boundary_y), 
                                     width = self.dim.pitch_length, 
                                     height = self.dim.boundary_width, 
-                                    theta1=180, theta2=360
+                                    theta1=bottom_theta_start, theta2=bottom_theta_end
                                     )
+        bottom_vertices = self._reverse_vertices_if_vertical(bottom_boundary_arc.get_verts()[:-1])
 
-        pitch_boundary_vertices = np.concatenate([top_boundary_arc.get_verts()[:-1], bottom_boundary_arc.get_verts()[:-1]])
+        pitch_boundary_vertices = np.concatenate([top_vertices, bottom_vertices])
 
         A = Polygon(pitch_boundary_vertices, color= "w", zorder=-1)
         ax.add_patch(A)
         for col in ax.collections:
             col.set_clip_path(A)
                 
         return kde
@@ -208,27 +220,39 @@
         mincnt = kwargs.pop('mincnt', 1)
         gridsize = kwargs.pop('gridsize', self.hexbin_gridsize)
         extent = kwargs.pop('extent', self.hex_extent)
         
         hexbin = ax.hexbin(x, y, mincnt = mincnt, gridsize=gridsize, extent=extent, **kwargs)
 
         # Clip to pitch boundary
-        top_boundary_arc = Arc((0, self.dim.behind_top), 
+        top_theta_start = 0
+        top_boundary_y = self.dim.behind_top
+        bottom_boundary_y = self.dim.behind_bottom
+        if self.vertical:
+            top_theta_start = 180
+            top_boundary_y = self.dim.behind_bottom
+            bottom_boundary_y = self.dim.behind_top
+        top_theta_end = top_theta_start + 180
+        top_boundary_arc = Arc((0, top_boundary_y), 
                                         width = self.dim.pitch_length, 
                                         height = self.dim.boundary_width, 
-                                        theta1=0, theta2=180
+                                        theta1=top_theta_start, theta2=top_theta_end
                                         )
+        top_vertices = self._reverse_vertices_if_vertical(top_boundary_arc.get_verts()[:-1])
 
-        bottom_boundary_arc = Arc((0, self.dim.behind_bottom), 
+        bottom_theta_start = top_theta_end
+        bottom_theta_end = bottom_theta_start + 180
+        bottom_boundary_arc = Arc((0, bottom_boundary_y), 
                                     width = self.dim.pitch_length, 
                                     height = self.dim.boundary_width, 
-                                    theta1=180, theta2=360
+                                    theta1=bottom_theta_start, theta2=bottom_theta_end
                                     )
+        bottom_vertices = self._reverse_vertices_if_vertical(bottom_boundary_arc.get_verts()[:-1])
 
-        pitch_boundary_vertices = np.concatenate([top_boundary_arc.get_verts()[:-1], bottom_boundary_arc.get_verts()[:-1]])
+        pitch_boundary_vertices = np.concatenate([top_vertices, bottom_vertices])
 
         A = Polygon(pitch_boundary_vertices, color= "w", zorder=-1)
         ax.add_patch(A)
         for col in ax.collections:
             col.set_clip_path(A)
 
         return hexbin        
@@ -267,29 +291,41 @@
         for vert in verts:
             vert = np.asarray(vert)
             vert = self._reverse_vertices_if_vertical(vert)
             polygon = Polygon(vert, closed=True, **kwargs)
             patch_list.append(polygon)
             ax.add_patch(polygon)
             
-        # Clip to pitch boundary 
-        top_boundary_arc = Arc((0, self.dim.behind_top), 
-                                width = self.dim.pitch_length, 
-                                height = self.dim.boundary_width, 
-                                theta1=0, theta2=180
-                                )
+        # Clip to pitch boundary
+        top_theta_start = 0
+        top_boundary_y = self.dim.behind_top
+        bottom_boundary_y = self.dim.behind_bottom
+        if self.vertical:
+            top_theta_start = 180
+            top_boundary_y = self.dim.behind_bottom
+            bottom_boundary_y = self.dim.behind_top
+        top_theta_end = top_theta_start + 180
+        top_boundary_arc = Arc((0, top_boundary_y), 
+                                        width = self.dim.pitch_length, 
+                                        height = self.dim.boundary_width, 
+                                        theta1=top_theta_start, theta2=top_theta_end
+                                        )
+        top_vertices = self._reverse_vertices_if_vertical(top_boundary_arc.get_verts()[:-1])
 
-        bottom_boundary_arc = Arc((0, self.dim.behind_bottom), 
+        bottom_theta_start = top_theta_end
+        bottom_theta_end = bottom_theta_start + 180
+        bottom_boundary_arc = Arc((0, bottom_boundary_y), 
                                     width = self.dim.pitch_length, 
                                     height = self.dim.boundary_width, 
-                                    theta1=180, theta2=360
+                                    theta1=bottom_theta_start, theta2=bottom_theta_end
                                     )
+        bottom_vertices = self._reverse_vertices_if_vertical(bottom_boundary_arc.get_verts()[:-1])
 
-        pitch_boundary_vertices = np.concatenate([top_boundary_arc.get_verts()[:-1], bottom_boundary_arc.get_verts()[:-1]])
-
+        pitch_boundary_vertices = np.concatenate([top_vertices, bottom_vertices])
+        
         A = Polygon(pitch_boundary_vertices, color= "w", zorder=-1)
         ax.add_patch(A)
         for patch in patch_list:
             patch.set_clip_path(A)    
              
         return patch_list
         
@@ -335,14 +371,15 @@
             raise ValueError("x and y must be the same size.")
         
         goal_coordinates = self.goal_right if goal == 'right' else self.goal_left
         verts = np.zeros((x.size, 3, 2))
         verts[:, 0, 0] = x
         verts[:, 0, 1] = y
         verts[:, 1:, :] = np.expand_dims(goal_coordinates, 0)
+                
         return self.polygon(verts, ax=ax, **kwargs)
 
     def annotate(self, text, xy, xytext=None, ax=None, **kwargs):
         """ Utility wrapper around ax.annotate
         which automatically flips the xy and xytext coordinates if the pitch is vertical.
         Annotate the point xy with text.
         See: https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.annotate.html
@@ -493,15 +530,15 @@
         mask_y_out = np.logical_or(binnumber[1, :] == 0,
                                    binnumber[1, :] == num_y + 1)
         binnumber[1, mask_y_out] = -1
         binnumber[1, ~mask_y_out] = binnumber[1, ~mask_y_out] - 1
         inside = np.logical_and(~mask_x_out, ~mask_y_out)
         return _BinnedStatisticResult(statistic, x_grid, y_grid, cx, cy, binnumber, inside)._asdict()
         
-    def heatmap(self, stats, ax=None, vertical=False, **kwargs):
+    def heatmap(self, stats, ax=None, **kwargs):
         """ Utility wrapper around matplotlib.axes.Axes.pcolormesh
         which automatically flips the x_grid and y_grid coordinates if the pitch is vertical.
 
         See: https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.pcolormesh.html
 
         Parameters
         ----------
@@ -529,32 +566,44 @@
         >>> y= np.random.uniform(low=-135/2, high=135/2, size=1000)
         >>> stats = pitch.bin_statistic(x, y, bins=(10, 8))
         >>> pitch.heatmap(stats, edgecolors="black", cmap="hot", ax=ax)
         """
         
         self.validate_ax(ax)
         
-        if vertical:
-            heatmap = ax.pcolormesh(stats['y_grid'], stats['x_grid'], stats['statistic'], **kwargs)
-        
         heatmap = ax.pcolormesh(stats['x_grid'], stats['y_grid'], stats['statistic'], **kwargs)
+        if self.vertical:
+            heatmap = ax.pcolormesh(stats['y_grid'], stats['x_grid'], stats['statistic'], **kwargs)
         
-        top_boundary_arc = Arc((0, self.dim.behind_top), 
+        # Clip to pitch boundary
+        top_theta_start = 0
+        top_boundary_y = self.dim.behind_top
+        bottom_boundary_y = self.dim.behind_bottom
+        if self.vertical:
+            top_theta_start = 180
+            top_boundary_y = self.dim.behind_bottom
+            bottom_boundary_y = self.dim.behind_top
+        top_theta_end = top_theta_start + 180
+        top_boundary_arc = Arc((0, top_boundary_y), 
                                         width = self.dim.pitch_length, 
                                         height = self.dim.boundary_width, 
-                                        theta1=0, theta2=180
+                                        theta1=top_theta_start, theta2=top_theta_end
                                         )
+        top_vertices = self._reverse_vertices_if_vertical(top_boundary_arc.get_verts()[:-1])
 
-        bottom_boundary_arc = Arc((0, self.dim.behind_bottom), 
+        bottom_theta_start = top_theta_end
+        bottom_theta_end = bottom_theta_start + 180
+        bottom_boundary_arc = Arc((0, bottom_boundary_y), 
                                     width = self.dim.pitch_length, 
                                     height = self.dim.boundary_width, 
-                                    theta1=180, theta2=360
+                                    theta1=bottom_theta_start, theta2=bottom_theta_end
                                     )
+        bottom_vertices = self._reverse_vertices_if_vertical(bottom_boundary_arc.get_verts()[:-1])
 
-        pitch_boundary_vertices = np.concatenate([top_boundary_arc.get_verts()[:-1], bottom_boundary_arc.get_verts()[:-1]])
+        pitch_boundary_vertices = np.concatenate([top_vertices, bottom_vertices])
 
         A = Polygon(pitch_boundary_vertices, color= "w", zorder=-1)
         ax.add_patch(A)
         for col in ax.collections:
             col.set_clip_path(A)
         
         return heatmap
```

### Comparing `mplfooty-0.0.3/mplfooty.egg-info/PKG-INFO` & `mplfooty-0.1.0/mplfooty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplfooty
-Version: 0.0.3
+Version: 0.1.0
 Summary: AFL pitch plotting using matplotlib
 Author-email: Ciaran Grant <ciaran.grant@hotmail.co.uk>
 License: MIT License
         
         Copyright (c) 2023 ciaran-grant
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mplfooty-0.0.3/pyproject.toml` & `mplfooty-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mplfooty"
-version = "0.0.3"
+version = "0.1.0"
 description = "AFL pitch plotting using matplotlib"
 readme = "README.md"
 authors = [{name = "Ciaran Grant", email = "ciaran.grant@hotmail.co.uk"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 dependencies = [
     "pandas == 1.5.3",
```

