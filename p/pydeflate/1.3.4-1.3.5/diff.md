# Comparing `tmp/pydeflate-1.3.4.tar.gz` & `tmp/pydeflate-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeflate-1.3.4.tar", max compression
+gzip compressed data, was "pydeflate-1.3.5.tar", max compression
```

## Comparing `pydeflate-1.3.4.tar` & `pydeflate-1.3.5.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-02-20 10:51:25.431917 pydeflate-1.3.4/LICENSE
--rw-r--r--   0        0        0     8999 2023-02-20 10:51:25.431917 pydeflate-1.3.4/README.md
--rw-r--r--   0        0        0       25 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/.pydeflate_data/README.md
--rw-r--r--   0        0        0      775 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/deflate/__init__.py
--rw-r--r--   0        0        0    11829 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/deflate/deflate.py
--rw-r--r--   0        0        0     2684 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/deflate/deflator.py
--rw-r--r--   0        0        0        0 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/get_data/__init__.py
--rw-r--r--   0        0        0     2285 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/get_data/deflate_data.py
--rw-r--r--   0        0        0    12091 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/get_data/exchange_data.py
--rw-r--r--   0        0        0     2693 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/get_data/imf_data.py
--rw-r--r--   0        0        0     6110 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/get_data/oecd_data.py
--rw-r--r--   0        0        0     2103 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/get_data/wb_data.py
--rw-r--r--   0        0        0      894 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/pydeflate_config.py
--rw-r--r--   0        0        0      133 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/settings/emu.json
--rw-r--r--   0        0        0      911 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/settings/oecd_codes.json
--rw-r--r--   0        0        0       47 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/tools/__init__.py
--rw-r--r--   0        0        0     5465 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/tools/exchange.py
--rw-r--r--   0        0        0     2110 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/tools/update_data.py
--rw-r--r--   0        0        0     1573 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pydeflate/utils.py
--rw-r--r--   0        0        0     1059 2023-02-20 10:51:25.431917 pydeflate-1.3.4/pyproject.toml
--rw-r--r--   0        0        0    10341 1970-01-01 00:00:00.000000 pydeflate-1.3.4/setup.py
--rw-r--r--   0        0        0    10147 1970-01-01 00:00:00.000000 pydeflate-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-13 15:58:40.696639 pydeflate-1.3.5/LICENSE
+-rw-r--r--   0        0        0     8999 2023-04-13 15:58:40.696639 pydeflate-1.3.5/README.md
+-rw-r--r--   0        0        0       25 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/.pydeflate_data/README.md
+-rw-r--r--   0        0        0      775 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/deflate/__init__.py
+-rw-r--r--   0        0        0    11829 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/deflate/deflate.py
+-rw-r--r--   0        0        0     2684 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/deflate/deflator.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/__init__.py
+-rw-r--r--   0        0        0     2285 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/deflate_data.py
+-rw-r--r--   0        0        0    12091 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/exchange_data.py
+-rw-r--r--   0        0        0     2693 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/imf_data.py
+-rw-r--r--   0        0        0     6177 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/oecd_data.py
+-rw-r--r--   0        0        0     2103 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/get_data/wb_data.py
+-rw-r--r--   0        0        0      894 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/pydeflate_config.py
+-rw-r--r--   0        0        0      133 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/settings/emu.json
+-rw-r--r--   0        0        0      911 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/settings/oecd_codes.json
+-rw-r--r--   0        0        0       47 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/tools/__init__.py
+-rw-r--r--   0        0        0     5465 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/tools/exchange.py
+-rw-r--r--   0        0        0     2110 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/tools/update_data.py
+-rw-r--r--   0        0        0     1573 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pydeflate/utils.py
+-rw-r--r--   0        0        0     1059 2023-04-13 15:58:40.700639 pydeflate-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0    10147 1970-01-01 00:00:00.000000 pydeflate-1.3.5/PKG-INFO
```

### Comparing `pydeflate-1.3.4/LICENSE` & `pydeflate-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/README.md` & `pydeflate-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/__init__.py` & `pydeflate-1.3.5/pydeflate/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = """Jorge Rivera"""
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 
 from pydeflate.deflate.deflate import deflate
 from pydeflate.tools.exchange import exchange
 from pydeflate.tools.update_data import update_all_data, warn_updates
 from pydeflate.get_data.oecd_data import update_dac1
 from pydeflate import get_data
```

### Comparing `pydeflate-1.3.4/pydeflate/deflate/deflate.py` & `pydeflate-1.3.5/pydeflate/deflate/deflate.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/deflate/deflator.py` & `pydeflate-1.3.5/pydeflate/deflate/deflator.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/get_data/deflate_data.py` & `pydeflate-1.3.5/pydeflate/get_data/deflate_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/get_data/exchange_data.py` & `pydeflate-1.3.5/pydeflate/get_data/exchange_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/get_data/imf_data.py` & `pydeflate-1.3.5/pydeflate/get_data/imf_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/get_data/oecd_data.py` & `pydeflate-1.3.5/pydeflate/get_data/oecd_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,17 +138,17 @@
     update_update_date("OECD DAC")
 
     # Log
     logger.info("Successfully downloaded DAC1 data")
 
 
 def _identify_base_year(df: pd.DataFrame) -> int:
-
     return (
-        df.groupby(["year"], as_index=False)
+        df.query("iso_code in ['FRA','GBR','USA','CAN','DEU','EUI']")
+        .groupby(["year"], as_index=False)
         .value.mean(numeric_only=True)
         .round(2)
         .loc[lambda d: d.value == 100.00]
         .year.dt.year.item()
     )
```

### Comparing `pydeflate-1.3.4/pydeflate/get_data/wb_data.py` & `pydeflate-1.3.5/pydeflate/get_data/wb_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/pydeflate_config.py` & `pydeflate-1.3.5/pydeflate/pydeflate_config.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/settings/oecd_codes.json` & `pydeflate-1.3.5/pydeflate/settings/oecd_codes.json`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/tools/exchange.py` & `pydeflate-1.3.5/pydeflate/tools/exchange.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/tools/update_data.py` & `pydeflate-1.3.5/pydeflate/tools/update_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pydeflate/utils.py` & `pydeflate-1.3.5/pydeflate/utils.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.4/pyproject.toml` & `pydeflate-1.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydeflate"
-version = "1.3.4"
+version = "1.3.5"
 description = "Package to convert current prices figures to constant prices and vice versa"
 authors = ["Jorge Rivera <jorge.rivera@one.org>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: End Users/Desktop',
```

### Comparing `pydeflate-1.3.4/setup.py` & `pydeflate-1.3.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,307 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydeflate
+Version: 1.3.5
+Summary: Package to convert current prices figures to constant prices and vice versa
+License: MIT
+Author: Jorge Rivera
+Author-email: jorge.rivera@one.org
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: bblocks (>=1.0.2,<2.0.0)
+Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
+Requires-Dist: country-converter (>=0.8.0,<0.9.0)
+Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: weo (>=0.7.4,<0.8.0)
+Requires-Dist: xlrd (>=2.0.1,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['pydeflate', 'pydeflate.deflate', 'pydeflate.get_data', 'pydeflate.tools']
+# pydeflate
 
-package_data = \
-{'': ['*'], 'pydeflate': ['.pydeflate_data/*', 'settings/*']}
+[![pypi](https://img.shields.io/pypi/v/pydeflate.svg)](https://pypi.python.org/pypi/pydeflate)
+[![Documentation Status](https://readthedocs.org/projects/pydeflate/badge/?version=latest)](https://pydeflate.readthedocs.io/en/latest/?version=latest)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Downloads](https://pepy.tech/badge/pydeflate/month)](https://pepy.tech/project/pydeflate)
+[![Coverage](https://codecov.io/gh/jm-rivera/pydeflate/branch/main/graph/badge.svg?token=uwKI5DyO3w)](https://codecov.io/gh/jm-rivera/pydeflate)
 
-install_requires = \
-['bblocks>=1.0.2,<2.0.0',
- 'beautifulsoup4>=4.11.2,<5.0.0',
- 'country-converter>=0.8.0,<0.9.0',
- 'numpy>=1.24.1,<2.0.0',
- 'pandas>=1.5.3,<2.0.0',
- 'pyarrow>=11.0.0,<12.0.0',
- 'requests>=2.28.2,<3.0.0',
- 'weo>=0.7.4,<0.8.0',
- 'xlrd>=2.0.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'pydeflate',
-    'version': '1.3.4',
-    'description': 'Package to convert current prices figures to constant prices and vice versa',
-    'long_description': '# pydeflate\n\n[![pypi](https://img.shields.io/pypi/v/pydeflate.svg)](https://pypi.python.org/pypi/pydeflate)\n[![Documentation Status](https://readthedocs.org/projects/pydeflate/badge/?version=latest)](https://pydeflate.readthedocs.io/en/latest/?version=latest)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Downloads](https://pepy.tech/badge/pydeflate/month)](https://pepy.tech/project/pydeflate)\n[![Coverage](https://codecov.io/gh/jm-rivera/pydeflate/branch/main/graph/badge.svg?token=uwKI5DyO3w)](https://codecov.io/gh/jm-rivera/pydeflate)\n\n**pydeflate** is a Python package to convert flows data to constant\nprices. This can be done from any source currency to any desired base\nyear and currency. **Pydeflate** can also be used to convert constant\ndata to current prices and to convert from one currency to another (in\ncurrent and constant prices). Users can choose the source of the\nexchange and deflator/prices data (currently, IMF, World Bank or OECD\nDAC).\n\n## Getting started\n\n### Installation\n\npydeflate can be installed from PyPI. From the command line:\n\n```bash\n\npip install pydeflate\n\n```\n\n## Basic usage\n\n### Current to constant\n\nConvert data expressed in current USD prices to constant EUR prices for\na given base year:\n\n```python\nfrom pydeflate import deflate, set_pydeflate_path\nimport pandas as pd\n\n# Specify where the deflator and exchange data should be saved\nset_pydeflate_path("path/to/data/folder")\n\n# example data\ndata = {\n    \'iso_code\': [\'FRA\', \'USA\', \'GTM\'],\n    \'year\': [2017, 2017, 2017],\n    \'value\': [50, 100, 200]\n}\n\n# create an example dataframe, in current USD prices\ndf = pd.DataFrame.from_dict(data)\n\n# convert to EUR 2015 constant prices\ndf_constant = deflate(\n    df=df,\n    base_year=2015,\n    deflator_source=\'world_bank\',\n    deflator_method=\'gdp\',\n    exchange_source="world_bank",\n    source_currency="USA",  # since data is in USD\n    target_currency="EMU",  # we want the result in constant EUR\n    id_column="iso_code",\n    id_type="ISO3",  # specifying this is optional in most cases\n    date_column="year",\n    source_column="value", # where the original data is\n    target_col="value_constant", # where the new data will be stored\n)\n```\n\nThis results in a dataframe containing a new column `value_constant` in\n2015 constant prices. In the background, pydeflate takes into account:\n\n- changes in princes, through a gdp deflator in this case\n- changes in exchange rates overtime\n\n### Current Local Currency Units to constant in a different currency\nPydeflate can also handle data that is expressed in local currency\nunits. In that case, users can specify `LCU` as the source currency.\n\n```python\nfrom pydeflate import deflate, set_pydeflate_path\nimport pandas as pd\n\n# Specify where the deflator and exchange data should be saved\nset_pydeflate_path("path/to/data/folder")\n\n# example data\ndata = {\n    \'country\': [\'United Kingdom\', \'United Kingdom\', \'Japan\'],\n    \'date\': [2011, 2015, 2015],\n    \'value\': [100, 100, 100]\n}\n\n# create an example dataframe, in current local currency units\ndf = pd.DataFrame.from_dict(data)\n\n# convert to USD 2018 constant prices\ndf_constant = deflate(\n    df=df,\n    base_year=2018,\n    deflator_source=\'imf\',\n    deflator_method=\'pcpi\',\n    exchange_source="imf",\n    source_currency="LCU",  # since data is in LCU\n    target_currency="USA",  # to get data in USD\n    id_column="iso_code",\n    date_column="date",\n    source_col="value",\n    target_col="value",  # to not create a new column\n)\n\n```\n\n### Constant to current\nUsers can also convert a dataset expressed in constant prices to current\nprices using pydeflate. To avoid introducing errors, users should know\nwhich methodology/ data was used to create constant prices by the\noriginal source. The basic usage is the same as before, but the\n`to_current` parameter is set to `True`.\n\nFor example, to convert DAC data expressed in 2016 USD constant prices\nto current US dollars:\n\n```python\nfrom pydeflate import deflate, set_pydeflate_path\nimport pandas as pd\n\n# Specify where the deflator and exchange data should be saved\nset_pydeflate_path("path/to/data/folder")\n\n# example data\ndata = {\n    \'dac_code\': [302, 4, 4],\n    \'date\': [2010, 2016, 2018],\n    \'value\': [100, 100, 100]\n}\n\n# create an example dataframe, in current local currency units\ndf = pd.DataFrame.from_dict(data)\n\n# convert to USD 2018 constant prices\ndf_current = deflate(\n    df=df,\n    base_year=2016,\n    deflator_source=\'oecd_dac\',\n    deflator_method=\'dac_deflator\',\n    exchange_source="oecd_dac",\n    source_currency="USA",  # since data is in USD constant\n    target_currency="LCU",  # to get the current LCU figures\n    id_column="dac_code",\n    id_type="DAC",\n    date_column="date",\n    source_column="value",\n    target_column="value_current",\n    to_current=True,\n)\n```\n\n## Data source and method options\n\nIn order to convert the data, pydeflate uses data on **price/gdp deflators** and\n**exchange rates**. Each of these data sources can come from the `OECD DAC`,\n`IMF (WEO)` or `World Bank`.\n\nFor all sources, Exchange rates between two non USD currency pairs are derived from\nthe LCU to USD exchange rates selected.\n\n### International Monetary Fund World Economic Outlook ("imf")\n\nFor price/gdp deflators from the IMF, the following options are available (`deflator_method`):\n- `gdp`: in order to use GDP deflators.\n- `pcpi`: in order to use Consumer Price Index data.\n- `pcpie`: to use end-of-period Consumer Price Index data\n  (e.g. for December each year).\n\nThe IMF provides estimates where data is not available, including for several\nyears into the future. Using these price deflators, combined with the corresponding\nexchange rates, allows users to convert data to constant prices for future years.\n\nFor exchange rates, the following options are available from the imf (`exchange_method`):\n- `implied`: to use the exchange rates used by the World Economic Outlook, derived from\n    the WEOs data on GDP in US Dollars and Local Currency Units.\n\n### World Bank ("world_bank")\n\nFor price/gdp deflators from the World Bank, the following options are available (`deflator_method`):\n\n\nIn terms of price or GDP deflators, pydeflate provides the following\n- `gdp`: in order to use GDP deflators.\n- `gdp_linked`: to use the World Bank\'s GDP deflator series which\n  has been linked to produce a consistent time series to\n  counteract breaks in series over time due to changes in base\n  years, sources or methodologies.\n- `cpi`: to use Consumer Price Index data\n\nFor exchange rates, the following options are available from the World Bank (`exchange_method`):\n- `yearly_average`: as used by the World Bank, based on IMF International Financial Statistics data.\n\n\n### OECD Development Assistance Committee ("oecd_dac")\n\nFor price/gdp deflators from the OECD DAC, the following options are available (`deflator_method`):\n\nIn terms of price or GDP deflators, pydeflate provides the following:\n- `dac_deflator`: in order to use the DAC\'s own deflator series.\n\nFor exchange rates, the following options are available from the OECD DAC (`exchange_method`):\n- `implied`: to use the exchange rates used and published by the DAC.\n\n\n\n## Additional features\n\nPydeflate relies on data from the World Bank, IMF and OECD for its\ncalculations. This data is updated periodically. If the version of the\ndata stored in the user\'s computer is older than 50 days, pydeflate will\nshow a warning on import.\n\nUsers can always update the underlying data by using:\n\n```python\nimport pydeflate\n\npydeflate.update_all_data()\n\n```\n\nPydeflate also provides users with a tool to exchange figures from one\ncurrency to another, without applying any deflators. This should only be\nused on numbers expressed in current prices, however.\n\nFor example, to convert numbers in current Local Currency Units (LCU) to\ncurrent Canadian Dollars:\n\n```python\nimport pydeflate\nimport pandas as pd\n\n# example data\ndata = {\n    \'iso_code\': [\'GBR\', \'CAN\', \'JPN\'],\n    \'date\': [2011, 2015, 2015],\n    \'value\': [100, 100, 100]\n}\n\n# create an example dataframe, in current local currency units\ndf = pd.DataFrame.from_dict(data)\n\n# convert to USD 2018 constant prices\ndf_can = pydeflate.exchange(\n    df=df,\n    source_currency="LCU",  # since data is in LCU\n    target_currency="CAN",  # to get data in Canadian Dollars\n    rates_source=\'imf\', \n    value_column=\'value\',\n    target_column=\'value_CAN\',\n    id_column="iso_code",\n    id_type="ISO3",\n    date_column="date",\n)\n\n```\n\n### Credits\n\nThis package relies on data from the following sources:\n\n- OECD DAC: <https://www.oecd.org/dac/> (Official Development\n  assistance data (DAC1), DAC deflators, and exchange rates used by\n  the DAC)\n- IMF World Economic Outlook:\n  <https://www.imf.org/en/Publications/WEO> (GDP and price deflators)\n- World Bank DataBank: <https://databank.worldbank.org/home.aspx>\n  (exchange rates, GDP and price deflators)\n\nThis data is provided based on the terms and conditions set by the\noriginal sources.',
-    'author': 'Jorge Rivera',
-    'author_email': 'jorge.rivera@one.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+**pydeflate** is a Python package to convert flows data to constant
+prices. This can be done from any source currency to any desired base
+year and currency. **Pydeflate** can also be used to convert constant
+data to current prices and to convert from one currency to another (in
+current and constant prices). Users can choose the source of the
+exchange and deflator/prices data (currently, IMF, World Bank or OECD
+DAC).
+
+## Getting started
+
+### Installation
+
+pydeflate can be installed from PyPI. From the command line:
+
+```bash
+
+pip install pydeflate
+
+```
+
+## Basic usage
+
+### Current to constant
+
+Convert data expressed in current USD prices to constant EUR prices for
+a given base year:
+
+```python
+from pydeflate import deflate, set_pydeflate_path
+import pandas as pd
+
+# Specify where the deflator and exchange data should be saved
+set_pydeflate_path("path/to/data/folder")
+
+# example data
+data = {
+    'iso_code': ['FRA', 'USA', 'GTM'],
+    'year': [2017, 2017, 2017],
+    'value': [50, 100, 200]
+}
+
+# create an example dataframe, in current USD prices
+df = pd.DataFrame.from_dict(data)
+
+# convert to EUR 2015 constant prices
+df_constant = deflate(
+    df=df,
+    base_year=2015,
+    deflator_source='world_bank',
+    deflator_method='gdp',
+    exchange_source="world_bank",
+    source_currency="USA",  # since data is in USD
+    target_currency="EMU",  # we want the result in constant EUR
+    id_column="iso_code",
+    id_type="ISO3",  # specifying this is optional in most cases
+    date_column="year",
+    source_column="value", # where the original data is
+    target_col="value_constant", # where the new data will be stored
+)
+```
+
+This results in a dataframe containing a new column `value_constant` in
+2015 constant prices. In the background, pydeflate takes into account:
+
+- changes in princes, through a gdp deflator in this case
+- changes in exchange rates overtime
+
+### Current Local Currency Units to constant in a different currency
+Pydeflate can also handle data that is expressed in local currency
+units. In that case, users can specify `LCU` as the source currency.
+
+```python
+from pydeflate import deflate, set_pydeflate_path
+import pandas as pd
+
+# Specify where the deflator and exchange data should be saved
+set_pydeflate_path("path/to/data/folder")
+
+# example data
+data = {
+    'country': ['United Kingdom', 'United Kingdom', 'Japan'],
+    'date': [2011, 2015, 2015],
+    'value': [100, 100, 100]
 }
 
+# create an example dataframe, in current local currency units
+df = pd.DataFrame.from_dict(data)
+
+# convert to USD 2018 constant prices
+df_constant = deflate(
+    df=df,
+    base_year=2018,
+    deflator_source='imf',
+    deflator_method='pcpi',
+    exchange_source="imf",
+    source_currency="LCU",  # since data is in LCU
+    target_currency="USA",  # to get data in USD
+    id_column="iso_code",
+    date_column="date",
+    source_col="value",
+    target_col="value",  # to not create a new column
+)
+
+```
+
+### Constant to current
+Users can also convert a dataset expressed in constant prices to current
+prices using pydeflate. To avoid introducing errors, users should know
+which methodology/ data was used to create constant prices by the
+original source. The basic usage is the same as before, but the
+`to_current` parameter is set to `True`.
+
+For example, to convert DAC data expressed in 2016 USD constant prices
+to current US dollars:
+
+```python
+from pydeflate import deflate, set_pydeflate_path
+import pandas as pd
+
+# Specify where the deflator and exchange data should be saved
+set_pydeflate_path("path/to/data/folder")
+
+# example data
+data = {
+    'dac_code': [302, 4, 4],
+    'date': [2010, 2016, 2018],
+    'value': [100, 100, 100]
+}
+
+# create an example dataframe, in current local currency units
+df = pd.DataFrame.from_dict(data)
+
+# convert to USD 2018 constant prices
+df_current = deflate(
+    df=df,
+    base_year=2016,
+    deflator_source='oecd_dac',
+    deflator_method='dac_deflator',
+    exchange_source="oecd_dac",
+    source_currency="USA",  # since data is in USD constant
+    target_currency="LCU",  # to get the current LCU figures
+    id_column="dac_code",
+    id_type="DAC",
+    date_column="date",
+    source_column="value",
+    target_column="value_current",
+    to_current=True,
+)
+```
+
+## Data source and method options
+
+In order to convert the data, pydeflate uses data on **price/gdp deflators** and
+**exchange rates**. Each of these data sources can come from the `OECD DAC`,
+`IMF (WEO)` or `World Bank`.
+
+For all sources, Exchange rates between two non USD currency pairs are derived from
+the LCU to USD exchange rates selected.
+
+### International Monetary Fund World Economic Outlook ("imf")
+
+For price/gdp deflators from the IMF, the following options are available (`deflator_method`):
+- `gdp`: in order to use GDP deflators.
+- `pcpi`: in order to use Consumer Price Index data.
+- `pcpie`: to use end-of-period Consumer Price Index data
+  (e.g. for December each year).
+
+The IMF provides estimates where data is not available, including for several
+years into the future. Using these price deflators, combined with the corresponding
+exchange rates, allows users to convert data to constant prices for future years.
+
+For exchange rates, the following options are available from the imf (`exchange_method`):
+- `implied`: to use the exchange rates used by the World Economic Outlook, derived from
+    the WEOs data on GDP in US Dollars and Local Currency Units.
+
+### World Bank ("world_bank")
+
+For price/gdp deflators from the World Bank, the following options are available (`deflator_method`):
+
+
+In terms of price or GDP deflators, pydeflate provides the following
+- `gdp`: in order to use GDP deflators.
+- `gdp_linked`: to use the World Bank's GDP deflator series which
+  has been linked to produce a consistent time series to
+  counteract breaks in series over time due to changes in base
+  years, sources or methodologies.
+- `cpi`: to use Consumer Price Index data
+
+For exchange rates, the following options are available from the World Bank (`exchange_method`):
+- `yearly_average`: as used by the World Bank, based on IMF International Financial Statistics data.
+
+
+### OECD Development Assistance Committee ("oecd_dac")
+
+For price/gdp deflators from the OECD DAC, the following options are available (`deflator_method`):
+
+In terms of price or GDP deflators, pydeflate provides the following:
+- `dac_deflator`: in order to use the DAC's own deflator series.
+
+For exchange rates, the following options are available from the OECD DAC (`exchange_method`):
+- `implied`: to use the exchange rates used and published by the DAC.
+
+
+
+## Additional features
+
+Pydeflate relies on data from the World Bank, IMF and OECD for its
+calculations. This data is updated periodically. If the version of the
+data stored in the user's computer is older than 50 days, pydeflate will
+show a warning on import.
+
+Users can always update the underlying data by using:
+
+```python
+import pydeflate
+
+pydeflate.update_all_data()
+
+```
+
+Pydeflate also provides users with a tool to exchange figures from one
+currency to another, without applying any deflators. This should only be
+used on numbers expressed in current prices, however.
+
+For example, to convert numbers in current Local Currency Units (LCU) to
+current Canadian Dollars:
+
+```python
+import pydeflate
+import pandas as pd
+
+# example data
+data = {
+    'iso_code': ['GBR', 'CAN', 'JPN'],
+    'date': [2011, 2015, 2015],
+    'value': [100, 100, 100]
+}
+
+# create an example dataframe, in current local currency units
+df = pd.DataFrame.from_dict(data)
+
+# convert to USD 2018 constant prices
+df_can = pydeflate.exchange(
+    df=df,
+    source_currency="LCU",  # since data is in LCU
+    target_currency="CAN",  # to get data in Canadian Dollars
+    rates_source='imf', 
+    value_column='value',
+    target_column='value_CAN',
+    id_column="iso_code",
+    id_type="ISO3",
+    date_column="date",
+)
+
+```
+
+### Credits
+
+This package relies on data from the following sources:
+
+- OECD DAC: <https://www.oecd.org/dac/> (Official Development
+  assistance data (DAC1), DAC deflators, and exchange rates used by
+  the DAC)
+- IMF World Economic Outlook:
+  <https://www.imf.org/en/Publications/WEO> (GDP and price deflators)
+- World Bank DataBank: <https://databank.worldbank.org/home.aspx>
+  (exchange rates, GDP and price deflators)
 
-setup(**setup_kwargs)
+This data is provided based on the terms and conditions set by the
+original sources.
```

