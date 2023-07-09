# Comparing `tmp/traceon-0.3.0.tar.gz` & `tmp/traceon-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceon-0.3.0.tar", last modified: Sun Jun 25 20:18:33 2023, max compression
+gzip compressed data, was "traceon-0.3.1.tar", last modified: Sun Jul  9 09:02:15 2023, max compression
```

## Comparing `traceon-0.3.0.tar` & `traceon-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.757537 traceon-0.3.0/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    34524 2023-03-21 09:42:58.000000 traceon-0.3.0/LICENSE.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       27 2023-04-09 12:34:12.000000 traceon-0.3.0/MANIFEST.in
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3838 2023-06-25 20:18:33.757537 traceon-0.3.0/PKG-INFO
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2628 2023-06-03 10:58:58.000000 traceon-0.3.0/README.md
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       38 2023-06-25 20:18:33.757537 traceon-0.3.0/setup.cfg
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     1818 2023-06-25 20:08:19.000000 traceon-0.3.0/setup.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.749536 traceon-0.3.0/traceon/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2876 2023-06-03 11:00:26.000000 traceon-0.3.0/traceon/__init__.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.749536 traceon-0.3.0/traceon/backend/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    19456 2023-06-25 19:37:04.000000 traceon-0.3.0/traceon/backend/__init__.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    46186 2023-06-25 20:09:32.000000 traceon-0.3.0/traceon/backend/traceon-backend.c
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.753536 traceon-0.3.0/traceon/data/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)  1023104 2023-04-09 12:34:12.000000 traceon-0.3.0/traceon/data/radial-series-3D-theta-dependent-coefficients.npy
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8128 2023-04-09 12:34:12.000000 traceon-0.3.0/traceon/data/radial-series-3D-thetas.npy
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     9224 2023-06-25 19:56:56.000000 traceon-0.3.0/traceon/excitation.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    18750 2023-06-25 20:02:06.000000 traceon-0.3.0/traceon/geometry.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8160 2023-06-25 11:54:05.000000 traceon-0.3.0/traceon/plotting.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    27673 2023-06-25 20:04:57.000000 traceon-0.3.0/traceon/solver.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    11829 2023-06-25 19:49:23.000000 traceon-0.3.0/traceon/tracing.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2204 2023-05-20 08:55:03.000000 traceon-0.3.0/traceon/util.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-06-25 20:18:33.749536 traceon-0.3.0/traceon.egg-info/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3838 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/PKG-INFO
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)      497 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/SOURCES.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)        1 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/dependency_links.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       53 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/requires.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)        8 2023-06-25 20:18:33.000000 traceon-0.3.0/traceon.egg-info/top_level.txt
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-07-09 09:02:15.743025 traceon-0.3.1/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    34524 2023-03-21 09:42:58.000000 traceon-0.3.1/LICENSE.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       27 2023-04-09 12:34:12.000000 traceon-0.3.1/MANIFEST.in
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     4288 2023-07-09 09:02:15.743025 traceon-0.3.1/PKG-INFO
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3006 2023-06-25 21:01:58.000000 traceon-0.3.1/README.md
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       38 2023-07-09 09:02:15.743025 traceon-0.3.1/setup.cfg
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     1818 2023-07-09 09:00:39.000000 traceon-0.3.1/setup.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-07-09 09:02:15.739025 traceon-0.3.1/traceon/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2876 2023-06-03 11:00:26.000000 traceon-0.3.1/traceon/__init__.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-07-09 09:02:15.743025 traceon-0.3.1/traceon/backend/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    19778 2023-07-09 08:54:38.000000 traceon-0.3.1/traceon/backend/__init__.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    47249 2023-07-01 19:55:22.000000 traceon-0.3.1/traceon/backend/traceon-backend.c
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-07-09 09:02:15.743025 traceon-0.3.1/traceon/data/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)  1023104 2023-04-09 12:34:12.000000 traceon-0.3.1/traceon/data/radial-series-3D-theta-dependent-coefficients.npy
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8128 2023-04-09 12:34:12.000000 traceon-0.3.1/traceon/data/radial-series-3D-thetas.npy
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     9224 2023-06-25 19:56:56.000000 traceon-0.3.1/traceon/excitation.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     1045 2023-07-08 06:45:02.000000 traceon-0.3.1/traceon/focus.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    18756 2023-07-01 19:28:25.000000 traceon-0.3.1/traceon/geometry.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8473 2023-07-09 08:54:28.000000 traceon-0.3.1/traceon/plotting.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    27672 2023-07-01 19:28:25.000000 traceon-0.3.1/traceon/solver.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    11829 2023-06-25 19:49:23.000000 traceon-0.3.1/traceon/tracing.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2204 2023-05-20 08:55:03.000000 traceon-0.3.1/traceon/util.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-07-09 09:02:15.739025 traceon-0.3.1/traceon.egg-info/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     4288 2023-07-09 09:02:15.000000 traceon-0.3.1/traceon.egg-info/PKG-INFO
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)      514 2023-07-09 09:02:15.000000 traceon-0.3.1/traceon.egg-info/SOURCES.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)        1 2023-07-09 09:02:15.000000 traceon-0.3.1/traceon.egg-info/dependency_links.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       53 2023-07-09 09:02:15.000000 traceon-0.3.1/traceon.egg-info/requires.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)        8 2023-07-09 09:02:15.000000 traceon-0.3.1/traceon.egg-info/top_level.txt
```

### Comparing `traceon-0.3.0/LICENSE.txt` & `traceon-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `traceon-0.3.0/PKG-INFO` & `traceon-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceon
-Version: 0.3.0
+Version: 0.3.1
 Summary: Solver and tracer for electrostatic problems
 Home-page: https://github.com/leon-vv/Traceon
 Author: Léon van Velzen
 Author-email: leonvanvelzen@protonmail.com
 License: AGPLv3
 Project-URL: Documentation, https://leon.science/traceon
 Project-URL: Code, https://github.com/leon-vv/traceon
@@ -22,15 +22,16 @@
         [API documentation](https://leon.science/traceon/index.html)
         
         ## Citation
         
         Please cite the software as follows:
         
         ```
-        L.B. van Velzen. Traceon software (version 0.2.0). 2023. https://doi.org/10.5281/zenodo.7812232
+        L.B. van Velzen. Traceon software (version 0.3.0). 2023. https://doi.org/10.5281/zenodo.8079985
+        
         ```
         
         ## Installation
         
         Install using the Python package manager:
         ```
         pip install traceon
@@ -62,14 +63,22 @@
         
         ## Gallery
         
         ![Image of 3D deflector](https://raw.githubusercontent.com/leon-vv/traceon/main/images/deflector-image.png)
         
         ## Features
         
+        v0.3.0:
+        - Use adaptive integration using GNU Scientific Library (GSL)
+        - Add support for boundary constraint
+        - Use [Vedo](https://vedo.embl.es/) for better plotting capabilities
+        - Use higher order triangle elements for 3D (curved triangles)
+        - Precompute jacobians/positions for better performance
+        - First implementation of element splitting based on charges (work in progress)
+        
         v0.2.0:
         - Use higher order charge distribution on line elements in radial symmetry
         - Use higher order line elements (polynomials) in radial symmetry
         - Better integration techniques, especially with regards to the logarithmic singularities
         
         v0.1.0:
         - Uses the powerful [GMSH library](https://gmsh.info/) for meshing
```

### Comparing `traceon-0.3.0/README.md` & `traceon-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 [API documentation](https://leon.science/traceon/index.html)
 
 ## Citation
 
 Please cite the software as follows:
 
 ```
-L.B. van Velzen. Traceon software (version 0.2.0). 2023. https://doi.org/10.5281/zenodo.7812232
+L.B. van Velzen. Traceon software (version 0.3.0). 2023. https://doi.org/10.5281/zenodo.8079985
+
 ```
 
 ## Installation
 
 Install using the Python package manager:
 ```
 pip install traceon
@@ -51,14 +52,22 @@
 
 ## Gallery
 
 ![Image of 3D deflector](https://raw.githubusercontent.com/leon-vv/traceon/main/images/deflector-image.png)
 
 ## Features
 
+v0.3.0:
+- Use adaptive integration using GNU Scientific Library (GSL)
+- Add support for boundary constraint
+- Use [Vedo](https://vedo.embl.es/) for better plotting capabilities
+- Use higher order triangle elements for 3D (curved triangles)
+- Precompute jacobians/positions for better performance
+- First implementation of element splitting based on charges (work in progress)
+
 v0.2.0:
 - Use higher order charge distribution on line elements in radial symmetry
 - Use higher order line elements (polynomials) in radial symmetry
 - Better integration techniques, especially with regards to the logarithmic singularities
 
 v0.1.0:
 - Uses the powerful [GMSH library](https://gmsh.info/) for meshing
```

### Comparing `traceon-0.3.0/setup.py` & `traceon-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     name='traceon.backend.traceon_backend',
     sources=['traceon/backend/traceon-backend.c'],
     extra_objects=extra_objects,
     **compiler_kwargs)
 
 setup(
     name='traceon',
-    version='0.3.0',
+    version='0.3.1',
     description='Solver and tracer for electrostatic problems',
     url='https://github.com/leon-vv/Traceon',
     author='Léon van Velzen',
     author_email='leonvanvelzen@protonmail.com',
     keywords=['boundary element method', 'BEM', 'electrostatic', 'electromagnetic', 'electron microscope', 'electron', 'tracing', 'particle', 'tracer', 'electron optics'],
     license='AGPLv3',
     ext_modules=[backend_extension],
```

### Comparing `traceon-0.3.0/traceon/__init__.py` & `traceon-0.3.1/traceon/__init__.py`

 * *Files identical despite different names*

### Comparing `traceon-0.3.0/traceon/backend/__init__.py` & `traceon-0.3.1/traceon/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     'ellipkm1' : (dbl, dbl),
     'ellipk' : (dbl, dbl),
     'ellipem1' : (dbl, dbl),
     'ellipe': (dbl, dbl),
     'normal_2d': (None, v2, v2, v2),
     'higher_order_normal_radial': (None, dbl, v2, v2, v2, v2, v2),
     'normal_3d': (None, v3, v3, v3, v3),
+    'higher_order_normal_3d': (None, dbl, dbl, arr(shape=(6,3)), v3),
     'position_and_jacobian_3d': (None, dbl, dbl, arr(ndim=2), v3, dbl_p),
     'position_and_jacobian_radial': (None, dbl, v2, v2, v2, v2, v2, dbl_p),
     'trace_particle': (sz, times_block, tracing_block, field_fun, bounds, dbl, vp),
     'potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
     'dr1_potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
     'dz1_potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
     'axial_derivatives_radial_ring': (None, arr(ndim=2), charges_2d, jac_buffer_2d, pos_buffer_2d, sz, z_values, sz),
@@ -159,14 +160,21 @@
     return normal
     
 def normal_2d(p1, p2):
     normal = np.zeros( (2,) )
     backend_lib.normal_2d(p1, p2, normal)
     return normal
 
+def higher_order_normal_3d(alpha, beta, vertices):
+    assert vertices.shape == (6,3)
+    normal = np.zeros(3)
+    backend_lib.higher_order_normal_3d(alpha, beta, vertices, normal)
+    assert np.isclose(np.linalg.norm(normal), 1.0)
+    return normal
+ 
 # Remove the last argument, which is usually a void pointer to optional data
 # passed to the function. In Python we don't need this functionality
 # as we can simply use closures.
 def remove_arg(fun):
     return lambda *args: fun(*args[:-1])
 
 def normal_3d(p1, p2, p3):
```

### Comparing `traceon-0.3.0/traceon/backend/traceon-backend.c` & `traceon-0.3.1/traceon/backend/traceon-backend.c`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #include <assert.h>
 #include <math.h>
 #include <stdlib.h>
 #include <stdint.h>
 #include <stdbool.h>
 
 #include <gsl/gsl_integration.h>
+#include <gsl/gsl_errno.h>
 
 #ifdef _MSC_VER
 #define EXPORT __declspec(dllexport)
 
 #include <Python.h>
 PyMODINIT_FUNC PyInit_traceon_backend(void) {
 	return NULL;
@@ -206,15 +207,14 @@
 	double dy = (2*alpha*(9*v4y-9*v3y-9*v2y+9*v1y)+3*a2*(9*v4y-27*v3y+27*v2y-9*v1y)-v4y+27*v3y-27*v2y+v1y)/16;
 
 	double zero[2] = {0., 0.};
 	double vec[2] = {dx, dy};
 	normal_2d(zero, vec, normal);
 }
 
-
 INLINE void position_and_jacobian_radial(double alpha, double *v1, double *v2, double *v3, double *v4, double *pos_out, double *jac) {
 
 	double v1x = v1[0], v1y = v1[1];
 	double v2x = v2[0], v2y = v2[1];
 	double v3x = v3[0], v3y = v3[1];
 	double v4x = v4[0], v4y = v4[1];
 		
@@ -251,14 +251,31 @@
 	double length = norm_3d(normal_x, normal_y, normal_z);
 	
 	normal[0] = normal_x/length;
 	normal[1] = normal_y/length;
 	normal[2] = normal_z/length;
 }
 
+INLINE void higher_order_normal_3d(double alpha, double beta, triangle6 triangle, double normal[3]) {
+	double v0x = triangle[0][0], v0y = triangle[0][1], v0z = triangle[0][2];
+	double v1x = triangle[1][0], v1y = triangle[1][1], v1z = triangle[1][2];
+	double v2x = triangle[2][0], v2y = triangle[2][1], v2z = triangle[2][2];
+	double v3x = triangle[3][0], v3y = triangle[3][1], v3z = triangle[3][2];
+	double v4x = triangle[4][0], v4y = triangle[4][1], v4z = triangle[4][2];
+	double v5x = triangle[5][0], v5y = triangle[5][1], v5z = triangle[5][2];
+
+	double a=alpha, b=beta;
+	
+	double da[3] = {-4*b*v5x+4*b*v4x+(-4*b-8*a+4)*v3x+(4*a-1)*v1x+(4*b+4*a-3)*v0x,-4*b*v5y+4*b*v4y+(-4*b-8*a+4)*v3y+(4*a-1)*v1y+(4*b+4*a-3)*v0y,-4*b*v5z+4*b*v4z+(-4*b-8*a+4)*v3z+(4*a-1)*v1z+(4*b+4*a-3)*v0z};
+	double db[3] = {(-8*b-4*a+4)*v5x+4*a*v4x-4*a*v3x+(4*b-1)*v2x+(4*b+4*a-3)*v0x,(-8*b-4*a+4)*v5y+4*a*v4y-4*a*v3y+(4*b-1)*v2y+(4*b+4*a-3)*v0y,(-8*b-4*a+4)*v5z+4*a*v4z-4*a*v3z+(4*b-1)*v2z+(4*b+4*a-3)*v0z};
+	
+	double zero[3] = {0, 0, 0};
+	normal_3d(zero, da, db, normal);
+}
+
 INLINE void barycentric_coefficients_higher_order_triangle_3d(double alpha, double beta,
 	double v0, double v1, double v2, double v3, double v4, double v5, double coeffs[6]) {
     coeffs[0] = v0;
 	coeffs[1] = 4*v3-v1-3*v0;
 	coeffs[2] = 4*v5-v2-3*v0;
 	coeffs[3] = -4*v3+2*v1+2*v0;
 	coeffs[4] = -4*v5+4*v4-4*v3+4*v0;
@@ -363,16 +380,16 @@
 	args->beta = eta;
 			
     gsl_function F;
     F.function = &triangle_integral_alpha;
 	F.params = args;
 		
     double result, error;
-    gsl_integration_qags(&F, 0, 1, 0, 1e-5, ADAPTIVE_MAX_ITERATION, args->inner_workspace, &result, &error);
-		
+    gsl_integration_qags(&F, 0, 1, 0, 1e-8, ADAPTIVE_MAX_ITERATION, args->inner_workspace, &result, &error);
+			
 	return Jeta*result;
 }
 
 double
 triangle_integral_adaptive(double target[3], triangle6 vertices, integration_cb_3d function, void *args) {
 	// TODO: optimize this, put outside the loop over the matrix diagonal
 	gsl_integration_workspace * w = gsl_integration_workspace_alloc(ADAPTIVE_MAX_ITERATION);
@@ -387,15 +404,15 @@
 	};
 		
     gsl_function F;
     F.function = &triangle_integral_beta;
 	F.params = &integration_args;
 		
     double result, error;
-    gsl_integration_qags(&F, 0, 1, 0, 1e-5, ADAPTIVE_MAX_ITERATION, w, &result, &error);
+    gsl_integration_qags(&F, 0, 1, 0, 1e-7, ADAPTIVE_MAX_ITERATION, w, &result, &error);
 	
     gsl_integration_workspace_free(w);
     gsl_integration_workspace_free(w_inner);
 		
 	return result;
 }
 
@@ -797,16 +814,16 @@
 EXPORT double dz1_potential_3d_point(double x0, double y0, double z0, double x, double y, double z, void *_) {
 	double r = norm_3d(x-x0, y-y0, z-z0);
     return (z-z0)/(4*pow(r, 3));
 }
 
 EXPORT void
 axial_coefficients_3d(double *restrict charges,
-	jacobian_buffer_3d jacobian_buffer,
-	position_buffer_3d position_buffer,
+	jacobian_buffer_3d restrict jacobian_buffer,
+	position_buffer_3d restrict position_buffer,
 	size_t N_v,
 	double *restrict zs, double *restrict output_coeffs_p, size_t N_z,
 	double *restrict thetas, double *restrict theta_coeffs_p, size_t N_t) {
 		
 	double (*theta_coeffs)[NU_MAX][M_MAX][4] = (double (*)[NU_MAX][M_MAX][4]) theta_coeffs_p;
 	double (*output_coeffs)[2][NU_MAX][M_MAX] = (double (*)[2][NU_MAX][M_MAX]) output_coeffs_p;
 	
@@ -818,29 +835,29 @@
 		
 		UNROLL
 		for (int k=0; k < N_TRIANGLE_QUAD; k++) {
 			double x = position_buffer[h][k][0];
 			double y = position_buffer[h][k][1];
 			double z = position_buffer[h][k][2];
 			
-			double r = norm_3d(x, y, z-zs[i]);
+			double r = 1/norm_3d(x, y, z-zs[i]);
 			double theta = atan2((z-zs[i]), norm_2d(x, y));
 			double mu = atan2(y, x);
 
 			int index = (int) ((theta-theta0)/dtheta);
 
 			double t = theta-thetas[index];
 			double (*C)[M_MAX][4] = &theta_coeffs[index][0];
 				
 			UNROLL
 			for (int nu=0; nu < NU_MAX; nu++)
 			UNROLL
 			for (int m=0; m < M_MAX; m++) {
 				double base = pow(t, 3)*C[nu][m][0] + pow(t, 2)*C[nu][m][1] + t*C[nu][m][2] + C[nu][m][3];
-				double r_dependence = pow(r, -2*nu - m - 1);
+				double r_dependence = pow(r, 2*nu + m + 1);
 					
 				double jac = jacobian_buffer[h][k];
 				
 				output_coeffs[i][0][nu][m] += charges[h]*jac*base*cos(m*mu)*r_dependence;
 				output_coeffs[i][1][nu][m] += charges[h]*jac*base*sin(m*mu)*r_dependence;
 			}
 		}
@@ -1128,15 +1145,15 @@
 			
 		gsl_function F;
 		F.function = &self_voltage_radial;
 		F.params = &integration_args;
 			
 		double result, error;
 		double singular_points[3] = {-1, 0, 1};
-		gsl_integration_qagp(&F, singular_points, 3, 1e-9, 5e-5, ADAPTIVE_MAX_ITERATION, w, &result, &error);
+		gsl_integration_qagp(&F, singular_points, 3, 1e-9, 1e-9, ADAPTIVE_MAX_ITERATION, w, &result, &error);
 
 		if(type_ == DIELECTRIC) {
 			matrix[N_matrix*i + i] = result - 1;
 		}
 		else {
 			matrix[N_matrix*i + i] = result;
 		}
@@ -1177,14 +1194,15 @@
 						jacobian_buffer_2d jacobian_buffer,
 						position_buffer_2d pos_buffer,
 						size_t N_lines,
 						size_t N_matrix,
                         int lines_range_start, 
                         int lines_range_end) {
     
+	gsl_set_error_handler_off();
 	assert(lines_range_start < N_lines && lines_range_end < N_lines);
 	assert(N_matrix >= N_lines);
 		
     for (int i = lines_range_start; i <= lines_range_end; i++) {
 		
 		double *target_v1 = &line_points[i][0][0];
 		double *target_v2 = &line_points[i][2][0];
@@ -1322,15 +1340,16 @@
                     double *excitation_values, 
 					jacobian_buffer_3d jacobian_buffer,
 					position_buffer_3d pos_buffer,
 					size_t N_lines,
 					size_t N_matrix,
                     int lines_range_start, 
                     int lines_range_end) {
-		
+	
+	gsl_set_error_handler_off();
 	assert(lines_range_start < N_lines && lines_range_end < N_lines);
 		
     for (int i = lines_range_start; i <= lines_range_end; i++) {
 		// TODO: higher order
 		double target[3], jac;
 		position_and_jacobian_3d(1/3., 1/3., &triangle_points[i][0], target, &jac);
 			
@@ -1345,24 +1364,21 @@
 					double *pos = pos_buffer[j][k];
 					double jac = jacobian_buffer[j][k];
 					matrix[i*N_matrix + j] += jac * potential_3d_point(target[0], target[1], target[2], pos[0], pos[1], pos[2], NULL);
 				}
             }
         } 
 		else if (type_ == DIELECTRIC) {  
-			double *p1 = &triangle_points[i][0][0];  
-			double *p2 = &triangle_points[i][1][0];  
-			double *p3 = &triangle_points[i][2][0];  
-
+			
 			double normal[3];  
-			normal_3d(p1, p2, p3, normal);  
+			higher_order_normal_3d(1/3., 1/3., &triangle_points[i][0], normal);
 			double K = excitation_values[i];  
-
+			
 			double factor = (2*K - 2) / (M_PI*(1 + K));  
-
+			
 			for (int j = 0; j < N_lines; j++) {  
 					
 				UNROLL  
 				for(int k = 0; k < N_TRIANGLE_QUAD; k++) {  
 					double *pos = pos_buffer[j][k];  
 					double jac = jacobian_buffer[j][k];
```

### Comparing `traceon-0.3.0/traceon/data/radial-series-3D-theta-dependent-coefficients.npy` & `traceon-0.3.1/traceon/data/radial-series-3D-theta-dependent-coefficients.npy`

 * *Files identical despite different names*

### Comparing `traceon-0.3.0/traceon/data/radial-series-3D-thetas.npy` & `traceon-0.3.1/traceon/data/radial-series-3D-thetas.npy`

 * *Files identical despite different names*

### Comparing `traceon-0.3.0/traceon/excitation.py` & `traceon-0.3.1/traceon/excitation.py`

 * *Files identical despite different names*

### Comparing `traceon-0.3.0/traceon/geometry.py` & `traceon-0.3.1/traceon/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,25 +423,25 @@
         thickness : float
             Add the given amount of space between the previous and next electrode.
 
         """
         self._current_z += thickness
     
     def _add_boundary(self):
-        points = [[0.0, self.z0],
-                  [self.rmax+self.margin_right, self.z0],
+        points = [[0.0, self._current_z+self.margin],
                   [self.rmax+self.margin_right, self._current_z+self.margin],
-                  [0.0, self._current_z+self.margin]]
+                  [self.rmax+self.margin_right, self.z0],
+                  [0.0, self.z0]]
         
         self._add_lines_from_points(points, 'boundary')
         self._current_z += self.margin
      
     def _add_lines_from_points(self, points, name):
         if self.symmetry == Symmetry.THREE_D:
-            points = [self.add_point([p[0], 0.0, p[1]]) for p in points]
+            points = [self.add_point([p[0], 0.0, p[1]]) for p in points[::-1]]
         else:
             points = [self.add_point(p) for p in points]
         
         Np = len(points)
         lines = [self.add_line(points[i], points[j]) for i, j in zip(range(0,Np-1), range(1,Np))]
          
         if self.symmetry == Symmetry.THREE_D:
```

### Comparing `traceon-0.3.0/traceon/plotting.py` & `traceon-0.3.1/traceon/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,25 +91,31 @@
 def plot_triangle_mesh(mesh, show_legend=True, show_normals=False, **colors):
     
     dict_ = _create_point_to_physical_dict(mesh)
     triangles = mesh.elements
      
     triangles_to_plot = []
     colors_ = []
+    
+    normal_coordinates = [(1/6, 1/6), (1/2-1/6, 1/2-1/6), (1/2-1/6, 1/6), (1/6, 1/2-1/6)]
+    normals = []
      
     for (v0, v1, v2, v3, v4, v5) in triangles:
-        for A, B, C in [(v0, v3, v5), (v3, v4, v5), (v3, v1, v4), (v5, v4, v2)]:
+        for i, (A, B, C) in enumerate([(v0, v3, v5), (v3, v4, v5), (v3, v1, v4), (v5, v4, v2)]):
             color = '#CCCCC'
             
             if A in dict_ and B in dict_ and C in dict_:
                 phys1, phys2, phys3 = dict_[A], dict_[B], dict_[C]
                 if phys1 == phys2 and phys2 == phys3 and phys1 in colors:
                     color = colors[phys1]
             
             triangles_to_plot.append( [A, B, C] )
+
+            alpha, beta = normal_coordinates[i]
+            normals.append(backend.higher_order_normal_3d(alpha, beta, mesh.points[[v0, v1, v2, v3, v4, v5]]))
             colors_.append(color)
      
     colors_, triangles_to_plot = np.array(colors_), np.array(triangles_to_plot)
     plotter = vedo.Plotter()
     meshes = []
     
     for c in set(colors_):
@@ -162,27 +168,27 @@
      
     start = []
     end = []
     colors_ = []
     normals = []
     
     for (P1, P2, P3, P4) in lines:
-        for A, B in [(P1, P3), (P3, P4), (P4, P2)]:
+        for i, (A, B) in enumerate([(P1, P3), (P3, P4), (P4, P2)]):
             color = '#CCCCC'
 
             if A in dict_ and B in dict_:
                 phys1, phys2 = dict_[A], dict_[B]
                 if phys1 == phys2 and phys1 in colors:
                     color = colors[phys1]
             
             p1, p2 = mesh.points[A], mesh.points[B]
             start.append(p1)
             end.append(p2)
-            normals.append(backend.higher_order_normal_radial(0.0, mesh.points[np.array([P1, P2, P3, P4])]))
             colors_.append(color)
+            normals.append(backend.higher_order_normal_radial(-2/3 + i*2/3, mesh.points[np.array([P1, P2, P3, P4])]))
     
     start, end = np.array(start), np.array(end)
     colors_ = np.array(colors_)
     plotter = vedo.Plotter()
     lines = []
      
     for c in set(colors_):
```

### Comparing `traceon-0.3.0/traceon/solver.py` & `traceon-0.3.1/traceon/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,19 +82,19 @@
     N_lines = len(vertices)
     N_matrix = N_lines + N_floating # Every floating conductor adds one constraint
 
     F = np.zeros( (N_matrix) )
      
     for name, indices in names.items():
         type_, value  = excitation.excitation_types[name]
-        
+         
         if type_ == E.ExcitationType.VOLTAGE_FIXED:
             F[indices] = value
         elif type_ == E.ExcitationType.VOLTAGE_FUN:
-            positions = [backend.position_and_jacobian_radial(0.5, vertices[i, 0], vertices[i, 2], vertices[i, 3], vertices[i, 1])[1] for i in indices]
+            positions = [backend.position_and_jacobian_radial(0, vertices[i, 0], vertices[i, 2], vertices[i, 3], vertices[i, 1])[1] for i in indices]
             F[indices] = [value(*p) for p in positions]
         elif type_ == E.ExcitationType.DIELECTRIC or \
                 type_ == E.ExcitationType.FLOATING_CONDUCTOR:
             F[indices] = 0
     
     # See comments in _add_floating_conductor_constraints_to_matrix
     for i, f in enumerate(floating_names):
```

### Comparing `traceon-0.3.0/traceon/tracing.py` & `traceon-0.3.1/traceon/tracing.py`

 * *Files identical despite different names*

### Comparing `traceon-0.3.0/traceon/util.py` & `traceon-0.3.1/traceon/util.py`

 * *Files identical despite different names*

### Comparing `traceon-0.3.0/traceon.egg-info/PKG-INFO` & `traceon-0.3.1/traceon.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceon
-Version: 0.3.0
+Version: 0.3.1
 Summary: Solver and tracer for electrostatic problems
 Home-page: https://github.com/leon-vv/Traceon
 Author: Léon van Velzen
 Author-email: leonvanvelzen@protonmail.com
 License: AGPLv3
 Project-URL: Documentation, https://leon.science/traceon
 Project-URL: Code, https://github.com/leon-vv/traceon
@@ -22,15 +22,16 @@
         [API documentation](https://leon.science/traceon/index.html)
         
         ## Citation
         
         Please cite the software as follows:
         
         ```
-        L.B. van Velzen. Traceon software (version 0.2.0). 2023. https://doi.org/10.5281/zenodo.7812232
+        L.B. van Velzen. Traceon software (version 0.3.0). 2023. https://doi.org/10.5281/zenodo.8079985
+        
         ```
         
         ## Installation
         
         Install using the Python package manager:
         ```
         pip install traceon
@@ -62,14 +63,22 @@
         
         ## Gallery
         
         ![Image of 3D deflector](https://raw.githubusercontent.com/leon-vv/traceon/main/images/deflector-image.png)
         
         ## Features
         
+        v0.3.0:
+        - Use adaptive integration using GNU Scientific Library (GSL)
+        - Add support for boundary constraint
+        - Use [Vedo](https://vedo.embl.es/) for better plotting capabilities
+        - Use higher order triangle elements for 3D (curved triangles)
+        - Precompute jacobians/positions for better performance
+        - First implementation of element splitting based on charges (work in progress)
+        
         v0.2.0:
         - Use higher order charge distribution on line elements in radial symmetry
         - Use higher order line elements (polynomials) in radial symmetry
         - Better integration techniques, especially with regards to the logarithmic singularities
         
         v0.1.0:
         - Uses the powerful [GMSH library](https://gmsh.info/) for meshing
```

