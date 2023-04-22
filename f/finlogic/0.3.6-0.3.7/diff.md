# Comparing `tmp/FinLogic-0.3.6.tar.gz` & `tmp/FinLogic-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinLogic-0.3.6.tar", last modified: Fri Apr 14 09:14:29 2023, max compression
+gzip compressed data, was "FinLogic-0.3.7.tar", last modified: Sat Apr 22 03:14:58 2023, max compression
```

## Comparing `FinLogic-0.3.6.tar` & `FinLogic-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 FinLogic-0.3.6/LICENSE
--rw-r--r--   0        0        0    10136 2023-04-03 10:41:08.794859 FinLogic-0.3.6/README.md
--rw-r--r--   0        0        0       37 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-04-10 11:28:54.467326 FinLogic-0.3.6/finlogic/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      423 2023-04-14 01:44:35.137202 FinLogic-0.3.6/finlogic/__init__.py
--rw-r--r--   0        0        0    21829 2023-04-14 09:12:15.664615 FinLogic-0.3.6/finlogic/company.py
--rw-r--r--   0        0        0      745 2023-03-19 09:29:48.278335 FinLogic-0.3.6/finlogic/config.py
--rw-r--r--   0        0        0    16130 2023-04-14 01:44:35.137202 FinLogic-0.3.6/finlogic/database.py
--rw-r--r--   0        0        0      996 2023-04-02 12:44:27.971854 FinLogic-0.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 FinLogic-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0     2125 2023-04-14 09:12:15.664615 FinLogic-0.3.6/tests/test_company.py
--rw-r--r--   0        0        0      597 2023-04-14 09:12:15.664615 FinLogic-0.3.6/tests/test_database.py
--rw-r--r--   0        0        0    10776 1970-01-01 00:00:00.000000 FinLogic-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 FinLogic-0.3.7/LICENSE
+-rw-r--r--   0        0        0    10060 2023-04-22 03:12:14.634867 FinLogic-0.3.7/README.md
+-rw-r--r--   0        0        0      423 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/__init__.py
+-rw-r--r--   0        0        0    22078 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/company.py
+-rw-r--r--   0        0        0     1024 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/config.py
+-rw-r--r--   0        0        0     9283 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/cvm.py
+-rw-r--r--   0        0        0     6806 2023-04-22 03:12:14.634867 FinLogic-0.3.7/finlogic/database.py
+-rw-r--r--   0        0        0      996 2023-04-02 12:44:27.971854 FinLogic-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 FinLogic-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0     2125 2023-04-14 09:12:15.664615 FinLogic-0.3.7/tests/test_company.py
+-rw-r--r--   0        0        0      598 2023-04-22 03:12:14.635867 FinLogic-0.3.7/tests/test_database.py
+-rw-r--r--   0        0        0    10700 1970-01-01 00:00:00.000000 FinLogic-0.3.7/PKG-INFO
```

### Comparing `FinLogic-0.3.6/LICENSE` & `FinLogic-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.6/README.md` & `FinLogic-0.3.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic) 
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Python Version](https://img.shields.io/pypi/pyversions/finlogic)](https://www.python.org/)
 [![Anaconda License](https://anaconda.org/conda-forge/finlogic/badges/license.svg)](https://anaconda.org/conda-forge/finlogic)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## FinLogic: finance data analysis toolkit for listed Brazilian companies
 
-
 <table border=1 cellpadding=10><tr><td>
 
 #### \*\*\* IMPORTANT LEGAL DISCLAIMER \*\*\*
 
 ---
 
 **FinLogic** is **not** affiliated, endorsed or vetted by the Securities and Exchange Commission of Brazil (CVM). It's an open-source tool that uses CVM publicly available data and is intended for research and educational purposes. This finance tool is distributed under the **MIT License** (see the [LICENSE](./LICENSE) file in the release for details).
@@ -23,40 +22,44 @@
 ---
 
 **FinLogic** offers a Pythonic way to analyze financial data of listed companies in Brazil from information made publicly avaible by local securities market authority (CVM). This finance tool is built on top of Pandas.
 
 ---
 
 ## Installation
+
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/finlogic) and on [Conda](https://anaconda.org/conda-forge/finlogic).
 
 ```sh
 # Conda:
-conda install -c conda-forge finlogic 
+conda install -c conda-forge finlogic
 ```
 
 ```sh
 # or PyPI:
 pip install finlogic
 ```
 
 ### Requirements
--   [Python](https://www.python.org) \>= 3.10
--   [Pandas](https://github.com/pydata/pandas) \>= 1.4.0)
--   [Requests](http://docs.python-requests.org/en/master/) \>= 2.27.0
--   [Zstandard](https://pypi.org/project/zstandard/) \>= 0.17.0
+
+- [Python](https://www.python.org) \>= 3.10
+- [Pandas](https://github.com/pydata/pandas) \>= 1.4.0)
+- [Requests](http://docs.python-requests.org/en/master/) \>= 2.27.0
+- [Zstandard](https://pypi.org/project/zstandard/) \>= 0.17.0
 
 ---
 
 ## Quick Start
+
 ### Create FinLogic Local Database
+
 The 'update_database' function is responsible for downloading raw financial files from CVM, processesing aprox. 18 millions rows of accounting values and storing it into a single Pandas DataFrame compressed file for local data analysis.
 In the firt run, the process can take 3 minutes depending on CVM Server connection and local CPU power. The database generation needs at least 8 GB of free memory and a quad core processor is recommended.
 For subsequent updates, only updated CVM files will be processed and inserted into the database, which will be faster.
 
 ```python
 >>> import finlogic as fl
 
@@ -67,46 +70,47 @@
 ...
 FinLogic database updated ✅
 
 # Show database info:
 >>> fl.database_info()
 ```
 
-| FinLogic Database Info      | Value                                   |
-|:----------------------------|----------------------------------------:|
+| FinLogic Database Info      |                                   Value |
+| :-------------------------- | --------------------------------------: |
 | Database Path               | /home/crcj/repos/FinLogic/finlogic/data |
-| File Size (MB)              | 39.0                                    |
-| Last Update Call            | 2022-04-20 07:29:08                     |
-| Finlogic Last Modified      | 2022-04-20 07:31:48                     |
-| CVM Last Update             | 2022-04-17 13:09:01                     |
-| Size in Memory (MB)         | 626.3                                   |
-| Accounting Rows             | 18,757,249                              |
-| Unique Accounting Codes     | 2,008                                   |
-| Companies                   | 1,093                                   |
-| Unique Financial Statements | 12,139                                  |
-| First Financial Statement   | 2009-01-31                              |
-| Last Financial Statement    | 2022-03-31                              |
+| File Size (MB)              |                                    39.0 |
+| Last Update Call            |                     2022-04-20 07:29:08 |
+| Finlogic Last Modified      |                     2022-04-20 07:31:48 |
+| CVM Last Update             |                     2022-04-17 13:09:01 |
+| Size in Memory (MB)         |                                   626.3 |
+| Accounting Rows             |                              18,757,249 |
+| Unique Accounting Codes     |                                   2,008 |
+| Companies                   |                                   1,093 |
+| Unique Financial Statements |                                  12,139 |
+| First Financial Statement   |                              2009-01-31 |
+| Last Financial Statement    |                              2022-03-31 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
 
-|   | co_name                                | cvm_id | fiscal_id          |
-|--:|:---------------------------------------|-------:|:-------------------|
-| 0 | 3R PETROLEUM ÓLEO E GÁS S.A.           |  25291 | 12.091.809/0001-55 |
-| 1 | PETRO RIO S.A.                         |  22187 | 10.629.105/0001-68 |
-| 2 | PETROBRAS DISTRIBUIDORA S/A            |  24295 | 34.274.233/0001-02 |
-| 3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |   9512 | 33.000.167/0001-01 |
-| 4 | PETROLEO LUB DO NORDESTE SA            |   9520 | 07.275.159/0001-68 |
-| 5 | PETRORECÔNCAVO S.A.                    |  25780 | 03.342.704/0001-30 |
-| 6 | PRONOR PETROQUIMICA SA                 |   9784 | 13.552.070/0001-02 |
-| 7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |   9989 | 33.412.081/0001-96 |
+|     | co_name                                | co_id | co_fiscal_id       |
+| --: | :------------------------------------- | ----: | :----------------- |
+|   0 | 3R PETROLEUM ÓLEO E GÁS S.A.           | 25291 | 12.091.809/0001-55 |
+|   1 | PETRO RIO S.A.                         | 22187 | 10.629.105/0001-68 |
+|   2 | PETROBRAS DISTRIBUIDORA S/A            | 24295 | 34.274.233/0001-02 |
+|   3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |  9512 | 33.000.167/0001-01 |
+|   4 | PETROLEO LUB DO NORDESTE SA            |  9520 | 07.275.159/0001-68 |
+|   5 | PETRORECÔNCAVO S.A.                    | 25780 | 03.342.704/0001-30 |
+|   6 | PRONOR PETROQUIMICA SA                 |  9784 | 13.552.070/0001-02 |
+|   7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |  9989 | 33.412.081/0001-96 |
 
 ### The Company Class
+
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
 # Both CVM (regulator) ID or Fiscal ID can be used as an identifier.
 >>> petro = fl.Company(9512, acc_method='separate', acc_unit='million')
 
@@ -117,15 +121,15 @@
 >>> petro.acc_unit = 'billion'
 
 # Show company info:
 >>> petro.info()
 ```
 
 | Company Info               |                             Values |
-|:---------------------------|-----------------------------------:|
+| :------------------------- | ---------------------------------: |
 | Name                       | PETROLEO BRASILEIRO S.A. PETROBRAS |
 | CVM ID                     |                               9512 |
 | Fiscal ID (CNPJ)           |                 33.000.167/0001-01 |
 | Total Accounting Rows      |                             39,292 |
 | Selected Tax Rate          |                               0.34 |
 | Selected Accounting Method |                       consolidated |
 | Selected Accounting Unit   |                      1,000,000,000 |
@@ -137,33 +141,33 @@
 # Show company assets in Brazilian currency:
 >>> petro.report(report_type='assets')
 ...
 # Show company liabilities with custom arguments:
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
 ```
 
-| acc_code   | acc_name            | acc_fixed   |   2020-12-31 |   2021-12-31 |   2022-12-31 |
-|:-----------|:--------------------|:------------|-------------:|-------------:|-------------:|
-| 2.01.04    | Loans and Financing | True        |       51.364 |       50.631 |       47.65  |
-| 2.01.04.01 | Loans and Financing | True        |       21.751 |       20.316 |       18.656 |
-| 2.01.04.02 | Debentures          | True        |        0     |        0     |        0     |
-| 2.01.04.03 | Lease Financing     | True        |       29.613 |       30.315 |       28.994 |
-| 2.02.01    | Loans and Financing | True        |      341.184 |      277.187 |      233.053 |
-| 2.02.01.01 | Loans and Financing | True        |      258.287 |      178.908 |      137.63  |
-| 2.02.01.02 | Debentures          | True        |        0     |        0     |        0     |
-| 2.02.01.03 | Lease Financing     | True        |       82.897 |       98.279 |       95.423 |
+| acc_code   | acc_name            | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 |
+| :--------- | :------------------ | :-------- | ---------: | ---------: | ---------: |
+| 2.01.04    | Loans and Financing | True      |     51.364 |     50.631 |      47.65 |
+| 2.01.04.01 | Loans and Financing | True      |     21.751 |     20.316 |     18.656 |
+| 2.01.04.02 | Debentures          | True      |          0 |          0 |          0 |
+| 2.01.04.03 | Lease Financing     | True      |     29.613 |     30.315 |     28.994 |
+| 2.02.01    | Loans and Financing | True      |    341.184 |    277.187 |    233.053 |
+| 2.02.01.01 | Loans and Financing | True      |    258.287 |    178.908 |     137.63 |
+| 2.02.01.02 | Debentures          | True      |          0 |          0 |          0 |
+| 2.02.01.03 | Lease Financing     | True      |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Change account names to Portuguese:
 >>> petro.language = "portuguese"
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
 ```
 
 | acc_code   | acc_name                       | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 |
-|------------|--------------------------------|-----------|-----------:|-----------:|-----------:|
+| ---------- | ------------------------------ | --------- | ---------: | ---------: | ---------: |
 | 2.01.04    | Empréstimos e Financiamentos   | True      |     51.364 |     50.631 |      47.65 |
 | 2.01.04.01 | Empréstimos e Financiamentos   | True      |     21.751 |     20.316 |     18.656 |
 | 2.01.04.02 | Debêntures                     | True      |          0 |          0 |          0 |
 | 2.01.04.03 | Financiamento por Arrendamento | True      |     29.613 |     30.315 |     28.994 |
 | 2.02.01    | Empréstimos e Financiamentos   | True      |    341.184 |    277.187 |    233.053 |
 | 2.02.01.01 | Empréstimos e Financiamentos   | True      |    258.287 |    178.908 |     137.63 |
 | 2.02.01.02 | Debêntures                     | True      |          0 |          0 |          0 |
@@ -171,15 +175,15 @@
 
 ```python
 # Show company main indicators:
 >>> petro.indicators(num_years=3)
 ```
 
 | Company Financial Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 |
-|:-----------------------------|-----------:|-----------:|-----------:|
+| :--------------------------- | ---------: | ---------: | ---------: |
 | revenues                     |    302.245 |    272.069 |    452.668 |
 | operating_cash_flow          |    101.766 |    148.106 |    203.126 |
 | ebitda                       |    140.203 |    107.926 |    273.879 |
 | ebit                         |     81.701 |     49.621 |    210.831 |
 | net_income                   |     40.970 |      6.246 |    107.264 |
 | total_cash                   |     33.294 |     64.280 |     62.040 |
 | total_debt                   |    351.161 |    392.548 |    327.818 |
```

#### html2text {}

```diff
@@ -34,71 +34,71 @@
 data analysis. In the firt run, the process can take 3 minutes depending on CVM
 Server connection and local CPU power. The database generation needs at least 8
 GB of free memory and a quad core processor is recommended. For subsequent
 updates, only updated CVM files will be processed and inserted into the
 database, which will be faster. ```python >>> import finlogic as fl # Compile
 FinLogic database for the first time: >>> fl.update_database() Updating CVM raw
 files... ... FinLogic database updated â # Show database info: >>>
-fl.database_info() ``` | FinLogic Database Info | Value | |:-------------------
----------|----------------------------------------:| | Database Path | /home/
+fl.database_info() ``` | FinLogic Database Info | Value | | :------------------
+-------- | --------------------------------------: | | Database Path | /home/
 crcj/repos/FinLogic/finlogic/data | | File Size (MB) | 39.0 | | Last Update
 Call | 2022-04-20 07:29:08 | | Finlogic Last Modified | 2022-04-20 07:31:48 | |
 CVM Last Update | 2022-04-17 13:09:01 | | Size in Memory (MB) | 626.3 | |
 Accounting Rows | 18,757,249 | | Unique Accounting Codes | 2,008 | | Companies
 | 1,093 | | Unique Financial Statements | 12,139 | | First Financial Statement
 | 2009-01-31 | | Last Financial Statement | 2022-03-31 | ```python # Search for
-a company in database: >>> fl.search_company('petro') ``` | | co_name | cvm_id
-| fiscal_id | |--:|:---------------------------------------|-------:|:---------
-----------| | 0 | 3R PETROLEUM ÃLEO E GÃS S.A. | 25291 | 12.091.809/0001-55 |
-| 1 | PETRO RIO S.A. | 22187 | 10.629.105/0001-68 | | 2 | PETROBRAS
+a company in database: >>> fl.search_company('petro') ``` | | co_name | co_id |
+co_fiscal_id | | --: | :------------------------------------- | ----: | :------
+----------- | | 0 | 3R PETROLEUM ÃLEO E GÃS S.A. | 25291 | 12.091.809/0001-55
+| | 1 | PETRO RIO S.A. | 22187 | 10.629.105/0001-68 | | 2 | PETROBRAS
 DISTRIBUIDORA S/A | 24295 | 34.274.233/0001-02 | | 3 | PETROLEO BRASILEIRO S.A.
 PETROBRAS | 9512 | 33.000.167/0001-01 | | 4 | PETROLEO LUB DO NORDESTE SA |
 9520 | 07.275.159/0001-68 | | 5 | PETRORECÃNCAVO S.A. | 25780 | 03.342.704/
 0001-30 | | 6 | PRONOR PETROQUIMICA SA | 9784 | 13.552.070/0001-02 | | 7 |
 REFINARIA DE PETROLEOS MANGUINHOS S.A. | 9989 | 33.412.081/0001-96 | ### The
 Company Class The Company Class allows you to easily access financial data from
 Brazilian companies. All values are in local currency (Real). ```python #
 Create a Company object to acces its financial data: # Both CVM (regulator) ID
 or Fiscal ID can be used as an identifier. >>> petro = fl.Company(9512,
 acc_method='separate', acc_unit='million') # Change company accounting method
 back to consolidated (default): >>> petro.acc_method = 'consolidated' # Change
 company accounting unit to billion (default is 1): >>> petro.acc_unit =
-'billion' # Show company info: >>> petro.info() ``` | Company Info | Values |
-|:---------------------------|-----------------------------------:| | Name |
+'billion' # Show company info: >>> petro.info() ``` | Company Info | Values | |
+:------------------------- | ---------------------------------: | | Name |
 PETROLEO BRASILEIRO S.A. PETROBRAS | | CVM ID | 9512 | | Fiscal ID (CNPJ) |
 33.000.167/0001-01 | | Total Accounting Rows | 39,292 | | Selected Tax Rate |
 0.34 | | Selected Accounting Method | consolidated | | Selected Accounting Unit
 | 1,000,000,000 | | First Annual Report | 2009-12-31 | | Last Annual Report |
 2021-12-31 | | Last Quarterly Report | 2021-09-30 | ```python # Show company
 assets in Brazilian currency: >>> petro.report(report_type='assets') ... # Show
 company liabilities with custom arguments: >>> petro.report(report_type='debt',
 acc_level=4, num_years=3) ``` | acc_code | acc_name | acc_fixed | 2020-12-31 |
-2021-12-31 | 2022-12-31 | |:-----------|:--------------------|:------------|---
-----------:|-------------:|-------------:| | 2.01.04 | Loans and Financing |
-True | 51.364 | 50.631 | 47.65 | | 2.01.04.01 | Loans and Financing | True |
-21.751 | 20.316 | 18.656 | | 2.01.04.02 | Debentures | True | 0 | 0 | 0 | |
-2.01.04.03 | Lease Financing | True | 29.613 | 30.315 | 28.994 | | 2.02.01 |
-Loans and Financing | True | 341.184 | 277.187 | 233.053 | | 2.02.01.01 | Loans
-and Financing | True | 258.287 | 178.908 | 137.63 | | 2.02.01.02 | Debentures |
+2021-12-31 | 2022-12-31 | | :--------- | :------------------ | :-------- | ----
+-----: | ---------: | ---------: | | 2.01.04 | Loans and Financing | True |
+51.364 | 50.631 | 47.65 | | 2.01.04.01 | Loans and Financing | True | 21.751 |
+20.316 | 18.656 | | 2.01.04.02 | Debentures | True | 0 | 0 | 0 | | 2.01.04.03 |
+Lease Financing | True | 29.613 | 30.315 | 28.994 | | 2.02.01 | Loans and
+Financing | True | 341.184 | 277.187 | 233.053 | | 2.02.01.01 | Loans and
+Financing | True | 258.287 | 178.908 | 137.63 | | 2.02.01.02 | Debentures |
 True | 0 | 0 | 0 | | 2.02.01.03 | Lease Financing | True | 82.897 | 98.279 |
 95.423 | ```python # Change account names to Portuguese: >>> petro.language =
 "portuguese" >>> petro.report(report_type='debt', acc_level=4, num_years=3) ```
-| acc_code | acc_name | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 | |---
----------|--------------------------------|-----------|-----------:|----------
--:|-----------:| | 2.01.04 | EmprÃ©stimos e Financiamentos | True | 51.364 |
+| acc_code | acc_name | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 | | --
+-------- | ------------------------------ | --------- | ---------: | ---------:
+| ---------: | | 2.01.04 | EmprÃ©stimos e Financiamentos | True | 51.364 |
 50.631 | 47.65 | | 2.01.04.01 | EmprÃ©stimos e Financiamentos | True | 21.751 |
 20.316 | 18.656 | | 2.01.04.02 | DebÃªntures | True | 0 | 0 | 0 | | 2.01.04.03
 | Financiamento por Arrendamento | True | 29.613 | 30.315 | 28.994 | | 2.02.01
 | EmprÃ©stimos e Financiamentos | True | 341.184 | 277.187 | 233.053 | |
 2.02.01.01 | EmprÃ©stimos e Financiamentos | True | 258.287 | 178.908 | 137.63
 | | 2.02.01.02 | DebÃªntures | True | 0 | 0 | 0 | | 2.02.01.03 | Financiamento
 por Arrendamento | True | 82.897 | 98.279 | 95.423 | ```python # Show company
 main indicators: >>> petro.indicators(num_years=3) ``` | Company Financial
-Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 | |:-------------------------
-----|-----------:|-----------:|-----------:| | revenues | 302.245 | 272.069 |
+Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 | | :------------------------
+--- | ---------: | ---------: | ---------: | | revenues | 302.245 | 272.069 |
 452.668 | | operating_cash_flow | 101.766 | 148.106 | 203.126 | | ebitda |
 140.203 | 107.926 | 273.879 | | ebit | 81.701 | 49.621 | 210.831 | | net_income
 | 40.970 | 6.246 | 107.264 | | total_cash | 33.294 | 64.280 | 62.040 | |
 total_debt | 351.161 | 392.548 | 327.818 | | net_debt | 317.867 | 328.268 |
 265.778 | | working_capital | -4.046 | 6.036 | 33.334 | | invested_capital |
 617.004 | 639.418 | 655.359 | | return_on_assets | 0.062 | 0.035 | 0.140 | |
 return_on_capital | 0.097 | 0.053 | 0.217 | | return_on_equity | 0.144 | 0.020
```

### Comparing `FinLogic-0.3.6/finlogic/company.py` & `FinLogic-0.3.7/finlogic/company.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         ValueError: If the input arguments are invalid.
     """
 
     def __init__(
         self,
         identifier: int | str,
         acc_method: Literal["consolidated", "separate"] = "consolidated",
-        acc_unit: float | str = 1.0,
+        acc_unit: int | float | str = 1,
         tax_rate: float = 0.34,
         language: str = "english",
     ):
         """Initializes a new instance of the Company class."""
         self.identifier = identifier
         self.acc_method = acc_method
         self.acc_unit = acc_unit
@@ -70,28 +70,30 @@
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier: int | str):
         # Create custom data frame for ID selection
         df = (
-            c.main_df[["cvm_id", "fiscal_id"]]
+            c.finlogic_df[["co_id", "co_fiscal_id"]]
             .drop_duplicates()
-            .astype({"cvm_id": int, "fiscal_id": str})
+            .astype({"co_id": int, "co_fiscal_id": str})
         )
-        if identifier in df["cvm_id"].values:
-            self._cvm_id = identifier
-            self._fiscal_id = df.loc[df["cvm_id"] == identifier, "fiscal_id"].item()
-        elif identifier in df["fiscal_id"].values:
-            self._fiscal_id = identifier
-            self._cvm_id = df.loc[df["fiscal_id"] == identifier, "cvm_id"].item()
+        if identifier in df["co_id"].values:
+            self._co_id = identifier
+            self._co_fiscal_id = df.loc[
+                df["co_id"] == identifier, "co_fiscal_id"
+            ].item()
+        elif identifier in df["co_fiscal_id"].values:
+            self._co_fiscal_id = identifier
+            self._co_id = df.loc[df["co_fiscal_id"] == identifier, "co_id"].item()
         else:
-            raise KeyError("Company 'identifier' not found in database")
+            raise KeyError("Company 'identifier' not found in FinLogic Database")
         # Only set company data after object identifier validation
-        self._set_main_data()
+        self._set_co_df()
         self._identifier = identifier
 
     @property
     def acc_method(self) -> Literal["consolidated", "separate"]:
         """Gets or sets the accounting method for registering investments in
         subsidiaries.
 
@@ -135,25 +137,28 @@
 
             To set the accounting unit to a custom factor, e.g., 10,000:
                 company.acc_unit = 10_000
         """
         return self._acc_unit
 
     @acc_unit.setter
-    def acc_unit(self, value: float | str):
-        if value == "thousand":
-            self._acc_unit = 1_000
-        elif value == "million":
-            self._acc_unit = 1_000_000
-        elif value == "billion":
-            self._acc_unit = 1_000_000_000
-        elif value > 0:
-            self._acc_unit = value
-        else:
-            raise ValueError("Accounting Unit is invalid")
+    def acc_unit(self, value: int | float | str) -> float | int:
+        match value:
+            case "thousand":
+                self._acc_unit = 1_000
+            case "million":
+                self._acc_unit = 1_000_000
+            case "billion":
+                self._acc_unit = 1_000_000_000
+            case str():  # Add this case to catch invalid strings
+                raise ValueError("Invalid string for Accounting Unit")
+            case v if v > 0:
+                self._acc_unit = v
+            case _:
+                raise ValueError("Accounting Unit is invalid")
 
     @property
     def tax_rate(self) -> float:
         """Gets or sets company 'tax_rate' property.
 
         The "tax_rate" is used to calculate some of the company
         indicators, such as EBIT and net income. The default value
@@ -205,62 +210,62 @@
         list_languages = ["english", "portuguese"]
         if language.lower() in list_languages:
             self._language = language.capitalize()
         else:
             sup_lang = f"Supported languages: {', '.join(list_languages)}"
             raise KeyError(f"'{language}' not supported. {sup_lang}")
 
-    def _set_main_data(self) -> pd.DataFrame:
-        self._COMP_DF = (
-            c.main_df.query("cvm_id == @self._cvm_id")
+    def _set_co_df(self) -> pd.DataFrame:
+        self._co_df = (
+            c.finlogic_df.query("co_id == @self._co_id")
             .astype(
                 {
                     "co_name": str,
-                    "cvm_id": np.uint32,
-                    "fiscal_id": str,
+                    "co_id": "UInt32",
+                    "co_fiscal_id": str,
                     "report_type": str,
                     "report_version": str,
                     "period_reference": "datetime64[ns]",
                     "period_begin": "datetime64[ns]",
                     "period_end": "datetime64[ns]",
-                    "period_order": np.int8,
+                    "period_order": str,
                     "acc_code": str,
                     "acc_name": str,
                     "acc_method": str,
                     "acc_fixed": bool,
                     "acc_value": float,
                     "equity_statement_column": str,
                 }
             )
             .sort_values(by="acc_code", ignore_index=True)
         )
-        self._NAME = self._COMP_DF["co_name"].iloc[0]
-        self._FIRST_ANNUAL = self._COMP_DF.query('report_type == "annual"')[
+        self._name = self._co_df["co_name"].iloc[0]
+        self._first_annual = self._co_df.query('report_type == "annual"')[
             "period_end"
         ].min()
-        self._LAST_ANNUAL = self._COMP_DF.query('report_type == "annual"')[
+        self._last_annual = self._co_df.query('report_type == "annual"')[
             "period_end"
         ].max()
-        self._LAST_QUARTERLY = self._COMP_DF.query('report_type == "quarterly"')[
+        self._last_quarterly = self._co_df.query('report_type == "quarterly"')[
             "period_end"
         ].max()
 
     def info(self) -> dict:
         """Return a dictionay with company info."""
         company_info = {
-            "Name": self._NAME,
-            "CVM ID": self._cvm_id,
-            "Fiscal ID (CNPJ)": self._fiscal_id,
-            "Total Accounting Rows": len(self._COMP_DF.index),
+            "Name": self._name,
+            "CVM ID": self._co_id,
+            "Fiscal ID (CNPJ)": self._co_fiscal_id,
+            "Total Accounting Rows": len(self._co_df.index),
             "Selected Tax Rate": self._tax_rate,
             "Selected Accounting Method": self._acc_method,
             "Selected Accounting Unit": self._acc_unit,
-            "First Annual Report": self._FIRST_ANNUAL.strftime("%Y-%m-%d"),
-            "Last Annual Report": self._LAST_ANNUAL.strftime("%Y-%m-%d"),
-            "Last Quarterly Report": self._LAST_QUARTERLY.strftime("%Y-%m-%d"),
+            "First Annual Report": self._first_annual.strftime("%Y-%m-%d"),
+            "Last Annual Report": self._last_annual.strftime("%Y-%m-%d"),
+            "Last Quarterly Report": self._last_quarterly.strftime("%Y-%m-%d"),
         }
         return company_info
 
     def report(
         self,
         report_type: str,
         acc_level: int | None = None,
@@ -294,15 +299,15 @@
         Raises:
             ValueError: If some argument is invalid.
         """
         # Check input arguments.
         if acc_level not in {None, 2, 3, 4}:
             raise ValueError("acc_level expects None, 2, 3 or 4")
 
-        df = self._COMP_DF.query("acc_method == @self._acc_method").copy()
+        df = self._co_df.query("acc_method == @self._acc_method").copy()
 
         # Set language
         class MyDict(dict):
             """Custom dictionary class to return key if key is not found."""
 
             def __missing__(self, key):
                 return "(pt) " + key
@@ -378,36 +383,36 @@
         if num_years > 0:
             cols = report_df.columns.to_list()
             cols = cols[0:2] + cols[-num_years:]
             report_df = report_df[cols]
         return report_df
 
     def _calculate_ttm(self, dfi: pd.DataFrame) -> pd.DataFrame:
-        if self._LAST_ANNUAL > self._LAST_QUARTERLY:
+        if self._last_annual > self._last_quarterly:
             return dfi.query('report_type == "annual"').copy()
 
-        df1 = dfi.query("period_end == @self._LAST_QUARTERLY").copy()
+        df1 = dfi.query("period_end == @self._last_quarterly").copy()
         df1.query("period_begin == period_begin.min()", inplace=True)
 
-        df2 = dfi.query("period_reference == @self._LAST_QUARTERLY").copy()
+        df2 = dfi.query("period_reference == @self._last_quarterly").copy()
         df2.query("period_begin == period_begin.min()", inplace=True)
         df2["acc_value"] = -df2["acc_value"]
 
-        df3 = dfi.query("period_end == @self._LAST_ANNUAL").copy()
+        df3 = dfi.query("period_end == @self._last_annual").copy()
 
         df_ttm = (
             pd.concat([df1, df2, df3], ignore_index=True)[["acc_code", "acc_value"]]
             .groupby(by="acc_code")
             .sum()
             .reset_index()
         )
         df1.drop(columns="acc_value", inplace=True)
         df_ttm = pd.merge(df1, df_ttm)
         df_ttm["report_type"] = "quarterly"
-        df_ttm["period_begin"] = self._LAST_QUARTERLY - pd.DateOffset(years=1)
+        df_ttm["period_begin"] = self._last_quarterly - pd.DateOffset(years=1)
 
         df_annual = dfi.query('report_type == "annual"').copy()
 
         return pd.concat([df_annual, df_ttm], ignore_index=True)
 
     def custom_report(
         self,
@@ -527,42 +532,42 @@
         # Show only the selected number of years
         if num_years > 0:
             dfo = dfo[dfo.columns[-num_years:]]
         return dfo
 
     def _make_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
         # keep only last quarterly fs
-        if self._LAST_ANNUAL > self._LAST_QUARTERLY:
+        if self._last_annual > self._last_quarterly:
             df = dfi.query('report_type == "annual"').copy()
             df.query(
-                "period_order == -1 or \
-                 period_end == @self._LAST_ANNUAL",
+                "period_order == 'PREVIOUS' or \
+                 period_end == @self._last_annual",
                 inplace=True,
             )
         else:
             df = dfi.query(
                 'report_type == "annual" or \
-                 period_end == @self._LAST_QUARTERLY'
+                 period_end == @self._last_quarterly'
             ).copy()
             df.query(
-                "period_order == -1 or \
-                 period_end == @self._LAST_QUARTERLY or \
-                 period_end == @self._LAST_ANNUAL",
+                "period_order == 'PREVIOUS' or \
+                 period_end == @self._last_quarterly or \
+                 period_end == @self._last_annual",
                 inplace=True,
             )
 
         # Create output dataframe with only the index
         dfo = df.sort_values(by="period_end", ascending=True)[
             ["acc_name", "acc_code", "acc_fixed"]
         ].drop_duplicates(subset="acc_code", ignore_index=True, keep="last")
 
         periods = list(df["period_end"].sort_values().unique())
         for period in periods:
             year_cols = ["acc_value", "acc_code"]
             df_year = df.query("period_end == @period")[year_cols].copy()
             period_str = period.strftime("%Y-%m-%d")
-            if period == self._LAST_QUARTERLY:
+            if period == self._last_quarterly:
                 period_str += " (ttm)"
             df_year.rename(columns={"acc_value": period_str}, inplace=True)
             dfo = pd.merge(dfo, df_year, how="left", on=["acc_code"])
 
         return dfo.sort_values("acc_code", ignore_index=True)
```

### Comparing `FinLogic-0.3.6/pyproject.toml` & `FinLogic-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "zstandard>=0.17.0",
 ]
-version = "0.3.6"
+version = "0.3.7"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.0.0",
```

### Comparing `FinLogic-0.3.6/tests/test_company.py` & `FinLogic-0.3.7/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `FinLogic-0.3.6/tests/test_database.py` & `FinLogic-0.3.7/tests/test_database.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import finlogic as fl
 
 
 def test_db_info():
     db_info = fl.database_info()
-    assert db_info["First Financial Statement"] == "2009-01-31"
-    assert db_info["Accounting Rows"] > 20_000_000
+    assert db_info["First financial statement"] == "2009-01-31"
+    assert db_info["Accounting rows"] > 20_000_000
 
 
 def test_search_company():
     # Search for petrobras
     search_result = fl.search_company("petrobras")
     """
-        co_name                            cvm_id  fiscal_id
+        co_name                            co_id  co_fiscal_id
     0   PETROBRAS DISTRIBUIDORA S/A         24295  34.274.233/0001-02
     1   PETROLEO BRASILEIRO S.A. PETROBRAS   9512  33.000.167/0001-01
     """
     # Check the results
-    assert set(search_result["cvm_id"]) == {9512, 24295}
+    assert set(search_result["co_id"]) == {9512, 24295}
```

### Comparing `FinLogic-0.3.6/PKG-INFO` & `FinLogic-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: FinLogic
-Version: 0.3.6
+Version: 0.3.7
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-email: Carlos Carvalho <cr.cj@outlook.com>
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Provides-Extra: test
 Project-URL: repository, https://github.com/crdcj/FinLogic
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic) 
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Python Version](https://img.shields.io/pypi/pyversions/finlogic)](https://www.python.org/)
 [![Anaconda License](https://anaconda.org/conda-forge/finlogic/badges/license.svg)](https://anaconda.org/conda-forge/finlogic)
 [![Code Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## FinLogic: finance data analysis toolkit for listed Brazilian companies
 
-
 <table border=1 cellpadding=10><tr><td>
 
 #### \*\*\* IMPORTANT LEGAL DISCLAIMER \*\*\*
 
 ---
 
 **FinLogic** is **not** affiliated, endorsed or vetted by the Securities and Exchange Commission of Brazil (CVM). It's an open-source tool that uses CVM publicly available data and is intended for research and educational purposes. This finance tool is distributed under the **MIT License** (see the [LICENSE](./LICENSE) file in the release for details).
@@ -39,40 +38,44 @@
 ---
 
 **FinLogic** offers a Pythonic way to analyze financial data of listed companies in Brazil from information made publicly avaible by local securities market authority (CVM). This finance tool is built on top of Pandas.
 
 ---
 
 ## Installation
+
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/finlogic) and on [Conda](https://anaconda.org/conda-forge/finlogic).
 
 ```sh
 # Conda:
-conda install -c conda-forge finlogic 
+conda install -c conda-forge finlogic
 ```
 
 ```sh
 # or PyPI:
 pip install finlogic
 ```
 
 ### Requirements
--   [Python](https://www.python.org) \>= 3.10
--   [Pandas](https://github.com/pydata/pandas) \>= 1.4.0)
--   [Requests](http://docs.python-requests.org/en/master/) \>= 2.27.0
--   [Zstandard](https://pypi.org/project/zstandard/) \>= 0.17.0
+
+- [Python](https://www.python.org) \>= 3.10
+- [Pandas](https://github.com/pydata/pandas) \>= 1.4.0)
+- [Requests](http://docs.python-requests.org/en/master/) \>= 2.27.0
+- [Zstandard](https://pypi.org/project/zstandard/) \>= 0.17.0
 
 ---
 
 ## Quick Start
+
 ### Create FinLogic Local Database
+
 The 'update_database' function is responsible for downloading raw financial files from CVM, processesing aprox. 18 millions rows of accounting values and storing it into a single Pandas DataFrame compressed file for local data analysis.
 In the firt run, the process can take 3 minutes depending on CVM Server connection and local CPU power. The database generation needs at least 8 GB of free memory and a quad core processor is recommended.
 For subsequent updates, only updated CVM files will be processed and inserted into the database, which will be faster.
 
 ```python
 >>> import finlogic as fl
 
@@ -83,46 +86,47 @@
 ...
 FinLogic database updated ✅
 
 # Show database info:
 >>> fl.database_info()
 ```
 
-| FinLogic Database Info      | Value                                   |
-|:----------------------------|----------------------------------------:|
+| FinLogic Database Info      |                                   Value |
+| :-------------------------- | --------------------------------------: |
 | Database Path               | /home/crcj/repos/FinLogic/finlogic/data |
-| File Size (MB)              | 39.0                                    |
-| Last Update Call            | 2022-04-20 07:29:08                     |
-| Finlogic Last Modified      | 2022-04-20 07:31:48                     |
-| CVM Last Update             | 2022-04-17 13:09:01                     |
-| Size in Memory (MB)         | 626.3                                   |
-| Accounting Rows             | 18,757,249                              |
-| Unique Accounting Codes     | 2,008                                   |
-| Companies                   | 1,093                                   |
-| Unique Financial Statements | 12,139                                  |
-| First Financial Statement   | 2009-01-31                              |
-| Last Financial Statement    | 2022-03-31                              |
+| File Size (MB)              |                                    39.0 |
+| Last Update Call            |                     2022-04-20 07:29:08 |
+| Finlogic Last Modified      |                     2022-04-20 07:31:48 |
+| CVM Last Update             |                     2022-04-17 13:09:01 |
+| Size in Memory (MB)         |                                   626.3 |
+| Accounting Rows             |                              18,757,249 |
+| Unique Accounting Codes     |                                   2,008 |
+| Companies                   |                                   1,093 |
+| Unique Financial Statements |                                  12,139 |
+| First Financial Statement   |                              2009-01-31 |
+| Last Financial Statement    |                              2022-03-31 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
 
-|   | co_name                                | cvm_id | fiscal_id          |
-|--:|:---------------------------------------|-------:|:-------------------|
-| 0 | 3R PETROLEUM ÓLEO E GÁS S.A.           |  25291 | 12.091.809/0001-55 |
-| 1 | PETRO RIO S.A.                         |  22187 | 10.629.105/0001-68 |
-| 2 | PETROBRAS DISTRIBUIDORA S/A            |  24295 | 34.274.233/0001-02 |
-| 3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |   9512 | 33.000.167/0001-01 |
-| 4 | PETROLEO LUB DO NORDESTE SA            |   9520 | 07.275.159/0001-68 |
-| 5 | PETRORECÔNCAVO S.A.                    |  25780 | 03.342.704/0001-30 |
-| 6 | PRONOR PETROQUIMICA SA                 |   9784 | 13.552.070/0001-02 |
-| 7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |   9989 | 33.412.081/0001-96 |
+|     | co_name                                | co_id | co_fiscal_id       |
+| --: | :------------------------------------- | ----: | :----------------- |
+|   0 | 3R PETROLEUM ÓLEO E GÁS S.A.           | 25291 | 12.091.809/0001-55 |
+|   1 | PETRO RIO S.A.                         | 22187 | 10.629.105/0001-68 |
+|   2 | PETROBRAS DISTRIBUIDORA S/A            | 24295 | 34.274.233/0001-02 |
+|   3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |  9512 | 33.000.167/0001-01 |
+|   4 | PETROLEO LUB DO NORDESTE SA            |  9520 | 07.275.159/0001-68 |
+|   5 | PETRORECÔNCAVO S.A.                    | 25780 | 03.342.704/0001-30 |
+|   6 | PRONOR PETROQUIMICA SA                 |  9784 | 13.552.070/0001-02 |
+|   7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |  9989 | 33.412.081/0001-96 |
 
 ### The Company Class
+
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
 # Both CVM (regulator) ID or Fiscal ID can be used as an identifier.
 >>> petro = fl.Company(9512, acc_method='separate', acc_unit='million')
 
@@ -133,15 +137,15 @@
 >>> petro.acc_unit = 'billion'
 
 # Show company info:
 >>> petro.info()
 ```
 
 | Company Info               |                             Values |
-|:---------------------------|-----------------------------------:|
+| :------------------------- | ---------------------------------: |
 | Name                       | PETROLEO BRASILEIRO S.A. PETROBRAS |
 | CVM ID                     |                               9512 |
 | Fiscal ID (CNPJ)           |                 33.000.167/0001-01 |
 | Total Accounting Rows      |                             39,292 |
 | Selected Tax Rate          |                               0.34 |
 | Selected Accounting Method |                       consolidated |
 | Selected Accounting Unit   |                      1,000,000,000 |
@@ -153,33 +157,33 @@
 # Show company assets in Brazilian currency:
 >>> petro.report(report_type='assets')
 ...
 # Show company liabilities with custom arguments:
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
 ```
 
-| acc_code   | acc_name            | acc_fixed   |   2020-12-31 |   2021-12-31 |   2022-12-31 |
-|:-----------|:--------------------|:------------|-------------:|-------------:|-------------:|
-| 2.01.04    | Loans and Financing | True        |       51.364 |       50.631 |       47.65  |
-| 2.01.04.01 | Loans and Financing | True        |       21.751 |       20.316 |       18.656 |
-| 2.01.04.02 | Debentures          | True        |        0     |        0     |        0     |
-| 2.01.04.03 | Lease Financing     | True        |       29.613 |       30.315 |       28.994 |
-| 2.02.01    | Loans and Financing | True        |      341.184 |      277.187 |      233.053 |
-| 2.02.01.01 | Loans and Financing | True        |      258.287 |      178.908 |      137.63  |
-| 2.02.01.02 | Debentures          | True        |        0     |        0     |        0     |
-| 2.02.01.03 | Lease Financing     | True        |       82.897 |       98.279 |       95.423 |
+| acc_code   | acc_name            | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 |
+| :--------- | :------------------ | :-------- | ---------: | ---------: | ---------: |
+| 2.01.04    | Loans and Financing | True      |     51.364 |     50.631 |      47.65 |
+| 2.01.04.01 | Loans and Financing | True      |     21.751 |     20.316 |     18.656 |
+| 2.01.04.02 | Debentures          | True      |          0 |          0 |          0 |
+| 2.01.04.03 | Lease Financing     | True      |     29.613 |     30.315 |     28.994 |
+| 2.02.01    | Loans and Financing | True      |    341.184 |    277.187 |    233.053 |
+| 2.02.01.01 | Loans and Financing | True      |    258.287 |    178.908 |     137.63 |
+| 2.02.01.02 | Debentures          | True      |          0 |          0 |          0 |
+| 2.02.01.03 | Lease Financing     | True      |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Change account names to Portuguese:
 >>> petro.language = "portuguese"
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
 ```
 
 | acc_code   | acc_name                       | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 |
-|------------|--------------------------------|-----------|-----------:|-----------:|-----------:|
+| ---------- | ------------------------------ | --------- | ---------: | ---------: | ---------: |
 | 2.01.04    | Empréstimos e Financiamentos   | True      |     51.364 |     50.631 |      47.65 |
 | 2.01.04.01 | Empréstimos e Financiamentos   | True      |     21.751 |     20.316 |     18.656 |
 | 2.01.04.02 | Debêntures                     | True      |          0 |          0 |          0 |
 | 2.01.04.03 | Financiamento por Arrendamento | True      |     29.613 |     30.315 |     28.994 |
 | 2.02.01    | Empréstimos e Financiamentos   | True      |    341.184 |    277.187 |    233.053 |
 | 2.02.01.01 | Empréstimos e Financiamentos   | True      |    258.287 |    178.908 |     137.63 |
 | 2.02.01.02 | Debêntures                     | True      |          0 |          0 |          0 |
@@ -187,15 +191,15 @@
 
 ```python
 # Show company main indicators:
 >>> petro.indicators(num_years=3)
 ```
 
 | Company Financial Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 |
-|:-----------------------------|-----------:|-----------:|-----------:|
+| :--------------------------- | ---------: | ---------: | ---------: |
 | revenues                     |    302.245 |    272.069 |    452.668 |
 | operating_cash_flow          |    101.766 |    148.106 |    203.126 |
 | ebitda                       |    140.203 |    107.926 |    273.879 |
 | ebit                         |     81.701 |     49.621 |    210.831 |
 | net_income                   |     40.970 |      6.246 |    107.264 |
 | total_cash                   |     33.294 |     64.280 |     62.040 |
 | total_debt                   |    351.161 |    392.548 |    327.818 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FinLogic Version: 0.3.6 Summary: Finance toolkit
+Metadata-Version: 2.1 Name: FinLogic Version: 0.3.7 Summary: Finance toolkit
 for listed Brazilian companies Keywords: pandas, cvm, finance, investment,
 accounting Author-email: Carlos Carvalho
 cj@outlook.com> Requires-Python: >=3.10 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Office/Business ::
 Financial :: Accounting Classifier: Topic :: Office/Business :: Financial ::
 Investment Provides-Extra: test Project-URL: repository, https://github.com/
@@ -42,71 +42,71 @@
 data analysis. In the firt run, the process can take 3 minutes depending on CVM
 Server connection and local CPU power. The database generation needs at least 8
 GB of free memory and a quad core processor is recommended. For subsequent
 updates, only updated CVM files will be processed and inserted into the
 database, which will be faster. ```python >>> import finlogic as fl # Compile
 FinLogic database for the first time: >>> fl.update_database() Updating CVM raw
 files... ... FinLogic database updated â # Show database info: >>>
-fl.database_info() ``` | FinLogic Database Info | Value | |:-------------------
----------|----------------------------------------:| | Database Path | /home/
+fl.database_info() ``` | FinLogic Database Info | Value | | :------------------
+-------- | --------------------------------------: | | Database Path | /home/
 crcj/repos/FinLogic/finlogic/data | | File Size (MB) | 39.0 | | Last Update
 Call | 2022-04-20 07:29:08 | | Finlogic Last Modified | 2022-04-20 07:31:48 | |
 CVM Last Update | 2022-04-17 13:09:01 | | Size in Memory (MB) | 626.3 | |
 Accounting Rows | 18,757,249 | | Unique Accounting Codes | 2,008 | | Companies
 | 1,093 | | Unique Financial Statements | 12,139 | | First Financial Statement
 | 2009-01-31 | | Last Financial Statement | 2022-03-31 | ```python # Search for
-a company in database: >>> fl.search_company('petro') ``` | | co_name | cvm_id
-| fiscal_id | |--:|:---------------------------------------|-------:|:---------
-----------| | 0 | 3R PETROLEUM ÃLEO E GÃS S.A. | 25291 | 12.091.809/0001-55 |
-| 1 | PETRO RIO S.A. | 22187 | 10.629.105/0001-68 | | 2 | PETROBRAS
+a company in database: >>> fl.search_company('petro') ``` | | co_name | co_id |
+co_fiscal_id | | --: | :------------------------------------- | ----: | :------
+----------- | | 0 | 3R PETROLEUM ÃLEO E GÃS S.A. | 25291 | 12.091.809/0001-55
+| | 1 | PETRO RIO S.A. | 22187 | 10.629.105/0001-68 | | 2 | PETROBRAS
 DISTRIBUIDORA S/A | 24295 | 34.274.233/0001-02 | | 3 | PETROLEO BRASILEIRO S.A.
 PETROBRAS | 9512 | 33.000.167/0001-01 | | 4 | PETROLEO LUB DO NORDESTE SA |
 9520 | 07.275.159/0001-68 | | 5 | PETRORECÃNCAVO S.A. | 25780 | 03.342.704/
 0001-30 | | 6 | PRONOR PETROQUIMICA SA | 9784 | 13.552.070/0001-02 | | 7 |
 REFINARIA DE PETROLEOS MANGUINHOS S.A. | 9989 | 33.412.081/0001-96 | ### The
 Company Class The Company Class allows you to easily access financial data from
 Brazilian companies. All values are in local currency (Real). ```python #
 Create a Company object to acces its financial data: # Both CVM (regulator) ID
 or Fiscal ID can be used as an identifier. >>> petro = fl.Company(9512,
 acc_method='separate', acc_unit='million') # Change company accounting method
 back to consolidated (default): >>> petro.acc_method = 'consolidated' # Change
 company accounting unit to billion (default is 1): >>> petro.acc_unit =
-'billion' # Show company info: >>> petro.info() ``` | Company Info | Values |
-|:---------------------------|-----------------------------------:| | Name |
+'billion' # Show company info: >>> petro.info() ``` | Company Info | Values | |
+:------------------------- | ---------------------------------: | | Name |
 PETROLEO BRASILEIRO S.A. PETROBRAS | | CVM ID | 9512 | | Fiscal ID (CNPJ) |
 33.000.167/0001-01 | | Total Accounting Rows | 39,292 | | Selected Tax Rate |
 0.34 | | Selected Accounting Method | consolidated | | Selected Accounting Unit
 | 1,000,000,000 | | First Annual Report | 2009-12-31 | | Last Annual Report |
 2021-12-31 | | Last Quarterly Report | 2021-09-30 | ```python # Show company
 assets in Brazilian currency: >>> petro.report(report_type='assets') ... # Show
 company liabilities with custom arguments: >>> petro.report(report_type='debt',
 acc_level=4, num_years=3) ``` | acc_code | acc_name | acc_fixed | 2020-12-31 |
-2021-12-31 | 2022-12-31 | |:-----------|:--------------------|:------------|---
-----------:|-------------:|-------------:| | 2.01.04 | Loans and Financing |
-True | 51.364 | 50.631 | 47.65 | | 2.01.04.01 | Loans and Financing | True |
-21.751 | 20.316 | 18.656 | | 2.01.04.02 | Debentures | True | 0 | 0 | 0 | |
-2.01.04.03 | Lease Financing | True | 29.613 | 30.315 | 28.994 | | 2.02.01 |
-Loans and Financing | True | 341.184 | 277.187 | 233.053 | | 2.02.01.01 | Loans
-and Financing | True | 258.287 | 178.908 | 137.63 | | 2.02.01.02 | Debentures |
+2021-12-31 | 2022-12-31 | | :--------- | :------------------ | :-------- | ----
+-----: | ---------: | ---------: | | 2.01.04 | Loans and Financing | True |
+51.364 | 50.631 | 47.65 | | 2.01.04.01 | Loans and Financing | True | 21.751 |
+20.316 | 18.656 | | 2.01.04.02 | Debentures | True | 0 | 0 | 0 | | 2.01.04.03 |
+Lease Financing | True | 29.613 | 30.315 | 28.994 | | 2.02.01 | Loans and
+Financing | True | 341.184 | 277.187 | 233.053 | | 2.02.01.01 | Loans and
+Financing | True | 258.287 | 178.908 | 137.63 | | 2.02.01.02 | Debentures |
 True | 0 | 0 | 0 | | 2.02.01.03 | Lease Financing | True | 82.897 | 98.279 |
 95.423 | ```python # Change account names to Portuguese: >>> petro.language =
 "portuguese" >>> petro.report(report_type='debt', acc_level=4, num_years=3) ```
-| acc_code | acc_name | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 | |---
----------|--------------------------------|-----------|-----------:|----------
--:|-----------:| | 2.01.04 | EmprÃ©stimos e Financiamentos | True | 51.364 |
+| acc_code | acc_name | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 | | --
+-------- | ------------------------------ | --------- | ---------: | ---------:
+| ---------: | | 2.01.04 | EmprÃ©stimos e Financiamentos | True | 51.364 |
 50.631 | 47.65 | | 2.01.04.01 | EmprÃ©stimos e Financiamentos | True | 21.751 |
 20.316 | 18.656 | | 2.01.04.02 | DebÃªntures | True | 0 | 0 | 0 | | 2.01.04.03
 | Financiamento por Arrendamento | True | 29.613 | 30.315 | 28.994 | | 2.02.01
 | EmprÃ©stimos e Financiamentos | True | 341.184 | 277.187 | 233.053 | |
 2.02.01.01 | EmprÃ©stimos e Financiamentos | True | 258.287 | 178.908 | 137.63
 | | 2.02.01.02 | DebÃªntures | True | 0 | 0 | 0 | | 2.02.01.03 | Financiamento
 por Arrendamento | True | 82.897 | 98.279 | 95.423 | ```python # Show company
 main indicators: >>> petro.indicators(num_years=3) ``` | Company Financial
-Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 | |:-------------------------
-----|-----------:|-----------:|-----------:| | revenues | 302.245 | 272.069 |
+Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 | | :------------------------
+--- | ---------: | ---------: | ---------: | | revenues | 302.245 | 272.069 |
 452.668 | | operating_cash_flow | 101.766 | 148.106 | 203.126 | | ebitda |
 140.203 | 107.926 | 273.879 | | ebit | 81.701 | 49.621 | 210.831 | | net_income
 | 40.970 | 6.246 | 107.264 | | total_cash | 33.294 | 64.280 | 62.040 | |
 total_debt | 351.161 | 392.548 | 327.818 | | net_debt | 317.867 | 328.268 |
 265.778 | | working_capital | -4.046 | 6.036 | 33.334 | | invested_capital |
 617.004 | 639.418 | 655.359 | | return_on_assets | 0.062 | 0.035 | 0.140 | |
 return_on_capital | 0.097 | 0.053 | 0.217 | | return_on_equity | 0.144 | 0.020
```

