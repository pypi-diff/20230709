# Comparing `tmp/pylinefinder-0.1.2.tar.gz` & `tmp/pylinefinder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinefinder-0.1.2.tar", max compression
+gzip compressed data, was "pylinefinder-0.1.3.tar", max compression
```

## Comparing `pylinefinder-0.1.2.tar` & `pylinefinder-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 18:25:21.168640 pylinefinder-0.1.2/README.md
--rw-r--r--   0        0        0      851 2023-07-09 19:14:26.710181 pylinefinder-0.1.2/pylinefinder/__main__.py
--rw-r--r--   0        0        0      294 2023-07-09 19:14:42.946611 pylinefinder-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pylinefinder-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 18:25:21.168640 pylinefinder-0.1.3/README.md
+-rw-r--r--   0        0        0      846 2023-07-09 19:18:53.769270 pylinefinder-0.1.3/pylinefinder/__main__.py
+-rw-r--r--   0        0        0      294 2023-07-09 19:19:01.549477 pylinefinder-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pylinefinder-0.1.3/PKG-INFO
```

### Comparing `pylinefinder-0.1.2/pylinefinder/__main__.py` & `pylinefinder-0.1.3/pylinefinder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 def greet(arquivo, trecho):
     results = []
     try:
         with open(arquivo) as f:
             for line in f:
                 if trecho.lower() in line.lower():
-                    results.line.append(line)
+                    results.append(line)
                     
         with open('resultado.txt', 'w') as f2:
             conteudo = ''.join(results)
             f2.write(conteudo)
             
             click.echo('Arquivo raspado com sucesso!')
             click.echo('Resultado:')
```

