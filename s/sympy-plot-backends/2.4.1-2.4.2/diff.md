# Comparing `tmp/sympy_plot_backends-2.4.1.tar.gz` & `tmp/sympy_plot_backends-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sympy_plot_backends-2.4.1.tar", last modified: Sat Jul  1 11:54:55 2023, max compression
+gzip compressed data, was "sympy_plot_backends-2.4.2.tar", last modified: Sun Jul  9 14:14:03 2023, max compression
```

## Comparing `sympy_plot_backends-2.4.1.tar` & `sympy_plot_backends-2.4.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.786936 sympy_plot_backends-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-01 11:54:55.786936 sympy_plot_backends-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 11:54:55.786936 sympy_plot_backends-2.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.774936 sympy_plot_backends-2.4.1/spb/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.774936 sympy_plot_backends-2.4.1/spb/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25283 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/base_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.774936 sympy_plot_backends-2.4.1/spb/backends/bokeh/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/bokeh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.778936 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/vector2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.778936 sympy_plot_backends-2.4.1/spb/backends/k3d/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/k3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.778936 sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.778936 sympy_plot_backends-2.4.1/spb/backends/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.778936 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/implicit2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/nichols.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/nyquist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/vector2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.778936 sympy_plot_backends-2.4.1/spb/backends/mayavi/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/mayavi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/mayavi/mayavi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.782935 sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/vector3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.782935 sympy_plot_backends-2.4.1/spb/backends/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.782935 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/hvline.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/implicit3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/line2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/line3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/vector2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/vector3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/backends/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.782935 sympy_plot_backends-2.4.1/spb/ccomplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/ccomplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78700 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/ccomplex/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/ccomplex/wegert.py
--rw-r--r--   0 runner    (1001) docker     (123)    41127 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   179849 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.782935 sympy_plot_backends-2.4.1/spb/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/interactive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.782935 sympy_plot_backends-2.4.1/spb/interactive/bootstrap_spb/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/interactive/bootstrap_spb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/interactive/bootstrap_spb/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/interactive/bootstrap_spb/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/interactive/ipywidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    39194 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/interactive/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/plotgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)   142578 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/series.py
--rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31071 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/spb/vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.782935 sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-01 11:54:55.000000 sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-01 11:54:55.000000 sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 11:54:55.000000 sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 11:54:55.000000 sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-01 11:54:55.000000 sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 11:54:55.000000 sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.786936 sympy_plot_backends-2.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 11:54:55.786936 sympy_plot_backends-2.4.1/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/backends/make_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/backends/test_base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    37300 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/backends/test_bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)    25876 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/backends/test_k3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    62918 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/backends/test_matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    55450 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/backends/test_plotly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    72837 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)    34886 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    75888 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23636 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_plotgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)   117233 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46627 2023-07-01 11:54:46.000000 sympy_plot_backends-2.4.1/tests/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.649411 sympy_plot_backends-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-09 14:14:03.649411 sympy_plot_backends-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:14:03.649411 sympy_plot_backends-2.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25407 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/base_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/bokeh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/vector2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/k3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/k3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.637410 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/implicit2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/nichols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/nyquist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/mayavi/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/mayavi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/vector3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.641410 sympy_plot_backends-2.4.2/spb/backends/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19219 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/hvline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/implicit3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/line2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/line3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/vector2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/vector3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21845 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/backends/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/spb/ccomplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/ccomplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78700 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/ccomplex/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/ccomplex/wegert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41127 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179849 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/spb/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39194 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/interactive/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24361 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/plotgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   142578 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31071 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/spb/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 14:14:03.000000 sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.645411 sympy_plot_backends-2.4.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:14:03.649411 sympy_plot_backends-2.4.2/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/make_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37300 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25876 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_k3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62918 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55450 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/backends/test_plotly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72837 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34886 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75888 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23636 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_plotgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117233 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46627 2023-07-09 14:13:54.000000 sympy_plot_backends-2.4.2/tests/test_vectors.py
```

### Comparing `sympy_plot_backends-2.4.1/LICENSE` & `sympy_plot_backends-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/PKG-INFO` & `sympy_plot_backends-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy_plot_backends
-Version: 2.4.1
+Version: 2.4.2
 Summary: Backends for plotting with SymPy
 Home-page: https://github.com/Davide-sd/sympy-plot-backends
 Author: Davide Sandona
 Author-email: sandona.davide@gmail.com
 License: BSD License
 Keywords: sympy plot plotting backend plotly bokeh mayavi k3d panel
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sympy_plot_backends-2.4.1/README.md` & `sympy_plot_backends-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/setup.py` & `sympy_plot_backends-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/__init__.py` & `sympy_plot_backends-2.4.2/spb/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/base_backend.py` & `sympy_plot_backends-2.4.2/spb/backends/base_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -613,14 +613,16 @@
         if isinstance(arg, BaseSeries):
             self._series.append(arg)
             # auto legend
             if len(self._series) > 1:
                 self.legend = True
         else:
             raise TypeError("Must specify element of plot to append.")
+        # recreate renderers
+        self._create_renderers()
 
     def extend(self, arg):
         """Adds all series from another plot.
 
         Parameters
         ==========
 
@@ -660,7 +662,9 @@
         elif is_sequence(arg) and all([isinstance(a, BaseSeries) for a in arg]):
             self._series.extend(arg)
         else:
             raise TypeError("Expecting Plot or sequence of BaseSeries")
         # auto legend
         if len(self._series) > 1:
             self.legend = True
+        # recreate renderers
+        self._create_renderers()
```

### Comparing `sympy_plot_backends-2.4.1/spb/backends/base_renderer.py` & `sympy_plot_backends-2.4.2/spb/backends/base_renderer.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/bokeh/bokeh.py` & `sympy_plot_backends-2.4.2/spb/backends/bokeh/bokeh.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/complex.py` & `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/contour.py` & `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/contour.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/generic.py` & `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/geometry.py` & `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/hvline.py` & `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/line2d.py` & `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/bokeh/renderers/vector2d.py` & `sympy_plot_backends-2.4.2/spb/backends/bokeh/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/k3d/k3d.py` & `sympy_plot_backends-2.4.2/spb/backends/k3d/k3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/complex.py` & `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/implicit3d.py` & `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/line3d.py` & `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/surface.py` & `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/k3d/renderers/vector3d.py` & `sympy_plot_backends-2.4.2/spb/backends/k3d/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/matplotlib.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/matplotlib.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/__init__.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/complex.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/contour.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/contour.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/generic.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/geometry.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/hvline.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/implicit2d.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/implicit2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/line2d.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/line3d.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/nichols.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/nichols.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/nyquist.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/nyquist.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/renderer.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/surface.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/vector2d.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/matplotlib/renderers/vector3d.py` & `sympy_plot_backends-2.4.2/spb/backends/matplotlib/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/mayavi/mayavi.py` & `sympy_plot_backends-2.4.2/spb/backends/mayavi/mayavi.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/implicit3d.py` & `sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/line3d.py` & `sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/surface.py` & `sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/mayavi/renderers/vector3d.py` & `sympy_plot_backends-2.4.2/spb/backends/mayavi/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/plotly.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/plotly.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/__init__.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/complex.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/contour.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/contour.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/generic.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/generic.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/geometry.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/geometry.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/hvline.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/hvline.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/implicit3d.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/implicit3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/line2d.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/line2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/line3d.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/line3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/surface.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/surface.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/vector2d.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/vector2d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/plotly/renderers/vector3d.py` & `sympy_plot_backends-2.4.2/spb/backends/plotly/renderers/vector3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/backends/utils.py` & `sympy_plot_backends-2.4.2/spb/backends/utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/ccomplex/complex.py` & `sympy_plot_backends-2.4.2/spb/ccomplex/complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/ccomplex/wegert.py` & `sympy_plot_backends-2.4.2/spb/ccomplex/wegert.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/control.py` & `sympy_plot_backends-2.4.2/spb/control.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/defaults.py` & `sympy_plot_backends-2.4.2/spb/defaults.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/doc_utils.py` & `sympy_plot_backends-2.4.2/spb/doc_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/functions.py` & `sympy_plot_backends-2.4.2/spb/functions.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/interactive/__init__.py` & `sympy_plot_backends-2.4.2/spb/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/interactive/bootstrap_spb/__init__.py` & `sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/interactive/bootstrap_spb/bootstrap.css` & `sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/bootstrap.css`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/interactive/bootstrap_spb/bootstrap.html` & `sympy_plot_backends-2.4.2/spb/interactive/bootstrap_spb/bootstrap.html`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/interactive/ipywidgets.py` & `sympy_plot_backends-2.4.2/spb/interactive/ipywidgets.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/interactive/panel.py` & `sympy_plot_backends-2.4.2/spb/interactive/panel.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/plotgrid.py` & `sympy_plot_backends-2.4.2/spb/plotgrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/series.py` & `sympy_plot_backends-2.4.2/spb/series.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/utils.py` & `sympy_plot_backends-2.4.2/spb/utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/spb/vectors.py` & `sympy_plot_backends-2.4.2/spb/vectors.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/PKG-INFO` & `sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympy-plot-backends
-Version: 2.4.1
+Version: 2.4.2
 Summary: Backends for plotting with SymPy
 Home-page: https://github.com/Davide-sd/sympy-plot-backends
 Author: Davide Sandona
 Author-email: sandona.davide@gmail.com
 License: BSD License
 Keywords: sympy plot plotting backend plotly bokeh mayavi k3d panel
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sympy_plot_backends-2.4.1/sympy_plot_backends.egg-info/SOURCES.txt` & `sympy_plot_backends-2.4.2/sympy_plot_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/backends/__init__.py` & `sympy_plot_backends-2.4.2/tests/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/backends/make_tests.py` & `sympy_plot_backends-2.4.2/tests/backends/make_tests.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/backends/test_base_backend.py` & `sympy_plot_backends-2.4.2/tests/backends/test_base_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from spb.backends.base_backend import Plot
-from spb.series import BaseSeries
+from spb.series import BaseSeries, HVLineSeries
 from pytest import raises
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import plotly.graph_objects as go
 import k3d
 import bokeh
@@ -174,7 +174,31 @@
             b: (0, 0, 2 * pi), # phase
             c: (0.25, 0, 1),   # damping
             n: (2, 0, 4)       # multiple of pi
         },
         ylim=(-1.25, 1.25), backend=MB, use_latex=False, show=False, n=10
     )
     p.backend.draw()
+
+
+def test_number_of_renderers():
+    # verify that once `extend` or `append` is executed, the number of
+    # renderers will be equal to the new number of series
+
+    x = symbols("x")
+    hor = HVLineSeries(0, True, show_in_legend=False)
+    ver1 = HVLineSeries(0, False, show_in_legend=False)
+    ver2 = HVLineSeries(1, False, show_in_legend=False)
+
+    def do_test(B):
+        p = plot(sin(x), (x, -5, 5), backend=B, show=False, n=5)
+        assert len(p.series) == len(p.renderers) == 1
+
+        p.extend([hor, ver1])
+        assert len(p.series) == len(p.renderers) == 3
+
+        p.append(ver2)
+        assert len(p.series) == len(p.renderers) == 4
+    
+    do_test(MB)
+    do_test(PB)
+    do_test(BB)
```

### Comparing `sympy_plot_backends-2.4.1/tests/backends/test_bokeh.py` & `sympy_plot_backends-2.4.2/tests/backends/test_bokeh.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/backends/test_k3d.py` & `sympy_plot_backends-2.4.2/tests/backends/test_k3d.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/backends/test_matplotlib.py` & `sympy_plot_backends-2.4.2/tests/backends/test_matplotlib.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/backends/test_plotly.py` & `sympy_plot_backends-2.4.2/tests/backends/test_plotly.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_color_utils.py` & `sympy_plot_backends-2.4.2/tests/test_color_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_complex.py` & `sympy_plot_backends-2.4.2/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_control.py` & `sympy_plot_backends-2.4.2/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_defaults.py` & `sympy_plot_backends-2.4.2/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_doc_utils.py` & `sympy_plot_backends-2.4.2/tests/test_doc_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_functions.py` & `sympy_plot_backends-2.4.2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_plotgrid.py` & `sympy_plot_backends-2.4.2/tests/test_plotgrid.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_series.py` & `sympy_plot_backends-2.4.2/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_utils.py` & `sympy_plot_backends-2.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sympy_plot_backends-2.4.1/tests/test_vectors.py` & `sympy_plot_backends-2.4.2/tests/test_vectors.py`

 * *Files identical despite different names*

