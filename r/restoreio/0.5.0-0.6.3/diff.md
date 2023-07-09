# Comparing `tmp/restoreio-0.5.0.tar.gz` & `tmp/restoreio-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restoreio-0.5.0.tar", last modified: Sat Jul  1 20:06:58 2023, max compression
+gzip compressed data, was "restoreio-0.6.3.tar", last modified: Sun Jul  9 08:07:47 2023, max compression
```

## Comparing `restoreio-0.5.0.tar` & `restoreio-0.6.3.tar`

### file list

```diff
@@ -1,191 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-01 20:06:40.000000 restoreio-0.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 20:06:40.000000 restoreio-0.5.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-01 20:06:40.000000 restoreio-0.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-01 20:06:40.000000 restoreio-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-01 20:06:40.000000 restoreio-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-01 20:06:58.984282 restoreio-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-01 20:06:40.000000 restoreio-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/source/_static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.972282 restoreio-0.5.0/docs/source/_static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/assets/fonts/synconew.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/assets/fonts/syncopate.bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/assets/fonts/syncopate.regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.972282 restoreio-0.5.0/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/css/custom-anaconda-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/css/custom-pydata.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/docs/source/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.972282 restoreio-0.5.0/docs/source/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.png
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.png
--rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-light.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/_static/images/plots/
--rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/cor_cov.png
--rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/deviation.png
--rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/ensembles.png
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/ensembles_js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/gdop_coverage.png
--rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/kl_eigenvalues.png
--rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/kl_eigenvectors.png
--rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/orig_vel_and_error.png
--rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/images/plots/rbf_kernel_2d.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_static/js/custom-pydata.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/ndarray_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/autosummary/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/_templates/version.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/cite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/cli_restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/cli_scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/generated/restoreio.restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/generated/restoreio.scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.976282 restoreio-0.5.0/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/notebooks/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-01 20:06:40.000000 restoreio-0.5.0/docs/source/recursive_glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 20:06:40.000000 restoreio-0.5.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.968282 restoreio-0.5.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/examples/restore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/main_VaryingNumModes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/plot_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/plot_fixed_size_artificial_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/plot_variable_d_artificial_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21771 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/restore/plot_variable_size_artificial_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/examples/uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/_plot_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/plot_gdop_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/plot_js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-01 20:06:40.000000 restoreio-0.5.0/examples/uncertainty_quant/restoreio_mwe.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-01 20:06:40.000000 restoreio-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-01 20:06:40.000000 restoreio-0.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24450 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_file_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_file_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_file_utilities/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_geography/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/_find_alpha_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/create_mask_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/detect_land_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_geography/locate_missing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_inpaint/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/_cast_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/_plot_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_inpaint/inpaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/get_datetime_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/load_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_input_output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_parser/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_parser/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_parser/parse_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio/_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/_plot_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots/plot_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_plots_uq/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/_refine_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/_shifted_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_cor_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_ensembles_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_kl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_restore/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/_make_array_masked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/refine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/restore_generated_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_restore/restore_main_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_scripts/examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44360 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_scripts/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_server_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_server_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_server_utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_server_utils/terminate_with_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_subset/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_subset/_array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_subset/subset_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_subset/subset_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/restoreio/_uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/_statistical_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/generate_image_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-07-01 20:06:40.000000 restoreio-0.5.0/restoreio/_uncertainty_quant/get_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.980282 restoreio-0.5.0/restoreio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 20:06:58.000000 restoreio-0.5.0/restoreio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-01 20:06:58.984282 restoreio-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-01 20:06:40.000000 restoreio-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:06:58.984282 restoreio-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-01 20:06:40.000000 restoreio-0.5.0/tests/test_restore_local_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-01 20:06:40.000000 restoreio-0.5.0/tests/test_restore_remote_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-01 20:06:40.000000 restoreio-0.5.0/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-01 20:06:40.000000 restoreio-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-09 08:07:34.000000 restoreio-0.6.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-09 08:07:34.000000 restoreio-0.6.3/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-09 08:07:34.000000 restoreio-0.6.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-09 08:07:34.000000 restoreio-0.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 08:07:34.000000 restoreio-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-09 08:07:47.080313 restoreio-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-09 08:07:34.000000 restoreio-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/docs/source/_static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/source/_static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/assets/fonts/synconew.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/assets/fonts/syncopate.bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/assets/fonts/syncopate.regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/css/custom-anaconda-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/css/custom-pydata.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/docs/source/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.064313 restoreio-0.6.3/docs/source/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23221 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/_static/images/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/cor_cov.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/deviation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/ensembles_js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/gdop_coverage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/kl_eigenvalues.png
+-rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/kl_eigenvectors.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/orig_vel_and_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/images/plots/rbf_kernel_2d.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_static/js/custom-pydata.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/ndarray_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/autosummary/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/_templates/version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/cli_restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/cli_scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/generated/restoreio.restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/generated/restoreio.scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/notebooks/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-09 08:07:34.000000 restoreio-0.6.3/docs/source/recursive_glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-09 08:07:34.000000 restoreio-0.6.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/restore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/main_VaryingNumModes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/plot_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/plot_fixed_size_artificial_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/plot_variable_d_artificial_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21771 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/restore/plot_variable_size_artificial_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.060313 restoreio-0.6.3/examples/uncertainty_quant/_utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/_utils/_load_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_load_variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_load_variables/_get_datetime_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_plot_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/terminate_with_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.072313 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/_utils/_subset/subset_domain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17491 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/plot_gdop_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/plot_js_divergence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-07-09 08:07:34.000000 restoreio-0.6.3/examples/uncertainty_quant/restoreio_mwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-09 08:07:34.000000 restoreio-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-09 08:07:34.000000 restoreio-0.6.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25367 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_file_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_file_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_file_utilities/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_geography/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/_find_alpha_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/create_mask_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/detect_land_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_geography/locate_missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_inpaint/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/_cast_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/_plot_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_inpaint/inpaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/get_datetime_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/load_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_input_output/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_parser/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_parser/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_parser/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio/_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/_plot_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots/plot_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_plots_uq/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/_refine_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/_shifted_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_cor_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_ensembles_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_kl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_restore/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/_make_array_masked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/refine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/restore_generated_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_restore/restore_main_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_scripts/examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45708 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_scripts/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_server_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_server_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_server_utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_server_utils/terminate_with_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_subset/subset_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/restoreio/_uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/_statistical_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/generate_image_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-07-09 08:07:34.000000 restoreio-0.6.3/restoreio/_uncertainty_quant/get_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.076313 restoreio-0.6.3/restoreio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-09 08:07:47.000000 restoreio-0.6.3/restoreio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 08:07:46.000000 restoreio-0.6.3/restoreio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-09 08:07:47.080313 restoreio-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-09 08:07:34.000000 restoreio-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 08:07:47.080313 restoreio-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-09 08:07:34.000000 restoreio-0.6.3/tests/test_restore_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-09 08:07:34.000000 restoreio-0.6.3/tests/test_restore_remote_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-09 08:07:34.000000 restoreio-0.6.3/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-09 08:07:34.000000 restoreio-0.6.3/tox.ini
```

### Comparing `restoreio-0.5.0/LICENSE.txt` & `restoreio-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/MANIFEST.in` & `restoreio-0.6.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/PKG-INFO` & `restoreio-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.5.0
+Version: 0.6.3
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.5.0/README.rst` & `restoreio-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/Makefile` & `restoreio-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/make.bat` & `restoreio-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_inspect.py` & `restoreio-0.6.3/docs/source/_inspect.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/assets/fonts/synconew.regular.ttf` & `restoreio-0.6.3/docs/source/_static/assets/fonts/synconew.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/assets/fonts/syncopate.bold.ttf` & `restoreio-0.6.3/docs/source/_static/assets/fonts/syncopate.bold.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/assets/fonts/syncopate.regular.ttf` & `restoreio-0.6.3/docs/source/_static/assets/fonts/syncopate.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/css/custom-anaconda-doc.css` & `restoreio-0.6.3/docs/source/_static/css/custom-anaconda-doc.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/css/custom-pydata.css` & `restoreio-0.6.3/docs/source/_static/css/custom-pydata.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/css/custom.css` & `restoreio-0.6.3/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/favicon.ico` & `restoreio-0.6.3/docs/source/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.ico` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.png` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-anaconda.svg` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-anaconda.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.ico` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.png` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-pypi.svg` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-dark.png` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-dark.svg` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-light.png` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-restoreio-light.svg` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-restoreio-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-dark.png` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-dark.svg` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-light.png` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/icons/logo-traceflows-light.svg` & `restoreio-0.6.3/docs/source/_static/images/icons/logo-traceflows-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/cor_cov.png` & `restoreio-0.6.3/docs/source/_static/images/plots/cor_cov.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/deviation.png` & `restoreio-0.6.3/docs/source/_static/images/plots/deviation.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/ensembles.png` & `restoreio-0.6.3/docs/source/_static/images/plots/ensembles.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/ensembles_js_distance.png` & `restoreio-0.6.3/docs/source/_static/images/plots/ensembles_js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/gdop_coverage.png` & `restoreio-0.6.3/docs/source/_static/images/plots/gdop_coverage.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/js_distance.png` & `restoreio-0.6.3/docs/source/_static/images/plots/js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/kl_eigenvalues.png` & `restoreio-0.6.3/docs/source/_static/images/plots/kl_eigenvalues.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/kl_eigenvectors.png` & `restoreio-0.6.3/docs/source/_static/images/plots/kl_eigenvectors.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/orig_vel_and_error.png` & `restoreio-0.6.3/docs/source/_static/images/plots/orig_vel_and_error.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/images/plots/rbf_kernel_2d.png` & `restoreio-0.6.3/docs/source/_static/images/plots/rbf_kernel_2d.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_static/js/custom-pydata.js` & `restoreio-0.6.3/docs/source/_static/js/custom-pydata.js`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_templates/autosummary/class.rst` & `restoreio-0.6.3/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_templates/layout.html` & `restoreio-0.6.3/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/_templates/version.html` & `restoreio-0.6.3/docs/source/_templates/version.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/cite.rst` & `restoreio-0.6.3/docs/source/cite.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/conf.py` & `restoreio-0.6.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/custom_domain.py` & `restoreio-0.6.3/docs/source/custom_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/index.rst` & `restoreio-0.6.3/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. module:: restoreio
 
 |project| Documentation
 ***********************
 
 |deploy-docs|
 
-|project| is a modular and high-performance Python package for machine learning using **G**\ aussian process regression with novel algorithms capable of petascale computation on multi-GPU devices.
+|project| is a python package to **Restore** **I**\ ncomplete **O**\ ceanographic datasets, with specific focus on ocean surface velocity data. It can also generate data ensembles and perform statistical analysis, enabling uncertainty qualification.
 
 .. .. toctree::
     :maxdepth: 1
 
     old/ComputeLogDeterminant.rst
     old/ComputeTraceOfInverse.rst
     old/examples.rst
@@ -30,16 +30,16 @@
         :class-card: custom-card-link
 
     .. grid-item-card:: Anaconda Cloud
         :link: https://anaconda.org/s-ameli/restoreio
         :text-align: center
         :class-card: custom-card-link
 
-    .. grid-item-card:: Docker Hub
-        :link: https://hub.docker.com/r/sameli/restoreio
+    .. grid-item-card:: Online Interface
+        :link: https://transport.me.berkeley.edu/restore
         :text-align: center
         :class-card: custom-card-link
 
 .. grid:: 4
 
     .. grid-item-card:: Install
         :link: install
```

### Comparing `restoreio-0.5.0/docs/source/install.rst` & `restoreio-0.6.3/docs/source/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,14 @@
 Install |project| and its Python dependencies through `PyPI <https://pypi.org/project/restoreio>`_ by
 
 .. prompt:: bash
     
     python -m pip install --upgrade pip
     python -m pip install restoreio
 
-If you are using PyPy instead of Python, install with
-
-.. prompt:: bash
-    
-    pypy -m pip install --upgrade pip
-    pypy -m pip install restoreio
-
 Install with ``conda``
 ----------------------
 
 |conda-version|
 
 Alternately, install |project| and its Python dependencies from `Anaconda Cloud <https://anaconda.org/s-ameli/restoreio>`_ by
```

### Comparing `restoreio-0.5.0/docs/source/notebooks/quick_start.ipynb` & `restoreio-0.6.3/docs/source/notebooks/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/docs/source/recursive_glob.py` & `restoreio-0.6.3/docs/source/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/examples/restore/main_VaryingNumModes.py` & `restoreio-0.6.3/examples/restore/main_VaryingNumModes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/examples/restore/plot_coverage.py` & `restoreio-0.6.3/examples/restore/plot_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/examples/restore/plot_fixed_size_artificial_mask.py` & `restoreio-0.6.3/examples/restore/plot_fixed_size_artificial_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/examples/restore/plot_variable_d_artificial_masks.py` & `restoreio-0.6.3/examples/restore/plot_variable_d_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/examples/restore/plot_variable_size_artificial_masks.py` & `restoreio-0.6.3/examples/restore/plot_variable_size_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/examples/uncertainty_quant/_display_utilities.py` & `restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/examples/uncertainty_quant/_draw_map.py` & `restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_draw_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # =======
 # Imports
 # =======
 
 import numpy
 from mpl_toolkits.basemap import Basemap
-from _plot_utilities import Polygon
+from ._plot_utilities import Polygon
 
 __all__ = ['draw_map', 'draw_axis']
 
 
 # ========
 # Draw map
 # ========
```

### Comparing `restoreio-0.5.0/examples/uncertainty_quant/_plot_utilities.py` & `restoreio-0.6.3/examples/uncertainty_quant/_utils/_plot_utils/_plot_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from mpl_toolkits.axes_grid1.inset_locator import InsetPosition    # noqa: F401
 from mpl_toolkits.axes_grid1.inset_locator import mark_inset       # noqa: F401
 from matplotlib.ticker import ScalarFormatter, NullFormatter       # noqa: F401
 from matplotlib.ticker import FormatStrFormatter                   # noqa: F401
 from mpl_toolkits.axes_grid1 import make_axes_locatable            # noqa: F401
 
 from distutils.spawn import find_executable
-from _display_utilities import is_notebook
+from ._display_utilities import is_notebook
 import logging
 import warnings
 
 # Check DISPLAY
 if ((not bool(os.environ.get('DISPLAY', None))) or
         (bool(os.environ.get('RESTOREIO_NO_DISPLAY', None)))) and \
         (not is_notebook()):
```

### Comparing `restoreio-0.5.0/examples/uncertainty_quant/plot_gdop_coverage.py` & `restoreio-0.6.3/examples/uncertainty_quant/plot_gdop_coverage.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 # =======
 # Imports
 # =======
 
 import sys
 import numpy
 import netCDF4
-from _plot_utilities import plt, make_axes_locatable, save_plot, \
-        load_plot_settings
+from _utils._plot_utils._plot_utilities import plt, make_axes_locatable, \
+        save_plot, load_plot_settings
 from matplotlib.colors import ListedColormap
 import matplotlib.ticker
-from _draw_map import draw_map
+from _utils._plot_utils._draw_map import draw_map
+from _utils._load_variables import get_datetime_info
+from _utils._subset import subset_domain, subset_datetime
 
 
 # ================
 # Compute Coverage
 # ================
 
 def _compute_coverage(u):
@@ -315,23 +317,59 @@
     # Data is obtained from http://hfrnet-tds.ucsd.edu/thredds. In this thredds
     # website, navigate to "HF RADAR, US West Coast", click on
     # "HFRADAR US West Coast 2km Resolution Hourly RTV" and then
     # "Best Time Series". From "Access" methods, select "NetcdfSubset", then
     # extract a subset of data between -122.843 to -121.698 longitudes and
     # 36.3992 to 37.2802 latitudes, from 2017-01-01 00:00:00Z to 2017-02-01
     # 00:00:00Z. After download, rename to the file below.
-    filename = '../files/Monterey_Large_2km_Hourly_2017_01.nc'
+    # filename = '../files/Monterey_Large_2km_Hourly_2017_01.nc'
 
-    nc = netCDF4.Dataset(filename)
+    # OpenDap URL of the remote netCDF data
+    url = 'http://hfrnet-tds.ucsd.edu/thredds/' + \
+          'dodsC/HFR/USWC/2km/hourly/RTV/HFRAD' + \
+          'AR_US_West_Coast_2km_Resolution_Hou' + \
+          'rly_RTV_best.ncd'
+
+    # nc = netCDF4.Dataset(filename)
+    nc = netCDF4.Dataset(url)
     # site_lon = nc.variables['site_lon'][:]
     # site_lat = nc.variables['site_lat'][:]
     # site_code = nc.variables['site_code'][:]
-    data_lon = nc.variables['lon']
-    data_lat = nc.variables['lat']
-    u = nc.variables['u']
+    datetime_obj = nc.variables['time']
+    lon_obj = nc.variables['lon']
+    lat_obj = nc.variables['lat']
+    east_vel_obj = nc.variables['u']
+
+    # Get datetime info from datetime netcdf object
+    datetime_info = get_datetime_info(datetime_obj)
+
+    # Subset settings
+    time = '2017-01-25T03:00:00'
+    min_time = ""
+    max_time = ""
+    min_lon = -122.843
+    max_lon = -121.698
+    min_lat = 36.3992
+    max_lat = 37.2802
+
+    # Subset time
+    min_datetime_index, max_datetime_index = subset_datetime(
+        datetime_info, min_time, max_time, time)
+
+    # Subset domain
+    min_lon_index, max_lon_index, min_lat_index, max_lat_index = \
+        subset_domain(lon_obj, lat_obj, min_lon, max_lon, min_lat, max_lat)
+    data_lon = nc.variables['lon'][min_lon_index:max_lon_index+1]
+    data_lat = nc.variables['lat'][min_lat_index:max_lat_index+1]
+
+    # Subset velocity
+    u = east_vel_obj[
+            min_datetime_index:max_datetime_index+1,
+            min_lat_index:max_lat_index+1,
+            min_lon_index:max_lon_index+1]
 
     # Site code names
     # site_codes = []
     # for i in range(site_code.shape[0]):
     #     code = site_code[i].tostring().decode('ascii').strip('\x00').strip(
     #             ' ')
     #     site_codes.append(code)
```

### Comparing `restoreio-0.5.0/examples/uncertainty_quant/plot_js_divergence.py` & `restoreio-0.6.3/examples/uncertainty_quant/plot_js_divergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/examples/uncertainty_quant/restoreio_mwe.py` & `restoreio-0.6.3/examples/uncertainty_quant/restoreio_mwe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+#! /usr/bin/env python
+
 # Install restoreio with ;#"\texttt{pip install restoreio}"#;
 from restoreio import restore
 
 # OpenDap URL of the remote netCDF data
 url = 'http://hfrnet-tds.ucsd.edu/thredds/' + \
        'dodsC/HFR/USWC/2km/hourly/RTV/HFRAD' + \
        'AR_US_West_Coast_2km_Resolution_Hou' + \
        'rly_RTV_best.ncd'
 
 # Generate ensembles and reconstruct gaps at ;#$ \OmegaMissing $#;
 restore(input=url, output='output.nc',
-         time='2017-01-25T03:00:00',
          min_lon=-122.344, max_lon=-121.781,
          min_lat=36.507, max_lat=36.992,
-         uncertainty_quant=True,
+         time='2017-01-25T03:00:00',
+         uncertainty_quant=True, plot=True,
          num_ensembles=2000, ratio_num_modes=1,
          kernel_width=5, scale_error=0.08,
          detect_land=True, fill_coast=True,
-         plot=True, verbose=True)
+         write_ensembles=True, verbose=True)
```

### Comparing `restoreio-0.5.0/restoreio/__main__.py` & `restoreio-0.6.3/restoreio/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,14 +148,15 @@
         alpha=20,
         refine_grid=1,
         uncertainty_quant=False,
         num_ensembles=1000,
         ratio_num_modes=1,
         kernel_width=5,
         scale_error=0.08,
+        write_ensembles=False,
         plot=False,
         save=True,
         verbose=False,
         terminate=False):
     """
     Restore incomplete oceanographic dataset.
 
@@ -316,14 +317,18 @@
     scale_error : float, default=0.08
         Scale velocity error of the input data by a factor. Often, the input
         velocity error is the dimensionless GDOP which needs to be scaled by
         the standard deviation of the velocity error to represent the actual
         velocity error. This value scales the error. This option is relevant if
         ``uncertainty_quant`` is set to `True`.
 
+    write_ensembles : bool, default=False,
+        If `True`, all generated ensembles will be written to the output file.
+        This option is relevant if ``uncertainty_quant`` is set to `True`.
+
     plot : bool, default=False
         Plots the results. In this case, instead of iterating through all time
         frames, only one time frame (given with option ``timeframe``) is
         restored and plotted. If in addition, the uncertainty quantification is
         enabled (with option ``uncertainty_quant=True``), the statistical
         analysis for the given time frame is also plotted.
 
@@ -335,15 +340,15 @@
 
     verbose : bool, default=False
         If `True`, prints verbose information during the computation process.
 
     terminate ; bool, default=False
         If `True`, on encountering errors, the program both raises error and
         exists with code 1 with printing the message starting with the keyword
-        ``ERROR: ``. This is useful when this package is executed on a server
+        ``ERROR``. This is useful when this package is executed on a server
         to pass exit signals to a Node application. On the downside, this
         option causes an interactive python environment to both terminate the
         script and the python environment itself. To avoid this, set this
         option to `False`. In this case, upon an error, the ``ValueError`` is
         raised, which cases the script to terminate, however, an interactive
         python environment will not be exited.
     """
@@ -407,77 +412,77 @@
         # if the velocity arrays have depth dimension, use only the first index
         depth_index = 0
         vel_array_dim = len(east_vel_obj.shape)
 
         # Subset velocity arrays both in datetime and domain
         if vel_array_dim == 3:
 
-            U_all_times = east_vel_obj[
+            u_all_times = east_vel_obj[
                     min_datetime_index:max_datetime_index+1,
                     min_lat_index:max_lat_index+1,
                     min_lon_index:max_lon_index+1]
 
-            V_all_times = north_vel_obj[
+            v_all_times = north_vel_obj[
                     min_datetime_index:max_datetime_index+1,
                     min_lat_index:max_lat_index+1,
                     min_lon_index:max_lon_index+1]
 
         elif vel_array_dim == 4:
 
-            U_all_times = east_vel_obj[
+            u_all_times = east_vel_obj[
                     min_datetime_index:max_datetime_index+1,
                     depth_index,
                     min_lat_index:max_lat_index+1,
                     min_lon_index:max_lon_index+1]
 
-            V_all_times = north_vel_obj[
+            v_all_times = north_vel_obj[
                     min_datetime_index:max_datetime_index+1,
                     depth_index,
                     min_lat_index:max_lat_index+1,
                     min_lon_index:max_lon_index+1]
 
         else:
             terminate_with_error('Velocity arrays should have three or four' +
                                  'dimensions.')
 
         # Velocity error
         if east_vel_error_obj is None:
             # When None, no uncertainty quantification should be used.
-            U_error_all_times = None
-            V_error_all_times = None
+            u_error_all_times = None
+            v_error_all_times = None
 
         else:
 
             # if the velocity error has depth dimension, use only the first
             # index
             depth_index = 0
             error_array_dim = len(east_vel_obj.shape)
 
             # Subset velocity arrays both in datetime and domain
             if error_array_dim == 3:
 
-                U_error_all_times = east_vel_error_obj[
+                u_error_all_times = east_vel_error_obj[
                         min_datetime_index:max_datetime_index+1,
                         min_lat_index:max_lat_index+1,
                         min_lon_index:max_lon_index+1]
 
-                V_error_all_times = north_vel_error_obj[
+                v_error_all_times = north_vel_error_obj[
                         min_datetime_index:max_datetime_index+1,
                         min_lat_index:max_lat_index+1,
                         min_lon_index:max_lon_index+1]
 
             elif error_array_dim == 4:
 
-                U_error_all_times = east_vel_obj[
+                u_error_all_times = east_vel_obj[
                         min_datetime_index:max_datetime_index+1,
                         depth_index,
                         min_lat_index:max_lat_index+1,
                         min_lon_index:max_lon_index+1]
 
-                V_error_all_times = north_vel_obj[
+                v_error_all_times = north_vel_obj[
                         min_datetime_index:max_datetime_index+1,
                         depth_index,
                         min_lat_index:max_lat_index+1,
                         min_lon_index:max_lon_index+1]
 
             else:
                 terminate_with_error(
@@ -485,16 +490,16 @@
                     'four dimensions.')
 
         # Refinement
         # Do not use this, because (1) lon and lat for original and refined
         # grids will be different, hence the plot functions should be aware of
         # these two grids, and (2) inpainted results on refined grid is poor.
         # if refine_grid != 1:
-        #     lon, lat, U_all_times, V_all_times = refine_grid(
-        #             refine_grid, lon, lat, U_all_times, V_all_times)
+        #     lon, lat, u_all_times, v_all_times = refine_grid(
+        #             refine_grid, lon, lat, u_all_times, v_all_times)
 
         # Determine the land
         land_indices, ocean_indices = detect_land_ocean(
                 lon, lat, detect_land, verbose=verbose)
 
         # If plotting, remove these files:
         if plot is True:
@@ -506,62 +511,75 @@
             if os.path.isfile(home_dir+'/.ICEauthority'):
                 os.remove(home_dir+'/.ICEauthority')
 
         # Check whether to perform uncertainty quantification or not
         if uncertainty_quant is True:
 
             # Restore all generated ensembles
-            U_all_ensembles_inpainted_mean, \
-                V_all_ensembles_inpainted_mean, \
-                U_all_ensembles_inpainted_std, \
-                V_all_ensembles_inpainted_std, mask_info = \
-                restore_generated_ensembles(
+            u_all_ensembles_inpainted, v_all_ensembles_inpainted, \
+                u_all_ensembles_inpainted_mean, \
+                v_all_ensembles_inpainted_mean, \
+                u_all_ensembles_inpainted_std, v_all_ensembles_inpainted_std, \
+                mask_info = restore_generated_ensembles(
                         diffusivity, sweep, fill_coast, alpha, convex_hull,
                         num_ensembles, ratio_num_modes, kernel_width,
-                        scale_error, lon, lat, land_indices, U_all_times,
-                        V_all_times, U_error_all_times, V_error_all_times,
-                        fill_value, plot, save=save, verbose=verbose)
+                        scale_error, lon, lat, land_indices, u_all_times,
+                        v_all_times, u_error_all_times, v_error_all_times,
+                        fill_value, file_index, num_files, plot=plot,
+                        save=save, verbose=verbose)
 
             # Write results to netcdf output file
             write_output_file(
+                    fullpath_output_filenames_list[file_index],
                     datetime_info,
                     lon,
                     lat,
                     mask_info,
-                    U_all_ensembles_inpainted_mean,
-                    V_all_ensembles_inpainted_mean,
-                    U_all_ensembles_inpainted_std,
-                    V_all_ensembles_inpainted_std,
                     fill_value,
-                    fullpath_output_filenames_list[file_index],
+                    u_all_ensembles_inpainted_mean,
+                    v_all_ensembles_inpainted_mean,
+                    u_all_ensembles_inpainted_std,
+                    v_all_ensembles_inpainted_std,
+                    u_all_ensembles_inpainted,
+                    v_all_ensembles_inpainted,
+                    write_ensembles=write_ensembles,
                     verbose=verbose)
 
         else:
 
+            if write_ensembles:
+                terminate_with_error('Cannot write ensembles to output ' +
+                                     'when uncertainty quantification is ' +
+                                     'not enabled.')
+
             # Restore With Central Ensemble (use original data, no uncertainty
             # quantification
-            U_all_times_inpainted, V_all_times_inpainted, \
-                U_all_times_inpainted_error, V_all_times_inpainted_error, \
+            u_all_times_inpainted, v_all_times_inpainted, \
+                u_all_times_inpainted_error, v_all_times_inpainted_error, \
                 mask_info_all_times = restore_main_ensemble(
                         diffusivity, sweep, fill_coast, alpha, convex_hull,
-                        lon, lat, land_indices, U_all_times, V_all_times,
-                        fill_value, plot, save=save, verbose=verbose)
+                        lon, lat, land_indices, u_all_times, v_all_times,
+                        fill_value, file_index, num_files, plot=plot,
+                        save=save, verbose=verbose)
 
             # Write results to netcdf output file
             write_output_file(
+                    fullpath_output_filenames_list[file_index],
                     datetime_info,
                     lon,
                     lat,
                     mask_info_all_times,
-                    U_all_times_inpainted,
-                    V_all_times_inpainted,
-                    U_all_times_inpainted_error,
-                    V_all_times_inpainted_error,
                     fill_value,
-                    fullpath_output_filenames_list[file_index],
+                    u_all_times_inpainted,
+                    v_all_times_inpainted,
+                    u_all_times_inpainted_error,
+                    v_all_times_inpainted_error,
+                    u_all_ensembles_inpainted=None,
+                    v_all_ensembles_inpainted=None,
+                    write_ensembles=False,
                     verbose=verbose)
 
         agg.close()
 
     # End of loop over files
 
     # If there are multiple files, zip them are delete (clean) written files
```

### Comparing `restoreio-0.5.0/restoreio/_file_utilities/__init__.py` & `restoreio-0.6.3/restoreio/_file_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_file_utilities/file_utilities.py` & `restoreio-0.6.3/restoreio/_file_utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_geography/__init__.py` & `restoreio-0.6.3/restoreio/_geography/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_geography/_find_alpha_shapes.py` & `restoreio-0.6.3/restoreio/_geography/_find_alpha_shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     triangulations = Delaunay(numpy.asarray(points_coord))
 
     # Initialize set of edges and list of edge points coordinates
     edges = set()
     edge_points_coord = []
 
     # Loop over triangles
-    for triangle_vertices_indices in triangulations.vertices:
+    for triangle_vertices_indices in triangulations.simplices:
 
         # Get coordinates of vertices
         triangle_vertices_coord = points_coord[triangle_vertices_indices, :]
 
         # Get circumcircle radius of the triangle
         circumcircle_radius = compute_triangle_circumcicle(
                 triangle_vertices_coord)
```

### Comparing `restoreio-0.5.0/restoreio/_geography/create_mask_info.py` & `restoreio-0.6.3/restoreio/_geography/create_mask_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_geography/detect_land_ocean.py` & `restoreio-0.6.3/restoreio/_geography/detect_land_ocean.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_geography/locate_missing_data.py` & `restoreio-0.6.3/restoreio/_geography/locate_missing_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_inpaint/_cast_types.py` & `restoreio-0.6.3/restoreio/_inpaint/_cast_types.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_inpaint/_image.py` & `restoreio-0.6.3/restoreio/_inpaint/_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_inpaint/_plot_image.py` & `restoreio-0.6.3/restoreio/_inpaint/_plot_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_inpaint/inpaint.py` & `restoreio-0.6.3/restoreio/_inpaint/inpaint.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_input_output/__init__.py` & `restoreio-0.6.3/restoreio/_input_output/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_input_output/get_datetime_info.py` & `restoreio-0.6.3/examples/uncertainty_quant/_utils/_load_variables/_get_datetime_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_input_output/load_dataset.py` & `restoreio-0.6.3/restoreio/_input_output/load_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 __all__ = ['load_dataset']
 
 
 # ==================
 # Load Local Dataset
 # ==================
 
-def load_local_dataset(filename, verbose=True):
+def load_local_dataset(filename, verbose=False):
     """
     Opens either ncml or nc file and returns the aggregation file object.
     """
 
     if verbose:
-        print("Message: Loading data ... ")
+        print("Message: Loading local data files ... ")
     sys.stdout.flush()
 
     # Check file extension
     file_extension = os.path.splitext(filename)[1]
     if file_extension in ['.ncml', '.ncml.gz']:
 
         # Change directory
@@ -84,19 +84,23 @@
             "File format %s is not recognized." % file_extension)
 
 
 # ===================
 # Load Remote Dataset
 # ===================
 
-def load_remote_dataset(url):
+def load_remote_dataset(url, verbose=False):
     """
     url can be point to a *.nc or *.ncml file.
     """
 
+    if verbose:
+        print("Message: Connecting to remote data server ... ")
+    sys.stdout.flush()
+
     # Check URL is opendap
     if (url.startswith('http://') is False) and \
        (url.startswith('https://') is False):
         terminate_with_error(
             'Input data URL does not seem to be a URL. A URL should start ' +
             'with "http://" or "https://".')
 
@@ -135,15 +139,15 @@
     return nc
 
 
 # ============
 # Load Dataset
 # ============
 
-def load_dataset(input_filename, verbose=True):
+def load_dataset(input_filename, verbose=False):
     """
     Dispatches the execution to either of the following two functions:
 
     1. load_local_dataset: For files where the input_filename is a path on the
        local machine.
     2. load_remote_dataset: For files remotely where input_filename is a url.
     """
@@ -152,11 +156,11 @@
         terminate_with_error(
             'Input data is empty. You should provide a local filename or an ' +
             'OpenDap URL or remote data.')
 
     # Check if the input_filename has a "host" name
     if bool(urlparse(input_filename).netloc):
         # input_filename is a url
-        return load_remote_dataset(input_filename)
+        return load_remote_dataset(input_filename, verbose=verbose)
     else:
         # input_filename is a path
         return load_local_dataset(input_filename, verbose=verbose)
```

### Comparing `restoreio-0.5.0/restoreio/_input_output/load_variables.py` & `restoreio-0.6.3/restoreio/_input_output/load_variables.py`

 * *Files 20% similar despite different names*

```diff
@@ -93,29 +93,59 @@
     lat_names_list = ['latitude', 'lat']
     lat_standard_names_list = ['latitude']
     lat_obj = search_variable(agg, lat_names_list, lat_standard_names_list)
     if lat_obj is None:
         raise RuntimeError('Latitude object can not be found in netCDF file.')
 
     # East Velocity
-    east_vel_names_list = ['east_vel', 'eastward_vel', 'u', 'east_velocity',
-                           'eastward_velocity']
-    east_vel_standard_names_list = ['surface_eastward_sea_water_velocity',
-                                    'eastward_sea_water_velocity']
+    east_vel_names_list = ['east_vel', 'eastward_vel', 'u', 'ugos',
+                           'east_velocity', 'eastward_velocity']
+    east_vel_standard_names_list = [
+        'surface_eastward_sea_water_velocity',
+        'eastward_sea_water_velocity',
+        'surface_geostrophic_eastward_sea_water_velocity',
+        'surface_geostrophic_sea_water_x_velocity',
+        'surface_geostrophic_eastward_sea_water_velocity_assuming_sea_' +
+        'level_for_geoid',
+        'surface_eastward_geostrophic_sea_water_velocity_assuming_sea_' +
+        'level_for_geoid',
+        'surface_geostrophic_sea_water_x_velocity_assuming_mean_sea_level_' +
+        'for_geoid',
+        'surface_geostrophic_sea_water_x_velocity_assuming_sea_level_for_' +
+        'geoid',
+        'surface_geostrophic_eastward_sea_water_velocity_assuming_mean_sea_' +
+        'level_for_geoid',
+        'sea_water_x_velocity',
+        'x_sea_water_velocity']
     east_vel_obj = search_variable(agg, east_vel_names_list,
                                    east_vel_standard_names_list)
     if east_vel_obj is None:
         raise RuntimeError('EastVelocity object can not be found in ' +
                            'netCDF file.')
 
     # North Velocity
-    north_vel_names_list = ['north_vel', 'northward_vel', 'v',
+    north_vel_names_list = ['north_vel', 'northward_vel', 'v', 'vgos',
                             'north_velocity', 'northward_velocity']
-    north_vel_standard_names_list = ['surface_northward_sea_water_velocity',
-                                     'northward_sea_water_velocity']
+    north_vel_standard_names_list = [
+        'surface_northward_sea_water_velocity',
+        'northward_sea_water_velocity',
+        'surface_geostrophic_northward_sea_water_velocity',
+        'surface_geostrophic_sea_water_y_velocity',
+        'surface_geostrophic_northward_sea_water_velocity_assuming_sea_' +
+        'level_for_geoid',
+        'surface_northward_geostrophic_sea_water_velocity_assuming_sea_' +
+        'level_for_geoid',
+        'surface_geostrophic_sea_water_y_velocity_assuming_mean_sea_level_' +
+        'for_geoid',
+        'surface_geostrophic_sea_water_y_velocity_assuming_sea_level_for_' +
+        'geoid',
+        'surface_geostrophic_northward_sea_water_velocity_assuming_mean_' +
+        'sea_level_for_geoid',
+        'sea_water_y_velocity',
+        'y_sea_water_velocity']
     north_vel_obj = search_variable(agg, north_vel_names_list,
                                     north_vel_standard_names_list)
     if north_vel_obj is None:
         raise RuntimeError('NorthVelocity object can not be found in ' +
                            'netCDF file.')
 
     # East Velocity Error
```

### Comparing `restoreio-0.5.0/restoreio/_input_output/writer.py` & `restoreio-0.6.3/restoreio/_input_output/writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,24 +34,27 @@
 
 
 # =================
 # Write Output File
 # =================
 
 def write_output_file(
+        output_filename,
         datetime_info,
         longitude,
         latitude,
         mask_info,
+        fill_value,
         u_all_times_inpainted,
         v_all_times_inpainted,
         u_all_times_inpainted_error,
         v_all_times_inpainted_error,
-        fill_value,
-        output_filename,
+        u_all_ensembles_inpainted=None,
+        v_all_ensembles_inpainted=None,
+        write_ensembles=False,
         verbose=True):
     """
     Writes the inpainted array to an output netcdf file.
     """
 
     if verbose:
         print("Message: Writing to NetCDF file ...")
@@ -63,14 +66,17 @@
     output_file = netCDF4.Dataset(output_filename, 'w',
                                   format='NETCDF4_CLASSIC')
 
     # Dimensions
     output_file.createDimension('time', None)
     output_file.createDimension('lon', len(longitude))
     output_file.createDimension('lat', len(latitude))
+    if write_ensembles:
+        num_ensembles = u_all_ensembles_inpainted.shape[0]
+        output_file.createDimension('ensemble', num_ensembles)
 
     # Datetime
     output_datetime = output_file.createVariable(
             'time', numpy.dtype('float64').char, ('time', ))
     output_datetime[:] = datetime_info['array']
     output_datetime.units = datetime_info['unit']
     output_datetime.calendar = datetime_info['calendar']
@@ -163,14 +169,38 @@
         output_v_error[:] = v_all_times_inpainted_error
         output_v_error.units = 'm s-1'
         output_v_error.positive = 'toward north'
         output_v_error.coordinates = 'longitude latitude datetime'
         output_v_error.missing_value = fill_value
         output_v_error.coordsys = "geographic"
 
+    # Velocity U Ensembles
+    if (write_ensembles is True) and (u_all_ensembles_inpainted is not None):
+        output_u_ens = output_file.createVariable(
+                'East_vel_ensembles', numpy.dtype('float64').char,
+                ('ensemble', 'lat', 'lon', ), fill_value=fill_value, zlib=True)
+        output_u_ens[:] = u_all_ensembles_inpainted
+        output_u_ens.units = 'm s-1'
+        output_u_ens.positive = 'toward east'
+        output_u_ens.coordinates = 'longitude latitude ensemble'
+        output_u_ens.missing_value = fill_value
+        output_u_ens.coordsys = "geographic"
+
+    # Velocity V Ensembles
+    if (write_ensembles is True) and (v_all_ensembles_inpainted is not None):
+        output_v_ens = output_file.createVariable(
+                'North_vel_ensembles', numpy.dtype('float64').char,
+                ('ensemble', 'lat', 'lon', ), fill_value=fill_value, zlib=True)
+        output_v_ens[:] = v_all_ensembles_inpainted
+        output_v_ens.units = 'm s-1'
+        output_v_ens.positive = 'toward east'
+        output_v_ens.coordinates = 'longitude latitude ensemble'
+        output_v_ens.missing_value = fill_value
+        output_v_ens.coordsys = "geographic"
+
     # Global Attributes
     output_file.Conventions = 'CF-1.6'
     output_file.COORD_SYSTEM = 'GEOGRAPHIC'
     output_file.contributor_name = 'Siavash Ameli'
     output_file.contributor_email = 'sameli@berkeley.edu'
     output_file.contributor_role = 'Post process data to fill missing points.'
     output_file.institution = 'University of California, Berkeley'
```

### Comparing `restoreio-0.5.0/restoreio/_parser/examples.py` & `restoreio-0.6.3/restoreio/_parser/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_parser/formatter.py` & `restoreio-0.6.3/restoreio/_parser/formatter.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_parser/parse_arguments.py` & `restoreio-0.6.3/restoreio/_parser/parse_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,25 +325,32 @@
     Instance, ``-i input -I 003 -J 012`` means to read the series of input
     files with iterators ``input003.nc``, ``input004.nc``, to ``input012.nc``.
     If this option is used, the option ``-I`` should also be given.
     """
     optional.add_argument('-J', type=str, default='', metavar="END_FILE",
                           help=help_max_file_index)
 
+    # Write ensembles
+    help_write_ensembles = """
+    If `True`, all generated ensembles will be written to the output file. This
+    option is relevant to uncertainty quantification (when ``-u`` is used).
+    """
+    optional.add_argument('-W', action='store_true', help=help_write_ensembles)
+
     # Verbose
     help_verbose = """
     Prints verbose information.
     """
     optional.add_argument('-v', action='store_true', help=help_verbose)
 
     # Terminate
     help_terminate = """
     If `True`, on encountering errors, the program both raises error and exists
     with code 1 with printing the message starting with the keyword
-    ``ERROR: ``. This is useful when this package is executed on a server to
+    ``ERROR``. This is useful when this package is executed on a server to
     pass exit signals to a Node application. On the downside, this option
     causes an interactive python environment to both terminate the script and
     the python environment itself. To avoid this, set this option to `False`.
     In this case, upon an error, the ``ValueError`` is raised, which cases the
     script to terminate, however, an interactive python environment will not be
     exited.
     """
@@ -401,12 +408,13 @@
         'uncertainty_quant': args.u,
         'num_ensembles': args.e,
         'ratio_num_modes': args.m,
         'kernel_width': args.w,
         'scale_error': args.E,
         "min_file_index": args.I,
         "max_file_index": args.J,
+        "write_ensembles": args.W,
         "verbose": args.v,
         "terminate": args.T,
     }
 
     return arguments
```

### Comparing `restoreio-0.5.0/restoreio/_plots/_display_utilities.py` & `restoreio-0.6.3/restoreio/_plots/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots/_draw_map.py` & `restoreio-0.6.3/restoreio/_plots/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots/_plot_grid.py` & `restoreio-0.6.3/restoreio/_plots/_plot_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots/_plot_quiver.py` & `restoreio-0.6.3/restoreio/_plots/_plot_quiver.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots/_plot_streamlines.py` & `restoreio-0.6.3/restoreio/_plots/_plot_streamlines.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots/_plot_utilities.py` & `restoreio-0.6.3/restoreio/_plots/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots/_plot_velocities.py` & `restoreio-0.6.3/restoreio/_plots/_plot_velocities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots/plot_results.py` & `restoreio-0.6.3/restoreio/_plots/plot_results.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/__init__.py` & `restoreio-0.6.3/restoreio/_plots_uq/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/_refine_mask.py` & `restoreio-0.6.3/restoreio/_plots_uq/_refine_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/_shifted_colormap.py` & `restoreio-0.6.3/restoreio/_plots_uq/_shifted_colormap.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/plot_auto_correlation.py` & `restoreio-0.6.3/restoreio/_plots_uq/plot_auto_correlation.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/plot_convergence.py` & `restoreio-0.6.3/restoreio/_plots_uq/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/plot_cor_cov.py` & `restoreio-0.6.3/restoreio/_plots_uq/plot_cor_cov.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/plot_ensembles_stat.py` & `restoreio-0.6.3/restoreio/_plots_uq/plot_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/plot_kl_transform.py` & `restoreio-0.6.3/restoreio/_plots_uq/plot_kl_transform.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/plot_rbf_kernel.py` & `restoreio-0.6.3/restoreio/_plots_uq/plot_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py` & `restoreio-0.6.3/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_restore/__init__.py` & `restoreio-0.6.3/restoreio/_restore/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_restore/_make_array_masked.py` & `restoreio-0.6.3/restoreio/_restore/_make_array_masked.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_restore/refine_grid.py` & `restoreio-0.6.3/restoreio/_restore/refine_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_restore/restore_generated_ensembles.py` & `restoreio-0.6.3/restoreio/_restore/restore_generated_ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,17 @@
         lat,
         land_indices,
         U_all_times,
         V_all_times,
         U_error_all_times,
         V_error_all_times,
         fill_value,
-        plot,
+        file_index,
+        num_files,
+        plot=False,
         save=True,
         verbose=False):
     """
     Restore all generated ensembles, and take their mean and std.
 
     Notes on parallelization:
         - We have used multiprocessing.Pool.imap_unordered. Other options are
@@ -237,15 +239,17 @@
     chunk_size = int(chunk_size / ratio)
     if chunk_size > 50:
         chunk_size = 50
     elif chunk_size < 5:
         chunk_size = 5
 
     # Parallel section
-    progress = 0
+    num_gen_ensembles = U_all_ensembles.shape[0]
+    progress = file_index * num_gen_ensembles
+    total_progress = num_files * num_gen_ensembles
     if verbose:
         print("Message: Restoring ensembles ...")
         sys.stdout.flush()
 
     # Parallel section
     for ensemble_index, U_inpainted, V_inpainted in \
             pool.imap_unordered(
@@ -257,15 +261,15 @@
         U_all_ensembles_inpainted[ensemble_index, :] = \
                 U_inpainted
         V_all_ensembles_inpainted[ensemble_index, :] = \
             V_inpainted
 
         progress += 1
         if verbose:
-            print("Progress: %d/%d" % (progress, U_all_ensembles.shape[0]))
+            print("Progress: %d/%d" % (progress, total_progress))
             sys.stdout.flush()
 
     # Get statistics of U inpainted ensembles
     U_all_ensembles_inpainted_stats = get_ensembles_stat(
             land_indices,
             valid_indices,
             missing_indices_in_ocean_inside_hull,
@@ -389,10 +393,10 @@
     if plot is True:
         plot_convergence(
                 missing_indices_in_ocean_inside_hull,
                 U_all_ensembles_inpainted, V_all_ensembles_inpainted,
                 U_all_ensembles_inpainted_stats,
                 V_all_ensembles_inpainted_stats, save=save, verbose=verbose)
 
-    return U_all_ensembles_inpainted_mean, \
-        V_all_ensembles_inpainted_mean, U_all_ensembles_inpainted_std, \
-        V_all_ensembles_inpainted_std, mask_info
+    return U_all_ensembles_inpainted, V_all_ensembles_inpainted, \
+        U_all_ensembles_inpainted_mean, V_all_ensembles_inpainted_mean, \
+        U_all_ensembles_inpainted_std, V_all_ensembles_inpainted_std, mask_info
```

### Comparing `restoreio-0.5.0/restoreio/_restore/restore_main_ensemble.py` & `restoreio-0.6.3/restoreio/_restore/restore_main_ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,15 +139,17 @@
         convex_hull,
         lon,
         lat,
         land_indices,
         U_all_times,
         V_all_times,
         fill_value,
-        plot,
+        file_index,
+        num_files,
+        plot=False,
         save=True,
         verbose=False):
     """
     Restore the given data (central ensemble).
 
     Notes on parallelization:
         - We have used multiprocessing.Pool.imap_unordered. Other options are
@@ -202,15 +204,17 @@
     if chunk_size > 50:
         chunk_size = 50
     elif chunk_size < 5:
         chunk_size = 5
 
     # Parallel section
     _plot_data = {}
-    progress = 0
+    num_time_indices = len(time_indices)
+    progress = file_index * num_time_indices
+    total_progress = num_files * num_time_indices
     if verbose:
         print("Message: Restoring time frames ...")
         sys.stdout.flush()
 
     if plot is True:
         # Use the last time for plot
         plot_time_index = time_indices[-1]
@@ -229,15 +233,15 @@
         # Set inpainted arrays
         U_all_times_inpainted[time_index, :] = U_inpainted
         V_all_times_inpainted[time_index, :] = V_inpainted
         mask_info_all_times[time_index, :] = mask_info
 
         progress += 1
         if verbose:
-            print("Progress: %d/%d" % (progress, len(time_indices)))
+            print("Progress: %d/%d" % (progress, total_progress))
             sys.stdout.flush()
 
     pool.terminate()
 
     # Plotting a single time frame
     if plot is True:
```

### Comparing `restoreio-0.5.0/restoreio/_scripts/examples.py` & `restoreio-0.6.3/restoreio/_scripts/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_scripts/scan.py` & `restoreio-0.6.3/restoreio/_scripts/scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -428,28 +428,57 @@
     """
     Finds the following variables from the aggregation object agg.
 
     - Eastward velocity U
     - Northward velocity V
     """
     # East Velocity
-    east_velocity_names_list = ['east_vel', 'eastward_vel', 'u',
+    east_velocity_names_list = ['east_vel', 'eastward_vel', 'u', 'ugos',
                                 'east_velocity', 'eastward_velocity']
-    east_velocity_standard_names_list = ['surface_eastward_sea_water_velocity',
-                                         'eastward_sea_water_velocity']
+    east_velocity_standard_names_list = [
+        'surface_eastward_sea_water_velocity',
+        'eastward_sea_water_velocity',
+        'surface_geostrophic_eastward_sea_water_velocity',
+        'surface_geostrophic_sea_water_x_velocity',
+        'surface_geostrophic_eastward_sea_water_velocity_assuming_sea_' +
+        'level_for_geoid',
+        'surface_eastward_geostrophic_sea_water_velocity_assuming_sea_' +
+        'level_for_geoid',
+        'surface_geostrophic_sea_water_x_velocity_assuming_mean_sea_level_' +
+        'for_geoid',
+        'surface_geostrophic_sea_water_x_velocity_assuming_sea_level_for_' +
+        'geoid',
+        'surface_geostrophic_eastward_sea_water_velocity_assuming_mean_sea_' +
+        'level_for_geoid',
+        'sea_water_x_velocity',
+        'x_sea_water_velocity']
     east_velocity_obj, east_velocity_name, east_velocity_standard_name = \
         _search_variable(agg, east_velocity_names_list,
                          east_velocity_standard_names_list)
 
     # North Velocity
-    north_velocity_names_list = ['north_vel', 'northward_vel', 'v',
+    north_velocity_names_list = ['north_vel', 'northward_vel', 'v', 'vgos',
                                  'north_velocity', 'northward_velocity']
     north_velocity_standard_names_list = [
         'surface_northward_sea_water_velocity',
-        'northward_sea_water_velocity']
+        'northward_sea_water_velocity',
+        'surface_geostrophic_northward_sea_water_velocity',
+        'surface_geostrophic_sea_water_y_velocity',
+        'surface_geostrophic_northward_sea_water_velocity_assuming_sea_' +
+        'level_for_geoid',
+        'surface_northward_geostrophic_sea_water_velocity_assuming_sea_' +
+        'level_for_geoid',
+        'surface_geostrophic_sea_water_y_velocity_assuming_mean_sea_level_' +
+        'for_geoid',
+        'surface_geostrophic_sea_water_y_velocity_assuming_sea_level_for_' +
+        'geoid',
+        'surface_geostrophic_northward_sea_water_velocity_assuming_mean_' +
+        'sea_level_for_geoid',
+        'sea_water_y_velocity',
+        'y_sea_water_velocity']
     north_velocity_obj, north_velocity_name, north_velocity_standard_name = \
         _search_variable(agg, north_velocity_names_list,
                          north_velocity_standard_names_list)
 
     return east_velocity_obj, north_velocity_obj, east_velocity_name, \
         north_velocity_name, east_velocity_standard_name, \
         north_velocity_standard_name
```

### Comparing `restoreio-0.5.0/restoreio/_server_utils/globals.py` & `restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/globals.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_server_utils/terminate_with_error.py` & `restoreio-0.6.3/examples/uncertainty_quant/_utils/_server_utils/terminate_with_error.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_subset/_array_utilities.py` & `restoreio-0.6.3/restoreio/_subset/_array_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_subset/subset_datetime.py` & `restoreio-0.6.3/restoreio/_subset/subset_datetime.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_subset/subset_domain.py` & `restoreio-0.6.3/restoreio/_subset/subset_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_uncertainty_quant/_compute_correlation_matrix.py` & `restoreio-0.6.3/restoreio/_uncertainty_quant/_compute_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py` & `restoreio-0.6.3/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_uncertainty_quant/_image_utils.py` & `restoreio-0.6.3/restoreio/_uncertainty_quant/_image_utils.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_uncertainty_quant/_statistical_distances.py` & `restoreio-0.6.3/restoreio/_uncertainty_quant/_statistical_distances.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_uncertainty_quant/generate_image_ensembles.py` & `restoreio-0.6.3/restoreio/_uncertainty_quant/generate_image_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio/_uncertainty_quant/get_ensembles_stat.py` & `restoreio-0.6.3/restoreio/_uncertainty_quant/get_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/restoreio.egg-info/PKG-INFO` & `restoreio-0.6.3/restoreio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.5.0
+Version: 0.6.3
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.5.0/restoreio.egg-info/SOURCES.txt` & `restoreio-0.6.3/restoreio.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -70,20 +70,30 @@
 docs/source/generated/restoreio.scan.rst
 docs/source/notebooks/quick_start.ipynb
 examples/restore/main_VaryingNumModes.py
 examples/restore/plot_coverage.py
 examples/restore/plot_fixed_size_artificial_mask.py
 examples/restore/plot_variable_d_artificial_masks.py
 examples/restore/plot_variable_size_artificial_masks.py
-examples/uncertainty_quant/_display_utilities.py
-examples/uncertainty_quant/_draw_map.py
-examples/uncertainty_quant/_plot_utilities.py
 examples/uncertainty_quant/plot_gdop_coverage.py
 examples/uncertainty_quant/plot_js_divergence.py
 examples/uncertainty_quant/restoreio_mwe.py
+examples/uncertainty_quant/_utils/_load_variables/__init__.py
+examples/uncertainty_quant/_utils/_load_variables/_get_datetime_info.py
+examples/uncertainty_quant/_utils/_plot_utils/__init__.py
+examples/uncertainty_quant/_utils/_plot_utils/_display_utilities.py
+examples/uncertainty_quant/_utils/_plot_utils/_draw_map.py
+examples/uncertainty_quant/_utils/_plot_utils/_plot_utilities.py
+examples/uncertainty_quant/_utils/_server_utils/__init__.py
+examples/uncertainty_quant/_utils/_server_utils/globals.py
+examples/uncertainty_quant/_utils/_server_utils/terminate_with_error.py
+examples/uncertainty_quant/_utils/_subset/__init__.py
+examples/uncertainty_quant/_utils/_subset/_array_utilities.py
+examples/uncertainty_quant/_utils/_subset/subset_datetime.py
+examples/uncertainty_quant/_utils/_subset/subset_domain.py
 restoreio/__init__.py
 restoreio/__main__.py
 restoreio/__version__.py
 restoreio.egg-info/PKG-INFO
 restoreio.egg-info/SOURCES.txt
 restoreio.egg-info/dependency_links.txt
 restoreio.egg-info/entry_points.txt
```

### Comparing `restoreio-0.5.0/setup.py` & `restoreio-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/tests/test_restore_local_data.py` & `restoreio-0.6.3/tests/test_restore_local_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,38 +57,40 @@
     max_lat = float('nan')
     time = '2017-01-25T03:00:00'
 
     # Absolute path
     dir = os.path.dirname(os.path.realpath(__file__))
     input = os.path.join(dir, input)
     output = os.path.join(dir, output)
+    plot = False
 
     # Check input exists
     if not os.path.exists(input):
         raise RuntimeError('File: %s does not exists.' % input)
 
     # Restore main file
     restore(input, min_file_index='', max_file_index='', output=output,
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
             time=time, sweep=False, detect_land=True, fill_coast=False,
             convex_hull=False, alpha=20, refine_grid=1,
-            uncertainty_quant=False, plot=True, verbose=True, terminate=False)
+            uncertainty_quant=False, plot=plot, verbose=True, terminate=False)
 
     # Uncertainty quantification
     restore(input, min_file_index='', max_file_index='', output=output,
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
             time=time, sweep=False, detect_land=True, fill_coast=False,
             convex_hull=False, alpha=20, refine_grid=1, uncertainty_quant=True,
             num_ensembles=200, ratio_num_modes=1, kernel_width=5,
-            scale_error=0.08, plot=True, verbose=True, terminate=False)
+            scale_error=0.08, write_ensembles=True, plot=plot, verbose=True,
+            terminate=False)
 
     # Remove outputs
-    # remove_file('*.svg')
-    # remove_file('*.pdf')
-    # remove_file(output)
+    remove_file('*.svg')
+    remove_file('*.pdf')
+    remove_file(output)
 
 
 # ===========
 # Script main
 # ===========
 
 if __name__ == "__main__":
```

### Comparing `restoreio-0.5.0/tests/test_restore_remote_data.py` & `restoreio-0.6.3/tests/test_restore_remote_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,34 +68,36 @@
     min_lat = 41.2
     max_lat = 41.3
     min_time = '2014-07-01T20:00:00'
     max_time = '2014-07-03T20:00:00'
 
     # Output
     output = 'output_remote_data.nc'
+    plot = True
 
     # Absolute path
     dir = os.path.dirname(os.path.realpath(__file__))
     output = os.path.join(dir, output)
 
     # Restore main file
     restore(input, min_file_index='', max_file_index='', output=output,
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
             min_time=min_time, max_time=max_time, sweep=False,
             detect_land=True, fill_coast=False, convex_hull=False, alpha=20,
-            refine_grid=1, uncertainty_quant=False, plot=False, verbose=True)
+            refine_grid=1, uncertainty_quant=False, plot=plot, verbose=True)
 
     # These lines are commented since WHOI-HFR data don't have error variables.
     # Uncertainty quantification
     # restore(input, min_file_index='', max_file_index='', output=output,
     #         min_lon=min_lon, max_lon=max_lon, min_lat=min_lat,
     #         max_lat=max_lat, time=time, sweep=False, detect_land=True,
     #         fill_coast=False, convex_hull=False, alpha=20, refine_grid=1,
     #         uncertainty_quant=True, num_ensembles=200, ratio_num_modes=1,
-    #         kernel_width=5, scale_error=0.08, plot=True, verbose=True)
+    #         kernel_width=5, scale_error=0.08, write_ensembles=True,
+    #         plot=plot, verbose=True)
 
     # Remove outputs
     remove_file('*.svg')
     remove_file('*.pdf')
     remove_file(output)
```

### Comparing `restoreio-0.5.0/tests/test_scan.py` & `restoreio-0.6.3/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.5.0/tox.ini` & `restoreio-0.6.3/tox.ini`

 * *Files identical despite different names*

