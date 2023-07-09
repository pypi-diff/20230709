# Comparing `tmp/RobustGaussianFittingLibrary-v0.1.8.tar.gz` & `tmp/RobustGaussianFittingLibrary-v0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RobustGaussianFittingLibrary-v0.1.8.tar", last modified: Tue Aug 18 21:30:37 2020, max compression
+gzip compressed data, was "dist/RobustGaussianFittingLibrary-v0.1.9.tar", last modified: Wed Aug 19 18:42:54 2020, max compression
```

## Comparing `RobustGaussianFittingLibrary-v0.1.8.tar` & `RobustGaussianFittingLibrary-v0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2020-08-18 21:30:37.480719 RobustGaussianFittingLibrary-v0.1.8/
--rw-rw-r--   0 ali       (1000) ali       (1000)       52 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)     1080 2020-08-18 21:30:37.480719 RobustGaussianFittingLibrary-v0.1.8/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     4947 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/README
--rw-rw-r--   0 ali       (1000) ali       (1000)     4947 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2020-08-18 21:30:37.480719 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/
--rw-rw-r--   0 ali       (1000) ali       (1000)    21065 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/RGFLib.c
--rw-rw-r--   0 ali       (1000) ali       (1000)     2503 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/RGFLib.h
--rw-rw-r--   0 ali       (1000) ali       (1000)     3076 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/RGFLib_mex_fitValue2Skewed.c
--rw-rw-r--   0 ali       (1000) ali       (1000)     1331 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/RGFLib_mex_fitValue2Skewed_Test.m
--rw-rw-r--   0 ali       (1000) ali       (1000)      475 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    27729 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/basic.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     7490 2020-08-18 21:30:30.488720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/cWrapper.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     9506 2020-08-18 21:30:30.492720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/misc.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    19491 2020-08-18 21:30:30.492720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/tests.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16553 2020-08-18 21:30:30.492720 RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/useMultiproc.py
--rw-rw-r--   0 ali       (1000) ali       (1000)       40 2020-08-18 21:30:30.492720 RobustGaussianFittingLibrary-v0.1.8/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     2677 2020-08-18 21:30:30.492720 RobustGaussianFittingLibrary-v0.1.8/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2020-08-19 18:42:54.689067 RobustGaussianFittingLibrary-v0.1.9/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       52 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1080 2020-08-19 18:42:54.689067 RobustGaussianFittingLibrary-v0.1.9/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4947 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/README
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4947 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2020-08-19 18:42:54.689067 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    21440 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/RGFLib.c
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2503 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/RGFLib.h
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3076 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/RGFLib_mex_fitValue2Skewed.c
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1331 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/RGFLib_mex_fitValue2Skewed_Test.m
+-rw-rw-r--   0 ali       (1000) ali       (1000)      475 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    27619 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/basic.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7702 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/cWrapper.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     9506 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/misc.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    20328 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/tests.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16553 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/useMultiproc.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)       40 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2677 2020-08-19 18:42:12.864737 RobustGaussianFittingLibrary-v0.1.9/setup.py
```

### Comparing `RobustGaussianFittingLibrary-v0.1.8/PKG-INFO` & `RobustGaussianFittingLibrary-v0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: RobustGaussianFittingLibrary
-Version: v0.1.8
+Version: v0.1.9
 Summary: A library for robust Gaussian fitting using geometric models in presence of outliers. 
 Home-page: https://github.com/ARSadri/RobustGaussianFittingLibrary
 Author: Alireza Sadri
 Author-email: ARSadri@domain.com
 License: MIT
-Download-URL: https://github.com/ARSadri/RobustGaussianFittingLibrary/archive/v0.1.8.tar.gz
+Download-URL: https://github.com/ARSadri/RobustGaussianFittingLibrary/archive/v0.1.9.tar.gz
 Description: UNKNOWN
 Keywords: outlier,outlier detection,outlier removal,anamoly detection,curve fitting,line fitting,plane fitting,fit a Gaussian,Gaussian fitting
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobustGaussianFittingLibrary-v0.1.8/README` & `RobustGaussianFittingLibrary-v0.1.9/README`

 * *Files identical despite different names*

### Comparing `RobustGaussianFittingLibrary-v0.1.8/README.md` & `RobustGaussianFittingLibrary-v0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/RGFLib.c` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/RGFLib.c`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,16 @@
 }
 
 void fitValue2Skewed(float *vec, float *weights, 
 					float *modelParams, float theta, unsigned int N,
 					float topkPerc, float botkPerc,
 					float MSSE_LAMBDA, unsigned char optIters) {
 
-	float tmp, estScale, theta_new, upperScale, lowerScale, errAtTopk;
+	float tmp, tmpH, tmpL, estScale, theta_new;
+	float upperScale, lowerScale, errAtTopk;
 	int i, topk, botk, iter, numPointsSide;
 		
 	topk = (int)(N*topkPerc);
 	botk = (int)(N*botkPerc);
 	
 	if(N<3)
 		return;
@@ -255,63 +256,70 @@
 	}
 	
 	float *residual;
 	residual = (float*) malloc(N * sizeof(float));
 	
 	struct sortStruct* errorVec;
 	errorVec = (struct sortStruct*) malloc(N * sizeof(struct sortStruct));
-	// lets do a symmetric fitting, half of the sample data points must come from either side
 	for(iter=0; iter<optIters; iter++) {
 		
-		for (i = 0; i < N; i++) {
-			errorVec[i].vecData = fabs(vec[i] - theta);
-			errorVec[i].indxs = i;
-		}
-		quickSort(errorVec,0,N-1);
-		errAtTopk = errorVec[topk-1].vecData;
-		
-		theta_new = 0;
-		tmp = 0;
-		numPointsSide = 0;
-		for (i = 0; i < N; i++) {
-			if((vec[i] >= theta) && (vec[i] <=  theta + errAtTopk)) {
-				errorVec[i].vecData  = vec[i] - theta;
-				numPointsSide++;
-			}
-			else {
-				errorVec[i].vecData  = 1e+9;
+		tmpH = 0;
+		tmpL = 0;
+		if(iter>=optIters/2) {
+			// lets do a symmetric fitting, half of the sample data points must come from either side
+			for (i = 0; i < N; i++) {
+				errorVec[i].vecData = fabs(vec[i] - theta);
+				errorVec[i].indxs = i;
 			}
-			errorVec[i].indxs = i;
-		}
-		if((int)(numPointsSide*topkPerc)>0) {
 			quickSort(errorVec,0,N-1);
-			for(i=(int)(numPointsSide*botkPerc); i<(int)(numPointsSide*topkPerc); i++) {
-				theta_new += weights[errorVec[i].indxs]*vec[errorVec[i].indxs];
-				tmp += weights[errorVec[i].indxs];
+			errAtTopk = errorVec[topk-1].vecData;
+
+			//////////////////////////////////////////////////////////////////
+			theta_new = 0;
+			numPointsSide = 0;
+			for (i = 0; i < N; i++) {
+				if((vec[i] >= theta) && (vec[i] <=  theta + errAtTopk)) {
+					errorVec[i].vecData  = vec[i] - theta;
+					numPointsSide++;
+				}
+				else {
+					errorVec[i].vecData  = 1e+9;
+				}
+				errorVec[i].indxs = i;
 			}
-		}		
-		numPointsSide = 0;
-		for (i = 0; i < N; i++) {
-			if((vec[i] < theta) && (vec[i] >= theta - errAtTopk) ) {
-				errorVec[i].vecData  = theta - vec[i];
-				numPointsSide++;
+			if((int)(numPointsSide*topkPerc)>0) {
+				quickSort(errorVec,0,N-1);
+				for(i=(int)(numPointsSide*botkPerc); i<(int)(numPointsSide*topkPerc); i++) {
+					theta_new += weights[errorVec[i].indxs]*vec[errorVec[i].indxs];
+					tmpH += weights[errorVec[i].indxs];
+				}
 			}
-			else {
-				errorVec[i].vecData  = 1e+9;
+			numPointsSide = 0;
+			for (i = 0; i < N; i++) {
+				if((vec[i] < theta) && (vec[i] >= theta - errAtTopk) ) {
+					errorVec[i].vecData  = theta - vec[i];
+					numPointsSide++;
+				}
+				else {
+					errorVec[i].vecData  = 1e+9;
+				}
+				errorVec[i].indxs = i;
 			}
-			errorVec[i].indxs = i;
-		}
-		if((int)(numPointsSide*topkPerc)>0) {
-			quickSort(errorVec,0,N-1);
-			for(i=(int)(numPointsSide*botkPerc); i<(int)(numPointsSide*topkPerc); i++) {
-				theta_new += weights[errorVec[i].indxs]*vec[errorVec[i].indxs];
-				tmp += weights[errorVec[i].indxs];
+			if((int)(numPointsSide*topkPerc)>0) {
+				quickSort(errorVec,0,N-1);
+				for(i=(int)(numPointsSide*botkPerc); i<(int)(numPointsSide*topkPerc); i++) {
+					theta_new += weights[errorVec[i].indxs]*vec[errorVec[i].indxs];
+					tmpL += weights[errorVec[i].indxs];
+				}
 			}
 		}
-		if(tmp==0) {
+		tmp = tmpL + tmpH;
+
+		//////////////////////////////////////////////////////////////////
+		if((tmpL==0) || (tmpH==0)) {
 			theta_new = 0;
 			tmp = 0;
 			for (i = 0; i < N; i++) {
 				errorVec[i].vecData = fabs(vec[i] - theta);
 				errorVec[i].indxs = i;
 			}
 			quickSort(errorVec,0,N-1);
@@ -729,28 +737,30 @@
 	inMask = (unsigned char*) malloc(X*Y * sizeof(unsigned char));
 			
 	for(frmCnt=0; frmCnt<N; frmCnt++) {
 		
 		for(rCnt=0; rCnt<X; rCnt++) {
 			for(cCnt=0; cCnt<Y; cCnt++) {
 				inImage[cCnt + rCnt*Y] = inImage_Tensor[cCnt + rCnt*Y + frmCnt*X*Y];
-				inMask[cCnt + rCnt*Y] = inImage_Tensor[cCnt + rCnt*Y + frmCnt*X*Y];
+				inMask[cCnt + rCnt*Y]  = inMask_Tensor[cCnt + rCnt*Y + frmCnt*X*Y];
+				modelParamsMap[cCnt + rCnt*Y + 0*X*Y] = 0;
+				modelParamsMap[cCnt + rCnt*Y + 1*X*Y] = 0;
 			}
 		}
 		
 		RSGImage(inImage, inMask, modelParamsMap,
-					winX, winY,	X, Y, 
-					topkPerc, botkPerc,
-					MSSE_LAMBDA, stretch2CornersOpt,
-					numModelParams, optIters);
+				 winX, winY, X, Y,
+				 topkPerc, botkPerc,
+				 MSSE_LAMBDA, stretch2CornersOpt,
+				 numModelParams, optIters);
 		
 		for(rCnt=0; rCnt<X; rCnt++) {
 			for(cCnt=0; cCnt<Y; cCnt++) {
 				model_mean[cCnt + rCnt*Y + frmCnt*X*Y] = modelParamsMap[cCnt + rCnt*Y + 0*X*Y];
-				model_std[cCnt + rCnt*Y + frmCnt*X*Y] = modelParamsMap[cCnt + rCnt*Y + 1*X*Y];
+				model_std[cCnt + rCnt*Y + frmCnt*X*Y]  = modelParamsMap[cCnt + rCnt*Y + 1*X*Y];
 			}
 		}
 	}		
 	free(modelParamsMap);
 	free(inImage);
 	free(inMask);
 }
```

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/RGFLib.h` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/RGFLib.h`

 * *Files identical despite different names*

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/RGFLib_mex_fitValue2Skewed.c` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/RGFLib_mex_fitValue2Skewed.c`

 * *Files identical despite different names*

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/RGFLib_mex_fitValue2Skewed_Test.m` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/RGFLib_mex_fitValue2Skewed_Test.m`

 * *Files identical despite different names*

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/basic.py` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,24 +300,26 @@
                                             topKthPerc,
                                             bottomKthPerc,
                                             MSSE_LAMBDA, 
                                             stretch2CornersOpt)
     return (modelParams)
 
 def fitBackground(inImage, 
-                inMask = None,
-                winX = None,
-                winY = None,
-                topKthPerc = 0.5,
-                bottomKthPerc = 0.45,
-                MSSE_LAMBDA = 3.0,
-                stretch2CornersOpt = 0,
-                numModelParams = 4,
-                optIters = 12):
-    """ fit a plane to the background of the image and calculate the value of the background plane and STD at the location of each pixel.
+                  inMask = None,
+                  winX = None,
+                  winY = None,
+                  topKthPerc = 0.5,
+                  bottomKthPerc = 0.45,
+                  MSSE_LAMBDA = 3.0,
+                  stretch2CornersOpt = 0,
+                  numModelParams = 4,
+                  optIters = 12,
+                  numStrides = 1):
+    """ fit a plane to the background of the image uainf convolving the window by number of strides
+        and calculate the value of the background plane and STD at the location of each pixel.
     
     Input arguments
     ~~~~~~~~~~~~~~~
         inImage: a 2D float32 numpy array as the image
         inMask: where 0 is bad and 1 is good. The masked pixels have not effect in the calculation of the parameters of the plane fit to background. However, the value of the background at their location can be found.
         winX: size of the window to fit the plane to in rows
         winY: size of the window to fit the plane to in coloumns
@@ -334,56 +336,90 @@
                     if you are not sure at all, refer to the note above this code.
                     default : 0.5
         bottomKthPerc: We'd like to make a sample out of worst inliers from data points that are
                        between bottomKthPerc and topKthPerc of sorted residuals.
                        set it to 0.9*topKthPerc, if N is number of data points, then make sure that
                        (topKthPerc - bottomKthPerc)*N>4, 
                        it is best if bottomKthPerc*N>12 then MSSE makes sense
-                       otherwise the code may return non-robust results.        
+                       otherwise the code may return non-robust results.
+        numStrides: Convolve the filter this number of times. For example, if the image is 32 by 32
+                    and winX and Y are 16 and numStrides is 1, from 0 to 15 and 15 to 31,
+                    will be analysed. But if numStrides is 2, from 0 to 15, 10 to 25 and 15 to 31
+                    will be analysed and averaged and so on ...
+
     Output
     ~~~~~~
-        2 parameters for each pixel : 2 x n_R, n_C : Rmean and RSTD.
+        numpy array with 2 parameters for each pixel : 2 x n_R, n_C : Rmean and RSTD.
     """
     
     stretch2CornersOpt = np.uint8(stretch2CornersOpt)
     if(inMask is None):
         inMask = np.ones((inImage.shape[0], inImage.shape[1]), dtype='uint8')
         
     if(winX is None):
         winX = inImage.shape[0]
     if(winY is None):
         winY = inImage.shape[1]
-    modelParamsMap = np.zeros((2, inImage.shape[0], inImage.shape[1]), dtype='float32')
 
+    n_R = inImage.shape[0]
+    n_C = inImage.shape[1]
+        
+    bckParam = np.zeros((2, n_R, n_C), dtype='float32')
     RGFCLib.RSGImage(inImage.astype('float32'),
-                                inMask,
-                                modelParamsMap,
-                                winX,
-                                winY,
-                                inImage.shape[0],
-                                inImage.shape[1],
-                                topKthPerc,
-                                bottomKthPerc,
-                                MSSE_LAMBDA,
-                                stretch2CornersOpt,
-                                numModelParams,
-                                optIters)
-    return (modelParamsMap)
+                     inMask,
+                     bckParam,
+                     winX,
+                     winY,
+                     inImage.shape[0],
+                     inImage.shape[1],
+                     topKthPerc,
+                     bottomKthPerc,
+                     MSSE_LAMBDA,
+                     stretch2CornersOpt,
+                     numModelParams,
+                     optIters)
+    
+    _sums = np.ones((2, n_R, n_C), dtype='uint8')
+    if(numStrides>1):
+        wSDListRows = np.linspace(0, winX, numStrides+2, dtype='uint8')[1:-1]
+        wSDListClms = np.linspace(0, winY, numStrides+2, dtype='uint8')[1:-1]
+        for wSDRow in wSDListRows:
+            for wSDClm in wSDListClms:
+                _inImage = inImage[wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm].copy()
+                _inMask = inMask[wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm].copy()
+                modelParamsMap = np.zeros((2, _inImage.shape[0], _inImage.shape[1]), dtype='float32')
+                RGFCLib.RSGImage(_inImage.astype('float32'),
+                                 _inMask,
+                                 modelParamsMap,
+                                 winX,
+                                 winY,
+                                 _inImage.shape[0],
+                                 _inImage.shape[1],
+                                 topKthPerc,
+                                 bottomKthPerc,
+                                 MSSE_LAMBDA,
+                                 stretch2CornersOpt,
+                                 numModelParams,
+                                 optIters)
+                bckParam[:,wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm] += modelParamsMap
+                _sums[:,wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm] += 1
+    return(bckParam / _sums)
 
 def fitBackgroundTensor(inImage_Tensor, 
-                inMask_Tensor = None,
-                winX = None,
-                winY = None,
-                topKthPerc = 0.5,
-                bottomKthPerc = 0.45,
-                MSSE_LAMBDA = 3.0,
-                stretch2CornersOpt = 0,
-                numModelParams = 4,
-                optIters = 12):
-    """ fit a plane to each image in the input Tensor and report background values and STD for each pixel for each plane
+                        inMask_Tensor = None,
+                        winX = None,
+                        winY = None,
+                        topKthPerc = 0.5,
+                        bottomKthPerc = 0.25,
+                        MSSE_LAMBDA = 3.0,
+                        stretch2CornersOpt = 0,
+                        numModelParams = 4,
+                        optIters = 12,
+                        numStrides = 1):
+    """ fit a plane by convolving the model to each image in the input Tensor and report background values and STD for each pixel for each plane
     
     Input arguments
     ~~~~~~~~~~~~~~~
         inImage_Tensor: n_F x n_R x n_C input Tensor, each image has size n_R x n_C
         inMask_Tensor: same size of inImage_Tensor
         MSSE_LAMBDA : How far (normalized by STD of the Gaussian) from the 
                         mean of the Gaussian, data is considered inlier.
@@ -393,117 +429,79 @@
                     if you are not sure at all, refer to the note above this code.
                     default : 0.5
         bottomKthPerc: We'd like to make a sample out of worst inliers from data points that are
                        between bottomKthPerc and topKthPerc of sorted residuals.
                        set it to 0.9*topKthPerc, if N is number of data points, then make sure that
                        (topKthPerc - bottomKthPerc)*N>4, 
                        it is best if bottomKthPerc*N>12 then MSSE makes sense
-                       otherwise the code may return non-robust results.        
+                       otherwise the code may return non-robust results.
+        numStrides: Convolve the filter this number of times. For example, if the image is 32 by 32
+                    and winX and Y are 16 and numStrides is 1, from 0 to 15 and 15 to 31,
+                    will be analysed. But if numStrides is 2, from 0 to 15, 10 to 25 and 15 to 31
+                    will be analysed and averaged. This means that the method will run 7 times.
     Output
     ~~~~~~
         2 x n_F x n_R x n_C where out[0] would be background mean and out[1] would be STD for each pixel in the Tensor.
     """
     
-                
     stretch2CornersOpt = np.uint8(stretch2CornersOpt)
     if(inMask_Tensor is None):
         inMask_Tensor = np.ones(inImage_Tensor.shape, dtype='uint8')
     if(winX is None):
         winX = inImage_Tensor.shape[1]
     if(winY is None):
         winY = inImage_Tensor.shape[2]
+    
+    n_F = inImage_Tensor.shape[0]
+    n_R = inImage_Tensor.shape[1]
+    n_C = inImage_Tensor.shape[2]
+        
     model_mean = np.zeros(inImage_Tensor.shape, dtype='float32')
     model_std  = np.zeros(inImage_Tensor.shape, dtype='float32')
-
     RGFCLib.RSGImage_by_Image_Tensor(inImage_Tensor.astype('float32'),
-                                                inMask_Tensor.astype('uint8'),
+                                    inMask_Tensor.astype('uint8'),
+                                    model_mean,
+                                    model_std,
+                                    winX,
+                                    winY,
+                                    inImage_Tensor.shape[0],
+                                    inImage_Tensor.shape[1],
+                                    inImage_Tensor.shape[2],
+                                    topKthPerc,
+                                    bottomKthPerc,
+                                    MSSE_LAMBDA,
+                                    stretch2CornersOpt,
+                                    numModelParams,
+                                    optIters)
+
+    bckParam = np.array([model_mean, model_std])    
+    _sums = np.ones((2, n_F, n_R, n_C), dtype='uint8')
+    if(numStrides>1):
+        wSDListRows = np.linspace(0, winX, numStrides+2, dtype='uint8')[1:-1]
+        wSDListClms = np.linspace(0, winY, numStrides+2, dtype='uint8')[1:-1]
+        for wSDRow in wSDListRows:
+            for wSDClm in wSDListClms:
+                _inImage_Tensor = inImage_Tensor[:, wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm].copy()
+                _inMask_Tensor = inMask_Tensor[:, wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm].copy()
+    
+                model_mean = np.zeros(_inImage_Tensor.shape, dtype='float32')
+                model_std  = np.zeros(_inImage_Tensor.shape, dtype='float32')
+            
+                RGFCLib.RSGImage_by_Image_Tensor(_inImage_Tensor.astype('float32'),
+                                                _inMask_Tensor.astype('uint8'),
                                                 model_mean,
                                                 model_std,
                                                 winX,
                                                 winY,
-                                                inImage_Tensor.shape[0],
-                                                inImage_Tensor.shape[1],
-                                                inImage_Tensor.shape[2],
+                                                _inImage_Tensor.shape[0],
+                                                _inImage_Tensor.shape[1],
+                                                _inImage_Tensor.shape[2],
                                                 topKthPerc,
                                                 bottomKthPerc,
                                                 MSSE_LAMBDA,
                                                 stretch2CornersOpt,
                                                 numModelParams,
                                                 optIters)
     
-    return ( np.array([model_mean, model_std]))
-
-def fitBackgroundTensorConv(inImage_Tensor, 
-                            inMask_Tensor = None,
-                            winX = None,
-                            winY = None,
-                            topKthPerc = 0.5,
-                            bottomKthPerc = 0.45,
-                            MSSE_LAMBDA = 3.0,
-                            stretch2CornersOpt = 0,
-                            numModelParams = 4,
-                            optIters = 12,
-                            numStrides = 1):
-    """ fit a plane by convolving the model to each image in the input Tensor and report background values and STD for each pixel for each plane
-    
-    Input arguments
-    ~~~~~~~~~~~~~~~
-        inImage_Tensor: n_F x n_R x n_C input Tensor, each image has size n_R x n_C
-        inMask_Tensor: same size of inImage_Tensor
-        MSSE_LAMBDA : How far (normalized by STD of the Gaussian) from the 
-                        mean of the Gaussian, data is considered inlier.
-                        default: 3.0
-        topKthPerc: A rough but certain guess of portion of inliers, between 0 and 1, e.g. 0.5. 
-                    Choose the topKthPerc to be as high as you are sure the portion of data is inlier.
-                    if you are not sure at all, refer to the note above this code.
-                    default : 0.5
-        bottomKthPerc: We'd like to make a sample out of worst inliers from data points that are
-                       between bottomKthPerc and topKthPerc of sorted residuals.
-                       set it to 0.9*topKthPerc, if N is number of data points, then make sure that
-                       (topKthPerc - bottomKthPerc)*N>4, 
-                       it is best if bottomKthPerc*N>12 then MSSE makes sense
-                       otherwise the code may return non-robust results.
-        numStrides: Convolve the filter this number of times. For example, if the image is 32 by 32
-                    and winX and Y are 16 and numStrides is 1, from 0 to 15 and 15 to 31,
-                    will be analysed. But if numStrides is 2, from 0 to 15, 10 to 25 and 15 to 31
-                    will be analysed and averaged. This means that the method will run 7 times.
-    Output
-    ~~~~~~
-        2 x n_F x n_R x n_C where out[0] would be background mean and out[1] would be STD for each pixel in the Tensor.
-    """
-    
-    stretch2CornersOpt = np.uint8(stretch2CornersOpt)
-    if(inMask_Tensor is None):
-        inMask_Tensor = np.ones(inImage_Tensor.shape, dtype='uint8')
-    if(winX is None):
-        winX = inImage_Tensor.shape[1]
-    if(winY is None):
-        winY = inImage_Tensor.shape[2]
-    model_mean = np.zeros(inImage_Tensor.shape, dtype='float32')
-    model_std  = np.zeros(inImage_Tensor.shape, dtype='float32')
-    
-    n_F = inImage_Tensor.shape[0]
-    n_R = inImage_Tensor.shape[1]
-    n_C = inImage_Tensor.shape[2]
-        
-    bckParam = np.zeros((2, n_F, n_R, n_C), dtype='float32')
-    bckParam += fitBckTM(inImage_Tensor, winX=winX, winY=winY, showProgress=True)
-    _sums = np.ones((2, n_F, n_R, n_C), dtype='uint8')
-    wSDListRows = np.linspace(0, winX, numStrides+2, dtype='uint8')[1:-1]
-    wSDListClms = np.linspace(0, winY, numStrides+2, dtype='uint8')[1:-1]
-    for wSDRow in wSDListRows:
-        for wSDClm in wSDListClms:
-            _data = inImage_Tensor[:, wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm]
-            _inMask = inMask_Tensor[:, wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm]
-            _bck = fitBackgroundTensorConv(_data, 
-                                           _inMask,
-                                           winX,
-                                           winY,
-                                           topKthPerc,
-                                           bottomKthPerc,
-                                           MSSE_LAMBDA,
-                                           stretch2CornersOpt,
-                                           numModelParams,
-                                           optIters)
-            bckParam[:,:,wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm] += _bck
-            _sums[:,:,wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm] += 1
+                bckParam[:,:,wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm] += np.array([model_mean, model_std])
+                _sums[:,:,wSDRow:n_R-winX+wSDRow ,wSDClm:n_C-winY+wSDClm] += 1
     return(bckParam / _sums)
```

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/cWrapper.py` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/cWrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 import ctypes
 import os
 import fnmatch
 
 dir_path = os.path.dirname(os.path.realpath(__file__)) + os.path.sep + '..' + os.path.sep
 fileNameTemplate = 'RGFLib*.so'
 flist = fnmatch.filter(os.listdir(dir_path + os.path.sep), fileNameTemplate)
+if(len(flist)==0):	#for those who use make
+	dir_path = os.path.dirname(os.path.realpath(__file__))
+	fileNameTemplate = 'RGFLib*.so'
+	flist = fnmatch.filter(os.listdir(dir_path + os.path.sep), fileNameTemplate)
+	
 RGFCLib = ctypes.cdll.LoadLibrary(dir_path + os.path.sep + flist[0])
 
 '''
 void islandRemoval(unsigned char* inMask, unsigned char* outMask, 
 					  unsigned int X, unsigned int Y, 
 					  unsigned int islandSizeThreshold)
 '''
```

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/misc.py` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/misc.py`

 * *Files identical despite different names*

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/tests.py` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import RobustGaussianFittingLibrary.misc
 
 import numpy as np
 import time
 import matplotlib.pyplot as plt
 import os
 import scipy.stats
+from cProfile import label
 np.set_printoptions(suppress = True)
 np.set_printoptions(precision = 2)
  
 LWidth = 3
 font = {
         'weight' : 'bold',
         'size'   : 8}
@@ -230,17 +231,26 @@
     winYL = 200
     winYU = 300
     im0 = axes[0].imshow(inImage*inMask, vmin=0, vmax=1000)
     axes[0].set_xlim([winXL, winXU])
     axes[0].set_ylim([winYL, winYU])
     fig.colorbar(im0, ax=axes[0], shrink =0.5)
 
-    mP = RobustGaussianFittingLibrary.fitBackground(inImage, inMask, winX = 64, winY = 64, stretch2CornersOpt=4, numModelParams = 4) \
-        + RobustGaussianFittingLibrary.fitBackground(inImage, inMask, winX = 32, winY = 32, stretch2CornersOpt=2, numModelParams = 4) \
-        + RobustGaussianFittingLibrary.fitBackground(inImage, inMask, winX = 16, winY = 16, stretch2CornersOpt=1, numModelParams = 4)
+    mP = RobustGaussianFittingLibrary.fitBackground(inImage, inMask, 
+                                                    winX = 64, 
+                                                    winY = 64, 
+                                                    numStrides=2) \
+        + RobustGaussianFittingLibrary.fitBackground(inImage, inMask, 
+                                                    winX = 32, 
+                                                    winY = 32, 
+                                                    numStrides=2) \
+        + RobustGaussianFittingLibrary.fitBackground(inImage, inMask, 
+                                                    winX = 16, 
+                                                    winY = 16, 
+                                                    numStrides=2)
     mP = mP/3
     
     im1 = axes[1].imshow(inMask*mP[0], vmin=0, vmax=1000)
     axes[1].set_xlim([winXL, winXU])
     axes[1].set_ylim([winYL, winYU])
     fig.colorbar(im1, ax=axes[1], shrink = 0.5)
     im2 = axes[2].imshow(inMask*(inImage - mP[0])/mP[1])
@@ -253,32 +263,43 @@
 def test_fitBackgroundTensor():
     print('test_fitBackgroundTensor')
     imgDimX = 100
     imgDimY = 100
     Xax = np.arange(imgDimX)
     Yax = np.arange(imgDimY)
     inX, inY = np.meshgrid(Xax, Yax)
-    img1 = np.random.randn(1, imgDimX,imgDimY)
+    img1 = 0+1*np.random.randn(1, imgDimX,imgDimY)
     mP = RobustGaussianFittingLibrary.fitPlane(inX = inX.flatten(), 
-                                       inY = inY.flatten(),
-                                       inZ = img1.flatten())
+                                               inY = inY.flatten(),
+                                               inZ = img1.flatten())
     print(mP)
-    img2 = 10+np.random.randn(1, imgDimX,imgDimY)
+
+    mP = RobustGaussianFittingLibrary.fitBackground(np.squeeze(img1))
+    print(mP)
+    
+    img2 = 3+1*np.random.randn(1, imgDimX,imgDimY)
     mP = RobustGaussianFittingLibrary.fitPlane(inX = inX.flatten(), 
-                                       inY = inY.flatten(),
-                                       inZ = img2.flatten())
+                                               inY = inY.flatten(),
+                                               inZ = img2.flatten())
     print(mP)
+    mP = RobustGaussianFittingLibrary.fitBackground(np.squeeze(img2))
+    print(mP)
+
     img3 = 100+10*np.random.randn(1, imgDimX,imgDimY)
     mP = RobustGaussianFittingLibrary.fitPlane(inX = inX.flatten(), 
-                                       inY = inY.flatten(),
-                                       inZ = img3.flatten())
+                                               inY = inY.flatten(),
+                                               inZ = img3.flatten())
     print(mP)
+    mP = RobustGaussianFittingLibrary.fitBackground(np.squeeze(img3))
+    print(mP)
+    
+    
     inTensor = np.concatenate((img1, img2, img3))
     print('input Tensor shape is: ', str(inTensor.shape))
-    modelParamsMap = RobustGaussianFittingLibrary.fitBackgroundTensor(inTensor)
+    modelParamsMap = RobustGaussianFittingLibrary.fitBackgroundTensor(inTensor, numStrides=5)
     print(modelParamsMap)
 
 def test_fitBackgroundTensor_multiproc():
     print('test_fitBackgroundTensor_multiproc')
     f_N, r_N, c_N = (100, 128, 512)
     inTensor = np.zeros((f_N, r_N, c_N), dtype='float32')
     for frmCnt in range(f_N):
@@ -327,15 +348,15 @@
     plt.plot(np.array([0, testData.shape[0]]), np.array([mP[0]+3*mP[1], mP[0]+3*mP[1]]))
     plt.show()
     RobustGaussianFittingLibrary.misc.sGHist(testData, mP)    
     
 def test_fitValue2Skewed_sweep_over_N():
     print('test_fitValue2Skewed_sweep_over_N')
     numIter = 100
-    maxN = 300
+    maxN = 500
     minN = 2
     mode_all = np.zeros((maxN-minN, numIter))
     std_all = np.zeros((maxN-minN, numIter))
     std_base = np.zeros((maxN-minN, numIter))
     rmod_all = np.zeros((maxN-minN, numIter))
     rstd_all = np.zeros((maxN-minN, numIter))
     pBar = RobustGaussianFittingLibrary.misc.textProgBar(maxN-minN)
@@ -345,15 +366,15 @@
             RNN0 = np.random.randn(N)
             RNN1 = 7+5*(np.random.rand(int(N*0.5))-0.5)
             testData = np.concatenate((RNN0, RNN1)).flatten()
             #testData = RNN0.flatten()
             np.random.shuffle(testData)
             rmode, rstd = RobustGaussianFittingLibrary.fitValue2Skewed(testData, 
                                                                 topKthPerc=0.5, 
-                                                                bottomKthPerc=0.4,
+                                                                bottomKthPerc=0.25,
                                                                 MSSE_LAMBDA=3.0)
             mode_all[N-minN, iter] = RNN0.mean()
             std_all[N-minN, iter] = RobustGaussianFittingLibrary.MSSE(np.squeeze(RNN0), MSSE_LAMBDA = 3.0, k=int(0.5*N))
             std_base[N-minN, iter] = RNN0.std()
             rmod_all[N-minN, iter] = rmode
             rstd_all[N-minN, iter] = rstd
         x[N-minN] = testData.shape[0]
@@ -366,18 +387,19 @@
     rmod_all = rmod_all.mean(1)
     rstd_all = rstd_all.mean(1)
     
     plt.plot(x, mode_all, '.')
     plt.plot(x, rmod_all, '.')
     plt.show()
     
-    plt.plot(x, std_base, '.')
-    plt.plot(x, std_all, '.')
-    plt.plot(x, rstd_all, '.')
+    plt.plot(x, std_base, '.', label='std_base')
+    plt.plot(x, std_all, '.', label='std_all')
+    plt.plot(x, rstd_all, '.', label='rstd_all')
     plt.grid()
+    plt.legend()
     plt.show()
     
 def test_flatField():    
     print('test_flatField')
     RNN0 =  0 + 1*np.random.randn(2048)
     RNN1 =  6 + 6**0.5*np.random.randn(1024)
     RNN2 =  12 + 12**0.5*np.random.randn(512)
@@ -473,23 +495,24 @@
     print(mP)
     #inds = np.where(np.fabs(testData)<50)
     #print('(' + str(testData[inds].mean())+ ', ' + str(testData[inds].std()) + ')')
     print('inliers mean ' + str(inliers.mean()) + ' inliers std ' + str(inliers.std()))                                   
     
 if __name__ == '__main__':
     print('PID ->' + str(os.getpid()))
+    test_fitBackgroundTensor()
+    test_fitBackgroundTensor_multiproc()
     test_RobustAlgebraicLineFittingPy()
-    test_fitValue2Skewed_sweep_over_N()
-    visOrderStat()
+    test_fitBackground()
     test_fitValue2Skewed()
     test_for_textProgBar()
     test_removeIslands()
     test_fitValueSmallSample()
     test_bigTensor2SmallsInds()
     test_RobustAlgebraicPlaneFittingPy()
     test_SginleGaussianVec()
     test_flatField()
-    test_fitBackground()
-    test_fitBackgroundTensor()
+    test_fitValue2Skewed_sweep_over_N()
     test_fitValueTensor_MultiProc()
     test_fitLineTensor_MultiProc()
-    test_fitBackgroundTensor_multiproc()
+    visOrderStat()
+    exit()
```

### Comparing `RobustGaussianFittingLibrary-v0.1.8/RobustGaussianFittingLibrary/useMultiproc.py` & `RobustGaussianFittingLibrary-v0.1.9/RobustGaussianFittingLibrary/useMultiproc.py`

 * *Files identical despite different names*

### Comparing `RobustGaussianFittingLibrary-v0.1.8/setup.py` & `RobustGaussianFittingLibrary-v0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #################################################################################################
 # This file is part of RobustGaussianFittingLibrary, a free library WITHOUT ANY WARRANTY        # 
 # Copyright: 2017-2020 LaTrobe University Melbourne, 2019-2020 Deutsches Elektronen-Synchrotron # 
 #################################################################################################
 from distutils.core import setup, Extension
-_version = 'v0.1.8'
+_version = 'v0.1.9'
 setup(
   name = 'RobustGaussianFittingLibrary',         # How you named your package folder (MyLib)
   packages = ['RobustGaussianFittingLibrary'],   # Chose the same as "name"
   version = _version,      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A library for robust Gaussian fitting using geometric models in presence of outliers. ',   # Give a short description about your library
   author = 'Alireza Sadri',                   # Type in your name
```

