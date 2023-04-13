# Comparing `tmp/dapla_statbank_client-1.0.0.tar.gz` & `tmp/dapla_statbank_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_statbank_client-1.0.0.tar", max compression
+gzip compressed data, was "dapla_statbank_client-1.0.2.tar", max compression
```

## Comparing `dapla_statbank_client-1.0.0.tar` & `dapla_statbank_client-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-02-16 13:36:37.155682 dapla_statbank_client-1.0.0/LICENSE
--rw-r--r--   0        0        0     8334 2023-02-16 13:36:53.195601 dapla_statbank_client-1.0.0/README.md
--rw-r--r--   0        0        0     1119 2023-02-16 13:36:53.195601 dapla_statbank_client-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      190 2023-02-16 13:36:53.195601 dapla_statbank_client-1.0.0/statbank/__init__.py
--rw-r--r--   0        0        0     5128 2023-02-16 13:36:37.155682 dapla_statbank_client-1.0.0/statbank/apidata.py
--rw-r--r--   0        0        0     3668 2023-02-16 13:36:37.155682 dapla_statbank_client-1.0.0/statbank/auth.py
--rw-r--r--   0        0        0    14068 2023-02-16 13:36:53.199601 dapla_statbank_client-1.0.0/statbank/client.py
--rw-r--r--   0        0        0    12909 2023-02-16 13:36:37.155682 dapla_statbank_client-1.0.0/statbank/transfer.py
--rw-r--r--   0        0        0    11862 2023-02-16 13:36:53.199601 dapla_statbank_client-1.0.0/statbank/uttrekk.py
--rw-r--r--   0        0        0    14187 2023-02-16 13:36:53.199601 dapla_statbank_client-1.0.0/statbank/uttrekk_validations.py
--rw-r--r--   0        0        0     9577 1970-01-01 00:00:00.000000 dapla_statbank_client-1.0.0/setup.py
--rw-r--r--   0        0        0     9033 1970-01-01 00:00:00.000000 dapla_statbank_client-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-13 09:20:19.222743 dapla_statbank_client-1.0.2/LICENSE
+-rw-r--r--   0        0        0     8938 2023-04-13 09:20:37.138836 dapla_statbank_client-1.0.2/README.md
+-rw-r--r--   0        0        0     1119 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/__init__.py
+-rw-r--r--   0        0        0     5651 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/apidata.py
+-rw-r--r--   0        0        0     3668 2023-04-13 09:20:19.226743 dapla_statbank_client-1.0.2/statbank/auth.py
+-rw-r--r--   0        0        0    17539 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/client.py
+-rw-r--r--   0        0        0    13609 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/transfer.py
+-rw-r--r--   0        0        0    13611 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/uttrekk.py
+-rw-r--r--   0        0        0    14153 2023-04-13 09:20:37.142836 dapla_statbank_client-1.0.2/statbank/uttrekk_validations.py
+-rw-r--r--   0        0        0     9637 1970-01-01 00:00:00.000000 dapla_statbank_client-1.0.2/PKG-INFO
```

### Comparing `dapla_statbank_client-1.0.0/LICENSE` & `dapla_statbank_client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.0/README.md` & `dapla_statbank_client-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fill out password
 # Default publishing-date is TOMORROW
 print(stat_client)
 # Printing will show you all the default settings on the client.
 # You can change for example date by specifying it: StatbankClient(loaduser = "LASTEBRUKER", date="2023-02-16")
 ```
 
-Be aware that from the **dapla staging environment** you will be sending to statbank-TEMP-database, your changes will not be published. But if you are in the main dapla-jupyterlab (prod), you WILL publish to statbanken, in the PROD database. So pay extra attention to the **publishing-date** when in dapla-main-prod-jupyterlab.
+Be aware that from the **dapla-staging environment** you will be sending to statbank-TEST-database, your changes will not be published. For this you need the "test-password", which is for the same user (lastebruker), but different from the ordinary password (lastepassord). If you are missing the test-password, have the statbank-team send it to you for you loaduser. If you are in the main dapla-jupyterlab (prod), you **WILL** publish to statbanken, in the PROD database. So pay extra attention to the **publishing-date** when in dapla-main-prod-jupyterlab. And be aware of which password you are entering, based on your environment. [To see data actually published to the test-database, you can use this link if you work at SSB.](https://i.test.ssb.no/pxwebi/pxweb/no/test_24v_intern/)
 
 
 ### Usage Transferring
 
 ```python
 stat_client.transfer({"deltabellfilnavn.dat" : df_06399}, "06339")
 ```
@@ -126,14 +126,15 @@
 filbesk_06339_new = stat_client.read_description_json("path.json")
 ```
 Some deeper data-structures, like the dataframes in the transfer will not be serialized and stored with the transfer-object in its json.
 
 ---
 
 ### Version history
+- 1.0.2 Doc-string style cleanup, a check on username and password on client init, changes to time and display of time, demo notebooks cleaned
 - 1.0.0 Finished going through initial issues, less complaining from verify on floats
 - 0.0.11 Statbank people wanted a user-agent-requesst-header to differentiate test from prod
 - 0.0.9 After further user-testing and requests
 - 0.0.5 Still some parameter issues
 - 0.0.4 More test coverage, some bugs fixed in rounding checks and parameter-passing
 - 0.0.3 Removed batches, stripping uttrekk from transfer, rounding function on uttrekk, data required in as a dict of dataframes, with "deltabell-navn". Tableid now works to transfer to instead of only "hovedtabellnavn"
 - 0.0.2 Starting alpha, fine-tuning release to Pypi on github-release
```

### Comparing `dapla_statbank_client-1.0.0/pyproject.toml` & `dapla_statbank_client-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-statbank-client"
-version = "1.0.0"
+version = "1.0.2"
 description = "Handles data transfer Statbank <-> Dapla for Statistics Norway"
 authors = ["Statistics Norway", "Carl F. Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "statbank"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dapla_statbank_client-1.0.0/statbank/apidata.py` & `dapla_statbank_client-1.0.2/statbank/apidata.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,25 @@
 
 def apidata(
     id_or_url: str = "",
     payload: dict = {"query": [], "response": {"format": "json-stat2"}},  # noqa: B006
     include_id: bool = False,
 ) -> pd.DataFrame:
     """
-    Parameter1 - id_or_url: The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
-    Parameter2: Payload, the query to include with the request.
-    Parameter3: If you want to include "codes" in the dataframe, set this to True
-    Returns: a pandas dataframe with the table
+    Get the contents of a published statbank-table as a pandas Dataframe, specifying a query to limit the return.
+
+    Parameters
+    -------
+    id_or_url: The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+    payload: a dict of the query to include with the request, can be copied from the statbank-webpage.
+    include_id: If you want to include "codes" in the dataframe, set this to True
+
+    Returns
+    -------
+    A pandas dataframe with the table-content
     """
     if len(id_or_url) == 5 and id_or_url.isdigit():
         url = f"https://data.ssb.no/api/v0/no/table/{id_or_url}/"
     else:
         test_url = urllib.parse.urlparse(id_or_url)
         if not all([test_url.scheme, test_url.netloc]):
             raise ValueError(
@@ -67,24 +74,38 @@
         )
     else:
         raise r.ConnectionError(f"Status code {resultat.status_code}: {resultat.text}")
 
 
 def apidata_all(id_or_url: str = "", include_id: bool = False) -> pd.DataFrame:
     """
-    Parameter1 - id_or_url: The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
-    Returns: a pandas dataframe with the table
+    Get ALL the contents of a published statbank-table as a pandas Dataframe.
+
+    Parameters
+    -------
+    id_or_url: The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+    include_id: If you want to include "codes" in the dataframe, set this to True
+
+    Returns
+    -------
+    A pandas dataframe with the table-content
     """
     return apidata(id_or_url, apidata_query_all(id_or_url), include_id=include_id)
 
 
 def apidata_query_all(id_or_url: str = "") -> dict:
-    """
-    Parameter1 - id_or_url: The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
-    Returns: A dict of the prepared query based on all the codes in the table.
+    """Builds a query for ALL THE DATA in a table based on a request for metadata on the table
+
+    Parameters
+    -------
+    id_or_url: The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+
+    Returns
+    -------
+    A dict of the prepared query based on all the codes in the table.
     """
     if len(id_or_url) == 5 and id_or_url.isdigit():
         url = f"https://data.ssb.no/api/v0/no/table/{id_or_url}/"
     else:
         test_url = urllib.parse.urlparse(id_or_url)
         if not all([test_url.scheme, test_url.netloc]):
             raise ValueError(
@@ -111,19 +132,23 @@
             f"Can't get query metadata in first of two requests. Status code {res.status_code}: {res.text}"
         )
 
 
 # Credit: https://github.com/sehyoun/SSB_API_helper/blob/master/src/ssb_api_helper.py
 def apidata_rotate(df, ind="year", val="value"):
     """Rotate the dataframe so that years are used as the index
-    Args:
-        df (pandas.dataframe): dataframe (from <get_from_ssb> function
-        ind (str): string of column name denoting time
-        val (str): string of column name denoting values
-    Returns:
-        dataframe: pivoted dataframe
+
+    Parameters
+    -------
+    df (pandas.dataframe): dataframe (from <get_from_ssb> function
+    ind (str): string of column name denoting time
+    val (str): string of column name denoting values
+
+    Returns
+    -------
+    dataframe: pivoted dataframe
     """
     return df.pivot_table(
         index=ind,
         values=val,
         columns=[i for i in df.columns if i != ind and i != val],
     )
```

### Comparing `dapla_statbank_client-1.0.0/statbank/auth.py` & `dapla_statbank_client-1.0.2/statbank/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.0.0/statbank/client.py` & `dapla_statbank_client-1.0.2/statbank/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -118,30 +118,36 @@
         loaduser: str = "",
         date: datetime.datetime = TOMORROW,
         shortuser: str = "",
         cc: str = "",
         bcc: str = "",
         overwrite: bool = True,
         approve: int = 2,  # Changing back to 2, after wish from Rakel Gading
+        check_username_password: bool = True,
     ):
         self.loaduser = loaduser
-        if isinstance(date, str):
-            self.date = datetime.datetime.strptime(date, "%Y-%m-%d")
-        else:
-            self.date = date
-        self._validate_date()
         self.shortuser = shortuser
         self.cc = cc
         self.bcc = bcc
         self.overwrite = overwrite
         self.approve = approve
         self._validate_params_init()
         self.__headers = self._build_headers()
         self.log = []
-        print(f"Publishing date set to {self.date}")
+        if isinstance(date, str):
+            self.date = datetime.datetime.strptime(date, "%Y-%m-%d")
+        else:
+            self.date = date
+        self.date = self.date.replace(hour=8, minute=0, second=0, microsecond=0)
+        self._validate_date()
+        if check_username_password:
+            self.get_description(
+                "05300", printing=False
+            )  # Random tableid to double check username&password early
+        print(f"Publishing date set to {self.date.isoformat('T', 'seconds')}")
 
     # Representation
     def __str__(self):
         return f"""StatbankClient for user {self.loaduser}
         Publishing at {self.date}
         Shortuser {self.shortuser}
         Sending mail to {self.cc}
@@ -155,63 +161,95 @@
         )
 
     def __repr__(self):
         return f'StatbankClient(loaduser = "{self.loaduser}")'
 
     # Publishing date handeling
     def date_picker(self) -> None:
-
         """Displays a datapicker-widget.
         Assign it to a variable, that you after editing the date,
         pass into set_publish_date()
         date = client.datepicker()
         # Edit date
         client.set_publish_date(date)
+
+        Returns
+        -------
+        A datepicker widget from ipywidgets, with its date set to what the client currently holds.
         """
         datepicker = widgets.DatePicker(
             description="Publish-date", disabled=False, value=self.date
         )
         display(datepicker)
         return datepicker
 
     def set_publish_date(self, date: datetime.datetime) -> None:
         """Set the publishing date on the client.
-        If sending a string, use the format 2000-12-31
+        Takes the widget from date_picker assigned to a variable, which is probably the intended use.
+        If sending a string, use the format 2000-12-31, you can also send in a datetime.
+        Hours, minutes and seconds are replaced with statbankens publish time: 08:00:00
+
+        Parameters
+        -------
+        date: datetime, date-picker widget, or a date-string formatted as 2000-12-31
         """
         if isinstance(date, widgets.widget_date.DatePicker):
             self.date = date.value
         elif isinstance(date, str):
             self.date = datetime.datetime.strptime(date, "%Y-%m-%d")
         else:
             self.date = date
+        self.date = self.date.replace(hour=8, minute=0, second=0, microsecond=0)
         self._validate_date()
         print("Publishing date set to:", self.date)
         self.log.append(
-            f'Date set to {self.date} at {datetime.datetime.now().strftime("%Y-%m-%d %H:%M")}'
+            f"Date set to {self.date.isoformat('T', 'seconds')} at {datetime.datetime.now().isoformat('T', 'seconds')}"
         )
 
     # Descriptions
-    def get_description(self, tableid: str = "00000") -> StatbankUttrekksBeskrivelse:
+    def get_description(
+        self, tableid: str = "00000", printing=True
+    ) -> StatbankUttrekksBeskrivelse:
         """Get the "uttrekksbeskrivelse" for the tableid, which describes metadata
         about shape of data to be transferred, and metadata about the table
         itself in Statbankens system, like ID, name and content of codelists.
+
+        Parameters
+        -------
+        tableid: str, The tableid of the "hovedtabell" in statbanken, a 5 digit string.
+
+        Returns
+        -------
+        An instance of the class StatbankUttrekksBeskrivelse, which is comparable to the old "filbeskrivelse".
         """
         self._validate_params_action(tableid)
         self.log.append(
-            f'Getting description for tableid {tableid} at {datetime.datetime.now().strftime("%Y-%m-%d %H:%M")}'
+            f"Getting description for tableid {tableid} at {datetime.datetime.now().isoformat('T', 'seconds')}"
         )
         return StatbankUttrekksBeskrivelse(
-            tableid=tableid, loaduser=self.loaduser, headers=self.__headers
+            tableid=tableid,
+            loaduser=self.loaduser,
+            headers=self.__headers,
+            printing=printing,
         )
 
     @staticmethod
     def read_description_json(json_path_or_str: str) -> StatbankUttrekksBeskrivelse:
-        """Checks if provided string exists on disk, if it does, tries to load it as json.
+        """Re-initializes a StatbankUttrekksBeskrivelse from a stored json file/string.
+        Checks if provided string exists on disk, if it does, tries to load it as json.
         Otherwise expects you to provide a json-string that works for json.loads.
         Inserts first layer in json as attributes under a blank StatbankUttrekksBeskrivelse-object.
+
+        Parameters
+        -------
+        json_path_or_str: str or path, Either a path on local storage, or a loaded json-string
+
+        Returns
+        -------
+        An instance of the class StatbankUttrekksBeskrivelse, which is comparable to the old "filbeskrivelse".
         """
         if os.path.exists(json_path_or_str):
             with open(json_path_or_str) as json_file:
                 json_path_or_str = json_file.read()
         new = StatbankUttrekksBeskrivelse.__new__(StatbankUttrekksBeskrivelse)
         for k, v in json.loads(json_path_or_str).items():
             setattr(new, k, v)
@@ -224,35 +262,56 @@
         tableid: str = "00000",
         raise_errors: bool = False,
         printing: bool = True,
     ) -> dict:
         """Gets an "uttrekksbeskrivelse" and validates the data against this.
         All validation happens locally, so dont be afraid of any data
         being sent to statbanken using this method.
-        Logic is built in Python, and can probably be expanded upon."""
+
+        Parameters
+        -------
+        dfs: dict of dataframes, The data to validate in a dictionary of deltabell-names as keys and pandas-dataframes as values.
+        tableid: str, The tableid of the "hovedtabell" in statbanken, a 5 digit string.
+        raise_errors: bool, True/False based on if you want the method to raise its own errors or not.
+        printing: bool, True/False based on if you want a verbose printing of everything the validation checks.
+
+        Returns
+        -------
+        A dictionary of the errors the validation wants to raise.
+        """
         self._validate_params_action(tableid)
         validator = StatbankUttrekksBeskrivelse(
             tableid=tableid,
             loaduser=self.loaduser,
             raise_errors=raise_errors,
             headers=self.__headers,
         )
         validation_errors = validator.validate(dfs, printing=printing)
         self.log.append(
-            f'Validated data for tableid {tableid} at {datetime.datetime.now().strftime("%Y-%m-%d %H:%M")}'
+            f"Validated data for tableid {tableid} at {datetime.datetime.now().isoformat('T', 'seconds')}"
         )
         return validation_errors
 
     # Transfer
-    def transfer(self, dfs: pd.DataFrame, tableid: str = "00000") -> StatbankTransfer:
+    def transfer(self, dfs: dict, tableid: str = "00000") -> StatbankTransfer:
         """Transfers your data to Statbanken.
-        Make sure you've set the publish-date correctly before sending."""
+        Make sure you've set the publish-date correctly before sending.
+
+        Parameters
+        -------
+        dfs: dict of dataframes, The data to validate in a dictionary of deltabell-names as keys and pandas-dataframes as values.
+        tableid: str, The tableid of the "hovedtabell" in statbanken, a 5 digit string.
+
+        Returns
+        -------
+        An instance of the class StatbankTransfer, which details the content of a successful transfer.
+        """
         self._validate_params_action(tableid)
         self.log.append(
-            f'Transferring tableid {tableid} at {datetime.datetime.now().strftime("%Y-%m-%d %H:%M")}'
+            f"Transferring tableid {tableid} at {datetime.datetime.now().isoformat('T', 'seconds')}"
         )
         return StatbankTransfer(
             dfs,
             tableid=tableid,
             loaduser=self.loaduser,
             headers=self.__headers,
             shortuser=self.shortuser,
@@ -264,14 +323,22 @@
         )
 
     @staticmethod
     def read_transfer_json(json_path_or_str: str) -> StatbankTransfer:
         """Checks if provided string exists on disk, if it does, tries to load it as json.
         Otherwise expects you to provide a json-string that works for json.loads.
         Inserts first layer in json as attributes under a blank StatbankTransfer-object.
+
+        Parameters
+        -------
+        json_path_or_str: str or path, Either a path on local storage, or a loaded json-string
+
+        Returns
+        -------
+        An instance of the class StatbankTransfer, missing the data transferred and some other bits probably.
         """
         if os.path.exists(json_path_or_str):
             with open(json_path_or_str) as json_file:
                 json_path_or_str = json_file.read()
         new = StatbankTransfer.__new__(StatbankTransfer)
         for k, v in json.loads(json_path_or_str).items():
             setattr(new, k, v)
@@ -281,68 +348,87 @@
     @staticmethod
     def apidata(
         id_or_url: str = "",
         payload: dict = None,
         include_id: bool = False,
     ) -> pd.DataFrame:
         """
-        Parameter1 - id_or_url: The id of the STATBANK-table to
-        get the total query for, or supply the total url, if the table is "internal".
-        Parameter2: Payload, the query to include with the request.
-        Parameter3: If you want to include "codes" in the dataframe, set this to True
-        Returns: a pandas dataframe with the table
+        Get the contents of a published statbank-table as a pandas Dataframe, specifying a query to limit the return.
+
+        Parameters
+        -------
+        id_or_url: str, The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+        payload: dict, a dict of the query to include with the request, can be copied from the statbank-webpage.
+        include_id: bool, If you want to include "codes" in the dataframe, set this to True
+
+        Returns
+        -------
+        A pandas dataframe with the table-content
         """
         if not payload:
             payload = {"query": [], "response": {"format": "json-stat2"}}
         return apidata(id_or_url=id_or_url, payload=payload, include_id=include_id)
 
     @staticmethod
     def apidata_all(id_or_url: str = "", include_id: bool = False) -> pd.DataFrame:
-
         """
-        Parameter1 - id_or_url: The id of the STATBANK-table to
-        get the total query for, or supply the total url, if the table is "internal".
-        Returns: a pandas dataframe with the table
+        Get ALL the contents of a published statbank-table as a pandas Dataframe.
+
+        Parameters
+        -------
+        id_or_url: str, The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+        include_id: bool, If you want to include "codes" in the dataframe, set this to True
+
+        Returns
+        -------
+        A pandas dataframe with the table-content
         """
         return apidata_all(id_or_url=id_or_url, include_id=include_id)
 
     @staticmethod
     def apidata_rotate(df, ind="year", val="value"):
         """Rotate the dataframe so that time is used as the index
-        Args:
-            df (pandas.dataframe): dataframe (from <get_from_ssb> function
-            ind (str): string of column name denoting time
-            val (str): string of column name denoting values
-        Returns:
-            dataframe: pivoted dataframe
+
+        Parameters
+        -------
+        df: pandas.dataframe, dataframe (from <get_from_ssb> function
+        ind: str, string of column name denoting time
+        val: str: string of column name denoting values
+
+        Returns
+        -------
+        dataframe: pivoted dataframe
         """
         return apidata_rotate(df, ind, val)
 
     def _validate_date(self) -> None:
+        """Validates dates provided to the client"""
         if not (
             isinstance(self.date, datetime.datetime)
             or isinstance(self.date, datetime.date)
         ):
             raise TypeError("Date must be a datetime.datetime or datetime.date")
         # Date should not be on a weekend
         if self.date.weekday() in [5, 6]:
             print(
                 "Warning, you are publishing during a weekend, this is not common practice."
             )
 
     # Class meta-validation
     def _validate_params_action(self, tableid: str) -> None:
+        """Validates tableid mainly, more actively than other params"""
         if not isinstance(tableid, str):
             raise TypeError(f"{tableid} is not a string.")
         if (
             tableid.isdigit() and not len(tableid) == 5
         ):  # Allow for "hovednavn" in addition to tableid
             raise ValueError(f"{tableid} is numeric, but not 5 characters long.")
 
     def _validate_params_init(self) -> None:
+        """Validates many of the parameters sent in on client-initialization."""
         if not self.loaduser or not isinstance(self.loaduser, str):
             raise TypeError('Please pass in "loaduser" as a string.')
         if not self.shortuser:
             self.shortuser = os.environ["JUPYTERHUB_USER"].split("@")[0]
         if not self.cc:
             self.cc = self.shortuser
         if not self.bcc:
```

### Comparing `dapla_statbank_client-1.0.0/statbank/transfer.py` & `dapla_statbank_client-1.0.2/statbank/transfer.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     """
     Class for talking with the "transfer-API",
     which actually recieves the data from the user and sends it to Statbank.
     ...
 
     Attributes
     ----------
-    data : pd.DataFrame or list of pd.DataFrames
+    data : dict of pd.DataFrames as values, name of "deltabell.dat" as keys.
         Number of DataFrames needs to match the number of "deltabeller" in
         the uttakksbeskrivelse.
-        Data-shape can be validated before transfer with the
+        Dict-shape can be retrieved and validated before transfer with the
         Uttakksbeskrivelses-class.
     loaduser : str
         Username for Statbanken, not the same as "shortuser" or
         "common personal username" in other SSB-systems
     tableid: str
         The numeric id of the table, matching the one found on the website.
         Should be a 5-length numeric-string. Alternativley it should be
@@ -133,14 +133,15 @@
         else:
             self.cc = self.shortuser
         if bcc:
             self.bcc = bcc
         else:
             self.bcc = self.cc
 
+        # At this point we want date to be a string?
         if isinstance(date, str):
             self.date = date
         else:
             self.date = date.strftime("%Y-%m-%d")
 
         self.overwrite = overwrite
         self.approve = approve
@@ -155,16 +156,22 @@
         if not self.delay:
             if headers:
                 self.transfer(headers)
             else:
                 self.transfer()
 
     def transfer(self, headers: dict = {}):  # noqa: B006
-        """The headers-parameter is for a future implemention
-        of a possible BatchTransfer, dont use it please."""
+        """Transfers your data to Statbanken.
+        Make sure you've set the publish-date correctly before sending.
+        Will only work if the transfer has not already been sent, meaning it was "delayed".
+
+        Parameters
+        -------
+        headers: mostly for internal use by the package. Needs to be a finished compiled headers for a request including Authorization.
+        """
         # In case transfer has already happened, dont transfer again
         if hasattr(self, "oppdragsnummer"):
             raise ValueError(
                 f"""Already transferred?
                 {self.urls['gui'] +self.oppdragsnummer}
                 Remake the StatbankTransfer-object if intentional."""
             )
@@ -206,16 +213,26 @@
         )
 
     @property
     def delay(self):
         return self.__delay
 
     def to_json(self, path: str = "") -> dict:
-        """If path is provided, tries to write to it,
+        """Store a copy of the current state of the transfer-object as a json.
+        If path is provided, tries to write to it,
         otherwise will return a json-string for you to handle like you wish.
+
+        Parameters
+        -------
+        path: if provided, will try to write a json to a local path
+
+        Returns
+        -------
+        If path is provided, tries to write a json there and returns nothing.
+        If path is not provided, returns the json-string for you to handle as you wish.
         """
         print(
             "Warning, some nested, deeper data-structures"
             + " like dataframes and other class-objects will not be serialized"
         )
         json_content = json.dumps(self.__dict__, default=lambda o: "<not serializable>")
         # If path provided write to it, otherwise return the string-content
@@ -295,19 +312,21 @@
             (date[4] + date[7]) == "--"
         ):
             return True
         return False
 
     def _build_params(self) -> dict:
         if isinstance(self.date, dt):
-            self.date = self.date.strftime("%Y-%m-%d")
+            date = self.date.strftime("%Y-%m-%d")
+        else:
+            date = self.date
         return {
             "initialier": self.shortuser,
             "hovedtabell": self.tableid,
-            "publiseringsdato": self.date,
+            "publiseringsdato": date,
             "fagansvarlig1": self.cc,
             "fagansvarlig2": self.bcc,
             "auto_overskriv_data": str(int(self.overwrite)),
             "auto_godkjenn_data": self.approve,
         }
 
     def _make_transfer_request(
@@ -338,21 +357,20 @@
             )
             publish_hour = int(response_msg.split("Publiseringstid '")[1].split(":")[0])
             publish_minute = int(
                 response_msg.split("Publiseringstid '")[1].split(":")[1].split("'")[0]
             )
             publish_time = publish_hour * 3600 + publish_minute * 60
             publish = publish_date + td(0, publish_time)
-            publish = publish.strftime("%Y-%m-%d %H:%M")
+            publish = publish.isoformat("T", "seconds")
             print(f"Publisering satt til: {publish}")
             print(
                 "Følg med på lasteloggen (tar noen minutter): "
                 + f"{self.urls['gui'] + self.oppdragsnummer}"
             )
-            print(f"Og evt APIen?: {self.urls['api'] + self.oppdragsnummer}")
             self.resp_json = resp_json
         else:
             print(
                 "Take a closer look at StatbankTransfer.response.text"
                 + "for more info about connection issues."
             )
             raise ConnectionError(resp_json)
```

### Comparing `dapla_statbank_client-1.0.0/statbank/uttrekk.py` & `dapla_statbank_client-1.0.2/statbank/uttrekk.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests as r
 from requests.exceptions import ConnectionError
 
 from .auth import StatbankAuth
 from .uttrekk_validations import StatbankUttrekkValidators
 
 
-class StatbankUttrekksBeskrivelse(StatbankAuth):
+class StatbankUttrekksBeskrivelse(StatbankAuth, StatbankUttrekkValidators):
     """
     Class for talking with the "uttrekksbeskrivelses-API",
     which describes metadata about shape of data to be transferred.
     And metadata about the table itself in Statbankens system,
     like ID, name of codelists etc.
     ...
 
@@ -67,15 +67,17 @@
     _split_attributes():
         After a successful response,
         split recieved data into attributes for easier access
     __init__():
 
     """
 
-    def __init__(self, tableid, loaduser, raise_errors=False, headers=None):
+    def __init__(
+        self, tableid, loaduser, raise_errors=False, headers=None, printing=True
+    ):
         self.loaduser = loaduser
         self.url = self._build_urls()["uttak"]
         self.time_retrieved = ""
         self.tableid = tableid
         self.raise_errors = raise_errors
         self.tablename = ""
         self.subtables = {}
@@ -83,26 +85,19 @@
         self.codelists = {}
         self.suppression = None
         if headers:
             self.headers = headers
         else:
             self.headers = self._build_headers()
         try:
-            self._get_uttrekksbeskrivelse()
+            self._get_uttrekksbeskrivelse(printing)
         finally:
             if hasattr(self, "headers"):
                 del self.headers
         self._split_attributes()
-        # Add methods from other placholder class
-        for method in [
-            method
-            for method in dir(StatbankUttrekkValidators)
-            if not method.startswith("__")
-        ]:
-            setattr(self, method, getattr(StatbankUttrekkValidators, method))
 
     def __str__(self):
         variabel_text = ""
         for i, deltabell in enumerate(self.variables):
             variabel_text += f"""\nDeltabell (DataFrame) nummer {i+1}:
                 {deltabell["deltabell"]}
                 """
@@ -134,75 +129,110 @@
     def __repr__(self):
         return (
             'StatbankUttrekksBeskrivelse(tableid="'
             + f'{self.tableid}", loaduser="{self.loaduser}")'
         )
 
     def transferdata_template(self) -> dict:
+        """Get the shape the data should have to name the "deltabeller".
+        If we didnt use a dictionary we would have to rely on the order of a list of "deltabeller".
+        Instead we chose to explicitly name the deltabller in this package.
+
+        Returns
+        -------
+        A dictionary with correct keys, but placeholders for where the dataframes should go.
+        """
         template = {k: f"df{i}" for i, (k, v) in enumerate(self.subtables.items())}
         print("{")
         for k, v in template.items():
             print(f'"{k}" : {v},')
         print("}")
         return template
 
     def to_json(self, path: str = "") -> dict:
-        """If path is provided, tries to write to it,
+        """Store a copy of the current state of the uttrekk-object as a json.
+        If path is provided, tries to write to it,
         otherwise will return a json-string for you to handle like you wish.
+
+        Parameters
+        -------
+        path: if provided, will try to write a json to a local path
+
+        Returns
+        -------
+        If path is provided, tries to write a json there and returns nothing.
+        If path is not provided, returns the json-string for you to handle as you wish.
         """
         # Need to this because im stupidly adding methods from other class as attributes
         content = {k: v for k, v in self.__dict__.items() if not callable(v)}
 
         if path:
             print(f"Writing to {path}")
             with open(path, mode="w") as json_file:
                 json_file.write(json.dumps(content))
         else:
             return json.dumps(content)
 
     def validate(self, data, raise_errors: bool = False, printing: bool = True) -> dict:
+        """Uses the contents of itself to validate the data against.
+        All validation happens locally, so dont be afraid of any data
+        being sent to statbanken using this method.
+
+        Parameters
+        -------
+        data: The data to validate in a dictionary of deltabell-names as keys and pandas-dataframes as values.
+        raise_errors: True/False based on if you want the method to raise its own errors or not.
+        printing: True/False based on if you want a verbose printing of everything the validation checks.
+
+        Returns
+        -------
+        A dictionary of the errors the validation wants to raise.
+        """
         if not raise_errors:
             raise_errors = self.raise_errors
 
         validation_errors = {}
         if printing:
             print("\nvalidating...")
 
-        self._validate_number_dataframes(self, data=data)
+        self._validate_number_dataframes(data=data)
         validation_errors = self._validate_number_columns(
-            self, data, validation_errors, printing
+            data, validation_errors, printing
         )
         (
             categorycode_outside,
             categorycode_missing,
             validation_errors,
-        ) = self._category_code_usage(self, data, validation_errors, printing)
-        validation_errors = self._check_for_floats(
-            self, data, validation_errors, printing
-        )
-        validation_errors = self._check_rounding(
-            self, data, validation_errors, printing
-        )
-        validation_errors = self._check_time_formats(
-            self, data, validation_errors, printing
-        )
-        validation_errors = self._check_suppression(
-            self, data, validation_errors, printing
-        )
+        ) = self._category_code_usage(data, validation_errors, printing)
+        validation_errors = self._check_for_floats(data, validation_errors, printing)
+        validation_errors = self._check_rounding(data, validation_errors, printing)
+        validation_errors = self._check_time_formats(data, validation_errors, printing)
+        validation_errors = self._check_suppression(data, validation_errors, printing)
         validation_errors = self._check_unique_combinations_categories(
-            self, data, validation_errors, printing
+            data, validation_errors, printing
         )
 
         if raise_errors and validation_errors:
             raise Exception(list(validation_errors.values()))
         return validation_errors
 
     def round_data(self, data) -> dict:
         """Checks that all decimal numbers are converted to strings,
-        with specific length after the decimal-seperator "," """
+        with specific length kept after the decimal-seperator ","
+        IMPORTANT: Rounds "real halves" UP, instead of "to even numbers" like Python does by default.
+        This is maybe the behaviour staticians are used to from Excel, SAS etc.
+
+        Parameters
+        -------
+        data: The data to validate in a dictionary of deltabell-names as keys and pandas-dataframes as values.
+
+        Returns
+        -------
+        A dictionary in the same shape as sent in, but with dataframes altered to correct for rounding.
+        """
         data_copy = copy.deepcopy(data)
         for deltabell in self.variables:
             deltabell_name = deltabell["deltabell"]
             for variabel in deltabell["variabler"] + deltabell["statistikkvariabler"]:
                 if "Antall_lagrede_desimaler" in variabel.keys():
                     col_num = int(variabel["kolonnenummer"]) - 1
                     decimal_num = int(variabel["Antall_lagrede_desimaler"])
@@ -244,31 +274,34 @@
                 return ""
             elif decimals and n:
                 n = round(Decimal(n), decimals)
             elif n:
                 n = Decimal(n).to_integral_value()
         return str(n)
 
-    def _get_uttrekksbeskrivelse(self) -> dict:
+    def _get_uttrekksbeskrivelse(self, printing) -> dict:
         filbeskrivelse_url = self.url + "tableId=" + self.tableid
         try:
             filbeskrivelse = self._make_request(filbeskrivelse_url, self.headers)
         finally:
             if hasattr(self, "headers"):
                 del self.headers
 
         if filbeskrivelse.status_code != 200:
             raise ConnectionError(filbeskrivelse, filbeskrivelse.text)
+        # Rakel encountered an error with a tab-character in the json, should we just strip this?
+        filbeskrivelse = filbeskrivelse.text.replace("\t", "")
         # Also deletes / overwrites returned Auth-header from get-request
-        filbeskrivelse = json.loads(filbeskrivelse.text)
-        print(
-            f"""Hentet uttaksbeskrivelsen for {filbeskrivelse['Huvudtabell']},
-        med tableid: {self.tableid}
-        den {filbeskrivelse['Uttaksbeskrivelse_lagd']}"""
-        )
+        filbeskrivelse = json.loads(filbeskrivelse)
+        if printing:
+            print(
+                f"""Hentet uttaksbeskrivelsen for {filbeskrivelse['Huvudtabell']},
+            med tableid: {self.tableid}
+            den {filbeskrivelse['Uttaksbeskrivelse_lagd']}"""
+            )
 
         # reset tableid and hovedkode after content of request
         self.filbeskrivelse = filbeskrivelse
 
     def _make_request(self, url: str, header: dict):
         return r.get(url, headers=self.headers)
```

### Comparing `dapla_statbank_client-1.0.0/statbank/uttrekk_validations.py` & `dapla_statbank_client-1.0.2/statbank/uttrekk_validations.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     def _check_time_formats(self, data, validation_errors: dict, printing) -> dict:
         # Time-columns should follow time format
         for deltabell in self.variables:
             for variabel in deltabell["variabler"]:
                 if "Kodeliste_text" in variabel.keys():
                     if "format = " in variabel["Kodeliste_text"]:
                         validation_errors = self._check_time_columns(
-                            self,
                             deltabell["deltabell"],
                             variabel,
                             data,
                             validation_errors,
                             printing,
                         )
         for k in validation_errors.keys():
```

### Comparing `dapla_statbank_client-1.0.0/PKG-INFO` & `dapla_statbank_client-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-statbank-client
-Version: 1.0.0
+Version: 1.0.2
 Summary: Handles data transfer Statbank <-> Dapla for Statistics Norway
 License: MIT
 Author: Statistics Norway
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -37,15 +37,15 @@
 # Fill out password
 # Default publishing-date is TOMORROW
 print(stat_client)
 # Printing will show you all the default settings on the client.
 # You can change for example date by specifying it: StatbankClient(loaduser = "LASTEBRUKER", date="2023-02-16")
 ```
 
-Be aware that from the **dapla staging environment** you will be sending to statbank-TEMP-database, your changes will not be published. But if you are in the main dapla-jupyterlab (prod), you WILL publish to statbanken, in the PROD database. So pay extra attention to the **publishing-date** when in dapla-main-prod-jupyterlab.
+Be aware that from the **dapla-staging environment** you will be sending to statbank-TEST-database, your changes will not be published. For this you need the "test-password", which is for the same user (lastebruker), but different from the ordinary password (lastepassord). If you are missing the test-password, have the statbank-team send it to you for you loaduser. If you are in the main dapla-jupyterlab (prod), you **WILL** publish to statbanken, in the PROD database. So pay extra attention to the **publishing-date** when in dapla-main-prod-jupyterlab. And be aware of which password you are entering, based on your environment. [To see data actually published to the test-database, you can use this link if you work at SSB.](https://i.test.ssb.no/pxwebi/pxweb/no/test_24v_intern/)
 
 
 ### Usage Transferring
 
 ```python
 stat_client.transfer({"deltabellfilnavn.dat" : df_06399}, "06339")
 ```
@@ -145,14 +145,15 @@
 filbesk_06339_new = stat_client.read_description_json("path.json")
 ```
 Some deeper data-structures, like the dataframes in the transfer will not be serialized and stored with the transfer-object in its json.
 
 ---
 
 ### Version history
+- 1.0.2 Doc-string style cleanup, a check on username and password on client init, changes to time and display of time, demo notebooks cleaned
 - 1.0.0 Finished going through initial issues, less complaining from verify on floats
 - 0.0.11 Statbank people wanted a user-agent-requesst-header to differentiate test from prod
 - 0.0.9 After further user-testing and requests
 - 0.0.5 Still some parameter issues
 - 0.0.4 More test coverage, some bugs fixed in rounding checks and parameter-passing
 - 0.0.3 Removed batches, stripping uttrekk from transfer, rounding function on uttrekk, data required in as a dict of dataframes, with "deltabell-navn". Tableid now works to transfer to instead of only "hovedtabellnavn"
 - 0.0.2 Starting alpha, fine-tuning release to Pypi on github-release
```

