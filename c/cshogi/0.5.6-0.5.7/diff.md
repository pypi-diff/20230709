# Comparing `tmp/cshogi-0.5.6.tar.gz` & `tmp/cshogi-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshogi-0.5.6.tar", last modified: Sat Jul  8 03:26:47 2023, max compression
+gzip compressed data, was "cshogi-0.5.7.tar", last modified: Sat Jul  8 09:47:15 2023, max compression
```

## Comparing `cshogi-0.5.6.tar` & `cshogi-0.5.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.229791 cshogi-0.5.6/
--rw-rw-rw-   0        0        0    35823 2023-07-08 03:26:06.000000 cshogi-0.5.6/LICENSE
--rw-rw-rw-   0        0        0      358 2023-07-08 03:26:47.229791 cshogi-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     5135 2023-07-08 03:26:06.000000 cshogi-0.5.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/
--rw-rw-rw-   0        0        0     2774 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/CSA.py
--rw-rw-rw-   0        0        0    18556 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/KI2.py
--rw-rw-rw-   0        0        0    17360 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/KIF.py
--rw-rw-rw-   0        0        0     2988 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/PGN.py
--rw-rw-rw-   0        0        0       27 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/__init__.py
--rw-rw-rw-   0        0        0    29185 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/_cshogi.pyx
--rw-rw-rw-   0        0        0    25971 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/dlshogi/
--rw-rw-rw-   0        0        0      327 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/dlshogi/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/elo.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/gym_shogi/
--rw-rw-rw-   0        0        0      132 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/gym_shogi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/gym_shogi/envs/
--rw-rw-rw-   0        0        0      118 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/gym_shogi/envs/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/gym_shogi/envs/shogi_env.pyx
--rw-rw-rw-   0        0        0      755 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/gym_shogi/envs/shogi_vec_env.pyx
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/usi/
--rw-rw-rw-   0        0        0     6725 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/usi/Engine.py
--rw-rw-rw-   0        0        0       26 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/usi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/web/
--rw-rw-rw-   0        0        0    13662 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/web/app.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/web/static/
--rw-rw-rw-   0        0        0    13931 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/web/static/board.js
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi/web/templates/
--rw-rw-rw-   0        0        0    17362 2023-07-08 03:26:06.000000 cshogi-0.5.6/cshogi/web/templates/board.html
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.213599 cshogi-0.5.6/cshogi.egg-info/
--rw-rw-rw-   0        0        0      358 2023-07-08 03:26:47.000000 cshogi-0.5.6/cshogi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-07-08 03:26:47.000000 cshogi-0.5.6/cshogi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 03:26:47.000000 cshogi-0.5.6/cshogi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-08 03:26:47.000000 cshogi-0.5.6/cshogi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 03:26:47.229791 cshogi-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0     2040 2023-07-08 03:26:06.000000 cshogi-0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.229791 cshogi-0.5.6/src/
--rw-rw-rw-   0        0        0     8208 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/bitboard.cpp
--rw-rw-rw-   0        0        0     3267 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/book.cpp
--rw-rw-rw-   0        0        0     1350 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/common.cpp
--rw-rw-rw-   0        0        0    28484 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/dfpn.cpp
--rw-rw-rw-   0        0        0    50568 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/generateMoves.cpp
--rw-rw-rw-   0        0        0     1789 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/hand.cpp
--rw-rw-rw-   0        0        0    19051 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/init.cpp
--rw-rw-rw-   0        0        0     6937 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/mate.cpp
--rw-rw-rw-   0        0        0     2163 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/move.cpp
--rw-rw-rw-   0        0        0     1172 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/mt64bit.cpp
--rw-rw-rw-   0        0        0   174059 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/position.cpp
--rw-rw-rw-   0        0        0     3308 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/search.cpp
--rw-rw-rw-   0        0        0     1416 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/square.cpp
--rw-rw-rw-   0        0        0     6627 2023-07-08 03:26:06.000000 cshogi-0.5.6/src/usi.cpp
-drwxrwxrwx   0        0        0        0 2023-07-08 03:26:47.229791 cshogi-0.5.6/test/
--rw-rw-rw-   0        0        0      824 2023-07-08 03:26:06.000000 cshogi-0.5.6/test/test_usi_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/
+-rw-rw-rw-   0        0        0    35823 2023-07-08 09:46:26.000000 cshogi-0.5.7/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-07-08 09:47:15.617637 cshogi-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5135 2023-07-08 09:46:26.000000 cshogi-0.5.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.602066 cshogi-0.5.7/cshogi/
+-rw-rw-rw-   0        0        0     2774 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/CSA.py
+-rw-rw-rw-   0        0        0    18556 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/KI2.py
+-rw-rw-rw-   0        0        0    17360 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/KIF.py
+-rw-rw-rw-   0        0        0     2988 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/PGN.py
+-rw-rw-rw-   0        0        0       27 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/__init__.py
+-rw-rw-rw-   0        0        0    29336 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/_cshogi.pyx
+-rw-rw-rw-   0        0        0    25971 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/cshogi/dlshogi/
+-rw-rw-rw-   0        0        0      327 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/dlshogi/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/elo.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/cshogi/gym_shogi/
+-rw-rw-rw-   0        0        0      132 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/gym_shogi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/cshogi/gym_shogi/envs/
+-rw-rw-rw-   0        0        0      118 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/gym_shogi/envs/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/gym_shogi/envs/shogi_env.pyx
+-rw-rw-rw-   0        0        0      755 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/gym_shogi/envs/shogi_vec_env.pyx
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/cshogi/usi/
+-rw-rw-rw-   0        0        0     6725 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/usi/Engine.py
+-rw-rw-rw-   0        0        0       26 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/usi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/cshogi/web/
+-rw-rw-rw-   0        0        0    13662 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/web/app.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/cshogi/web/static/
+-rw-rw-rw-   0        0        0    13931 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/web/static/board.js
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/cshogi/web/templates/
+-rw-rw-rw-   0        0        0    17362 2023-07-08 09:46:26.000000 cshogi-0.5.7/cshogi/web/templates/board.html
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/cshogi.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-07-08 09:47:15.000000 cshogi-0.5.7/cshogi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-08 09:47:15.000000 cshogi-0.5.7/cshogi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 09:47:15.000000 cshogi-0.5.7/cshogi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 09:47:15.000000 cshogi-0.5.7/cshogi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 09:47:15.617637 cshogi-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     2040 2023-07-08 09:46:26.000000 cshogi-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/src/
+-rw-rw-rw-   0        0        0     8208 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/bitboard.cpp
+-rw-rw-rw-   0        0        0     3267 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/book.cpp
+-rw-rw-rw-   0        0        0     1350 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/common.cpp
+-rw-rw-rw-   0        0        0    28484 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/dfpn.cpp
+-rw-rw-rw-   0        0        0    50568 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/generateMoves.cpp
+-rw-rw-rw-   0        0        0     1789 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/hand.cpp
+-rw-rw-rw-   0        0        0    19051 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/init.cpp
+-rw-rw-rw-   0        0        0     6937 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/mate.cpp
+-rw-rw-rw-   0        0        0     2163 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/move.cpp
+-rw-rw-rw-   0        0        0     1172 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/mt64bit.cpp
+-rw-rw-rw-   0        0        0   174059 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/position.cpp
+-rw-rw-rw-   0        0        0     3308 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/search.cpp
+-rw-rw-rw-   0        0        0     1416 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/square.cpp
+-rw-rw-rw-   0        0        0     6627 2023-07-08 09:46:26.000000 cshogi-0.5.7/src/usi.cpp
+drwxrwxrwx   0        0        0        0 2023-07-08 09:47:15.617637 cshogi-0.5.7/test/
+-rw-rw-rw-   0        0        0      824 2023-07-08 09:46:26.000000 cshogi-0.5.7/test/test_usi_engine.py
```

### Comparing `cshogi-0.5.6/LICENSE` & `cshogi-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/README.rst` & `cshogi-0.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/CSA.py` & `cshogi-0.5.7/cshogi/CSA.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/KI2.py` & `cshogi-0.5.7/cshogi/KI2.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/KIF.py` & `cshogi-0.5.7/cshogi/KIF.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/PGN.py` & `cshogi-0.5.7/cshogi/PGN.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/_cshogi.pyx` & `cshogi-0.5.7/cshogi/_cshogi.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,15 @@
 		int piece(const int sq)
 		bool inCheck()
 		int mateMoveIn1Ply()
 		int mateMove(int ply);
 		bool is_mate(int ply);
 		unsigned long long getKey()
 		bool moveIsPseudoLegal(const int move)
+		bool pseudoLegalMoveIsLegal(const int move)
 		bool moveIsLegal(const int move)
 		vector[int] pieces_in_hand(const int color)
 		vector[int] pieces()
 		bool is_nyugyoku()
 		void piece_planes(char* mem)
 		void piece_planes_rotate(char* mem)
 		void _dlshogi_make_input_features(char* mem1, char* mem2)
@@ -471,14 +472,17 @@
 
 	def zobrist_hash(self):
 		return self.__board.getKey()
 
 	def is_pseudo_legal(self, int move):
 		return self.__board.moveIsPseudoLegal(move)
 
+	def pseudo_legal_move_is_legal(self, int move):
+		return self.__board.pseudoLegalMoveIsLegal(move)
+
 	def is_legal(self, int move):
 		return self.__board.moveIsLegal(move)
 
 	@property
 	def pieces_in_hand(self):
 		return (self.__board.pieces_in_hand(BLACK), self.__board.pieces_in_hand(WHITE))
```

### Comparing `cshogi-0.5.6/cshogi/cli.py` & `cshogi-0.5.7/cshogi/cli.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/elo.py` & `cshogi-0.5.7/cshogi/elo.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/gym_shogi/envs/shogi_env.pyx` & `cshogi-0.5.7/cshogi/gym_shogi/envs/shogi_env.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/gym_shogi/envs/shogi_vec_env.pyx` & `cshogi-0.5.7/cshogi/gym_shogi/envs/shogi_vec_env.pyx`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/usi/Engine.py` & `cshogi-0.5.7/cshogi/usi/Engine.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/web/app.py` & `cshogi-0.5.7/cshogi/web/app.py`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/web/static/board.js` & `cshogi-0.5.7/cshogi/web/static/board.js`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi/web/templates/board.html` & `cshogi-0.5.7/cshogi/web/templates/board.html`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/cshogi.egg-info/SOURCES.txt` & `cshogi-0.5.7/cshogi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/setup.py` & `cshogi-0.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     Extension('cshogi.gym_shogi.envs.shogi_vec_env',
         ['cshogi/gym_shogi/envs/shogi_vec_env.pyx'],
         language='c++'),
 ]
 
 setup(
     name='cshogi',
-    version='0.5.6',
+    version='0.5.7',
     packages=['cshogi', 'cshogi.usi', 'cshogi.gym_shogi', 'cshogi.gym_shogi.envs', 'cshogi.dlshogi', 'cshogi.web', 'cshogi.web.templates', 'cshogi.web.static'],
     package_data={'cshogi.web.templates': ['*'], 'cshogi.web.static': ['*']},
     ext_modules=ext_modules,
     cmdclass={'build_ext': my_build_ext},
     author='Tadao Yamaoka',
     url='https://github.com/TadaoYamaoka/cshogi',
     description = 'A fast Python shogi library',
```

### Comparing `cshogi-0.5.6/src/bitboard.cpp` & `cshogi-0.5.7/src/bitboard.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/book.cpp` & `cshogi-0.5.7/src/book.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/common.cpp` & `cshogi-0.5.7/src/common.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/dfpn.cpp` & `cshogi-0.5.7/src/dfpn.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/generateMoves.cpp` & `cshogi-0.5.7/src/generateMoves.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/hand.cpp` & `cshogi-0.5.7/src/hand.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/init.cpp` & `cshogi-0.5.7/src/init.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/mate.cpp` & `cshogi-0.5.7/src/mate.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/move.cpp` & `cshogi-0.5.7/src/move.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/mt64bit.cpp` & `cshogi-0.5.7/src/mt64bit.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/position.cpp` & `cshogi-0.5.7/src/position.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/search.cpp` & `cshogi-0.5.7/src/search.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/square.cpp` & `cshogi-0.5.7/src/square.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/src/usi.cpp` & `cshogi-0.5.7/src/usi.cpp`

 * *Files identical despite different names*

### Comparing `cshogi-0.5.6/test/test_usi_engine.py` & `cshogi-0.5.7/test/test_usi_engine.py`

 * *Files identical despite different names*

