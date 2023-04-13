# Comparing `tmp/pdxtra-1.0.1-py3-none-any.whl.zip` & `tmp/pdxtra-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 34867 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    28526 b- defN 23-Mar-25 08:17 pdxtra.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Mar-25 08:38 pdxtra-1.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx    43600 b- defN 23-Mar-25 08:38 pdxtra-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-25 08:38 pdxtra-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-25 08:38 pdxtra-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      449 b- defN 23-Mar-25 08:38 pdxtra-1.0.1.dist-info/RECORD
-6 files, 107823 bytes uncompressed, 34063 bytes compressed:  68.4%
+Zip file size: 35023 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    29099 b- defN 23-Apr-13 02:26 pdxtra.py
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-13 02:28 pdxtra-1.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    43600 b- defN 23-Apr-13 02:28 pdxtra-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-13 02:28 pdxtra-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-13 02:28 pdxtra-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      449 b- defN 23-Apr-13 02:28 pdxtra-1.0.2.dist-info/RECORD
+6 files, 108396 bytes uncompressed, 34219 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pdxtra.py
 Comment: 
 
-Filename: pdxtra-1.0.1.dist-info/LICENSE
+Filename: pdxtra-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: pdxtra-1.0.1.dist-info/METADATA
+Filename: pdxtra-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pdxtra-1.0.1.dist-info/WHEEL
+Filename: pdxtra-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pdxtra-1.0.1.dist-info/top_level.txt
+Filename: pdxtra-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pdxtra-1.0.1.dist-info/RECORD
+Filename: pdxtra-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pdxtra.py

```diff
@@ -554,15 +554,17 @@
             self,
             values: Sequence,
             column: str,
             method: Optional[str] = None,
             tolerance: Optional[
                 Union[int, float, date, datetime, type(None)]
             ] = None,
-            ) -> Series:
+            fillna: Any = np.nan,
+            filter_nan: bool = False,
+            ) -> NDArray:
         """
         Performs an Excel-like, veritcal lookup. In this case, the "v" in the
         function name has a double meaning. It stands for both "vertical"
         and "vector", because unlike the typical vertical lookup in Excel,
         the function returns a vector of values (``numpy.array``) from the
         specified column, rather than a scalar. Can perform nearest match on
         the index column.
@@ -587,25 +589,39 @@
             The maximum distance to search on either side of the index value
             when performing nearest match. If searching a series containing
             ``date`` or ``datetime`` objects, the user is responsible for
             providing the appropriate ``timedelta`` for computing differences
             between the index values and the values supplied in the function
             call. This argument is ignored when the method is ``None``. See
             ``pandas.Index.get_indexer`` for further explanation.
+        fillna : `Any`, default `np.nan`
+            Fill missing values with the value specified. Has no effect if
+            ``filter_nan`` is ``True``.
+        filter_nan : `bool`, default `False`
+            Filter out values which whose corresponding index value is not
+            found in the index.
 
         Returns
         -------
         A 1-d Numpy array, which can be empty if no values are found.
         """
         mask = self.index.get_indexer(
             values,
             tolerance=tolerance,
             method=method,
         )
-        lookup = self.iloc[mask[np.nonzero(mask >= 0)]][column]
+        if filter_nan:
+            lookup = self.loc[mask[np.nonzero(mask >= 0)]][column].values
+        else:
+            lookup = np.where(
+                mask != -1,
+                self.iloc[mask][column].values,
+                fillna,
+            )
+
         return lookup
 
 
 class TimeSeries(Series):
 
     def __init__(self, *args, **kwargs) -> None:
         super(TimeSeries, self).__init__(*args, **kwargs)
@@ -626,15 +642,14 @@
         Returns
         -------
         A PDXtra ``Series`` object.
         """
         close_delta = self.diff()
         up = close_delta.clip(lower=0)
         down = -1 * close_delta.clip(upper=0)
-
         return up.true_ema(span) / down.true_ema(span)
 
     def macd(self, short_span: int = 12, long_span: int = 26) -> Series:
         """
         Converts the ``Series`` to moving average convergence-divergence.
 
         Parameters
```

## Comparing `pdxtra-1.0.1.dist-info/LICENSE` & `pdxtra-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pdxtra-1.0.1.dist-info/METADATA` & `pdxtra-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdxtra
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pandas with time-series data analysis in mind.
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

