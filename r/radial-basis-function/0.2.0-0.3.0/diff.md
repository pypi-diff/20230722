# Comparing `tmp/radial_basis_function-0.2.0.tar.gz` & `tmp/radial_basis_function-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radial_basis_function-0.2.0.tar", max compression
+gzip compressed data, was "radial_basis_function-0.3.0.tar", max compression
```

## Comparing `radial_basis_function-0.2.0.tar` & `radial_basis_function-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1097 2023-06-21 04:30:39.171530 radial_basis_function-0.2.0/LICENSE
--rw-r--r--   0        0        0      940 2023-06-21 04:49:28.209051 radial_basis_function-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      142 2023-06-21 04:49:16.483812 radial_basis_function-0.2.0/radial_basis_function/__init__.py
--rw-r--r--   0        0        0     1952 2023-06-21 04:14:33.497639 radial_basis_function-0.2.0/radial_basis_function/pseudo_inversa.py
--rw-r--r--   0        0        0     6396 2023-06-21 04:16:11.508336 radial_basis_function-0.2.0/radial_basis_function/rbf.py
--rw-r--r--   0        0        0     2781 2023-06-21 05:26:54.329205 radial_basis_function-0.2.0/README.md
--rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 radial_basis_function-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-06-21 04:30:39.171530 radial_basis_function-0.3.0/LICENSE
+-rw-r--r--   0        0        0      940 2023-07-21 10:07:31.183145 radial_basis_function-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-07-21 10:07:21.460533 radial_basis_function-0.3.0/radial_basis_function/__init__.py
+-rw-r--r--   0        0        0     2090 2023-07-22 05:35:52.950681 radial_basis_function-0.3.0/radial_basis_function/pseudo_inversa.py
+-rw-r--r--   0        0        0     7736 2023-07-22 06:04:50.568327 radial_basis_function-0.3.0/radial_basis_function/rbf.py
+-rw-r--r--   0        0        0     2780 2023-07-22 05:16:21.009458 radial_basis_function-0.3.0/README.md
+-rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 radial_basis_function-0.3.0/PKG-INFO
```

### Comparing `radial_basis_function-0.2.0/LICENSE` & `radial_basis_function-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radial_basis_function-0.2.0/pyproject.toml` & `radial_basis_function-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radial-basis-function"
-version = "0.2.0"
+version = "0.3.0"
 description = "Radial Basis Function e Multiplicação de Matriz Pseudo-Inversa, para modelos de Regressão e Multi-Classificatórios."
 authors = ["Victor Venites <contato@victorvenites.com>"]
 maintainers = ["Victor Venites <contato@victorvenites.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "radial_basis_function"}]
 homepage = "https://github.com/VictorVenites/Radial-Basis-Function"
```

### Comparing `radial_basis_function-0.2.0/radial_basis_function/pseudo_inversa.py` & `radial_basis_function-0.3.0/radial_basis_function/pseudo_inversa.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,32 +9,37 @@
 import time
 
 class PseudoInversa:
     """Multiplicacao de Matriz Pseudo-Inversa
     Original Author: Victor Venites
     """
     def __init__(self, bias = 1):
-        self.weights = None
         self.bias = bias
+        self.weights = None
         self.feature_names_in_ = None
         self.n_feature_in_ = None
         self.n_linhas_in_ = None
         self.time = None
+    
+    def bias_increment(self, dados):
+        if self.bias != 0:
+            if self.n_linhas_in_ > self.n_feature_in_:
+                dados["Bias_Vies_Intercept"] = self.bias
+        return dados
 
     def fit(self, X, y):
         try:
             self.feature_names_in_ = X.columns
             self.n_feature_in_ = X.shape[1]
             self.n_linhas_in_ = X.shape[0]
         except:
             self.n_feature_in_ = len(X[0])
             self.n_linhas_in_ = len(X)
         Matriz_X = pd.DataFrame(X)
-        if self.bias != 0:
-            Matriz_X["Bias_Vies_Intercept"] = self.bias
+        Matriz_X = self.bias_increment(Matriz_X)
         tempo_Inicial = time.time()
         # Base_T * Base
         Matriz_Quadrada = np.dot(Matriz_X.T, Matriz_X)
         # Matriz Inversa
         try:
             Matriz_Inversa = np.linalg.inv(Matriz_Quadrada)
         except np.linalg.LinAlgError as err:
@@ -45,14 +50,13 @@
         Matriz_Pseudo_Inversa = pd.DataFrame(np.dot(Matriz_Inversa, Matriz_X.T))
         # Isola o peso final
         self.weights = np.dot(Matriz_Pseudo_Inversa, y)
         self.time = time.time() - tempo_Inicial
 
     def predict(self, X):
         Matriz_X = pd.DataFrame(X)
-        if self.bias != 0:
-            Matriz_X["Bias_Vies_Intercept"] = self.bias
+        Matriz_X = self.bias_increment(Matriz_X)
         return np.dot(Matriz_X, self.weights)
 
     def score(self, x, y):
         # TODO: adicionar métricas do próprio Sklearn
         pass
```

### Comparing `radial_basis_function-0.2.0/radial_basis_function/rbf.py` & `radial_basis_function-0.3.0/radial_basis_function/rbf.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,31 +12,81 @@
 import time
 
 
 class RadialBasisFunction:
     """Radial Basis Function
     Original Author: Victor Venites
     """
-    def __init__(self, funcao = 'Gaussiana',
+    def __init__(self, funcao = 'Gaussiana', bias = 1,
                  Qtd_Polos = 0, Polos_iniciais_fixos = False, Polos_Otimizados = None):
         self.funcao = funcao
+        self.bias = bias
         self.Qtd_Polos = Qtd_Polos
         self.Polos_iniciais_fixos = Polos_iniciais_fixos
         self.C = Polos_Otimizados
+        self.numero_polos_definidos = None
         self.sigma = None
         self.pesos = None
         self.R = None
         self.feature_names_in_ = None
         self.n_feature_in_ = None
         self.n_linhas_in_ = None
         self.time = None
-        
+    
+    def definir_numero_de_polos(self):
+        if self.Qtd_Polos == "50percent":
+            if self.n_feature_in_ > 5:
+                aux_polos_desejados = int(round(self.n_feature_in_/2))
+        else:
+            aux_polos_desejados = int(self.Qtd_Polos)
+
+        # Coordenada dos Polos:
+        if self.n_feature_in_ <= 2:
+            self.numero_polos_definidos = 2
+        else:
+            if self.n_feature_in_ > 2:
+                self.numero_polos_definidos = int(self.n_feature_in_)
+            if aux_polos_desejados > 1:
+                self.numero_polos_definidos = aux_polos_desejados
+            if aux_polos_desejados > self.n_feature_in_ * 8:
+                # TODO: Avaliar uma bordagem melhor para evitar Overfitting
+                self.numero_polos_definidos = int(round((aux_polos_desejados + self.n_feature_in_ * 8) / 9))
+            if self.numero_polos_definidos > self.n_linhas_in_:
+                # -1 para evitar Matriz Indeterminada após adicionar Bias
+                self.numero_polos_definidos = self.n_linhas_in_ - 1
+    
+    def Gerar_Polos(self, variaveis):
+        # Gerando os Polos Aleatórios
+        # TODO: Centróides do K-means, ou gerados por Algoritmo Genéticos)
+        if self.C is None:
+            C = np.zeros((self.numero_polos_definidos, self.n_feature_in_), dtype = float)
+            C = np.random.rand(self.numero_polos_definidos, self.n_feature_in_)
+            # Limite por Coluna (apenas entre as escalas de cada coluna)
+            Limite = np.array(variaveis.max() - variaveis.min())
+            C = pd.DataFrame(C) * Limite + np.array(variaveis.min())
+            C = np.array(C)
+            dist_entre_os_polos = np.zeros((self.numero_polos_definidos, self.numero_polos_definidos))
+            for i in range(0, self.numero_polos_definidos, 1):
+                for j in range(0, self.numero_polos_definidos, 1):
+                    dist_entre_os_polos[i, j] = np.linalg.norm(C[i] - C[j])
+            if self.Polos_iniciais_fixos:
+                C[0] = variaveis.mean()
+                C[1] = variaveis.std()
+                if self.numero_polos_definidos > 2:
+                    C[2] = variaveis.max()
+                if self.numero_polos_definidos > 3:
+                    C[3] = variaveis.min()
+            dps_max = np.max(dist_entre_os_polos)
+            self.sigma = dps_max / np.sqrt(2 * self.numero_polos_definidos)
+            self.C = C
+    
     # # # Funções Base
-    def FuncoesBase(self, t, n_PoloAtual, N_TotalPolos, X, C):
+    def FuncoesBase(self, X, C, t, n_PoloAtual, N_TotalPolos):
         # TODO: revisar as funções, para se aproximarem do original de inspiração
+        # TODO: Adicionar Função Aleatória
         Gama = 1 / (2 * self.sigma ** 2) # Por Convensão
         Radial = np.linalg.norm(X - C)
         #Radial = (np.linalg.norm(X - C)) ** 2 # 
         if self.funcao == "Gaussiana":
             calculo = np.exp(-Gama * (Radial ** 2))
             #calculo = np.exp(- Gama * Radial)
         #elif funcao == "Multiquadratica":
@@ -44,91 +94,63 @@
         elif self.funcao == "Sigmoide":
             calculo = np.tanh(-Gama * (Radial ** 2))
         elif self.funcao == "Senoidal":
             calculo = np.sin(-Gama * (Radial ** 2))
         elif self.funcao == "Logistica":
             calculo = 1 / (1 + np.exp(Gama * (Radial**2)))
         elif self.funcao == "ReLu":
-            calculo = max(0, Radial)
+            calculo = max(0, Gama * Radial)
+        elif self.funcao == "ELU":
+            alpha = 1
+            x = Gama * Radial
+            if x >= 0:
+                calculo = x
+            else:
+                calculo = alpha * (np.exp(x) - 1)
+        elif self.funcao == "GELU":
+            # Gaussian Error Linear Unit
+            # https://towardsai.net/p/l/gelu-gaussian-error-linear-unit-code-python-tf-torch
+            # acurado -> 0.5*x*(tanh[((2/pi)**(1/2))*(x + 0.044715*(x**(3)))])
+            # rapido -> x*sigma*(1.702*x)
+            x = Gama * Radial
+            calculo = 0.5*x*(np.tanh[((2/np.pi)**(1/2))*(x + 0.044715*(x**(3)))])
         elif self.funcao == "Fractal":
             # Seed Function 1 /((x**2 + y**2 + 1)**(1/2))
             calculo = 1 / ((Radial**2 + Gama**2 + 1) ** (1/2))
         elif self.funcao == "Aurea":
             golden = (1 + 5 ** 0.5) / 2
             calculo = golden * Gama * Radial
         elif self.funcao == "Fourier":
             # Altura_da_Onda * Sinal( CICLO * TEMPO_X / Tamanho_Periodo )
             calculo = np.sqrt(2) * np.sin(- Gama * 2 * np.pi * t * (Radial ** 2) * n_PoloAtual)
         return calculo
 
+
     # # # Radial - Cálculo
     def Radial(self, X):
-        variaveis = pd.DataFrame(X)
-        num_de_licoes = variaveis.shape[0]
-        num_de_variaveis = variaveis.shape[1]
-        if self.Qtd_Polos == "50percent":
-            if num_de_variaveis > 5:
-                self.Qtd_Polos = int(round(num_de_variaveis/2))
-
-        # Coordenada dos Polos:
-        if num_de_variaveis <= 2:
-            num_de_polos = 2
-        elif num_de_variaveis > 2:
-            num_de_polos = num_de_variaveis
-        if self.Qtd_Polos > 1:
-            num_de_polos = self.Qtd_Polos
-        if self.Qtd_Polos > num_de_licoes:
-            num_de_polos = num_de_licoes - 2
-        if self.Qtd_Polos > num_de_variaveis * 8:
-            # TODO: Avaliar uma bordagem melhor para evitar Overfitting
-            num_de_polos = int(round((self.Qtd_Polos + num_de_variaveis * 8) / 9 + 2))
-        if num_de_polos > num_de_licoes:
-            #num_de_polos = num_de_licoes - 2
-            num_de_polos = num_de_licoes
-
-        # Gerando os Polos Aleatórios
-        # TODO: Centróides do K-means, ou gerados por Algoritmo Genéticos)
-        C = np.zeros((num_de_polos, num_de_variaveis), dtype = float)
-        C = np.random.rand(num_de_polos, num_de_variaveis)
-        # Limite por Coluna (apenas entre as escalas de cada coluna)
-        Limite = np.array(variaveis.max() - variaveis.min())
-        C = pd.DataFrame(C) * Limite + np.array(variaveis.min())
-        C = np.array(C)
+        self.definir_numero_de_polos()
+        self.Gerar_Polos(pd.DataFrame(X))
         
-        # TODO: Criar Função específica para geração dos Polos
-        #if self.C is not None:
-
-        dist_entre_os_polos = np.zeros((num_de_polos, num_de_polos))
-        for i in range(0, num_de_polos, 1):
-            for j in range(0, num_de_polos, 1):
-                dist_entre_os_polos[i, j] = np.linalg.norm(C[i] - C[j])
-        if self.Polos_iniciais_fixos:
-            C[0] = variaveis.mean()
-            C[1] = variaveis.std()
-            if num_de_polos > 2:
-                C[2] = variaveis.max()
-            if num_de_polos > 3:
-                C[3] = variaveis.min()
-        dps_max = np.max(dist_entre_os_polos)
-        self.sigma = dps_max / np.sqrt(2 * num_de_polos)
-        variaveis = np.array(variaveis)
-
+        # TODO: Otimizar hidden layer
+        variaveis = np.array(X)
         # Matrix [R]:
         # R = Matrix de Base Radial [R]
-        R = np.zeros((num_de_licoes, num_de_polos))
-        for n in range(0, num_de_licoes, 1):
+        R = np.zeros((self.n_linhas_in_, self.numero_polos_definidos))
+        for n in range(0, self.n_linhas_in_, 1):
             # Input Layer
-            for i in range(0, num_de_polos, 1):
+            for i in range(0, self.numero_polos_definidos, 1):
                 # Hidden Layer
-                R[n, i] = self.FuncoesBase(n, (i+1), len(C), variaveis[n], C[i])
+                R[n, i] = self.FuncoesBase(variaveis[n], self.C[i], n, (i+1), len(self.C))
+        R = pd.DataFrame(R)
         #print(f"R.shape -> {R.shape}")
-        R[R.shape[1]] = 1
+        # TODO: Revisar e discutir o Bias
+        #R[R.shape[1]] = 1
         #print(f"R.shape -> {R.shape}")
-        self.R = pd.DataFrame(R)
-        self.C = C
+        self.R = R
+        
 
     def fit(self, X, Matriz_Y):
         try:
             self.feature_names_in_ = X.columns
             self.n_feature_in_ = X.shape[1]
             self.n_linhas_in_ = X.shape[0]
         except:
@@ -138,26 +160,26 @@
         self.Radial(X)
         Matriz_Pseudo_Inversa = PseudoInversa()
         Matriz_Pseudo_Inversa.fit(np.array(self.R), Matriz_Y)
         self.pesos = Matriz_Pseudo_Inversa.weights
         self.time = time.time() - tempo_Inicial
 
     def predict(self, X):
+        # TODO: Melhorar o desempenho e estrutura do predict
         #A = np.dot(variaveis_X, W) # Valores finais da predição
         variaveis_X = np.array(X)
         Predicao_Y = np.zeros(len(variaveis_X))
         W = [i for i in self.pesos]
-        C = self.C
         
         for i in range(0, len(variaveis_X), 1):
             # Input
             Predicao_Y[i] = W[-1]
             for j in range(0, len(W) - 1, 1):
                 # Somatorio + Pesos * Funcoes_Ativa
-                Predicao_Y[i] = Predicao_Y[i] + W[j] * self.FuncoesBase(i, (i+1), len(C), variaveis_X[i], C[j])
+                Predicao_Y[i] = Predicao_Y[i] + W[j] * self.FuncoesBase(variaveis_X[i], self.C[j], i, (j+1), len(self.C))
 
         return Predicao_Y
 
     def score(self, x, y):
         # TODO: adicionar métricas do próprio Sklearn
         pass
```

### Comparing `radial_basis_function-0.2.0/README.md` & `radial_basis_function-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 metrics.balanced_accuracy_score(Y_Treino, predicao)
 metrics.f1_score(Y_Treino, predicao)
 
 ```
 
 ## Radial Basis Function
 
-A estrutura básica de um Radial Basis Function (RBF Network) consiste em três componentes principais: as funções de base radial, os pesos associados a essas funções e uma camada de saída linear solucionada pela matriz pseudo-inversa. 
+A estrutura básica de um Radial Basis Function (RBF Network) consiste em três componentes principais: as funções de base radial, os pesos associados a essas funções e uma camada de saída linear solucionada pela matriz pseudo-inversa.
 
 Para usar a dependencia no código python, foram criados os métodos fit e predict com nome inspirados nos moldes do Sklearn.
 
 ```
 
 # Instancia do modelo
 modelo_rbf = radial_basis_function.RadialBasisFunction()
```

### Comparing `radial_basis_function-0.2.0/PKG-INFO` & `radial_basis_function-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radial-basis-function
-Version: 0.2.0
+Version: 0.3.0
 Summary: Radial Basis Function e Multiplicação de Matriz Pseudo-Inversa, para modelos de Regressão e Multi-Classificatórios.
 Home-page: https://github.com/VictorVenites/Radial-Basis-Function
 License: MIT
 Keywords: rbf,Radial Basis Function,Pseudo-Inverse Matrix,Matriz Pseudo-Inversa,Victor Venites
 Author: Victor Venites
 Author-email: contato@victorvenites.com
 Maintainer: Victor Venites
@@ -69,15 +69,15 @@
 metrics.balanced_accuracy_score(Y_Treino, predicao)
 metrics.f1_score(Y_Treino, predicao)
 
 ```
 
 ## Radial Basis Function
 
-A estrutura básica de um Radial Basis Function (RBF Network) consiste em três componentes principais: as funções de base radial, os pesos associados a essas funções e uma camada de saída linear solucionada pela matriz pseudo-inversa. 
+A estrutura básica de um Radial Basis Function (RBF Network) consiste em três componentes principais: as funções de base radial, os pesos associados a essas funções e uma camada de saída linear solucionada pela matriz pseudo-inversa.
 
 Para usar a dependencia no código python, foram criados os métodos fit e predict com nome inspirados nos moldes do Sklearn.
 
 ```
 
 # Instancia do modelo
 modelo_rbf = radial_basis_function.RadialBasisFunction()
```

