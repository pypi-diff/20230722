# Comparing `tmp/python_bcb-0.1.9.tar.gz` & `tmp/python_bcb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_bcb-0.1.9.tar", max compression
+gzip compressed data, was "python_bcb-0.2.0.tar", max compression
```

## Comparing `python_bcb-0.1.9.tar` & `python_bcb-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    16003 2022-09-11 20:49:09.883282 python_bcb-0.1.9/bcb/__init__.py
--rw-r--r--   0        0        0     5888 2022-09-10 20:51:28.515769 python_bcb-0.1.9/bcb/currency.py
--rw-r--r--   0        0        0    15443 2022-09-10 20:51:40.176864 python_bcb-0.1.9/bcb/odata.py
--rw-r--r--   0        0        0     4513 2022-09-13 08:18:17.540281 python_bcb-0.1.9/bcb/sgs.py
--rw-r--r--   0        0        0     1089 2022-09-10 20:51:53.559187 python_bcb-0.1.9/bcb/utils.py
--rw-r--r--   0        0        0     1070 2021-01-16 19:16:53.504736 python_bcb-0.1.9/LICENSE
--rw-r--r--   0        0        0      761 2023-06-26 20:21:16.356313 python_bcb-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2065 2022-03-30 10:14:29.317008 python_bcb-0.1.9/README.md
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 python_bcb-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      386 2023-07-07 08:40:06.179489 python_bcb-0.2.0/bcb/__init__.py
+-rw-r--r--   0        0        0     6114 2023-07-06 09:47:23.877338 python_bcb-0.2.0/bcb/currency.py
+-rw-r--r--   0        0        0      380 2023-07-07 10:19:46.549769 python_bcb-0.2.0/bcb/odata/__init__.py
+-rw-r--r--   0        0        0    18136 2023-07-22 10:04:27.606046 python_bcb-0.2.0/bcb/odata/api.py
+-rw-r--r--   0        0        0    15860 2023-07-22 10:30:49.143965 python_bcb-0.2.0/bcb/odata/framework.py
+-rw-r--r--   0        0        0     4513 2022-09-13 08:18:17.540281 python_bcb-0.2.0/bcb/sgs.py
+-rw-r--r--   0        0        0     1089 2022-09-10 20:51:53.559187 python_bcb-0.2.0/bcb/utils.py
+-rw-r--r--   0        0        0     1070 2021-01-16 19:16:53.504736 python_bcb-0.2.0/LICENSE
+-rw-r--r--   0        0        0      777 2023-07-22 10:42:16.011585 python_bcb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2065 2023-06-27 00:00:48.547931 python_bcb-0.2.0/README.md
+-rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 python_bcb-0.2.0/PKG-INFO
```

### Comparing `python_bcb-0.1.9/bcb/__init__.py` & `python_bcb-0.2.0/bcb/odata/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from .odata import (
+from .framework import (
     ODataEntitySet,
     ODataFunctionImport,
     ODataQuery,
     ODataPropertyFilter,
     ODataPropertyOrderBy,
     ODataProperty,
     ODataService,
 )
 import pandas as pd
 
-
 OLINDA_BASE_URL = "https://olinda.bcb.gov.br/olinda/servico"
 
 
 class EndpointMeta(type):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -26,25 +25,79 @@
         elif isinstance(entity, ODataFunctionImport):
             for name, prop in entity.entity_set.entity.properties.items():
                 setattr(obj, name, prop)
         return obj
 
 
 class EndpointQuery(ODataQuery):
+    _DATE_COLUMN_NAMES_BY_ENDPOINT = {
+        "IfDataCadastro": {"Data": "%Y%m"}
+    }
+    _DATE_COLUMN_NAMES = {
+        "Data",
+        "dataHoraCotacao",
+        "InicioPeriodo",
+        "FimPeriodo",
+        "DataVigencia",
+    }
+
     def collect(self):
-        data = super().collect()
-        return pd.DataFrame(data["value"])
+        raw_data = super().collect()
+        data = pd.DataFrame(raw_data["value"])
+        if not self._raw:
+            for col in self._DATE_COLUMN_NAMES:
+                if self.entity.name in self._DATE_COLUMN_NAMES_BY_ENDPOINT and col in self._DATE_COLUMN_NAMES_BY_ENDPOINT[self.entity.name]:
+                    data[col] = pd.to_datetime(data[col], format=self._DATE_COLUMN_NAMES_BY_ENDPOINT[self.entity.name][col])
+                elif col in data.columns:
+                    data[col] = pd.to_datetime(data[col])
+        return data
 
 
 class Endpoint(metaclass=EndpointMeta):
+    """
+    Classe que representa os tipos de *endpoints* de APIs OData.
+
+    As APIs OData têm 2 tipos de *endpoints*: *entity sets* e *functions imports*.
+    Esta classe provê todos os mecanismos para acessar tanto os *entity sets* quanto os *functions imports* e
+    realizar consultas em através de suas APIs de maneira transparente.
+
+    Esta classe não deveria ser instanciada diretamente.
+    Objetos dessa classe são retornados pelo método
+    :py:meth:`bcb.odata.api.BaseODataAPI.get_endpoint` das classes que herdam
+    :py:class:`bcb.odata.api.BaseODataAPI`.
+    """
     def __init__(self, entity, url):
+        """
+        Construtor da classe Endpoint.
+
+        Parameters
+        ----------
+        entity : bcb.odata.api.ODataEntity
+            Objeto que representa um *entity set* ou um *function import*.
+            Obtidos da classe ``bcb.odata.framework.ODataService``.
+        url : str
+            URL da API OData.
+        """
         self._entity = entity
         self._url = url
 
     def get(self, *args, **kwargs):
+        """
+        Executa a consulta na API OData e retorna o resultado.
+
+        Parameters
+        ----------
+        *args : argumentos para a consulta
+
+        **kwargs : argumentos para a consulta
+
+        Returns
+        -------
+        pd.DataFrame: resultado da consulta
+        """
         _query = EndpointQuery(self._entity, self._url)
         for arg in args:
             if isinstance(arg, ODataPropertyFilter):
                 _query.filter(arg)
             elif isinstance(arg, ODataPropertyOrderBy):
                 _query.orderby(arg)
             elif isinstance(arg, ODataProperty):
@@ -61,17 +114,24 @@
                 _query.parameters(**{k: val})
         _query.format("application/json")
 
         if verbose:
             _query.show()
         data = _query.collect()
         _query.reset()
-        return pd.DataFrame(data["value"])
+        return data
 
     def query(self):
+        """
+        Retorna uma instância de EndpointQuery através da qual se construirá a consulta na API OData.
+
+        Returns
+        -------
+        bcb.odata.api.EndpointQuery
+        """
         return EndpointQuery(self._entity, self._url)
 
 
 class BaseODataAPI:
     """
     Classe que abstrai qualquer API OData
 
@@ -114,15 +174,15 @@
         ----------
 
         endpoint : str
             nome do endpoint
 
         Returns
         -------
-        bcb.Endpoint
+        bcb.odata.api.Endpoint
             Retorna o *endpoint* referente ao nome fornecido
 
         Raises
         ------
         ValueError
             Se o *endpoint* fornecido é errado.
         """
@@ -138,16 +198,14 @@
 
     Uma boa alternativa para acessar APIs que ainda
     não possuem implementação específica.
     """
 
     def __init__(self, url):
         """
-        ODataAPI construtor
-
         Parameters
         ----------
 
         url : str
             URL de API OData
 
             Em geral tem o padrão
@@ -259,15 +317,15 @@
     """
 
     BASE_URL = f"{OLINDA_BASE_URL}/IFDATA/versao/v1/odata/"
 
 
 class TaxaJuros(BaseODataAPI):
     """
-    Taxas de juros de operações de crédito por instituição financeira – Médias
+    Taxas de juros de operações de crédito por instituição financeira - Médias
     dos últimos 5 dias
 
     As taxas de juros por instituição financeira apresentadas nesse conjunto de
     tabelas representam médias aritméticas das taxas de juros pactuadas nas
     operações realizadas nos cinco dias úteis referidos em cada publicação,
     ponderadas pelos respectivos valores contratados.
```

### Comparing `python_bcb-0.1.9/bcb/currency.py` & `python_bcb-0.2.0/bcb/currency.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from lxml import html
 
 import pandas as pd
 import numpy as np
 
 from .utils import Date
 
+"""
+O módulo :py:mod:`bcb.currency` tem como objetivo fazer consultas no site do conversor de moedas do BCB.
+"""
+
 
 def _currency_url(currency_id, start_date, end_date):
     start_date = Date(start_date)
     end_date = Date(end_date)
     url = (
         "https://ptax.bcb.gov.br/ptax_internet/consultaBoletim.do?"
         "method=gerarCSVFechamentoMoedaNoPeriodo&"
@@ -60,18 +64,21 @@
         return res
     else:
         return _get_valid_currency_list(_date - timedelta(1), 0)
 
 
 def get_currency_list():
     """
-    Return a DataFrame with information of all available currencies.
+    Listagem com todas as moedas disponíveis na API e suas configurações de paridade.
 
-    :return: DataFrame
-    :rtype: pandas.DataFrame
+    Returns
+    -------
+
+    DataFrame :
+        Tabela com a listagem de moedas disponíveis.
     """
     if CACHE.get("TEMP_FILE_CURRENCY_LIST") is not None:
         return CACHE.get("TEMP_FILE_CURRENCY_LIST")
     else:
         res = _get_valid_currency_list(date.today())
         df = pd.read_csv(StringIO(res.text), delimiter=";")
         df.columns = [
@@ -156,15 +163,15 @@
         Define se os índices de coluna são agrupados por ``symbol`` ou
         por ``side``.
 
     Returns
     -------
 
     DataFrame :
-        série temporal.
+        Série temporal com cotações diárias das moedas solicitadas.
     """
     if isinstance(symbols, str):
         symbols = [symbols]
     dss = []
     for symbol in symbols:
         df1 = _get_symbol(symbol, start, end)
         if df1 is not None:
```

### Comparing `python_bcb-0.1.9/bcb/odata.py` & `python_bcb-0.2.0/bcb/odata/framework.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,34 +151,42 @@
     def __init__(self, obj, order):
         self.obj = obj
         self.order = order
 
     def __str__(self):
         return f"{self.obj.name} {self.order}"
 
+    def __repr__(self):
+        return f"<{str(self)}>"
+
 
 class ODataPropertyFilter:
     def __init__(self, obj, oth, operator):
         self.obj = obj
         self.other = oth
         self.operator = operator
 
     def statement(self):
         if self.obj.type == "Edm.Decimal":
             return f"{self.obj.name} {self.operator} {float(self.other)}"
         elif self.obj.type == "Edm.Int32":
             return f"{self.obj.name} {self.operator} {int(self.other)}"
         elif self.obj.type == "Edm.String":
             return f"{self.obj.name} {self.operator} '{str(self.other)}'"
+        elif self.obj.type == "Edm.Date":
+            return f"{self.obj.name} {self.operator} {self.other.strftime('%Y-%m-%d')}"
         else:
             return f"{self.obj.name} {self.operator} '{self.other}'"
 
     def __str__(self):
         return self.statement()
 
+    def __repr__(self):
+        return f"<filter: {str(self)}>"
+
 
 class ODataProperty:
     def __init__(self, **kwargs):
         self.data = kwargs
 
     @property
     def name(self):
@@ -210,15 +218,15 @@
     def __le__(self, other):
         return ODataPropertyFilter(self, other, "le")
 
     def __eq__(self, other):
         return ODataPropertyFilter(self, other, "eq")
 
     def __repr__(self):
-        return f"<Property {self.name}>"
+        return f"<Property {self.name}<{self.ftype}>>"
 
 
 class ODataFunction:
     def __init__(self, **kwargs):
         self.name = kwargs["Name"]
         self.parameters = kwargs["parameters"]
         self.return_type = kwargs["return_type"]
@@ -390,14 +398,15 @@
         self.entity = entity
         self.base_url = url
         self._params = {}
         self.function_parameters = {}
         self._filter = []
         self._select = []
         self._orderby = []
+        self._raw = False
         self.is_function = isinstance(entity, ODataFunctionImport)
         if self.is_function:
             self.function_parameters = {
                 p.name: None for p in self.entity.function.parameters
             }
 
     def odata_url(self):
@@ -444,16 +453,20 @@
         return self
 
     def select(self, *args):
         if len(args):
             self._select.extend(args)
         return self
 
+    def raw(self):
+        self._raw = True
+        return self
+
     def _build_parameters(self):
-        params = {"$format": "json"}
+        params = {"$format": self._params.get("$format", "json")}
         if len(self._filter):
             _filter = " and ".join(str(f) for f in self._filter)
             params["$filter"] = _filter
         if len(self._orderby):
             _orderby = ",".join(str(f) for f in self._orderby)
             params["$orderby"] = _orderby
         if len(self._select):
@@ -464,26 +477,28 @@
 
     def reset(self):
         self._filter = []
         self._orderby = []
         self._params = {}
 
     def collect(self):
+        return json.loads(self.text())
+
+    def text(self):
         params = self._build_parameters()
         if self.is_function and len(self.function_parameters):
             for p in self.entity.function.parameters:
                 val = self.function_parameters[p.name]
                 if p.required and val is None:
                     raise ValueError("Parameter not set: " + p.name)
                 params["@" + p.name] = p.format(val)
         qs = "&".join([f"{quote(k)}={quote(str(v))}" for k, v in params.items()])
         headers = {"OData-Version": "4.0", "OData-MaxVersion": "4.0"}
         res = httpx.get(self.odata_url() + "?" + qs, headers=headers, timeout=60.0)
-        logging.debug(res.text)
-        return json.loads(res.text)
+        return res.text
 
     def show(self):
         print(f"URL:")
         print(f"  {self.odata_url()}")
         if self.is_function and len(self.function_parameters):
             print("Function Parameters:")
             for p in self.entity.function.parameters:
```

### Comparing `python_bcb-0.1.9/bcb/sgs.py` & `python_bcb-0.2.0/bcb/sgs.py`

 * *Files identical despite different names*

### Comparing `python_bcb-0.1.9/bcb/utils.py` & `python_bcb-0.2.0/bcb/utils.py`

 * *Files identical despite different names*

### Comparing `python_bcb-0.1.9/LICENSE` & `python_bcb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_bcb-0.1.9/pyproject.toml` & `python_bcb-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "python-bcb"
-version = "0.1.9"
+version = "0.2.0"
 description = ""
 authors = ["wilsonfreitas <wilson.freitas@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bcb"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.24.0"
 lxml = "^4.9.2"
 pandas = "^2.0.0"
 requests = "^2.31.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
+flaky = "^3.7.0"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.1.1"
 pydata-sphinx-theme = "^0.10.1"
 matplotlib = "^3.5.3"
 ipython = "^8.14.0"
 furo = "^2022.6.21"
 
-
 [tool.poetry.group.dev.dependencies]
 pycodestyle = "^2.9.1"
 ipykernel = "^6.15.2"
 black = {version = "^22.8.0", allow-prereleases = true}
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `python_bcb-0.1.9/README.md` & `python_bcb-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 Utiliza o webservice do SGS
 (`Sistema Gerenciador de Séries Temporais <https://www3.bcb.gov.br/sgspub/>`_)
 para obter os dados.
 
 ## Conversor de Moedas
 
 Implementado no módulo `currency`, um conjunto de funções que realiza webscraping
-no site do [Conversos de Moedas](https://www.bcb.gov.br/conversao)
+no site do [Conversor de Moedas](https://www.bcb.gov.br/conversao)
 do Banco Central, possível obter séries temporais de frequência diária
 de diversas moedas.
 
 ## Moedas OData
 
 O Banco Central disponibiliza diversas informações em APIs que
 seguem o padrão [OData](https://odata.org).
```

### Comparing `python_bcb-0.1.9/PKG-INFO` & `python_bcb-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bcb
-Version: 0.1.9
+Version: 0.2.0
 Summary: 
 Author: wilsonfreitas
 Author-email: wilson.freitas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -49,15 +49,15 @@
 Utiliza o webservice do SGS
 (`Sistema Gerenciador de Séries Temporais <https://www3.bcb.gov.br/sgspub/>`_)
 para obter os dados.
 
 ## Conversor de Moedas
 
 Implementado no módulo `currency`, um conjunto de funções que realiza webscraping
-no site do [Conversos de Moedas](https://www.bcb.gov.br/conversao)
+no site do [Conversor de Moedas](https://www.bcb.gov.br/conversao)
 do Banco Central, possível obter séries temporais de frequência diária
 de diversas moedas.
 
 ## Moedas OData
 
 O Banco Central disponibiliza diversas informações em APIs que
 seguem o padrão [OData](https://odata.org).
```

