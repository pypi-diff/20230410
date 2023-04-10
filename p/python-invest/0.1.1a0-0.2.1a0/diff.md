# Comparing `tmp/python-invest-0.1.1a0.tar.gz` & `tmp/python-invest-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-invest-0.1.1a0.tar", max compression
+gzip compressed data, was "python-invest-0.2.1a0.tar", max compression
```

## Comparing `python-invest-0.1.1a0.tar` & `python-invest-0.2.1a0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     1090 2023-03-03 03:31:35.824810 python-invest-0.1.1a0/LICENSE
--rw-r--r--   0        0        0      790 2023-03-06 18:07:50.791201 python-invest-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       28 2023-03-03 04:51:04.355492 python-invest-0.1.1a0/python_invest/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 04:51:04.355492 python-invest-0.1.1a0/python_invest/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 04:51:04.356515 python-invest-0.1.1a0/python_invest/cli/cli.py
--rw-r--r--   0        0        0      391 2023-03-06 16:50:20.727600 python-invest-0.1.1a0/python_invest/const.py
--rw-r--r--   0        0        0       50 2023-03-03 04:51:04.358029 python-invest-0.1.1a0/python_invest/invest/__init__.py
--rw-r--r--   0        0        0     4925 2023-03-06 16:50:20.732257 python-invest-0.1.1a0/python_invest/invest/crypto.py
--rw-r--r--   0        0        0      545 2023-03-06 16:50:20.737468 python-invest-0.1.1a0/python_invest/invest/firebase.py
--rw-r--r--   0        0        0        0 2023-03-06 14:38:55.460328 python-invest-0.1.1a0/python_invest/invest/founds.py
--rw-r--r--   0        0        0     1484 2023-03-06 14:38:55.461333 python-invest-0.1.1a0/python_invest/invest/main.py
--rw-r--r--   0        0        0        0 2023-03-03 04:51:04.360226 python-invest-0.1.1a0/python_invest/invest/stocks.py
--rw-r--r--   0        0        0     1139 2023-03-04 16:26:27.588409 python-invest-0.1.1a0/python_invest/invest/utils.py
--rw-r--r--   0        0        0     1390 2023-03-03 04:51:04.361479 python-invest-0.1.1a0/python_invest/invest/validators.py
--rw-r--r--   0        0        0     2910 2023-03-03 16:54:59.467728 python-invest-0.1.1a0/README.md
--rw-r--r--   0        0        0     3656 1970-01-01 00:00:00.000000 python-invest-0.1.1a0/setup.py
--rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 python-invest-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-03-03 03:31:35.824810 python-invest-0.2.1a0/LICENSE
+-rw-r--r--   0        0        0      964 2023-04-10 20:35:44.268073 python-invest-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-03-03 04:51:04.355492 python-invest-0.2.1a0/python_invest/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-10 20:34:22.675043 python-invest-0.2.1a0/python_invest/cli/__init__.py
+-rw-r--r--   0        0        0     1337 2023-04-10 20:34:22.676051 python-invest-0.2.1a0/python_invest/cli/cli.py
+-rw-r--r--   0        0        0       73 2023-04-10 20:34:22.677059 python-invest-0.2.1a0/python_invest/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2436 2023-04-10 20:34:22.677059 python-invest-0.2.1a0/python_invest/cli/commands/config.py
+-rw-r--r--   0        0        0     4200 2023-04-10 20:34:22.678065 python-invest-0.2.1a0/python_invest/cli/commands/crypto.py
+-rw-r--r--   0        0        0      696 2023-04-10 20:34:22.679066 python-invest-0.2.1a0/python_invest/cli/commands/pandas_to_rich.py
+-rw-r--r--   0        0        0      236 2023-04-10 20:34:22.679066 python-invest-0.2.1a0/python_invest/cli/commands/utils.py
+-rw-r--r--   0        0        0      675 2023-04-10 20:34:22.680074 python-invest-0.2.1a0/python_invest/const.py
+-rw-r--r--   0        0        0       50 2023-03-03 04:51:04.358029 python-invest-0.2.1a0/python_invest/invest/__init__.py
+-rw-r--r--   0        0        0     4925 2023-04-10 20:34:22.681170 python-invest-0.2.1a0/python_invest/invest/crypto.py
+-rw-r--r--   0        0        0      545 2023-03-06 16:50:20.737468 python-invest-0.2.1a0/python_invest/invest/firebase.py
+-rw-r--r--   0        0        0        0 2023-03-06 14:38:55.460328 python-invest-0.2.1a0/python_invest/invest/founds.py
+-rw-r--r--   0        0        0     1484 2023-03-06 14:38:55.461333 python-invest-0.2.1a0/python_invest/invest/main.py
+-rw-r--r--   0        0        0        0 2023-03-03 04:51:04.360226 python-invest-0.2.1a0/python_invest/invest/stocks.py
+-rw-r--r--   0        0        0     1329 2023-04-10 20:34:22.681170 python-invest-0.2.1a0/python_invest/invest/utils.py
+-rw-r--r--   0        0        0     1824 2023-04-10 20:34:46.596327 python-invest-0.2.1a0/python_invest/invest/validators.py
+-rw-r--r--   0        0        0     4145 2023-04-10 20:34:22.661337 python-invest-0.2.1a0/README.md
+-rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 python-invest-0.2.1a0/setup.py
+-rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 python-invest-0.2.1a0/PKG-INFO
```

### Comparing `python-invest-0.1.1a0/LICENSE` & `python-invest-0.2.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-invest-0.1.1a0/pyproject.toml` & `python-invest-0.2.1a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 [tool.poetry]
 name = "python-invest"
-version = "0.1.1-alpha"
+version = "0.2.1-alpha"
 description = "Package to financial data extraction with Python."
 authors = ["Claudio Lima <clcostaf@hotmail.com>"]
 readme = "README.md"
+packages = [{include = "python_invest"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^1.5.3"
 httpx = "^0.23.3"
+typer = "^0.7.0"
+rich = "^13.3.3"
 
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.1.0"
+mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.11.0"
 pytest = "^7.2.1"
-mkdocs = "^1.4.2"
-mkdocs-material = "^9.1.0"
 pre-commit = "^3.1.1"
 pytest-cov = "^4.0.0"
 isort = "^5.12.0"
 blue = "^0.9.1"
-mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Documentation" = "https://pyinvest.readthedocs.io/en/latest/"
 "GitHub" = "https://github.com/clcosta/python-invest"
+
+[tool.poetry.scripts]
+pinv = "python_invest.cli:cli"
```

### Comparing `python-invest-0.1.1a0/python_invest/invest/crypto.py` & `python-invest-0.2.1a0/python_invest/invest/crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,30 @@
 
     def __init__(self, invest_instance):
         self.__invest_intance = invest_instance
 
     def get_historical_data(
         self,
         symbol: str = None,
-        from_date: str | date = '01/01/2023',
-        to_date: str | date = '01/02/2023',
+        from_date: str | date = '2023-01-01',
+        to_date: str | date = '2023-02-01',
         name: str = None,
         time_frame: str = 'Daily',
         as_dict: bool = False,
     ) -> dict | pd.DataFrame:
         """
         Get historical data from crypto, the return could be raw in dict or filtered DataFrame.
 
         Note:
             The `symbol` or `name` is required, if not provided, the method will return an error.
 
         Args:
             symbol (str, optional): The symbol of the crypto. Defaults to None.
-            from_date (str | date, optional): The start date of the historical data. Defaults to '01/01/2023'.
-            to_date (str | date, optional): The end date of the historical data. Defaults to '01/02/2023'.
+            from_date (str | date, optional): The start date of the historical data. Defaults to '2023-01-01'.
+            to_date (str | date, optional): The end date of the historical data. Defaults to '2023-02-01'.
             name (str, optional): The name of the crypto. Defaults to None.
             time_frame (str, optional): The time frame of the historical data. Defaults to 'Daily'.
             as_dict (bool, optional): Whether to return the data as dict. Defaults to False.
 
         Returns:
             (dict | pd.DataFrame): The historical data.
         """
@@ -117,15 +117,15 @@
                 'change_precent': 'Change',
             },
             inplace=True,
             axis=1,
         )
         df['Date'] = pd.to_datetime(
             pd.to_datetime(raw_df.rowDateTimestamp)
-        ).dt.strftime('%m/%d/%Y')
+        ).dt.strftime('%Y-%m-%d')
         return df
 
     def get_list(self) -> list:
         """
         Get the list of cryptos.
 
         Returns:
```

### Comparing `python-invest-0.1.1a0/python_invest/invest/firebase.py` & `python-invest-0.2.1a0/python_invest/invest/firebase.py`

 * *Files identical despite different names*

### Comparing `python-invest-0.1.1a0/python_invest/invest/main.py` & `python-invest-0.2.1a0/python_invest/invest/main.py`

 * *Files identical despite different names*

### Comparing `python-invest-0.1.1a0/python_invest/invest/utils.py` & `python-invest-0.2.1a0/python_invest/invest/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 __all__ = ['convert_dates_to_str', 'dict_to_url_params']
 import re
-from datetime import date
+from datetime import date, datetime
 from urllib import parse
 
+from .validators import validate_date_in_out
+
 
 def convert_dates_to_str(
     from_date: str | date, to_date: str | date
 ) -> tuple[str, str]:
     """
     Convert date objects to string and validate string date format.
-    Return tuple of string dates in format d/m/Y.
+    Return tuple of string dates in format Y-m-d.
     """
-    pattern = r'([0-9]{2}\/[0-9]{2}\/[0-9]{4})'
+    pattern = r'([0-9]{4}-[0-9]{2}-[0-9]{2})'
     try:
-        from_date = from_date.strftime('%m/%d/%Y')
+        from_date = from_date.strftime('%Y-%m-%d')
     except AttributeError:
         if not re.fullmatch(pattern, from_date):
             raise ValueError(
-                f'The date format is invalid, please use d/m/Y format in from_date argument.'
+                f'The date format is invalid, please use Y-m-d format in from_date argument.'
             )
     try:
-        to_date = to_date.strftime('%m/%d/%Y')
+        to_date = to_date.strftime('%Y-%m-%d')
     except AttributeError:
         if not re.fullmatch(pattern, to_date):
             raise ValueError(
-                f'The date format is invalid, please use d/m/Y format in to_date argument.'
+                f'The date format is invalid, please use Y-m-d format in to_date argument.'
             )
+    validate_date_in_out(
+        datetime.strptime(from_date, '%Y-%m-%d'),
+        datetime.strptime(to_date, '%Y-%m-%d'),
+    )
     return from_date, to_date
 
 
 def dict_to_url_params(data: dict) -> str:
     """
     Convert dictionary to url parameters.
     """
```

### Comparing `python-invest-0.1.1a0/python_invest/invest/validators.py` & `python-invest-0.2.1a0/python_invest/invest/validators.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from datetime import date
+from datetime import date, datetime
+
 from python_invest.const import PRODUCT_LIST, TIME_FRAME_LIST
 
 
 def validate_args(func):
     """
     Validate the arguments passed in a function used inside a Invest class.
     The arguments the wrapper expected to validate:
@@ -20,16 +21,29 @@
             )
         if time_frame.lower() not in TIME_FRAME_LIST:
             raise ValueError(
                 f'Time frame "{time_frame}" not in accepted. Please select a based on {" or ".join(TIME_FRAME_LIST)}.'
             )
         if not isinstance(from_date, (str, date)):
             raise TypeError(
-                f'Argument from_date must be a string containning a date in format m/d/Y or date. Got a "{type(from_date)}"'
+                f'Argument from_date must be a string containning a date in format Y-m-d or date. Got a "{type(from_date)}"'
             )
         if not isinstance(to_date, (str, date)):
             raise TypeError(
-                f'Argument to_date must be a string containning a date in format m/d/Y or date. Got a "{type(from_date)}"'
+                f'Argument to_date must be a string containning a date in format Y-m-d or date. Got a "{type(from_date)}"'
             )
         return func(*args, **kwargs)
 
     return wrapper
+
+
+def validate_date_in_out(from_date: datetime, to_date: datetime) -> None:
+    """
+    Validate if the date in (from_date) and date out (to_date) is valid.
+
+    Raises:
+        ValueError: If the date in (from_date) is greater then date out (to_date).
+    """
+    if from_date > to_date:
+        raise ValueError(
+            f'The start date "{from_date}" is greater then final date "{to_date}".'
+        )
```

