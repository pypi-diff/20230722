# Comparing `tmp/anybomt-0.1.0.tar.gz` & `tmp/anybomt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anybomt-0.1.0.tar", last modified: Fri Jul 21 21:17:20 2023, max compression
+gzip compressed data, was "anybomt-0.1.1.tar", last modified: Sat Jul 22 03:57:56 2023, max compression
```

## Comparing `anybomt-0.1.0.tar` & `anybomt-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 21:17:20.525362 anybomt-0.1.0/
--rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    24402 2023-07-21 21:17:20.523932 anybomt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    23973 2023-07-21 21:15:13.000000 anybomt-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 21:17:20.521877 anybomt-0.1.0/anybomt.egg-info/
--rw-rw-rw-   0        0        0    24402 2023-07-21 21:17:20.000000 anybomt-0.1.0/anybomt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-07-21 21:17:20.000000 anybomt-0.1.0/anybomt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 21:17:20.000000 anybomt-0.1.0/anybomt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 21:17:20.000000 anybomt-0.1.0/anybomt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    39320 2023-07-21 20:54:05.000000 anybomt-0.1.0/anybomt.py
--rw-rw-rw-   0        0        0       42 2023-07-21 21:17:20.526362 anybomt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-07-21 21:16:55.000000 anybomt-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-22 03:57:56.359347 anybomt-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    24524 2023-07-22 03:57:56.358236 anybomt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    24095 2023-07-22 03:57:12.000000 anybomt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-22 03:57:56.354493 anybomt-0.1.1/anybomt.egg-info/
+-rw-rw-rw-   0        0        0    24524 2023-07-22 03:57:56.000000 anybomt-0.1.1/anybomt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-07-22 03:57:56.000000 anybomt-0.1.1/anybomt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 03:57:56.000000 anybomt-0.1.1/anybomt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-22 03:57:56.000000 anybomt-0.1.1/anybomt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    39320 2023-07-21 20:54:05.000000 anybomt-0.1.1/anybomt.py
+-rw-rw-rw-   0        0        0       42 2023-07-22 03:57:56.359347 anybomt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-07-22 03:57:38.000000 anybomt-0.1.1/setup.py
```

### Comparing `anybomt-0.1.0/LICENSE` & `anybomt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anybomt-0.1.0/PKG-INFO` & `anybomt-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anybomt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Uma biblioteca para facilitar sua jornada em matemática
 Author: AnyBoMath
 Author-email: bidjorys@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,16 +23,21 @@
 Para instalar a biblioteca **AnyBomT**, voce pode utilizar o gerenciador de pacotes `pip`. Execute o seguinte comando:
 
 ```bash
 pip install anybomt
 ```
 
 ## Como usar
+Antes de tudo, devem instalar o numpy e scipy para usar o anybomt.
+```bash
+pip install numpy
+pip install scipy
+```
 
-Apos a instalacao, voce pode importar as funcoes da biblioteca no seu codigo Python da seguinte maneira:
+Apos as instalacoes, voce pode importar as funcoes da biblioteca no seu codigo Python da seguinte maneira:
 
 ```python
 from anybomt import fatorial, potencia, valor_maximo, valor_minimo, raiz_quadrada, somar
 ```
 
 Agora, voce pode utilizar as funcoes em seu codigo para realizar os calculos necessarios.
```

### Comparing `anybomt-0.1.0/README.md` & `anybomt-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,21 @@
 Para instalar a biblioteca **AnyBomT**, voce pode utilizar o gerenciador de pacotes `pip`. Execute o seguinte comando:
 
 ```bash
 pip install anybomt
 ```
 
 ## Como usar
+Antes de tudo, devem instalar o numpy e scipy para usar o anybomt.
+```bash
+pip install numpy
+pip install scipy
+```
 
-Apos a instalacao, voce pode importar as funcoes da biblioteca no seu codigo Python da seguinte maneira:
+Apos as instalacoes, voce pode importar as funcoes da biblioteca no seu codigo Python da seguinte maneira:
 
 ```python
 from anybomt import fatorial, potencia, valor_maximo, valor_minimo, raiz_quadrada, somar
 ```
 
 Agora, voce pode utilizar as funcoes em seu codigo para realizar os calculos necessarios.
```

### Comparing `anybomt-0.1.0/anybomt.egg-info/PKG-INFO` & `anybomt-0.1.1/anybomt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anybomt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Uma biblioteca para facilitar sua jornada em matemática
 Author: AnyBoMath
 Author-email: bidjorys@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,16 +23,21 @@
 Para instalar a biblioteca **AnyBomT**, voce pode utilizar o gerenciador de pacotes `pip`. Execute o seguinte comando:
 
 ```bash
 pip install anybomt
 ```
 
 ## Como usar
+Antes de tudo, devem instalar o numpy e scipy para usar o anybomt.
+```bash
+pip install numpy
+pip install scipy
+```
 
-Apos a instalacao, voce pode importar as funcoes da biblioteca no seu codigo Python da seguinte maneira:
+Apos as instalacoes, voce pode importar as funcoes da biblioteca no seu codigo Python da seguinte maneira:
 
 ```python
 from anybomt import fatorial, potencia, valor_maximo, valor_minimo, raiz_quadrada, somar
 ```
 
 Agora, voce pode utilizar as funcoes em seu codigo para realizar os calculos necessarios.
```

### Comparing `anybomt-0.1.0/anybomt.py` & `anybomt-0.1.1/anybomt.py`

 * *Files identical despite different names*

### Comparing `anybomt-0.1.0/setup.py` & `anybomt-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Leitura do arquivo README.md
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 # Configuração do pacote
 setup(
     name='anybomt',
-    version='0.1.0',
+    version='0.1.1',
     license='MIT',
     author='AnyBoMath',
     author_email='bidjorys@gmail.com',
     description='Uma biblioteca para facilitar sua jornada em matemática',
     long_description=long_description,
     long_description_content_type='text/markdown',
   # Substitua com o link do seu repositório no GitHub
```

