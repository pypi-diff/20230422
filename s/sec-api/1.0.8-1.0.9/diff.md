# Comparing `tmp/sec-api-1.0.8.tar.gz` & `tmp/sec-api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sec-api-1.0.8.tar", last modified: Sat Oct 30 14:51:42 2021, max compression
+gzip compressed data, was "dist/sec-api-1.0.9.tar", last modified: Mon Feb  7 10:25:51 2022, max compression
```

## Comparing `sec-api-1.0.8.tar` & `sec-api-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2021-10-30 14:51:42.000000 sec-api-1.0.8/
--rw-r--r--   0 jan        (501) staff       (20)    28428 2021-10-30 14:51:42.000000 sec-api-1.0.8/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)    22263 2021-10-30 14:47:39.000000 sec-api-1.0.8/README.md
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2021-10-30 14:51:42.000000 sec-api-1.0.8/sec_api/
--rw-r--r--   0 jan        (501) staff       (20)      205 2021-09-17 11:32:56.000000 sec-api-1.0.8/sec_api/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     2921 2021-10-30 14:42:14.000000 sec-api-1.0.8/sec_api/index.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2021-10-30 14:51:42.000000 sec-api-1.0.8/sec_api.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)    28428 2021-10-30 14:51:42.000000 sec-api-1.0.8/sec_api.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)      219 2021-10-30 14:51:42.000000 sec-api-1.0.8/sec_api.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2021-10-30 14:51:42.000000 sec-api-1.0.8/sec_api.egg-info/dependency_links.txt
--rw-r--r--   0 jan        (501) staff       (20)        9 2021-10-30 14:51:42.000000 sec-api-1.0.8/sec_api.egg-info/requires.txt
--rw-r--r--   0 jan        (501) staff       (20)        8 2021-10-30 14:51:42.000000 sec-api-1.0.8/sec_api.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)       79 2021-10-30 14:51:42.000000 sec-api-1.0.8/setup.cfg
--rw-r--r--   0 jan        (501) staff       (20)     1638 2021-10-30 14:46:48.000000 sec-api-1.0.8/setup.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2022-02-07 10:25:51.000000 sec-api-1.0.9/
+-rw-r--r--   0 jan        (501) staff       (20)    31839 2022-02-07 10:25:51.000000 sec-api-1.0.9/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)    25066 2022-02-07 10:21:11.000000 sec-api-1.0.9/README.md
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2022-02-07 10:25:51.000000 sec-api-1.0.9/sec_api/
+-rw-r--r--   0 jan        (501) staff       (20)      242 2022-02-07 09:44:46.000000 sec-api-1.0.9/sec_api/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     6813 2022-02-07 09:54:30.000000 sec-api-1.0.9/sec_api/index.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2022-02-07 10:25:51.000000 sec-api-1.0.9/sec_api.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)    31839 2022-02-07 10:25:51.000000 sec-api-1.0.9/sec_api.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)      219 2022-02-07 10:25:51.000000 sec-api-1.0.9/sec_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2022-02-07 10:25:51.000000 sec-api-1.0.9/sec_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jan        (501) staff       (20)        9 2022-02-07 10:25:51.000000 sec-api-1.0.9/sec_api.egg-info/requires.txt
+-rw-r--r--   0 jan        (501) staff       (20)        8 2022-02-07 10:25:51.000000 sec-api-1.0.9/sec_api.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)       79 2022-02-07 10:25:51.000000 sec-api-1.0.9/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)     1638 2022-02-07 10:21:58.000000 sec-api-1.0.9/setup.py
```

### Comparing `sec-api-1.0.8/PKG-INFO` & `sec-api-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: SEC EDGAR Filings API
 Home-page: UNKNOWN
 Author: SEC API
 Author-email: support@sec-api.io
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/janlukasschroeder/sec-api-python/issues
 Project-URL: Repository, https://github.com/janlukasschroeder/sec-api-python
@@ -432,14 +432,90 @@
         
         print(filing)
         ```
         
         > See the documentation for more details: https://sec-api.io/docs/sec-filings-render-api
         
         
+        # CUSIP/CIK/Ticker Mapping API
+        
+        Resolve a CUSIP, CIK, ticker symbol or company name to a set of standardized company details. Listing companies by exchange, sector and industry is also supported.
+        
+        Map any of the following parameters to company details:
+        - CUSIP
+        - CIK
+        - Ticker
+        - Company name
+        - Exchange
+        - Sector
+        - Industry
+        
+        The function returns an array of all matching companies in JSON format. For example, a look up of the ticker `IBM` returns multiple matches including `IBMD` and `IBME`.
+        
+        A company object includes the following properties:
+        
+        - `name` (string) - the name of the company, e.g. Tesla Inc
+        - `ticker` (string) - the ticker symbol of the company.
+        - `cik` (string) - the CIK of the company. Trailing zeros are removed.
+        - `cusip` (string) - one or multiple CUSIPs linked to the company. Multiple CUSIPs are delimited by space, e.g. "054748108 92931L302 92931L401"
+        - `exchange` (string) - the main exchange the company is listed on, e.g. NASDAQ
+        - `isDelisted` (boolean) - true if the company is no longer listed, false otherwise.
+        - `category` (string) - the security category, e.g. "Domestic Common Stock"
+        - `sector` (string) - the sector of the company, e.g. "Consumer Cyclical"
+        - `industry` (string) - the industry of the company, e.g. "Auto Manufacturers"
+        - `sic` (string) - four-digit SIC code, e.g. "3711"
+        - `sicSector` (string) - SIC sector name of the company, e.g. "Manufacturing"
+        - `sicIndustry` (string) - SIC industry name of the company, e.g. "Motor Vehicles & Passenger Car Bodies"
+        - `currency` (string) - operating currency of the company, e.g. "USD"
+        - `location` (string) - location of the company's headquarters
+        - `id` (string) - unique internal ID of the company, e.g. "e27d6e9606f216c569e46abf407685f3"
+        
+        Response type: `JSON`
+        
+        ## Usage
+        
+        ```python
+        from sec_api import MappingApi
+        
+        mappingApi = MappingApi(api_key="YOUR_API_KEY")
+        
+        result1 = mappingApi.resolve("ticker", "TSLA")
+        result2 = mappingApi.resolve("cik", "1318605")
+        result3 = mappingApi.resolve("cusip", "88160R101")
+        result4 = mappingApi.resolve("exchange", "NASDAQ")
+        ```
+        
+        ### Response Example
+        ```json
+        [
+            {
+                "name": "Tesla Inc",
+                "ticker": "TSLA",
+                "cik": "1318605",
+                "cusip": "88160R101",
+                "exchange": "NASDAQ",
+                "isDelisted": false,
+                "category": "Domestic Common Stock",
+                "sector": "Consumer Cyclical",
+                "industry": "Auto Manufacturers",
+                "sic": "3711",
+                "sicSector": "Manufacturing",
+                "sicIndustry": "Motor Vehicles & Passenger Car Bodies",
+                "famaSector": "",
+                "famaIndustry": "Automobiles and Trucks",
+                "currency": "USD",
+                "location": "California; U.S.A",
+                "id": "e27d6e9606f216c569e46abf407685f3"
+            }
+        ]
+        ```
+        
+        > See the documentation for more details: https://sec-api.io/docs/mapping-api
+        
+        
         # Query API Response Format
         
         - `accessionNo` (string) - Accession number of filing, e.g. 0000028917-20-000033
         - `cik` (string) - CIK of the filing issuer. Important: trailing `0` are removed.
         - `ticker` (string) - Ticker of company, e.g. AMOT. A ticker is not available when non-publicly traded companies report filings (e.g. form 4 reported by directors). Please contact us if you find filings that you think should have tickers (but don't).
         - `companyName` (string) - Name of company, e.g. Allied Motion Technologies Inc
         - `companyNameLong` (string) - Long version of company name including the filer type (Issuer, Filer, Reporting), e.g. ALLIED MOTION TECHNOLOGIES INC (0000046129) (Issuer)
```

### Comparing `sec-api-1.0.8/README.md` & `sec-api-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -421,14 +421,90 @@
 
 print(filing)
 ```
 
 > See the documentation for more details: https://sec-api.io/docs/sec-filings-render-api
 
 
+# CUSIP/CIK/Ticker Mapping API
+
+Resolve a CUSIP, CIK, ticker symbol or company name to a set of standardized company details. Listing companies by exchange, sector and industry is also supported.
+
+Map any of the following parameters to company details:
+- CUSIP
+- CIK
+- Ticker
+- Company name
+- Exchange
+- Sector
+- Industry
+
+The function returns an array of all matching companies in JSON format. For example, a look up of the ticker `IBM` returns multiple matches including `IBMD` and `IBME`.
+
+A company object includes the following properties:
+
+- `name` (string) - the name of the company, e.g. Tesla Inc
+- `ticker` (string) - the ticker symbol of the company.
+- `cik` (string) - the CIK of the company. Trailing zeros are removed.
+- `cusip` (string) - one or multiple CUSIPs linked to the company. Multiple CUSIPs are delimited by space, e.g. "054748108 92931L302 92931L401"
+- `exchange` (string) - the main exchange the company is listed on, e.g. NASDAQ
+- `isDelisted` (boolean) - true if the company is no longer listed, false otherwise.
+- `category` (string) - the security category, e.g. "Domestic Common Stock"
+- `sector` (string) - the sector of the company, e.g. "Consumer Cyclical"
+- `industry` (string) - the industry of the company, e.g. "Auto Manufacturers"
+- `sic` (string) - four-digit SIC code, e.g. "3711"
+- `sicSector` (string) - SIC sector name of the company, e.g. "Manufacturing"
+- `sicIndustry` (string) - SIC industry name of the company, e.g. "Motor Vehicles & Passenger Car Bodies"
+- `currency` (string) - operating currency of the company, e.g. "USD"
+- `location` (string) - location of the company's headquarters
+- `id` (string) - unique internal ID of the company, e.g. "e27d6e9606f216c569e46abf407685f3"
+
+Response type: `JSON`
+
+## Usage
+
+```python
+from sec_api import MappingApi
+
+mappingApi = MappingApi(api_key="YOUR_API_KEY")
+
+result1 = mappingApi.resolve("ticker", "TSLA")
+result2 = mappingApi.resolve("cik", "1318605")
+result3 = mappingApi.resolve("cusip", "88160R101")
+result4 = mappingApi.resolve("exchange", "NASDAQ")
+```
+
+### Response Example
+```json
+[
+    {
+        "name": "Tesla Inc",
+        "ticker": "TSLA",
+        "cik": "1318605",
+        "cusip": "88160R101",
+        "exchange": "NASDAQ",
+        "isDelisted": false,
+        "category": "Domestic Common Stock",
+        "sector": "Consumer Cyclical",
+        "industry": "Auto Manufacturers",
+        "sic": "3711",
+        "sicSector": "Manufacturing",
+        "sicIndustry": "Motor Vehicles & Passenger Car Bodies",
+        "famaSector": "",
+        "famaIndustry": "Automobiles and Trucks",
+        "currency": "USD",
+        "location": "California; U.S.A",
+        "id": "e27d6e9606f216c569e46abf407685f3"
+    }
+]
+```
+
+> See the documentation for more details: https://sec-api.io/docs/mapping-api
+
+
 # Query API Response Format
 
 - `accessionNo` (string) - Accession number of filing, e.g. 0000028917-20-000033
 - `cik` (string) - CIK of the filing issuer. Important: trailing `0` are removed.
 - `ticker` (string) - Ticker of company, e.g. AMOT. A ticker is not available when non-publicly traded companies report filings (e.g. form 4 reported by directors). Please contact us if you find filings that you think should have tickers (but don't).
 - `companyName` (string) - Name of company, e.g. Allied Motion Technologies Inc
 - `companyNameLong` (string) - Long version of company name including the filer type (Issuer, Filer, Reporting), e.g. ALLIED MOTION TECHNOLOGIES INC (0000046129) (Issuer)
```

### Comparing `sec-api-1.0.8/sec_api.egg-info/PKG-INFO` & `sec-api-1.0.9/sec_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sec-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: SEC EDGAR Filings API
 Home-page: UNKNOWN
 Author: SEC API
 Author-email: support@sec-api.io
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/janlukasschroeder/sec-api-python/issues
 Project-URL: Repository, https://github.com/janlukasschroeder/sec-api-python
@@ -432,14 +432,90 @@
         
         print(filing)
         ```
         
         > See the documentation for more details: https://sec-api.io/docs/sec-filings-render-api
         
         
+        # CUSIP/CIK/Ticker Mapping API
+        
+        Resolve a CUSIP, CIK, ticker symbol or company name to a set of standardized company details. Listing companies by exchange, sector and industry is also supported.
+        
+        Map any of the following parameters to company details:
+        - CUSIP
+        - CIK
+        - Ticker
+        - Company name
+        - Exchange
+        - Sector
+        - Industry
+        
+        The function returns an array of all matching companies in JSON format. For example, a look up of the ticker `IBM` returns multiple matches including `IBMD` and `IBME`.
+        
+        A company object includes the following properties:
+        
+        - `name` (string) - the name of the company, e.g. Tesla Inc
+        - `ticker` (string) - the ticker symbol of the company.
+        - `cik` (string) - the CIK of the company. Trailing zeros are removed.
+        - `cusip` (string) - one or multiple CUSIPs linked to the company. Multiple CUSIPs are delimited by space, e.g. "054748108 92931L302 92931L401"
+        - `exchange` (string) - the main exchange the company is listed on, e.g. NASDAQ
+        - `isDelisted` (boolean) - true if the company is no longer listed, false otherwise.
+        - `category` (string) - the security category, e.g. "Domestic Common Stock"
+        - `sector` (string) - the sector of the company, e.g. "Consumer Cyclical"
+        - `industry` (string) - the industry of the company, e.g. "Auto Manufacturers"
+        - `sic` (string) - four-digit SIC code, e.g. "3711"
+        - `sicSector` (string) - SIC sector name of the company, e.g. "Manufacturing"
+        - `sicIndustry` (string) - SIC industry name of the company, e.g. "Motor Vehicles & Passenger Car Bodies"
+        - `currency` (string) - operating currency of the company, e.g. "USD"
+        - `location` (string) - location of the company's headquarters
+        - `id` (string) - unique internal ID of the company, e.g. "e27d6e9606f216c569e46abf407685f3"
+        
+        Response type: `JSON`
+        
+        ## Usage
+        
+        ```python
+        from sec_api import MappingApi
+        
+        mappingApi = MappingApi(api_key="YOUR_API_KEY")
+        
+        result1 = mappingApi.resolve("ticker", "TSLA")
+        result2 = mappingApi.resolve("cik", "1318605")
+        result3 = mappingApi.resolve("cusip", "88160R101")
+        result4 = mappingApi.resolve("exchange", "NASDAQ")
+        ```
+        
+        ### Response Example
+        ```json
+        [
+            {
+                "name": "Tesla Inc",
+                "ticker": "TSLA",
+                "cik": "1318605",
+                "cusip": "88160R101",
+                "exchange": "NASDAQ",
+                "isDelisted": false,
+                "category": "Domestic Common Stock",
+                "sector": "Consumer Cyclical",
+                "industry": "Auto Manufacturers",
+                "sic": "3711",
+                "sicSector": "Manufacturing",
+                "sicIndustry": "Motor Vehicles & Passenger Car Bodies",
+                "famaSector": "",
+                "famaIndustry": "Automobiles and Trucks",
+                "currency": "USD",
+                "location": "California; U.S.A",
+                "id": "e27d6e9606f216c569e46abf407685f3"
+            }
+        ]
+        ```
+        
+        > See the documentation for more details: https://sec-api.io/docs/mapping-api
+        
+        
         # Query API Response Format
         
         - `accessionNo` (string) - Accession number of filing, e.g. 0000028917-20-000033
         - `cik` (string) - CIK of the filing issuer. Important: trailing `0` are removed.
         - `ticker` (string) - Ticker of company, e.g. AMOT. A ticker is not available when non-publicly traded companies report filings (e.g. form 4 reported by directors). Please contact us if you find filings that you think should have tickers (but don't).
         - `companyName` (string) - Name of company, e.g. Allied Motion Technologies Inc
         - `companyNameLong` (string) - Long version of company name including the filer type (Issuer, Filer, Reporting), e.g. ALLIED MOTION TECHNOLOGIES INC (0000046129) (Issuer)
```

### Comparing `sec-api-1.0.8/setup.py` & `sec-api-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="sec-api",
-    version="1.0.8",
+    version="1.0.9",
     author="SEC API",
     author_email="support@sec-api.io",
     description="SEC EDGAR Filings API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
```

