# Comparing `tmp/idf_analysis-0.1.8-py3-none-any.whl.zip` & `tmp/idf_analysis-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 28498 bytes, number of entries: 17
+Zip file size: 28390 bytes, number of entries: 17
 -rwxrwxrwx  2.0 unx      606 b- defN 20-Feb-12 08:32 idf_analysis/__init__.py
 -rwxrwxrwx  2.0 unx      280 b- defN 20-Feb-12 08:32 idf_analysis/__main__.py
--rwxrwxrwx  2.0 unx     7716 b- defN 20-Mar-16 17:40 idf_analysis/additional_scripts.py
+-rwxrwxrwx  2.0 unx     7656 b- defN 20-Mar-16 18:13 idf_analysis/additional_scripts.py
 -rwxrwxrwx  2.0 unx     4125 b- defN 20-Feb-12 08:32 idf_analysis/arg_parser.py
--rwxrwxrwx  2.0 unx    19211 b- defN 20-Mar-16 16:49 idf_analysis/calculation_methods.py
+-rwxrwxrwx  2.0 unx    19132 b- defN 20-Mar-16 18:13 idf_analysis/calculation_methods.py
 -rwxrwxrwx  2.0 unx     1067 b- defN 20-Mar-15 22:34 idf_analysis/definitions.py
 -rwxrwxrwx  2.0 unx    25045 b- defN 20-Mar-16 17:30 idf_analysis/idf_class.py
 -rwxrwxrwx  2.0 unx     2050 b- defN 20-Mar-15 22:10 idf_analysis/in_out.py
 -rwxrwxrwx  2.0 unx     2525 b- defN 20-Mar-16 14:14 idf_analysis/little_helpers.py
 -rwxrwxrwx  2.0 unx     2921 b- defN 20-Mar-05 16:05 idf_analysis/plot_helpers.py
--rwxrwxrwx  2.0 unx     7939 b- defN 20-Mar-16 10:27 idf_analysis/sww_utils.py
--rwxrwxrwx  2.0 unx      394 b- defN 20-Mar-16 17:52 idf_analysis-0.1.8.data/scripts/idf_analysis
--rwxrwxrwx  2.0 unx     1063 b- defN 20-Mar-16 17:52 idf_analysis-0.1.8.dist-info/LICENSE
--rwxrwxrwx  2.0 unx    10369 b- defN 20-Mar-16 17:52 idf_analysis-0.1.8.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 20-Mar-16 17:52 idf_analysis-0.1.8.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       13 b- defN 20-Mar-16 17:52 idf_analysis-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1439 b- defN 20-Mar-16 17:52 idf_analysis-0.1.8.dist-info/RECORD
-17 files, 86855 bytes uncompressed, 26128 bytes compressed:  69.9%
+-rwxrwxrwx  2.0 unx     7771 b- defN 20-Mar-16 18:13 idf_analysis/sww_utils.py
+-rwxrwxrwx  2.0 unx      394 b- defN 20-Mar-16 18:14 idf_analysis-0.1.9.data/scripts/idf_analysis
+-rwxrwxrwx  2.0 unx     1063 b- defN 20-Mar-16 18:14 idf_analysis-0.1.9.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx    10369 b- defN 20-Mar-16 18:14 idf_analysis-0.1.9.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 20-Mar-16 18:14 idf_analysis-0.1.9.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       13 b- defN 20-Mar-16 18:14 idf_analysis-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1439 b- defN 20-Mar-16 18:14 idf_analysis-0.1.9.dist-info/RECORD
+17 files, 86548 bytes uncompressed, 26020 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: idf_analysis/plot_helpers.py
 Comment: 
 
 Filename: idf_analysis/sww_utils.py
 Comment: 
 
-Filename: idf_analysis-0.1.8.data/scripts/idf_analysis
+Filename: idf_analysis-0.1.9.data/scripts/idf_analysis
 Comment: 
 
-Filename: idf_analysis-0.1.8.dist-info/LICENSE
+Filename: idf_analysis-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: idf_analysis-0.1.8.dist-info/METADATA
+Filename: idf_analysis-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: idf_analysis-0.1.8.dist-info/WHEEL
+Filename: idf_analysis-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: idf_analysis-0.1.8.dist-info/top_level.txt
+Filename: idf_analysis-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: idf_analysis-0.1.8.dist-info/RECORD
+Filename: idf_analysis-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## idf_analysis/additional_scripts.py

```diff
@@ -2,15 +2,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.lines import Line2D
 from webbrowser import open as show_file
 
 from .definitions import COL, PARAM_COL, PARAM
-# from .idf_class import IntensityDurationFrequencyAnalyse
 from .little_helpers import minutes_readable
 from .sww_utils import agg_events
 
 
 def get_interim_results_from_parameters(parameters):
     """
     extract interim results from parameters
```

## idf_analysis/calculation_methods.py

```diff
@@ -5,25 +5,22 @@
 __version__ = "0.1"
 __license__ = "MIT"
 
 import warnings
 
 import pandas as pd
 import numpy as np
-from numpy import NaN
 from math import e, floor
 from collections import OrderedDict
 
 from tqdm import tqdm
 
 from .sww_utils import guess_freq, rain_events, agg_events, year_delta
 from .definitions import DWA, ATV, DWA_adv, PARTIAL, ANNUAL, LOG1, LOG2, HYP, LIN, COL, PARAM, PARAM_COL
 
-from mp.helpers.check_time import timeit, Timer
-
 
 ########################################################################################################################
 def annual_series(events):
     """
     create an annual series of the maximum overlapping sum per year and calculate the "u" and "w" parameters
     acc. to DWA-A 531 chap. 5.1.5
 
@@ -123,15 +120,14 @@
 
     return np.interp(interval,
                      list(improve_factor.keys()),
                      list(improve_factor.values()))
 
 
 ########################################################################################################################
-@timeit
 def calculate_u_w(file_input, duration_steps, series_kind):
     """
     statistical analysis for each duration step acc. to DWA-A 531 chap. 5.1
     save the parameters of the distribution function as interim results
     acc. to DWA-A 531 chap. 4.4: use the annual series only for measurement periods over 20 years
```

## idf_analysis/sww_utils.py

```diff
@@ -1,17 +1,13 @@
 import pytz
 from datetime import tzinfo
 import pandas as pd
 from pandas.tseries.frequencies import to_offset
-from pandas.tseries.offsets import _delta_to_tick as delta_to_freq
-from pandas import DatetimeIndex, DateOffset, Timedelta
-from tqdm import tqdm
 import numpy as np
 
-from mp.helpers import timeit
 from .definitions import COL
 
 __author__ = "David Camhy, Markus Pichler"
 __copyright__ = "Copyright 2018, University of Technology Graz"
 __credits__ = ["David Camhy", "Markus Pichler"]
 __license__ = "MIT"
 __version__ = "1.0.0"
@@ -72,15 +68,15 @@
     guess the frequency by evaluating the most often frequency
 
     Args:
         date_time_index (pandas.DatetimeIndex): index of a time-series
         default (pandas.Timedelta):
 
     Returns:
-        DateOffset: frequency of the date-time-index
+        pandas.DateOffset: frequency of the date-time-index
     """
     freq = date_time_index.freq
     if pd.notnull(freq):
         return to_offset(freq)
 
     if not len(date_time_index) <= 3:
         freq = pd.infer_freq(date_time_index)  # 'T'
```

## Comparing `idf_analysis-0.1.8.dist-info/LICENSE` & `idf_analysis-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `idf_analysis-0.1.8.dist-info/METADATA` & `idf_analysis-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-analysis
-Version: 0.1.8
+Version: 0.1.9
 Summary: heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
 Home-page: https://github.com/MarkusPic/intensity_duration_frequency_analysis
 Author: Markus Pichler
 Author-email: markus.pichler@tugraz.at
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `idf_analysis-0.1.8.dist-info/RECORD` & `idf_analysis-0.1.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 idf_analysis/__init__.py,sha256=sYARO7Y9GZQeDCu-IGobbwRFAlBS3J73q1ahjRbORq8,606
 idf_analysis/__main__.py,sha256=PdT_M85QIIHMVF9A9-i-B2MpKnQULnSGa8R3pRupnSc,280
-idf_analysis/additional_scripts.py,sha256=7tiMa-5sMlII_nhk2e8rUqYnXMkV_Rrr35uTfwhrQHA,7716
+idf_analysis/additional_scripts.py,sha256=7l4yAp1Am0YDL_6QnnWCDUt_HYVx66VP23xAEWwVTc0,7656
 idf_analysis/arg_parser.py,sha256=HlKUBZY_iCKgVtpIRLYzSrr9t_TzG4wh0FjCEZuiSjc,4125
-idf_analysis/calculation_methods.py,sha256=cWVyv2FRr6Zii17_R0qvmtQ0hmJ_u1lELI_R-UlAlac,19211
+idf_analysis/calculation_methods.py,sha256=f-KG8ZwRp3zh-wZsT9bmEfEw7INiOBHotY8DQffX398,19132
 idf_analysis/definitions.py,sha256=ubF67e7VNfnP9CFsemIuzS-Xw7I5nl7I2ZrOMrugmNY,1067
 idf_analysis/idf_class.py,sha256=VUNDls4kglkhxACDEdtqcb_sddLH_w44ZEOMNwBtyjo,25045
 idf_analysis/in_out.py,sha256=OL34UXqcZcpH3W5_GeP4OTDEIWsnkHhykYjOBiBPHRs,2050
 idf_analysis/little_helpers.py,sha256=XOmePLkcD38fra9Mt5uki-ym9ruDtT1Mv4XSAH2MZbY,2525
 idf_analysis/plot_helpers.py,sha256=8kqkw0wFnfQsHdBMoJ7XzwU1vnxRMlc7-P9rmd8ow3w,2921
-idf_analysis/sww_utils.py,sha256=iaQOmGS-aPg_XkQJBy2cE1B3vBFCIIuIMKy5gcNs89c,7939
-idf_analysis-0.1.8.data/scripts/idf_analysis,sha256=ZdafUuSmqKn8uTIm1qf7y5eeGtPpO41v5gR3xNvJkmM,394
-idf_analysis-0.1.8.dist-info/LICENSE,sha256=Gb7p8qLfOkyeIr3EwWdid6hms_Gk-_58Lg2Uu1Q9B10,1063
-idf_analysis-0.1.8.dist-info/METADATA,sha256=f7TpkLus-XjG9s0j9QWQCxdo5NhG7HOz4H5vP-daLRk,10369
-idf_analysis-0.1.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-idf_analysis-0.1.8.dist-info/top_level.txt,sha256=ye2G1NLdo-Prv43P8IhlTFlHBWBQ5JSiNGJ6L4uSarA,13
-idf_analysis-0.1.8.dist-info/RECORD,,
+idf_analysis/sww_utils.py,sha256=ZycxyO1vB3OcEdPdQkSaVvFGNUbS1S9ye32wVVSt5jw,7771
+idf_analysis-0.1.9.data/scripts/idf_analysis,sha256=ZdafUuSmqKn8uTIm1qf7y5eeGtPpO41v5gR3xNvJkmM,394
+idf_analysis-0.1.9.dist-info/LICENSE,sha256=Gb7p8qLfOkyeIr3EwWdid6hms_Gk-_58Lg2Uu1Q9B10,1063
+idf_analysis-0.1.9.dist-info/METADATA,sha256=CW8zde5h_C1vyo3yMSalUyviYfzvZzj1ky9zzC7e8cs,10369
+idf_analysis-0.1.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+idf_analysis-0.1.9.dist-info/top_level.txt,sha256=ye2G1NLdo-Prv43P8IhlTFlHBWBQ5JSiNGJ6L4uSarA,13
+idf_analysis-0.1.9.dist-info/RECORD,,
```

