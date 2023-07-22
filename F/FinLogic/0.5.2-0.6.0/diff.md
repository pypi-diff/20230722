# Comparing `tmp/finlogic-0.5.2.tar.gz` & `tmp/finlogic-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.5.2.tar", last modified: Sat Jun 17 11:00:14 2023, max compression
+gzip compressed data, was "finlogic-0.6.0.tar", last modified: Sat Jul 22 08:35:15 2023, max compression
```

## Comparing `finlogic-0.5.2.tar` & `finlogic-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.5.2/LICENSE
--rw-r--r--   0        0        0     9039 2023-06-10 09:56:21.909374 finlogic-0.5.2/README.md
--rw-r--r--   0        0        0      420 2023-06-17 10:42:32.134009 finlogic-0.5.2/finlogic/__init__.py
--rw-r--r--   0        0        0    20572 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/company.py
--rw-r--r--   0        0        0      718 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/config.py
--rw-r--r--   0        0        0    10639 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/cvm.py
--rw-r--r--   0        0        0     8060 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/data_manager.py
--rw-r--r--   0        0        0     8463 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/indicators.py
--rw-r--r--   0        0        0      708 2023-06-04 17:35:17.287141 finlogic-0.5.2/finlogic/language.py
--rw-r--r--   0        0        0     6685 2023-06-17 10:40:57.986130 finlogic-0.5.2/finlogic/reports.py
--rw-r--r--   0        0        0     1017 2023-06-17 11:00:14.741943 finlogic-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     3284 2023-06-08 13:02:11.720947 finlogic-0.5.2/tests/test_company.py
--rw-r--r--   0        0        0      923 2023-06-17 10:40:57.986130 finlogic-0.5.2/tests/test_data.py
--rw-r--r--   0        0        0    11118 1970-01-01 00:00:00.000000 finlogic-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.6.0/LICENSE
+-rw-r--r--   0        0        0     9812 2023-07-22 08:24:02.186627 finlogic-0.6.0/README.md
+-rw-r--r--   0        0        0      378 2023-07-22 08:24:02.222628 finlogic-0.6.0/finlogic/__init__.py
+-rw-r--r--   0        0        0    20400 2023-07-22 08:24:02.223628 finlogic-0.6.0/finlogic/company.py
+-rw-r--r--   0        0        0     7580 2023-07-22 08:24:02.223628 finlogic-0.6.0/finlogic/data.py
+-rw-r--r--   0        0        0     8017 2023-07-22 08:24:02.223628 finlogic-0.6.0/finlogic/indicators.py
+-rw-r--r--   0        0        0      949 2023-07-22 08:35:15.041046 finlogic-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     2880 2023-07-22 08:24:02.223628 finlogic-0.6.0/tests/test_company.py
+-rw-r--r--   0        0        0      709 2023-07-22 08:24:02.223628 finlogic-0.6.0/tests/test_data.py
+-rw-r--r--   0        0        0    11799 1970-01-01 00:00:00.000000 finlogic-0.6.0/PKG-INFO
```

### Comparing `finlogic-0.5.2/LICENSE` & `finlogic-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.5.2/README.md` & `finlogic-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 <!-- [![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)" -->
 
 ## FinLogic: finance toolkit for listed Brazilian companies.
 
 ---
 
-**FinLogic** offers a Pythonic way to analyze the financial data of companies listed in Brazil, using information made publicly available by the local securities market authority, CVM. FinLogic processes approximately 20 million accounting entries using Pandas, and constructs a local DataFrame for ultra-fast access to this information.
+**FinLogic** provides a Pythonic approach to analyzing the financial data of companies listed in Brazil. The library pre-processes approximately 50 million accounting entries from the local securities market authority data repository.
+
+The extensive pre-processing stage is automated using Polars within an AWS Lambda Function, and it is scheduled to check for updates overnight. After the CVM repository data is updated and pre-processed, the job saves the cleaned data in FinLogic data folder on GitHub. This arrangement allows the library to access the data quickly and easily.
 
 ---
 
 ## Installation
 
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
@@ -25,66 +27,75 @@
 pip install finlogic
 ```
 
 ### Requirements
 
 - [Python](https://www.python.org) \>= 3.10
 - [Pandas](https://github.com/pydata/pandas) \>= 1.5.0
-- [Requests](http://docs.python-requests.org/en/master/) \>= 2.30.0
-- [tqdm](https://github.com/tqdm/tqdm) \>= 4.1.0
-- [Zstandard](https://python-zstandard.readthedocs.io/en/latest/) \>= 0.21.0
 
 ---
 
 ## Quick Start
 
-### Create FinLogic Database
+### Load FinLogic Data
 
-The 'update' function is responsible for downloading and updating raw financial data from the CVM, processing approximately 20 million accounting entries, and storing them for local data analysis. During the initial run, the process might take some minutes, depending on the CVM server connection and local CPU power. For subsequent updates, only the updated CVM files will be downloaded and processed, which should expedite the operation.
+The 'load' function is responsible for downloading and reading the financial data stored on GitHub data folder.
 
 ```python
 >>> import finlogic as fl
 
-# Compile FinLogic database for the first time:
->>> fl.update()
-
-Updating CVM raw files...
-...
-FinLogic database updated ✅
+# Load the accounting data in memory:
+>>> fl.load()
+```
+    Loading "language" data...
+    Loading trading data...
+    Loading financials data...
+    Building indicators data...
+    ✔ FinLogic is ready!
 
+```python
 # Show database info:
 >>> fl.info()
 ```
 
-|                     |       FinLogic Info |
-| :------------------ | ------------------: |
-| data_path           |   .../finlogic/data |
-| data_size           |             12.1 MB |
-| last_modified_on    | 2023-04-20 07:29:08 |
-| accounting_entries  |           2,806,635 |
-| number_of_reports   |              11,635 |
-| first_report        |          2009-01-31 |
-| last_report         |          2023-03-31 |
-| number_of_companies |               1,139 |
+|                     |                    FinLogic Info |
+| :------------------ | -------------------------------: |
+| data_url            | https://raw.githubusercontent... |
+| memory_usage        |                         255.1 MB |
+| accounting_entries  |                          755,635 |
+| number_of_reports   |                            2,635 |
+| first_report        |                       2009-01-31 |
+| last_report         |                       2023-03-31 |
+| number_of_companies |                              210 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
 
-|     | name_id                                | cvm_id | tax_id             |
-| --: | :------------------------------------- | -----: | :----------------- |
-|   0 | 3R PETROLEUM ÓLEO E GÁS S.A.           |  25291 | 12.091.809/0001-55 |
-|   1 | PETRO RIO S.A.                         |  22187 | 10.629.105/0001-68 |
-|   2 | PETROBRAS DISTRIBUIDORA S/A            |  24295 | 34.274.233/0001-02 |
-|   3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |   9512 | 33.000.167/0001-01 |
-|   4 | PETROLEO LUB DO NORDESTE SA            |   9520 | 07.275.159/0001-68 |
-|   5 | PETRORECÔNCAVO S.A.                    |  25780 | 03.342.704/0001-30 |
-|   6 | PRONOR PETROQUIMICA SA                 |   9784 | 13.552.070/0001-02 |
-|   7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |   9989 | 33.412.081/0001-96 |
+| name_id                            | cvm_id | tax_id             | segment        | is_restructuring | most_traded_stock |
+|:-----------------------------------|-------:|:-------------------|:---------------|:-----------------|:------------------|
+| PETROLEO BRASILEIRO S.A. PETROBRAS |   9512 | 33.000.167/0001-01 | exploration... | False            | PETR4             |
+| 3R PETROLEUM ÓLEO E GÁS S.A.       |  25291 | 12.091.809/0001-55 | exploration... | False            | RRRP3             |
+| PETRORECÔNCAVO S.A.                |  25780 | 03.342.704/0001-30 | exploration... | False            | RECV3             |
+
+```python
+# Search company by segment:
+fl.search_company(search_by="segment", search_value="electric")
+```
+| name_id                                | cvm_id | tax_id             | segment            | is_restructuring | most_traded_stock |
+|:---------------------------------------|-------:|:-------------------|:-------------------|:-----------------|:------------------|
+| CENTRAIS ELET BRAS S.A. - ELETROBRAS   |   2437 | 00.001.180/0001-26 | electric utilities | False            | ELET3             |
+| CIA ENERGETICA DE MINAS GERAIS - CEMIG |   2453 | 17.155.730/0001-64 | electric utilities | False            | CMIG4             |
+| CIA PARANAENSE DE ENERGIA - COPEL      |  14311 | 76.483.817/0001-20 | electric utilities | False            | CPLE6             |
+| CIA ENERGETICA DO CEARA - COELCE       |  14869 | 07.047.251/0001-70 | electric utilities | False            | COCE5             |
+| ENERGISA S.A.                          |  15253 | 00.864.214/0001-06 | electric utilities | False            | ENGI11            |
+| NEOENERGIA S.A.                        |  15539 | 01.083.200/0001-18 | electric utilities | False            | NEOE3             |
+| ENGIE BRASIL ENERGIA S.A.              |  17329 | 02.474.103/0001-19 | electric utilities | False            | EGIE3             |
+...
 
 ### The Company Class
 
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
@@ -107,16 +118,15 @@
 | CVM ID                     |                               9512 |
 | Tax ID (CNPJ)              |                 33.000.167/0001-01 |
 | Total Accounting Rows      |                              3,292 |
 | Selected Tax Rate          |                               0.34 |
 | Selected Accounting Method |                       consolidated |
 | Selected Accounting Unit   |                      1,000,000,000 |
 | First Report               |                         2009-12-31 |
-| Last Report                |                         2021-12-31 |
-| Last Report Type           |                          quarterly |
+| Last Report                |                         2023-03-31 |
 
 ```python
 # Show company assets in Brazilian currency:
 >>> petro.report(report_type='assets')
 ...
 # Show company liabilities with custom arguments:
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
@@ -151,33 +161,43 @@
 | 2.02.01.03 | Financiamento por Arrendamento |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Show company main indicators:
 >>> petro.indicators(num_years=3)
 ```
 
-| Company Financial Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 |
-| :--------------------------- | ---------: | ---------: | ---------: |
-| revenues                     |    302.245 |    272.069 |    452.668 |
-| operating_cash_flow          |    101.766 |    148.106 |    203.126 |
-| ebitda                       |    140.203 |    107.926 |    273.879 |
-| ebit                         |     81.701 |     49.621 |    210.831 |
-| net_income                   |     40.970 |      6.246 |    107.264 |
-| total_cash                   |     33.294 |     64.280 |     62.040 |
-| total_debt                   |    351.161 |    392.548 |    327.818 |
-| net_debt                     |    317.867 |    328.268 |    265.778 |
-| working_capital              |     -4.046 |      6.036 |     33.334 |
-| invested_capital             |    617.004 |    639.418 |    655.359 |
-| return_on_assets             |      0.062 |      0.035 |      0.140 |
-| return_on_equity             |      0.144 |      0.020 |      0.344 |
-| roic                         |      0.097 |      0.053 |      0.217 |
-| gross_margin                 |      0.403 |      0.455 |      0.485 |
-| ebitda_margin                |      0.463 |      0.396 |      0.605 |
-| operating_margin             |      0.178 |      0.120 |      0.307 |
-| net_margin                   |      0.135 |      0.022 |      0.236 |
+| 2021-12-31 | 2022-12-31 | 2023-03-31 |
+|-----------:|-----------:|-----------:|
+|    972.951 |    976.709 |    978.577 |
+|    168.247 |    163.052 |    157.194 |
+|     62.04  |     56.193 |     66.906 |
+|     33.334 |     -0.679 |     28.744 |
+|    655.359 |    588.895 |    607.53  |
+|    134.913 |    163.731 |    128.45  |
+|    327.818 |    280.703 |    271.031 |
+|    265.778 |    224.51  |    204.125 |
+|    389.581 |    364.385 |    403.405 |
+|    452.668 |    641.256 |    638.683 |
+|    219.637 |    334.1   |    332.645 |
+|    107.264 |    189.005 |    182.529 |
+|    273.879 |    362.457 |    355.838 |
+|    210.831 |    294.255 |    289.054 |
+|    151.575 |    274.998 |    263.614 |
+|    -44.311 |    -85.993 |    -81.085 |
+|    203.126 |    255.41  |    256.345 |
+|     63.048 |     68.202 |     66.784 |
+|      0.292 |      0.312 |      0.307 |
+|      0.141 |      0.199 |      0.192 |
+|      0.397 |      0.515 |      0.453 |
+|      0.214 |      0.312 |      0.309 |
+|      0.485 |      0.521 |      0.520 |
+|      0.605 |      0.565 |      0.557 |
+|      0.465 |      0.458 |      0.452 |
+|      0.236 |      0.294 |      0.285 |
+|      8.18  |     14.44  |     13.95  |
 
 ---
 
 P.S.: All contributors are welcome, from beginner to advanced.
 
 **Felipe Costa and Carlos Carvalho**
```

### Comparing `finlogic-0.5.2/finlogic/company.py` & `finlogic-0.6.0/finlogic/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,16 @@
     yet). Please set your engine to python manually. That means that the query
     method has to use engine='python' to work with category dtype. N.B. Only
     FinLogic Dataframe uses category dtype for efficiency.
 
 """
 from typing import Literal
 import pandas as pd
-from .language import language_df
-from . import reports as rep
-from . import indicators as ind
+from . import data as dt
+from . import indicators as ic
 
 
 class Company:
     """A class to represent a company financial data.
 
      This class provides methods to create financial reports and to calculate
      financial indicators based on a company's accounting data. The class also
@@ -71,14 +70,19 @@
         self.acc_unit = acc_unit
         self.tax_rate = tax_rate
         self.language = language
         self._initialized = True
         # Only set _df after identifier, is_consolidated and acc_unit are setted
         self._set_df()
 
+    @staticmethod
+    def convert_to_sl(expr: str) -> str:
+        """Converts a string to a single line."""
+        return expr.replace("\n", "")
+
     @property
     def identifier(self) -> int | str:
         """Set a unique identifier to select the company in FinLogic Database.
 
         This method sets the company's CVM and fiscal ID based on a given
         identifier. The identifier can be either the CVM ID or the Fiscal ID
         (CNPJ). If the identifier is not found in the database, a KeyError is
@@ -98,15 +102,15 @@
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier: int | str):
         # Create custom data frame for ID selection
         df = (
-            rep.get_reports()[["cvm_id", "tax_id", "name_id"]]
+            dt.FINANCIALS_DF[["cvm_id", "tax_id", "name_id"]]
             .query("cvm_id == @identifier or tax_id == @identifier")
             .drop_duplicates(ignore_index=True)
         )
         if not df.empty:
             self._cvm_id = df.loc[0, "cvm_id"]
             self.tax_id = df.loc[0, "tax_id"]
             self.name_id = df.loc[0, "name_id"]
@@ -248,30 +252,24 @@
 
     def _set_df(self) -> pd.DataFrame:
         """Sets the company data frame.
 
         This method creates a dataframe with the company's financial
         statements.
         """
-        df = (
-            rep.get_reports()
-            .query(
-                "cvm_id == @self._cvm_id and \
-                 is_consolidated == @self._is_consolidated"
-            )
-            .reset_index(drop=True)
-        )
+        expr = "cvm_id == @self._cvm_id and is_consolidated == @self._is_consolidated"
+        df = dt.FINANCIALS_DF.query(expr).reset_index(drop=True)
 
         # Convert category columns back to string
         columns = df.columns
         cat_cols = [c for c in columns if df[c].dtype == "category"]
         df[cat_cols] = df[cat_cols].astype("string")
 
         # Adjust for unit change only where it is not EPS (acc_code 8...)
-        mask = ~df["acc_code"].str.startswith("8")
+        mask = ~df["acc_code"].str.startswith("3.99")
         df.loc[mask, "acc_value"] = df.loc[mask, "acc_value"] / self._acc_unit
 
         self._first_period = df["period_end"].min()
         self._last_period = df["period_end"].max()
 
         # Not necessarily there will be a quarterly report for the last period
         self._last_annual = df.query("is_annual")["period_end"].max()
@@ -307,15 +305,14 @@
             "Selected Accounting Method": "consolidated"
             if self._is_consolidated
             else "separate",
             "Selected Accounting Unit": self._acc_unit,
             "Selected Tax Rate": self._tax_rate,
             "First Report": self._first_period.strftime("%Y-%m-%d"),
             "Last Report": self._last_period.strftime("%Y-%m-%d"),
-            "Last Report Type": self._last_period_type,
         }
         s = pd.Series(company_info)
         s.name = "Company Info"
         return s.to_frame()
 
     @staticmethod
     def _build_report_index(dfi: pd.DataFrame) -> pd.DataFrame:
@@ -378,17 +375,15 @@
             "liabilities",
             "debt",
             "current_liabilities",
             "non_current_liabilities",
             "liabilities_and_equity",
             "equity",
             "income_statement",
-            "comprehensive_income",
             "cash_flow",
-            "added_value",
             "earnings_per_share",
         ],
         acc_level: Literal[0, 1, 2, 3, 4] = 0,
         num_years: int = 0,
     ) -> pd.DataFrame:
         """Generate an accounting report for the company.
 
@@ -445,15 +440,15 @@
         class MyDict(dict):
             """Custom dictionary class to return key if key is not found."""
 
             def __missing__(self, key):
                 return "(pt) " + key
 
         if self._language == "English":
-            _pten_dict = dict(language_df.values)
+            _pten_dict = dict(dt.LANGUAGE_DF.values)
             _pten_dict = MyDict(_pten_dict)
             df["acc_name"] = df["acc_name"].map(_pten_dict)
 
         """
         Filter dataframe for selected acc_code
         df['acc_code'].str[0].unique() -> [1, 2, 3, 4, 5, 6, 7]
         The first part of 'acc_code' is the report type
@@ -476,18 +471,16 @@
             "liabilities": ("2.01", "2.02"),
             "debt": ("2.01.04", "2.02.01"),
             "current_liabilities": ("2.01"),
             "non_current_liabilities": ("2.02"),
             "liabilities_and_equity": ("2"),
             "equity": ("2.03"),
             "income_statement": ("3"),
-            "comprehensive_income": ("4"),
+            "earnings_per_share": ("3.99"),
             "cash_flow": ("6"),
-            "added_value": ("7"),
-            "earnings_per_share": ("8"),
         }
         acc_codes = report_types[report_type]  # noqa
         df.query("acc_code.str.startswith(@acc_codes)", inplace=True)
         df.reset_index(drop=True, inplace=True)
 
         # Show only selected years
         all_periods = sorted(df["period_end"].drop_duplicates())
@@ -532,16 +525,16 @@
             num_years: Number of years to consider for calculation. If 0, use
                 all available years. Defaults to 0.
 
         Returns:
             pd.DataFrame: Dataframe containing calculated financial indicators.
         """
         expr = "cvm_id == @self._cvm_id and is_consolidated == @self._is_consolidated"
-        dfi = ind.get_indicators().query(expr)
-        dfo = ind.format_indicators(dfi, unit=self._acc_unit)
+        df = dt.INDICATORS_DF.query(expr)
+        df = ic.format_indicators(df, unit=self._acc_unit)
         # Columns cvm_id and is_consolidated are redundant for the Company class
-        dfo.drop(columns=["cvm_id", "is_consolidated"], inplace=True)
+        df.drop(columns=["cvm_id", "is_consolidated"], inplace=True)
         # Show only the selected number of years
         if num_years > 0:
-            dfo = dfo[dfo.columns[-num_years:]].copy()
+            df = df[df.columns[-num_years:]].copy()
 
-        return dfo
+        return df
```

### Comparing `finlogic-0.5.2/finlogic/data_manager.py` & `finlogic-0.6.0/finlogic/data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,69 @@
 """Finlogic manager module.
 
 This module provides upper level functions to handle financial data from the CVM
 Portal. It allows updating, processing and consolidating financial statements,
 as well as searching for company names in the FinLogic Database and retrieving
 information about the database itself.
 """
-from pathlib import Path
 from typing import Literal
-from datetime import datetime
 import pandas as pd
-from . import config as cfg
-from . import cvm
-from . import language as lng
-from . import reports as rep
 from . import indicators as ind
 
 CHECKMARK = "\033[32m\u2714\033[0m"
+# Load last session data
+TRADE_DATA_URL = (
+    "https://raw.githubusercontent.com/crdcj/FinLogic/main/data/trades.csv.gz"
+)
+TRADED_FINANCIALS_URL = "https://raw.githubusercontent.com/crdcj/FinLogic/main/data/traded_companies_financials.csv.gz"
+NOT_TRADED_FINANCIALS_URL = "https://raw.githubusercontent.com/crdcj/FinLogic/main/data/not_traded_companies_financials.csv.gz"
+LANGUAGE_DATA_URL = (
+    "https://raw.githubusercontent.com/crdcj/FinLogic/main/data/pten_df.csv.gz"
+)
+FINANCIALS_DF = pd.DataFrame()
+TRADES_DF = pd.DataFrame()
+LANGUAGE_DF = pd.DataFrame()
 
 
-def get_filepaths_to_process(df1: pd.DataFrame, df2: pd.DataFrame) -> list[Path]:
-    """Return a list of CVM files that has to be processed by comparing
-    the files mtimes from the raw folder.
-    """
-    df = pd.concat([df1, df2]).drop_duplicates(keep=False)
-    file_sources = sorted(df["file_source"].drop_duplicates())
-    return [cfg.CVM_RAW_DIR / file_source for file_source in file_sources]
-
-
-def update(
-    rebuild: bool = False,
-    is_listed: bool = True,
-    min_volume: int = 100_000,
-):
+def load(is_traded: bool = True, min_volume: int = 100_000):
     """Verify changes in CVM files and update Finlogic Database if necessary.
 
     Args:
-        rebuild (bool, optional): If True, process all CVM files and rebuilds
-            the database. Defaults to False.
-        is_listed (bool, optional): If True, only currently listed companies are
-        processed.
+        is_traded (bool, optional): If True, only currently traded companies are
+        loaded.
         min_volume (int): The minimum daily volume of the stock. Defaults
-            to 100,000, which is a reasonable value to remove extremely illiquid
-            stocks.
+            to R$ 100k (aprox. USD 20k), which is a reasonable value to remove
+            extremely illiquid stocks.
 
     Returns:
         None
     """
-    # Language files
-    print('\nUpdating "language" database...')
-    lng.process_language_df()
-
-    # CVM raw files
-    # Get files mtimes from the raw folder before updating
-    df_raw1 = cvm.get_raw_file_mtimes()
-    urls = cvm.get_all_file_urls()
-    updated_raw_filepaths = cvm.update_raw_files(urls)
-    print(f"Number of CVM files updated = {len(updated_raw_filepaths)}")
-    # Get files mtimes from the raw folder after updating
-    df_raw2 = cvm.get_raw_file_mtimes()
-
-    # CVM processed files
-    if rebuild:
-        # Process all files
-        filepaths_to_process = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
-    else:
-        # Process only updated files
-        filepaths_to_process = get_filepaths_to_process(df1=df_raw1, df2=df_raw2)
-    print(f"Number of new files to process = {len(filepaths_to_process)}")
-
-    # Determine which companies to process
-    if is_listed:
-        companies_to_process = sorted(
-            cfg.LAST_SESSION_DF.query("volume >= @min_volume")["cvm_id"]
+    global LANGUAGE_DF
+    global TRADES_DF
+    global FINANCIALS_DF
+    print('Loading "language" data...')
+    LANGUAGE_DF = pd.read_csv(LANGUAGE_DATA_URL)
+    print("Loading trading data...")
+    TRADES_DF = pd.read_csv(TRADE_DATA_URL)
+    print("Loading financials data...")
+    date_cols = ["period_begin", "period_end"]
+    FINANCIALS_DF = pd.read_csv(TRADED_FINANCIALS_URL, parse_dates=date_cols)
+    if not is_traded:
+        FINANCIALS_DF = pd.concat(
+            [FINANCIALS_DF, pd.read_csv(NOT_TRADED_FINANCIALS_URL)], ignore_index=True
         )
-    else:
-        companies_to_process = None
-
-    cvm.process_files_with_progress(filepaths_to_process, companies_to_process)
-
-    # FinLogic Database
-    print("\nBuilding FinLogic main DataFrame...")
-    rep.save_reports()
-    ind.save_indicators()
-    print(f"{CHECKMARK} FinLogic updated!")
+    TRADES_DF = TRADES_DF.query("volume >= @min_volume")
+    TRADED_CVM_IDS = TRADES_DF["cvm_id"].unique()  # noqa
+    FINANCIALS_DF = FINANCIALS_DF.query("cvm_id in @TRADED_CVM_IDS").reset_index(
+        drop=True
+    )
+    print("Building indicators data...")
+    global INDICATORS_DF
+    INDICATORS_DF = ind.build_indicators(FINANCIALS_DF)
+    print(f"{CHECKMARK} FinLogic is ready!")
 
 
 def info() -> pd.DataFrame:
     """Print a concise summary of FinLogic available data.
 
     This function returns a dataframe containing main information about
     FinLogic Database, such as the database path, file size, last update call,
@@ -97,42 +74,42 @@
     Args:
         return_dict (bool, optional): If True, returns a dictionary with the
             database information and do not print it.
 
     Returns: None
     """
     info = {}
-    df = rep.get_reports()
-    if df.empty:
+    if FINANCIALS_DF.empty:
         return pd.DataFrame()
 
-    info["data_path"] = f"{cfg.DATA_PATH}"
-    info["data_size"] = f"{cfg.REPORTS_PATH.stat().st_size / 1024**2:.1f} MB"
-    db_last_modified = datetime.fromtimestamp(cfg.REPORTS_PATH.stat().st_mtime)
-    info["updated_on"] = db_last_modified.strftime("%Y-%m-%d %H:%M:%S")
+    info["data_url"] = f"{TRADED_FINANCIALS_URL}"
+    data_size = (
+        FINANCIALS_DF.memory_usage(deep=True).sum()
+        + TRADES_DF.memory_usage(deep=True).sum()
+    )
+    info["memory_usage"] = f"{data_size / 1024**2:.1f} MB"
+    # info["updated_on"] = db_last_modified.strftime("%Y-%m-%d %H:%M:%S")
 
-    info["accounting_entries"] = df.shape[0]
+    info["accounting_entries"] = FINANCIALS_DF.shape[0]
 
     report_cols = ["cvm_id", "is_annual", "period_end"]
-    info["number_of_reports"] = df[report_cols].drop_duplicates().shape[0]
-    info["first_report"] = df["period_end"].min().strftime("%Y-%m-%d")
-    info["last_report"] = df["period_end"].max().strftime("%Y-%m-%d")
+    info["number_of_reports"] = FINANCIALS_DF[report_cols].drop_duplicates().shape[0]
+    info["first_report"] = FINANCIALS_DF["period_end"].min().strftime("%Y-%m-%d")
+    info["last_report"] = FINANCIALS_DF["period_end"].max().strftime("%Y-%m-%d")
 
-    info["number_of_companies"] = df["cvm_id"].nunique()
+    info["number_of_companies"] = FINANCIALS_DF["cvm_id"].nunique()
 
     s = pd.Series(info)
     s.name = "FinLogic Info"
 
     return s.to_frame()
 
 
 def search_segment(search_value: str):
-    series = (
-        cfg.LAST_SESSION_DF["segment"].drop_duplicates().sort_values(ignore_index=True)
-    )
+    series = TRADES_DF["segment"].drop_duplicates().sort_values(ignore_index=True)
     mask = series.str.contains(search_value)
     return series[mask].reset_index(drop=True)
 
 
 def search_company(
     search_value: str,
     search_by: Literal["name_id", "cvm_id", "tax_id", "segment"] = "name_id",
@@ -151,18 +128,18 @@
 
     Returns:
         pd.DataFrame: A DataFrame containing the search results, with columns
             'name_id', 'cvm_id', and 'tax_id' for each unique company that
             matches the search criteria.
     """
     search_cols = ["name_id", "cvm_id", "tax_id"]
-    df = rep.get_reports()[search_cols].drop_duplicates(
+    df = FINANCIALS_DF[search_cols].drop_duplicates(
         subset=["cvm_id"], ignore_index=True
     )
-    df = pd.merge(df, cfg.LAST_SESSION_DF, on="cvm_id")
+    df = pd.merge(df, TRADES_DF, on="cvm_id")
     match search_by:
         case "name_id":
             # Company name is stored in uppercase in the database
             df.query(f"name_id.str.contains('{search_value.upper()}')", inplace=True)
         case "cvm_id":
             df.query(f"cvm_id == {search_value}", inplace=True)
         case "tax_id":
@@ -213,14 +190,14 @@
         rank_by,
     ]
     df = (
         ind.get_indicators()
         .sort_values(by=["cvm_id", "period_end", "is_consolidated"], ignore_index=True)
         # .query("cvm_id == 922")
         .drop_duplicates(subset=["cvm_id"], keep="last")
-        .merge(cfg.LAST_SESSION_DF, on="cvm_id")
+        .merge(TRADES_DF, on="cvm_id")
         .query("segment.str.contains(@segment)")
         .sort_values(by=[rank_by], ascending=False, ignore_index=True)
         .head(n)[show_cols]
     )
 
     return df
```

### Comparing `finlogic-0.5.2/finlogic/indicators.py` & `finlogic-0.6.0/finlogic/indicators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
-from . import config as cfg
-from . import reports as rep
+
 
 TAX_RATE = 0.34
 INDICATORS_CODES = {
     "1": "total_assets",
     "1.01": "current_assets",
     "1.01.01": "cash_equivalents",
     "1.01.02": "financial_investments",
@@ -16,46 +15,38 @@
     "3.03": "gross_profit",
     "3.05": "ebit",
     "3.07": "ebt",
     "3.08": "effective_tax",
     "3.11": "net_income",
     "6.01": "operating_cash_flow",
     "6.01.01.04": "depreciation_amortization",
-    "8.01.01": "eps",
+    "3.99.01.01": "eps",
 }
 
 
-def get_indicators_data() -> pd.DataFrame:
+def filter_indicators_data(dfi: pd.DataFrame) -> pd.DataFrame:
     codes = list(INDICATORS_CODES.keys())  # noqa: used in query below
-
     """There are 137 repeated entries in 208784 rows. These are from companies
     with some exotic period_end dates, as for cvm_id 3450. These entries will be
     removed in the next step, when we drop duplicates and the last entry
     published will be kept.
     """
     drop_cols = ["tax_id", "acc_name", "period_begin"]
-    sort_cols = [
-        "cvm_id",
-        "is_consolidated",
-        "acc_code",
-        "period_end",
-        "period_reference",
-    ]
+    sort_cols = ["cvm_id", "is_consolidated", "acc_code", "period_end"]
     subset_cols = ["cvm_id", "is_consolidated", "acc_code", "period_end"]
 
-    df = (
-        rep.get_reports()
-        .query("acc_code in @codes")
+    dfo = (
+        dfi.query("acc_code in @codes")
         .drop(columns=drop_cols)
         # .query("cvm_id == 9512 and is_consolidated")  # for testing
         .sort_values(by=sort_cols, ignore_index=True)
         .drop_duplicates(subset=subset_cols, keep="last", ignore_index=True)
         .astype({"acc_code": "string"})
     )
-    return df
+    return dfo
 
 
 def pivot_df(df) -> pd.DataFrame:
     index_cols = ["cvm_id", "name_id", "is_annual", "is_consolidated", "period_end"]
     dfp = (
         pd.pivot(df, values="acc_value", index=index_cols, columns=["acc_code"])
         .fillna(0)
@@ -104,15 +95,15 @@
     df["effective_tax_rate"] = -1 * df["effective_tax"] / df["ebt"]
     df["ebitda"] = df["ebit"] + df["depreciation_amortization"]
     df["invested_capital"] = df["total_debt"] + df["equity"] - df["total_cash"]
 
     return df
 
 
-def build_indicators(df, is_annual: bool, insert_avg_col) -> pd.DataFrame:
+def process_indicators(df, is_annual: bool, insert_avg_col) -> pd.DataFrame:
     df.rename(columns=INDICATORS_CODES, inplace=True)
     df = insert_key_cols(df)
 
     avg_cols = ["invested_capital", "total_assets", "equity"]
     for col_name in avg_cols:
         df = insert_avg_col(col_name, df)
 
@@ -141,35 +132,31 @@
     # Drop avg_cols
     avg_cols = ["avg_total_assets", "avg_equity", "avg_invested_capital"]
     df.drop(columns=avg_cols, inplace=True)
 
     return df
 
 
-def save_indicators() -> pd.DataFrame:
-    """Save indicators as pickle file.
-    dfi = input dataframe
-    dfo = output dataframe
-    """
-    dfi = get_indicators_data()
+def build_indicators(financials_df: pd.DataFrame) -> pd.DataFrame:
+    """Build indicators dataframe."""
+    start_df = filter_indicators_data(financials_df)
 
     # Construct pivot tables for annual and quarterly
-    dfa = pivot_df(dfi.query("is_annual"))
-    dfq = pivot_df(dfi.query("not is_annual"))
+    dfa = pivot_df(start_df.query("is_annual"))
+    dfq = pivot_df(start_df.query("not is_annual"))
 
     # Build indicators
-    dfai = build_indicators(dfa, True, insert_annual_avg_col)
-    dfqi = build_indicators(dfq, False, insert_quarterly_avg_col)
+    dfai = process_indicators(dfa, True, insert_annual_avg_col)
+    dfqi = process_indicators(dfq, False, insert_quarterly_avg_col)
 
     # Build output dataframe
     sort_cols = ["cvm_id", "is_consolidated", "period_end"]
-    dfo = pd.concat([dfai, dfqi]).sort_values(by=sort_cols, ignore_index=True)
-    dfo.columns.name = None
-    dfo.to_pickle(cfg.INDICATORS_PATH, compression="zstd")
-    return dfo
+    df = pd.concat([dfai, dfqi]).sort_values(by=sort_cols, ignore_index=True)
+    df.columns.name = None
+    return df
 
 
 def adjust_unit(df: pd.DataFrame, unit: float) -> pd.DataFrame:
     currency_cols = [
         "total_assets",
         "current_assets",
         "current_liabilities",
@@ -185,15 +172,15 @@
         "total_cash",
         "total_debt",
         "net_debt",
         "working_capital",
         "ebitda",
         "invested_capital",
     ]
-    df[currency_cols] = df[currency_cols] / unit
+    df.loc[:, currency_cols] /= unit
     return df
 
 
 def reorder_index(df: pd.DataFrame) -> pd.DataFrame:
     new_order = [
         "total_assets",
         "current_assets",
@@ -242,16 +229,7 @@
         .reset_index()
         .set_index("indicator")
     )
     df.columns.name = None
     df.index.name = None
     df = reorder_index(df)
     return df
-
-
-def get_indicators() -> pd.DataFrame:
-    """Return a DataFrame with all indicators data"""
-    if cfg.INDICATORS_PATH.is_file():
-        df = pd.read_pickle(cfg.INDICATORS_PATH, compression="zstd")
-    else:
-        df = pd.DataFrame()
-    return df
```

### Comparing `finlogic-0.5.2/pyproject.toml` & `finlogic-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -21,19 +21,16 @@
     "Topic :: Office/Business :: Financial :: Investment",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.5.0",
-    "requests>=2.30.0",
-    "tqdm>=4.1.0",
-    "zstandard>=0.21.0",
 ]
-version = "0.5.2"
+version = "0.6.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `finlogic-0.5.2/PKG-INFO` & `finlogic-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: finlogic
-Version: 0.5.2
+Name: FinLogic
+Version: 0.6.0
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -29,17 +29,14 @@
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/crdcj/FinLogic
 Requires-Python: >=3.10
 Requires-Dist: pandas>=1.5.0
-Requires-Dist: requests>=2.30.0
-Requires-Dist: tqdm>=4.1.0
-Requires-Dist: zstandard>=0.21.0
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Made with Python](https://img.shields.io/badge/Python->=3.10-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
@@ -48,15 +45,17 @@
 
 <!-- [![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)" -->
 
 ## FinLogic: finance toolkit for listed Brazilian companies.
 
 ---
 
-**FinLogic** offers a Pythonic way to analyze the financial data of companies listed in Brazil, using information made publicly available by the local securities market authority, CVM. FinLogic processes approximately 20 million accounting entries using Pandas, and constructs a local DataFrame for ultra-fast access to this information.
+**FinLogic** provides a Pythonic approach to analyzing the financial data of companies listed in Brazil. The library pre-processes approximately 50 million accounting entries from the local securities market authority data repository.
+
+The extensive pre-processing stage is automated using Polars within an AWS Lambda Function, and it is scheduled to check for updates overnight. After the CVM repository data is updated and pre-processed, the job saves the cleaned data in FinLogic data folder on GitHub. This arrangement allows the library to access the data quickly and easily.
 
 ---
 
 ## Installation
 
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
@@ -68,66 +67,75 @@
 pip install finlogic
 ```
 
 ### Requirements
 
 - [Python](https://www.python.org) \>= 3.10
 - [Pandas](https://github.com/pydata/pandas) \>= 1.5.0
-- [Requests](http://docs.python-requests.org/en/master/) \>= 2.30.0
-- [tqdm](https://github.com/tqdm/tqdm) \>= 4.1.0
-- [Zstandard](https://python-zstandard.readthedocs.io/en/latest/) \>= 0.21.0
 
 ---
 
 ## Quick Start
 
-### Create FinLogic Database
+### Load FinLogic Data
 
-The 'update' function is responsible for downloading and updating raw financial data from the CVM, processing approximately 20 million accounting entries, and storing them for local data analysis. During the initial run, the process might take some minutes, depending on the CVM server connection and local CPU power. For subsequent updates, only the updated CVM files will be downloaded and processed, which should expedite the operation.
+The 'load' function is responsible for downloading and reading the financial data stored on GitHub data folder.
 
 ```python
 >>> import finlogic as fl
 
-# Compile FinLogic database for the first time:
->>> fl.update()
-
-Updating CVM raw files...
-...
-FinLogic database updated ✅
+# Load the accounting data in memory:
+>>> fl.load()
+```
+    Loading "language" data...
+    Loading trading data...
+    Loading financials data...
+    Building indicators data...
+    ✔ FinLogic is ready!
 
+```python
 # Show database info:
 >>> fl.info()
 ```
 
-|                     |       FinLogic Info |
-| :------------------ | ------------------: |
-| data_path           |   .../finlogic/data |
-| data_size           |             12.1 MB |
-| last_modified_on    | 2023-04-20 07:29:08 |
-| accounting_entries  |           2,806,635 |
-| number_of_reports   |              11,635 |
-| first_report        |          2009-01-31 |
-| last_report         |          2023-03-31 |
-| number_of_companies |               1,139 |
+|                     |                    FinLogic Info |
+| :------------------ | -------------------------------: |
+| data_url            | https://raw.githubusercontent... |
+| memory_usage        |                         255.1 MB |
+| accounting_entries  |                          755,635 |
+| number_of_reports   |                            2,635 |
+| first_report        |                       2009-01-31 |
+| last_report         |                       2023-03-31 |
+| number_of_companies |                              210 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
 
-|     | name_id                                | cvm_id | tax_id             |
-| --: | :------------------------------------- | -----: | :----------------- |
-|   0 | 3R PETROLEUM ÓLEO E GÁS S.A.           |  25291 | 12.091.809/0001-55 |
-|   1 | PETRO RIO S.A.                         |  22187 | 10.629.105/0001-68 |
-|   2 | PETROBRAS DISTRIBUIDORA S/A            |  24295 | 34.274.233/0001-02 |
-|   3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |   9512 | 33.000.167/0001-01 |
-|   4 | PETROLEO LUB DO NORDESTE SA            |   9520 | 07.275.159/0001-68 |
-|   5 | PETRORECÔNCAVO S.A.                    |  25780 | 03.342.704/0001-30 |
-|   6 | PRONOR PETROQUIMICA SA                 |   9784 | 13.552.070/0001-02 |
-|   7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |   9989 | 33.412.081/0001-96 |
+| name_id                            | cvm_id | tax_id             | segment        | is_restructuring | most_traded_stock |
+|:-----------------------------------|-------:|:-------------------|:---------------|:-----------------|:------------------|
+| PETROLEO BRASILEIRO S.A. PETROBRAS |   9512 | 33.000.167/0001-01 | exploration... | False            | PETR4             |
+| 3R PETROLEUM ÓLEO E GÁS S.A.       |  25291 | 12.091.809/0001-55 | exploration... | False            | RRRP3             |
+| PETRORECÔNCAVO S.A.                |  25780 | 03.342.704/0001-30 | exploration... | False            | RECV3             |
+
+```python
+# Search company by segment:
+fl.search_company(search_by="segment", search_value="electric")
+```
+| name_id                                | cvm_id | tax_id             | segment            | is_restructuring | most_traded_stock |
+|:---------------------------------------|-------:|:-------------------|:-------------------|:-----------------|:------------------|
+| CENTRAIS ELET BRAS S.A. - ELETROBRAS   |   2437 | 00.001.180/0001-26 | electric utilities | False            | ELET3             |
+| CIA ENERGETICA DE MINAS GERAIS - CEMIG |   2453 | 17.155.730/0001-64 | electric utilities | False            | CMIG4             |
+| CIA PARANAENSE DE ENERGIA - COPEL      |  14311 | 76.483.817/0001-20 | electric utilities | False            | CPLE6             |
+| CIA ENERGETICA DO CEARA - COELCE       |  14869 | 07.047.251/0001-70 | electric utilities | False            | COCE5             |
+| ENERGISA S.A.                          |  15253 | 00.864.214/0001-06 | electric utilities | False            | ENGI11            |
+| NEOENERGIA S.A.                        |  15539 | 01.083.200/0001-18 | electric utilities | False            | NEOE3             |
+| ENGIE BRASIL ENERGIA S.A.              |  17329 | 02.474.103/0001-19 | electric utilities | False            | EGIE3             |
+...
 
 ### The Company Class
 
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
@@ -150,16 +158,15 @@
 | CVM ID                     |                               9512 |
 | Tax ID (CNPJ)              |                 33.000.167/0001-01 |
 | Total Accounting Rows      |                              3,292 |
 | Selected Tax Rate          |                               0.34 |
 | Selected Accounting Method |                       consolidated |
 | Selected Accounting Unit   |                      1,000,000,000 |
 | First Report               |                         2009-12-31 |
-| Last Report                |                         2021-12-31 |
-| Last Report Type           |                          quarterly |
+| Last Report                |                         2023-03-31 |
 
 ```python
 # Show company assets in Brazilian currency:
 >>> petro.report(report_type='assets')
 ...
 # Show company liabilities with custom arguments:
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
@@ -194,33 +201,43 @@
 | 2.02.01.03 | Financiamento por Arrendamento |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Show company main indicators:
 >>> petro.indicators(num_years=3)
 ```
 
-| Company Financial Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 |
-| :--------------------------- | ---------: | ---------: | ---------: |
-| revenues                     |    302.245 |    272.069 |    452.668 |
-| operating_cash_flow          |    101.766 |    148.106 |    203.126 |
-| ebitda                       |    140.203 |    107.926 |    273.879 |
-| ebit                         |     81.701 |     49.621 |    210.831 |
-| net_income                   |     40.970 |      6.246 |    107.264 |
-| total_cash                   |     33.294 |     64.280 |     62.040 |
-| total_debt                   |    351.161 |    392.548 |    327.818 |
-| net_debt                     |    317.867 |    328.268 |    265.778 |
-| working_capital              |     -4.046 |      6.036 |     33.334 |
-| invested_capital             |    617.004 |    639.418 |    655.359 |
-| return_on_assets             |      0.062 |      0.035 |      0.140 |
-| return_on_equity             |      0.144 |      0.020 |      0.344 |
-| roic                         |      0.097 |      0.053 |      0.217 |
-| gross_margin                 |      0.403 |      0.455 |      0.485 |
-| ebitda_margin                |      0.463 |      0.396 |      0.605 |
-| operating_margin             |      0.178 |      0.120 |      0.307 |
-| net_margin                   |      0.135 |      0.022 |      0.236 |
+| 2021-12-31 | 2022-12-31 | 2023-03-31 |
+|-----------:|-----------:|-----------:|
+|    972.951 |    976.709 |    978.577 |
+|    168.247 |    163.052 |    157.194 |
+|     62.04  |     56.193 |     66.906 |
+|     33.334 |     -0.679 |     28.744 |
+|    655.359 |    588.895 |    607.53  |
+|    134.913 |    163.731 |    128.45  |
+|    327.818 |    280.703 |    271.031 |
+|    265.778 |    224.51  |    204.125 |
+|    389.581 |    364.385 |    403.405 |
+|    452.668 |    641.256 |    638.683 |
+|    219.637 |    334.1   |    332.645 |
+|    107.264 |    189.005 |    182.529 |
+|    273.879 |    362.457 |    355.838 |
+|    210.831 |    294.255 |    289.054 |
+|    151.575 |    274.998 |    263.614 |
+|    -44.311 |    -85.993 |    -81.085 |
+|    203.126 |    255.41  |    256.345 |
+|     63.048 |     68.202 |     66.784 |
+|      0.292 |      0.312 |      0.307 |
+|      0.141 |      0.199 |      0.192 |
+|      0.397 |      0.515 |      0.453 |
+|      0.214 |      0.312 |      0.309 |
+|      0.485 |      0.521 |      0.520 |
+|      0.605 |      0.565 |      0.557 |
+|      0.465 |      0.458 |      0.452 |
+|      0.236 |      0.294 |      0.285 |
+|      8.18  |     14.44  |     13.95  |
 
 ---
 
 P.S.: All contributors are welcome, from beginner to advanced.
 
 **Felipe Costa and Carlos Carvalho**
```

