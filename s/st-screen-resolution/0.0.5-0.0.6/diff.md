# Comparing `tmp/st_screen_resolution-0.0.5.tar.gz` & `tmp/st_screen_resolution-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_screen_resolution-0.0.5.tar", last modified: Sun Jul  9 03:11:17 2023, max compression
+gzip compressed data, was "st_screen_resolution-0.0.6.tar", last modified: Sun Jul  9 03:40:29 2023, max compression
```

## Comparing `st_screen_resolution-0.0.5.tar` & `st_screen_resolution-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.760336 st_screen_resolution-0.0.5/
--rw-rw-rw-   0        0        0     1082 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-09 03:10:41.000000 st_screen_resolution-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      295 2023-07-09 03:11:17.759828 st_screen_resolution-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-09 03:11:17.760336 st_screen_resolution-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-07-09 03:11:09.000000 st_screen_resolution-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.732190 st_screen_resolution-0.0.5/st_screen_resolution/
--rw-rw-rw-   0        0        0     3355 2023-07-09 02:47:54.000000 st_screen_resolution-0.0.5/st_screen_resolution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.727064 st_screen_resolution-0.0.5/st_screen_resolution/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.748041 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/
--rw-rw-rw-   0        0        0      691 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0     2087 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.728093 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.758301 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/
--rw-rw-rw-   0        0        0   464228 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js
--rw-rw-rw-   0        0        0     2059 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1600815 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.map
--rw-rw-rw-   0        0        0     1093 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/main.1a50ca2c.chunk.js
--rw-rw-rw-   0        0        0     2794 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/main.1a50ca2c.chunk.js.map
--rw-rw-rw-   0        0        0     1584 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js
--rw-rw-rw-   0        0        0     8369 2023-07-09 03:07:16.000000 st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js.map
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:17.743934 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/
--rw-rw-rw-   0        0        0      295 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-09 03:11:17.000000 st_screen_resolution-0.0.5/st_screen_resolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 03:40:29.456882 st_screen_resolution-0.0.6/
+-rw-rw-rw-   0        0        0     1082 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-09 03:10:41.000000 st_screen_resolution-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      295 2023-07-09 03:40:29.456371 st_screen_resolution-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-09 03:40:29.456882 st_screen_resolution-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-07-09 03:40:21.000000 st_screen_resolution-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 03:40:29.429769 st_screen_resolution-0.0.6/st_screen_resolution/
+-rw-rw-rw-   0        0        0     3355 2023-07-09 03:39:12.000000 st_screen_resolution-0.0.6/st_screen_resolution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 03:40:29.425178 st_screen_resolution-0.0.6/st_screen_resolution/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-09 03:40:29.444572 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/
+-rw-rw-rw-   0        0        0      691 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-07-09 01:25:50.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0     2087 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-09 03:40:29.425694 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-09 03:40:29.454829 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   464228 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js
+-rw-rw-rw-   0        0        0     2059 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1600815 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.map
+-rw-rw-rw-   0        0        0     1248 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/main.cba499ab.chunk.js
+-rw-rw-rw-   0        0        0     3256 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/main.cba499ab.chunk.js.map
+-rw-rw-rw-   0        0        0     1584 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js
+-rw-rw-rw-   0        0        0     8369 2023-07-09 03:39:44.000000 st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js.map
+drwxrwxrwx   0        0        0        0 2023-07-09 03:40:29.441001 st_screen_resolution-0.0.6/st_screen_resolution.egg-info/
+-rw-rw-rw-   0        0        0      295 2023-07-09 03:40:29.000000 st_screen_resolution-0.0.6/st_screen_resolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-07-09 03:40:29.000000 st_screen_resolution-0.0.6/st_screen_resolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 03:40:29.000000 st_screen_resolution-0.0.6/st_screen_resolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-09 03:40:29.000000 st_screen_resolution-0.0.6/st_screen_resolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-09 03:40:29.000000 st_screen_resolution-0.0.6/st_screen_resolution.egg-info/top_level.txt
```

### Comparing `st_screen_resolution-0.0.5/LICENSE` & `st_screen_resolution-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.5/setup.py` & `st_screen_resolution-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_screen_resolution",
-    version="0.0.5",
+    version="0.0.6",
     author="YM",
     author_email="",
     description="",
     long_description="get screen resolution in streamlit",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/__init__.py` & `st_screen_resolution-0.0.6/st_screen_resolution/__init__.py`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/asset-manifest.json` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/asset-manifest.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.84375%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/main.cba499ab.chunk.js')], delete: [2]}",*

 * * "'files'": "{'main.js': './static/js/main.cba499ab.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.cba499ab.chunk.js.map'}"}*

```diff
@@ -1,17 +1,17 @@
 {
     "entrypoints": [
         "static/js/runtime-main.0f051bbb.js",
         "static/js/2.409ed399.chunk.js",
-        "static/js/main.1a50ca2c.chunk.js"
+        "static/js/main.cba499ab.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.1a50ca2c.chunk.js",
-        "main.js.map": "./static/js/main.1a50ca2c.chunk.js.map",
+        "main.js": "./static/js/main.cba499ab.chunk.js",
+        "main.js.map": "./static/js/main.cba499ab.chunk.js.map",
         "runtime-main.js": "./static/js/runtime-main.0f051bbb.js",
         "runtime-main.js.map": "./static/js/runtime-main.0f051bbb.js.map",
         "static/js/2.409ed399.chunk.js": "./static/js/2.409ed399.chunk.js",
         "static/js/2.409ed399.chunk.js.LICENSE.txt": "./static/js/2.409ed399.chunk.js.LICENSE.txt",
         "static/js/2.409ed399.chunk.js.map": "./static/js/2.409ed399.chunk.js.map"
     }
 }
```

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/bootstrap.min.css` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/index.html` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,p=t[0],f=t[1],i=t[2],c=0,s=[];c<p.length;c++)l=p[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in f)Object.prototype.hasOwnProperty.call(f,n)&&(e[n]=f[n]);for(a&&a(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,p=1;p<r.length;p++){var f=r[p];0!==o[f]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var p=this.webpackJsonpst_blogpost_component=this.webpackJsonpst_blogpost_component||[],f=p.push.bind(p);p.push=t,p=p.slice();for(var i=0;i<p.length;i++)t(p[i]);var a=f;r()}([])</script><script src="./static/js/2.409ed399.chunk.js"></script><script src="./static/js/main.1a50ca2c.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,p=t[0],f=t[1],i=t[2],c=0,s=[];c<p.length;c++)l=p[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in f)Object.prototype.hasOwnProperty.call(f,n)&&(e[n]=f[n]);for(a&&a(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,p=1;p<r.length;p++){var f=r[p];0!==o[f]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var p=this.webpackJsonpst_blogpost_component=this.webpackJsonpst_blogpost_component||[],f=p.push.bind(p);p.push=t,p=p.slice();for(var i=0;i<p.length;i++)t(p[i]);var a=f;r()}([])</script><script src="./static/js/2.409ed399.chunk.js"></script><script src="./static/js/main.cba499ab.chunk.js"></script></body></html>
```

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.LICENSE.txt` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.map` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/main.1a50ca2c.chunk.js` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/main.cba499ab.chunk.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -4,57 +4,64 @@
             "use strict";
             t.r(n);
             var i = t(5),
                 o = t.n(i),
                 s = t(15),
                 d = t.n(s),
                 r = t(0),
-                c = t(1),
-                a = t(7),
+                a = t(1),
+                c = t(7),
                 h = t(2),
                 u = t(3),
-                l = t(13),
-                b = t(9),
-                w = function(e) {
+                w = t(13),
+                l = t(9),
+                b = function() {
+                    var e = window;
+                    return {
+                        innerWidth: e.innerWidth,
+                        innerHeight: e.innerHeight
+                    }
+                },
+                j = function(e) {
                     Object(h.a)(t, e);
                     var n = Object(u.a)(t);
 
                     function t(e) {
                         var i;
-                        return Object(r.a)(this, t), (i = n.call(this, e)).render = function() {
-                            return Object(b.jsx)("div", {})
-                        }, i._handleWindowResize = i._handleWindowResize.bind(Object(a.a)(i)), i
+                        return Object(r.a)(this, t), (i = n.call(this, e)).state = {
+                            window: 0
+                        }, i.render = function() {
+                            return Object(l.jsx)("div", {})
+                        }, i._handleWindowResize = i._handleWindowResize.bind(Object(c.a)(i)), i
                     }
-                    return Object(c.a)(t, [{
+                    return Object(a.a)(t, [{
                         key: "componentDidMount",
                         value: function() {
                             window.addEventListener("resize", this._handleWindowResize), this._handleWindowResize()
                         }
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
                             window.removeEventListener("resize", this._handleWindowResize), this._handleWindowResize()
                         }
                     }, {
                         key: "_handleWindowResize",
                         value: function() {
-                            l.a.setComponentValue(function() {
-                                var e = window;
+                            (0 == this.state.window || Math.abs(this.state.window - b().innerWidth) > 10) && (this.setState((function() {
                                 return {
-                                    innerWidth: e.innerWidth,
-                                    innerHeight: e.innerHeight
+                                    window: b().innerWidth
                                 }
-                            }())
+                            })), w.a.setComponentValue(b()))
                         }
                     }]), t
-                }(l.b),
-                j = Object(l.c)(w);
-            d.a.render(Object(b.jsx)(o.a.StrictMode, {
-                children: Object(b.jsx)(j, {})
+                }(w.b),
+                p = Object(w.c)(j);
+            d.a.render(Object(l.jsx)(o.a.StrictMode, {
+                children: Object(l.jsx)(p, {})
             }), document.getElementById("root"))
         }
     },
     [
         [24, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.1a50ca2c.chunk.js.map
+//# sourceMappingURL=main.cba499ab.chunk.js.map
```

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/main.1a50ca2c.chunk.js.map` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/main.cba499ab.chunk.js.map`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7867965367965368%*

 * *Differences: {"'file'": "'static/js/main.cba499ab.chunk.js'",*

 * * "'mappings'": "'6NASMA,EAAgB,WACpB,IAAAC,EAAoCC,OACpC,MAAO,CAAEC,WADSF,EAAVE,WACaC,YADUH,EAAXG,YAGtB,EACMC,EAAM,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GACV,SAAAA,EAAYK,GAAa,IAADC,EAEwC,OAFxCC,YAAA,KAAAP,IACtBM,EAAAH,EAAAK,KAAA,KAAMH,IAIDI,MAAQ,CAAEZ,OAAQ,GAAGS,EAqBrBI,OAAS,WAId,OACEC,cAAA,SAGJ,EAhCEL,EAAKM,oBAAsBN,EAAKM,oBAAoBC,KAAIC,YAAAR,IAAMA,CAChE,CAqBC,OArBAS,YAAAf,EAAA,EAAAgB,IAAA,oBAAAC,MAID,WACEpB,OAAOqB,iBAAiB,SAAUC,KAAKP,qBACvCO,KAAKP,qBACP […]*

```diff
@@ -1,38 +1,42 @@
 {
-    "file": "static/js/main.1a50ca2c.chunk.js",
-    "mappings": "6NAaMA,EAAM,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GACV,SAAAA,EAAYK,GAAa,IAADC,EAEwC,OAFxCC,YAAA,KAAAP,IACtBM,EAAAH,EAAAK,KAAA,KAAMH,IAgBDI,OAAS,WAId,OACEC,cAAA,SAGJ,EAvBEJ,EAAKK,oBAAsBL,EAAKK,oBAAoBC,KAAIC,YAAAP,IAAMA,CAChE,CAYC,OAZAQ,YAAAd,EAAA,EAAAe,IAAA,oBAAAC,MAED,WACEC,OAAOC,iBAAiB,SAAUC,KAAKR,qBACvCQ,KAAKR,qBACP,GAAC,CAAAI,IAAA,uBAAAC,MACD,WACEC,OAAOG,oBAAoB,SAAUD,KAAKR,qBAC1CQ,KAAKR,qBACP,GAAC,CAAAI,IAAA,sBAAAC,MACD,WACEK,IAAUC,kBAnBQ,WACpB,IAAAC,EAAoCN,OACpC,MAAO,CAAEO,WADSD,EAAVC,WACaC,YADUF,EAAXE,YAEtB,CAgBgCC,GAC9B,KAAC1B,CAAA,CAhBS,CAAS2B,KA8BNC,cAAwB5B,GCvCvC6B,IAASpB,OACPC,cAACoB,IAAMC,WAAU,CAAAC,SACftB,cAACV,EAAM,MAETiC,SAASC,eAAe,Q",
+    "file": "static/js/main.cba499ab.chunk.js",
+    "mappings": "6NASMA,EAAgB,WACpB,IAAAC,EAAoCC,OACpC,MAAO,CAAEC,WADSF,EAAVE,WACaC,YADUH,EAAXG,YAGtB,EACMC,EAAM,SAAAC,GAAAC,YAAAF,EAAAC,GAAA,IAAAE,EAAAC,YAAAJ,GACV,SAAAA,EAAYK,GAAa,IAADC,EAEwC,OAFxCC,YAAA,KAAAP,IACtBM,EAAAH,EAAAK,KAAA,KAAMH,IAIDI,MAAQ,CAAEZ,OAAQ,GAAGS,EAqBrBI,OAAS,WAId,OACEC,cAAA,SAGJ,EAhCEL,EAAKM,oBAAsBN,EAAKM,oBAAoBC,KAAIC,YAAAR,IAAMA,CAChE,CAqBC,OArBAS,YAAAf,EAAA,EAAAgB,IAAA,oBAAAC,MAID,WACEpB,OAAOqB,iBAAiB,SAAUC,KAAKP,qBACvCO,KAAKP,qBACP,GAAC,CAAAI,IAAA,uBAAAC,MACD,WACEpB,OAAOuB,oBAAoB,SAAUD,KAAKP,qBAC1CO,KAAKP,qBACP,GAAC,CAAAI,IAAA,sBAAAC,MAED,YAC2B,GAArBE,KAAKV,MAAMZ,QAAewB,KAAKC,IAAKH,KAAKV,MAAMZ,OAASF,IAAgBG,YAAc,MACxFqB,KAAKI,UAAS,iBAAO,CACnB1B,OAAQF,IAAgBG,WACzB,IACD0B,IAAUC,kBAAkB9B,KAGhC,KAACK,CAAA,CAzBS,CAAS0B,KAuCNC,cAAwB3B,GCjDvC4B,IAASlB,OACPC,cAACkB,IAAMC,WAAU,CAAAC,SACfpB,cAACX,EAAM,MAETgC,SAASC,eAAe,Q",
     "names": [
+        "getWindowSize",
+        "_window",
+        "window",
+        "innerWidth",
+        "innerHeight",
         "Screen",
         "_StreamlitComponentBa",
         "_inherits",
         "_super",
         "_createSuper",
         "props",
         "_this",
         "_classCallCheck",
         "call",
+        "state",
         "render",
         "_jsx",
         "_handleWindowResize",
         "bind",
         "_assertThisInitialized",
         "_createClass",
         "key",
         "value",
-        "window",
         "addEventListener",
         "this",
         "removeEventListener",
+        "Math",
+        "abs",
+        "setState",
         "Streamlit",
         "setComponentValue",
-        "_window",
-        "innerWidth",
-        "innerHeight",
-        "getWindowSize",
         "StreamlitComponentBase",
         "withStreamlitConnection",
         "ReactDOM",
         "React",
         "StrictMode",
         "children",
         "document",
@@ -40,12 +44,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "Screen.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\"\r\nimport React, { ReactNode } from \"react\"\r\n\r\n// the `render()` function is called when component is re-rendered\r\n\r\nconst getWindowSize = () => {\r\n  const { innerWidth, innerHeight } = window\r\n  return { innerWidth, innerHeight }\r\n}\r\nclass Screen extends StreamlitComponentBase<any> {\r\n  constructor(props: any) {\r\n    super(props)\r\n    this._handleWindowResize = this._handleWindowResize.bind(this)\r\n  }\r\n\r\n  componentDidMount() {\r\n    window.addEventListener(\"resize\", this._handleWindowResize)\r\n    this._handleWindowResize()\r\n  }\r\n  componentWillUnmount() {\r\n    window.removeEventListener(\"resize\", this._handleWindowResize)\r\n    this._handleWindowResize()\r\n  }\r\n  _handleWindowResize() {\r\n    Streamlit.setComponentValue(getWindowSize())\r\n  }\r\n\r\n  public render = (): ReactNode => {\r\n    // Arguments that are passed to the plugin in Python are accessible\r\n    // via `this.props.args`\r\n    \r\n    return (\r\n      <div >\r\n      </div>\r\n    )\r\n  }\r\n}\r\n\r\n// connection between component and Streamlit\r\nexport default withStreamlitConnection(Screen)\r\n",
+        "import {\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\"\r\nimport React, { ReactNode } from \"react\"\r\n\r\n// the `render()` function is called when component is re-rendered\r\n\r\nconst getWindowSize = () => {\r\n  const { innerWidth, innerHeight } = window\r\n  return { innerWidth, innerHeight }\r\n  \r\n}\r\nclass Screen extends StreamlitComponentBase<any> {\r\n  constructor(props: any) {\r\n    super(props)\r\n    this._handleWindowResize = this._handleWindowResize.bind(this)\r\n  }\r\n\r\n  public state = { window: 0 }\r\n\r\n  componentDidMount() {\r\n    window.addEventListener(\"resize\", this._handleWindowResize)\r\n    this._handleWindowResize()\r\n  }\r\n  componentWillUnmount() {\r\n    window.removeEventListener(\"resize\", this._handleWindowResize)\r\n    this._handleWindowResize()\r\n  }\r\n\r\n  _handleWindowResize() {\r\n    if (this.state.window == 0 || Math.abs( this.state.window - getWindowSize().innerWidth) > 10) {\r\n      this.setState(() => ({\r\n        window: getWindowSize().innerWidth,\r\n      }))\r\n      Streamlit.setComponentValue(getWindowSize())\r\n    }\r\n    \r\n  }\r\n\r\n  public render = (): ReactNode => {\r\n    // Arguments that are passed to the plugin in Python are accessible\r\n    // via `this.props.args`\r\n    \r\n    return (\r\n      <div >\r\n      </div>\r\n    )\r\n  }\r\n}\r\n\r\n// connection between component and Streamlit\r\nexport default withStreamlitConnection(Screen)\r\n",
         "import React from \"react\"\r\nimport ReactDOM from \"react-dom\"\r\nimport Screen from \"./Screen\"\r\n\r\nReactDOM.render(\r\n  <React.StrictMode>\r\n    <Screen />\r\n  </React.StrictMode>,\r\n  document.getElementById(\"root\")\r\n)\r\n"
     ],
     "version": 3
 }
```

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js.map` & `st_screen_resolution-0.0.6/st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js.map`

 * *Files identical despite different names*

### Comparing `st_screen_resolution-0.0.5/st_screen_resolution.egg-info/SOURCES.txt` & `st_screen_resolution-0.0.6/st_screen_resolution.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 st_screen_resolution.egg-info/top_level.txt
 st_screen_resolution/frontend/build/asset-manifest.json
 st_screen_resolution/frontend/build/bootstrap.min.css
 st_screen_resolution/frontend/build/index.html
 st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js
 st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.LICENSE.txt
 st_screen_resolution/frontend/build/static/js/2.409ed399.chunk.js.map
-st_screen_resolution/frontend/build/static/js/main.1a50ca2c.chunk.js
-st_screen_resolution/frontend/build/static/js/main.1a50ca2c.chunk.js.map
+st_screen_resolution/frontend/build/static/js/main.cba499ab.chunk.js
+st_screen_resolution/frontend/build/static/js/main.cba499ab.chunk.js.map
 st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js
 st_screen_resolution/frontend/build/static/js/runtime-main.0f051bbb.js.map
```

