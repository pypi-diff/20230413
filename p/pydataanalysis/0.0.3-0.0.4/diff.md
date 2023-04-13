# Comparing `tmp/pydataanalysis-0.0.3.tar.gz` & `tmp/pydataanalysis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydataanalysis-0.0.3.tar", last modified: Sun Apr  9 09:10:17 2023, max compression
+gzip compressed data, was "pydataanalysis-0.0.4.tar", last modified: Thu Apr 13 09:23:27 2023, max compression
```

## Comparing `pydataanalysis-0.0.3.tar` & `pydataanalysis-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.825854 pydataanalysis-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-03-22 14:25:57.000000 pydataanalysis-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2964 2023-04-09 09:10:17.823854 pydataanalysis-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1933 2023-04-09 09:03:16.000000 pydataanalysis-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.595840 pydataanalysis-0.0.3/descriptive/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:19:42.000000 pydataanalysis-0.0.3/descriptive/__init__.py
--rw-rw-rw-   0        0        0    10312 2023-04-09 08:54:11.000000 pydataanalysis-0.0.3/descriptive/pydataprocessing.py
--rw-rw-rw-   0        0        0    17822 2023-04-04 09:31:18.000000 pydataanalysis-0.0.3/descriptive/pyeda.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.618842 pydataanalysis-0.0.3/diagnostic/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:20:23.000000 pydataanalysis-0.0.3/diagnostic/__init__.py
--rw-rw-rw-   0        0        0     5884 2023-04-04 09:31:18.000000 pydataanalysis-0.0.3/diagnostic/pydiagnostic.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.666844 pydataanalysis-0.0.3/predictive/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:18:06.000000 pydataanalysis-0.0.3/predictive/__init__.py
--rw-rw-rw-   0        0        0    13946 2023-04-04 09:31:19.000000 pydataanalysis-0.0.3/predictive/pypredictive.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.697846 pydataanalysis-0.0.3/prescriptive/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:18:42.000000 pydataanalysis-0.0.3/prescriptive/__init__.py
--rw-rw-rw-   0        0        0     1351 2023-04-04 09:31:17.000000 pydataanalysis-0.0.3/prescriptive/pyprescriptive.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:10:17.819853 pydataanalysis-0.0.3/pydataanalysis.egg-info/
--rw-rw-rw-   0        0        0     2964 2023-04-09 09:10:16.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-04-09 09:10:17.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 09:10:16.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-09 09:10:16.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       47 2023-04-09 09:10:16.000000 pydataanalysis-0.0.3/pydataanalysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 09:10:17.827854 pydataanalysis-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-04-02 13:19:45.000000 pydataanalysis-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:23:27.853678 pydataanalysis-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-03-22 14:25:57.000000 pydataanalysis-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2964 2023-04-13 09:23:27.848677 pydataanalysis-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1933 2023-04-09 09:03:16.000000 pydataanalysis-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 09:23:27.649666 pydataanalysis-0.0.4/descriptive/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:19:42.000000 pydataanalysis-0.0.4/descriptive/__init__.py
+-rw-rw-rw-   0        0        0    10309 2023-04-13 09:15:57.000000 pydataanalysis-0.0.4/descriptive/pydataprocessing.py
+-rw-rw-rw-   0        0        0    17875 2023-04-13 09:15:58.000000 pydataanalysis-0.0.4/descriptive/pyeda.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:23:27.666667 pydataanalysis-0.0.4/diagnostic/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:20:23.000000 pydataanalysis-0.0.4/diagnostic/__init__.py
+-rw-rw-rw-   0        0        0     5780 2023-04-13 09:15:57.000000 pydataanalysis-0.0.4/diagnostic/pydiagnostic.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:23:27.725670 pydataanalysis-0.0.4/predictive/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:18:06.000000 pydataanalysis-0.0.4/predictive/__init__.py
+-rw-rw-rw-   0        0        0    15161 2023-04-13 09:15:58.000000 pydataanalysis-0.0.4/predictive/pypredictive.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:23:27.746672 pydataanalysis-0.0.4/prescriptive/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:18:42.000000 pydataanalysis-0.0.4/prescriptive/__init__.py
+-rw-rw-rw-   0        0        0     1352 2023-04-13 09:15:58.000000 pydataanalysis-0.0.4/prescriptive/pyprescriptive.py
+drwxrwxrwx   0        0        0        0 2023-04-13 09:23:27.842677 pydataanalysis-0.0.4/pydataanalysis.egg-info/
+-rw-rw-rw-   0        0        0     2964 2023-04-13 09:23:26.000000 pydataanalysis-0.0.4/pydataanalysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-04-13 09:23:26.000000 pydataanalysis-0.0.4/pydataanalysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 09:23:26.000000 pydataanalysis-0.0.4/pydataanalysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-13 09:23:26.000000 pydataanalysis-0.0.4/pydataanalysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       47 2023-04-13 09:23:26.000000 pydataanalysis-0.0.4/pydataanalysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 09:23:27.854678 pydataanalysis-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1118 2023-04-13 09:17:47.000000 pydataanalysis-0.0.4/setup.py
```

### Comparing `pydataanalysis-0.0.3/LICENSE` & `pydataanalysis-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydataanalysis-0.0.3/PKG-INFO` & `pydataanalysis-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydataanalysis
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Analysis and  Visualization Functions
 Home-page: UNKNOWN
 Author: Tamer Samara
 Author-email: tamer.samara@gmail.com
 License: MIT
 Description: <h1>Data Analysis CheatSheet (everything you might need )</h1>
         <p>
```

### Comparing `pydataanalysis-0.0.3/README.md` & `pydataanalysis-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pydataanalysis-0.0.3/descriptive/pydataprocessing.py` & `pydataanalysis-0.0.4/descriptive/pydataprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 
 def unique_values(data, categorical_column: str):
     """
     Print out all the unique values in a categorical column.
 
     :param data: variable
 
-    :param categorical_column:string
+    :param categorical_column: string
 
-    :return:unique values in dataset
+    :return: unique values in dataset
     """
     cat_col = data[categorical_column].unique()
     cat_col.sort()
     return cat_col
 
 
 def columns_with_missing_values(data) -> list:
     """
     Missing values.
 
-    :param data:variable
+    :param data: variable
 
-    :return:a list of columns with missing values
+    :return: list of columns with missing values
     """
     cols_with_missing = [col for col in data.columns if data[col].isnull().any()]
     return cols_with_missing
 
 
 def replace_NaN_value(data, column_name: str, value_by: str):
     """
     Replace value by median, mode or mean.
 
-    :param data:variable
+    :param data: variable
 
     :param column_name: str
 
     :param value_by: str
 
     :return: column
 
@@ -58,45 +58,45 @@
         print("Enter mean, median or mode to fill in the missing values")
 
 
 def drop_missing_rows(data):
     """
     Drop rows with missing values.
 
-    :param data:variable
+    :param data: variable
 
-    :return:dataframe
+    :return: dataframe
 
     """
     dataframe_without_missing_rows = data.copy()
     dataframe_without_missing_rows.dropna(inplace=True)
     return dataframe_without_missing_rows
 
 
 def replace_missing_values_with_zero(data):
     """
     Replace all NaN values with 0.
 
-    :param data:variable
+    :param data: variable
 
-    :return:dataframe
+    :return: dataframe
 
     """
     data_filled_with_zero = data.copy()
     data_filled_with_zero.fillna(0, inplace=True)
     return data_filled_with_zero
 
 
 def replace_missing_values_with_what_comes_after_it(data):
     """
     Replace missing values that comes directly after it in the same column.
 
-    :param data:variable
+    :param data: variable
 
-    :return:filled dataframe
+    :return: filled dataframe
     """
     bfill_data = data.copy()
     bfill_data.fillna(method="bfill", axis=0, inplace=True)
     return bfill_data
 
 
 def replace_missing_values_with_string(data, column_name: str, my_string: str):
@@ -128,17 +128,17 @@
     return data_without_duplicates
 
 
 def one_hot_encoding(data, categorical_col: list):
     """
     Encode categorical variables using one-hot encoding.
 
-    :param data:variable
+    :param data: variable
 
-    :param categorical_col:list
+    :param categorical_col: list
 
     :return: dataframe
     """
     try:
         one_hot_encoded_data = pd.get_dummies(data, columns=categorical_col)
 
     except TypeError:
@@ -149,17 +149,17 @@
         return one_hot_encoded_data
 
 
 def label_encoding(data, categorical_col: list):
     """
     Encode categorical variables using label encoder.
 
-    :param data:variable
+    :param data: variable
 
-    :param categorical_col:list
+    :param categorical_col: list
 
     :return:  dataframe
     """
     try:
         label_encoder = LabelEncoder()
         data[categorical_col] = data[categorical_col].apply(label_encoder.fit_transform)
     except ValueError:
@@ -172,15 +172,15 @@
 
 def standardization_numerical_columns(data, numerical_column: list):
     """
     Scale values of a numeric column so that they have zero mean and unit variance.
 
     :param data: variable
 
-    :param numerical_column:String
+    :param numerical_column: str
 
     :return: scale dataframe
     """
     std_scaler = StandardScaler()
     df_scaled = std_scaler.fit_transform(data[numerical_column])
     df_scaled = pd.DataFrame(df_scaled, columns=numerical_column)
     return df_scaled
@@ -203,94 +203,94 @@
 
 def divide_num_col_into_cat_col_using_bins(data, numerical_col: str, number_bins: int):
     """
     Divide the values of a continuous numeric column into categorical column using bins.
 
     :param data: variable
 
-    :param numerical_col: string
+    :param numerical_col: str
 
     :param number_bins: integer
 
     :return: dataframe
     """
     discretizer = KBinsDiscretizer(n_bins=number_bins, encode="ordinal")
     data[numerical_col] = discretizer.fit_transform(data[[numerical_col]])
     return data
 
 
 def min_max_scaler_to_numerical_column(data, numerical_column: list):
     """
-    Scale the values of a numeric column so that they have a minimum value of 0 and a maximum value of 1.
+    Scale value of numeric column so that they have a minimum value of 0 and a maximum value of 1.
 
     :param data: variable
 
-    :param numerical_column:string
+    :param numerical_column: str
 
-    :return:dataframe
+    :return: dataframe
     """
     scaler = MinMaxScaler()
     df_scaled = scaler.fit_transform(data.to_numpy())
     df_scaled = pd.DataFrame(df_scaled, columns=numerical_column)
     return df_scaled
 
 
 def robust_scaling_to_numerical_column(data, numerical_column: str):
     """
     Scale values of a numeric column using the median and interquartile range.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_column:string
+    :param numerical_column: str
 
-    :return:dataframe
+    :return: dataframe
     """
     scaler = RobustScaler()
     data[numerical_column] = scaler.fit_transform(data[[numerical_column]])
     return data
 
 
 def power_transformation_to_numerical_column(data, numerical_column: str):
     """
     Transform values of a numeric column in order to stabilize or improve the assumptions of certain statistical models.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_column:string
+    :param numerical_column: str
 
-    :return:dataframe
+    :return: dataframe
     """
     transformer = PowerTransformer()
     data[numerical_column] = transformer.fit_transform(data[[numerical_column]])
     return data
 
 
 def quantile_transformation_to_numerical_column(data, numerical_column: str):
     """
     Transform column value so that they have a uniform or normal distribution.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_column: string
+    :param numerical_column: str
 
-    :return:dataframe
+    :return: dataframe
 
     """
     transformer = QuantileTransformer()
     data[numerical_column] = transformer.fit_transform(data[[numerical_column]])
     return data
 
 
 def box_cox_transformation_to_numerical_column(data, numerical_column: str):
     """
     Box cox transformation.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_column: string
+    :param numerical_column: str
 
     :return: dataframe
 
     """
     data[numerical_column], lambda_ = boxcox(data[numerical_column])
     return data
```

### Comparing `pydataanalysis-0.0.3/descriptive/pyeda.py` & `pydataanalysis-0.0.4/descriptive/pyeda.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     
     :param file_name: string contain the csv file name
     
     :return: pandas dataframe
     
     """
     try:
-        df = pd.read_csv(file_name, parse_dates=True)
+        df = pd.read_csv(file_name, parse_dates=True, header=0, index_col=0)
         return df
     except FileNotFoundError:
         print("No such File, upload your dataset CSV file to the project")
 
 
 def display_summary_data(dataframe):
     """
@@ -90,15 +90,15 @@
 
 def visualize_different_plots_of_numeric_col(data_frame, column_name: str):
     """
     Visualize different plots of numeric column.
     
     :param data_frame: variable
     
-    :param column_name: string with column name
+    :param column_name: str
     
     :return: chart
     
     """
     if data_frame[column_name].dtype != object:
         fig, ax = plt.subplots(1, 5, figsize=(24, 4))
         sns.histplot(data_frame[column_name], bins=30, kde=True, ax=ax[0])
@@ -211,39 +211,39 @@
 
 def visualize_bar_plot_for_each_category_of_categorical_column(data, cat_column: str, num_column: str):
     """
     Visualize the mean of a numeric column for each category of a categorical column.
     
     :param data: variable
     
-    :param cat_column:str
+    :param cat_column: str
     
-    :param num_column:str
+    :param num_column: str
     
     :return: bar chart
     
     """
     data.groupby(cat_column)[num_column].mean().plot(kind="bar")
     plt.ylabel(f"Average {num_column}")
     plt.show()
 
 
 def pivot_tabel(data, index_col: list, columns: list, values: list, agg: str):
     """
     Create a pivot table to summarize the data.
 
-    :param data:variable
+    :param data: variable
 
-    :param index_col:list of column name
+    :param index_col: list of column name
 
-    :param columns:list of columns name
+    :param columns: list of columns name
 
-    :param values:list of columns name
+    :param values: list of columns name
 
-    :param agg:string of aggfunction
+    :param agg: string of aggfunction
 
     :return: pivot table
     """
 
     pivot_table = pd.pivot_table(data, index=index_col, columns=columns, values=values, aggfunc=agg, margins=True)
     return pivot_table
 
@@ -265,35 +265,35 @@
         print("Not enough values to unpack ")
 
 
 def visualize_relationship_between_multiple_numeric_columns(data, numerical_columns: list):
     """
     Create a pair plot to visualize the relationship between multiple numeric columns.
     
-    :param data:variable
+    :param data: variable
     
-    :param numerical_columns:list of numerical column names
+    :param numerical_columns: list of numerical column names
     
-    :return:pair-plot chart
+    :return: pair-plot chart
     """
     sns.pairplot(data, vars=numerical_columns)
     plt.title("Relationship Between Columns")
     plt.show()
 
 
 def visualize_the_mean_by_categories_of_categorical_column(data, numerical_col: str, categorical_col: str):
     """
     Create a point plot to visualize the mean of a numerical column
     by the categories of a categorical column.
     
-    :param data:variable
+    :param data: variable
     
-    :param numerical_col:str
+    :param numerical_col: str
     
-    :param categorical_col:str
+    :param categorical_col: str
     
     :return: point plot chart
     """
     sns.pointplot(data, x=categorical_col, y=numerical_col)
     plt.ylabel(f"Average {numerical_col}")
     plt.show()
 
@@ -315,19 +315,19 @@
 
 
 def visualize_boxplot_of_numeric_column_by_categorical_col(data, categorical_col: str, numerical_col: str):
     """
     Create a box plot to visualize the distribution of a numeric column
     by the categories of a categorical column.
     
-    :param data:variable
+    :param data: variable
     
-    :param categorical_col:string with categorical column name
+    :param categorical_col: string with categorical column name
     
-    :param numerical_col:string with numerical column name
+    :param numerical_col: string with numerical column name
     
     :return: boxplot chart
     """
     sns.boxplot(data=data, x=categorical_col, y=numerical_col)
     plt.ylabel(f"{numerical_col}")
     plt.show()
 
@@ -351,64 +351,64 @@
     
 
 def visualize_numeric_column_by_the_categories_of_cat_col(data, categorical_colum: str, numerical_column: str):
     """
     Create a faceting grid to visualize the distribution of multiple numeric
     columns by the categories of a categorical column.
     
-    :param data:variable
+    :param data: variable
     
-    :param categorical_colum:str
+    :param categorical_colum: str
     
-    :param numerical_column:str
+    :param numerical_column: str
     
     :return: visualize chart
     """
     g = sns.FacetGrid(data, col=categorical_colum)
     g.map(plt.hist, numerical_column)
     plt.show()
 
 
 def scatter_plot_matrix_between_multiple_numeric_columns(data, numerical_columns: list):
     """
     Create a scatter plot matrix to visualize the relationship between
     multiple numeric columns.
     
-    :param data:variable
+    :param data: variable
     
-    :param numerical_columns:string with numerical column name
+    :param numerical_columns: string with numerical column name
     
     :return: scatter plot matrix
     """
     scatter_matrix(data[numerical_columns], alpha=0.2, figsize=(6, 6))
     plt.show()
 
 
 def visualize_heatmap(data):
     """
     Visualize the correlation between multiple numeric column.
     
-    :param data:variable
+    :param data: variable
     
-    :return: Heatmap 
+    :return: heatmap
     
     """
     numeric_features = data.select_dtypes(exclude="object")
     plt.figure(figsize=(12, 8))
     sns.heatmap(numeric_features.corr(), cmap="RdYlGn", annot=True)
     plt.show()
 
 
 def visualize_check_of_auto_correlation_in_numerical_col(data, numerical_colum: str):
     """
     Create a lag plot to check for auto correlation in a numeric column.
      
-    :param data:variable 
+    :param data: variable
     
-    :param numerical_colum:str
+    :param numerical_colum: str
     
     :return: auto correlation chart
     """
     lag_plot(data[numerical_colum])
     plt.show()
 
 
@@ -426,125 +426,125 @@
     plt.show()
 
 
 def regression_plot_between_two_numerical_col(data, numerical_column: str, numerical_col: str):
     """
     Visualize the relationship between two numeric column.
     
-    :param data:variable
+    :param data: variable
     
-    :param numerical_column:str
+    :param numerical_column: str
     
-    :param numerical_col:str
+    :param numerical_col: str
     
     :return: regression plot
     """
     sns.regplot(x=numerical_column, y=numerical_col, data=data)
     plt.show()
 
 
 def mean_confidence_interval_of_numeric_by_categories_col(data, categorical_col: str, numerical_col: str):
     """
     Visualize the mean and confidence interval of a numerical column by the categories of a categorical column.
     
-    :param data:variable
+    :param data: variable
     
-    :param categorical_col:str
+    :param categorical_col: str
     
     :param numerical_col: str
     
     :return: point plot 
     """
     sns.pointplot(x=categorical_col, y=numerical_col, data=data, errorbar=("ci", 95))
     plt.ylabel(f"Average {numerical_col}")
     plt.show()
 
 
 def visualize_relationship_by_two_numeric_and_categories_col(data, numeric_column: str, numeric_col: str, cat_col: str):
     """
     Visualize the relationship between two numeric column and the categories of a categorical column.
     
-    :param data:variable
+    :param data: variable
     
-    :param numeric_column:str
+    :param numeric_column: str
     
-    :param numeric_col:str
+    :param numeric_col: str
     
-    :param cat_col:str
+    :param cat_col: str
     
     :return: line plot 
     """
     sns.lmplot(data=data, x=numeric_column, y=numeric_col, hue=cat_col)
     plt.show()
 
 
 def boxen_plot_distribution_of_numeric_and_categories_col(data, num_col: str, cat_col: str):
     """
-    Visualize the distribution of a numerical column by the categories of a categorical column.
+    Visualize distribution of a numerical column by the categories of a categorical column.
 
-    :param data:variable
+    :param data: variable
 
-    :param num_col:str
+    :param num_col: str
 
-    :param cat_col:str
+    :param cat_col: str
 
     :return: boxen plot
     """
     sns.boxenplot(data=data, x=cat_col, y=num_col)
     plt.ylabel(f"{num_col}")
     plt.show()
 
 
 def visualize_distribution_of_numerical_column(data, numerical_col: str):
     """
     Create a histogram to visualize the distribution of numerical column.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_col:str
+    :param numerical_col: str
 
     :return: histogram chart
     """
     sns.histplot(data[numerical_col])
     plt.show()
 
 
 def kernel_density_estimate(data, numerical_col: str):
     """
     Create a kdeplot to visualize the kernel density estimate of a numerical column.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_col:str
+    :param numerical_col: str
 
-    :return:visualize kernel density estimate
+    :return: visualize kernel density estimate
     """
     sns.kdeplot(data[numerical_col])
     plt.show()
 
 
 def rugplot(data, numerical_col: str):
     """
     Create a rugplot to visualize the distribution of numerical column.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_col:str
+    :param numerical_col: str
 
     :return: rugplot distribution
     """
     sns.rugplot(data[numerical_col])
     plt.show()
 
 
 def visualize_joint_plot(data, numerical_column: str, num_column: str):
     """
     Visualize the relationship between two numerical column and their distribution.
 
-    :param data:variable
+    :param data: variable
 
     :param numerical_column: str
 
     :param num_column: str
 
     :return: joint chart
     """
@@ -601,19 +601,19 @@
 #                 ----------------  Analysis Functions  ----------------
 
 
 def calculate_the_skewness(data, numerical_colum: str) -> float:
     """
     Calculate skewness of a numerical column.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_colum:string
+    :param numerical_colum: string
 
-    :return:skewness value
+    :return: skewness value
 
     """
     skew = data[numerical_colum].skew()
     if skew == 0:
         print("Symmetric Column")
     elif skew > 0:
         print("Right Skewed ---> most values on the left")
@@ -622,19 +622,19 @@
     return skew
 
 
 def calculate_the_kurtosis(data, numerical_colum: str) -> float:
     """
     Calculate kurtosis of a numerical column.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_colum:
+    :param numerical_colum: str
 
-    :return:kurtosis value
+    :return: kurtosis value
 
     """
     kurt = data[numerical_colum].kurtosis()
     if kurt == 0:
         print("Mesokurtic ---> (Normal)")
     elif kurt > 0:
         print("Leptokurtic ---> (Thin)")
@@ -643,32 +643,32 @@
     return kurt
 
 
 def visualize_normal_probability_plot(data, numerical_column: str):
     """
     Visualize normal probability.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_column:string
+    :param numerical_column: string
 
     :return: probability chart
 
     """
     fig, ax = plt.subplots(1, 2, figsize=(12, 7))
     sns.histplot(data[numerical_column], kde=True, color="blue", ax=ax[0])
     sm.ProbPlot(data[numerical_column]).qqplot(line="s", ax=ax[1])
     plt.show()
 
 
 def display_summary_statistics(data, column_name: str):
     """
     Display statistical summary.
 
-    :param data:variable
+    :param data: variable
 
     :param column_name: string
 
     :return: statistical summary
     """
     print(data[column_name].describe())
```

### Comparing `pydataanalysis-0.0.3/diagnostic/pydiagnostic.py` & `pydataanalysis-0.0.4/diagnostic/pydiagnostic.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """
 
 
 def display_test_p_value(p_value: float):
     """
     Significance level of  0.05.
 
-    :param p_value:float
+    :param p_value: float
 
     :return: result of test
 
     """
     alpha = 0.05
     p_value = ceil(p_value)
     if p_value < alpha:
@@ -47,19 +47,19 @@
 
 def chi2_test(data, categorical_column: str, categorical_col: str) -> float:
     """
     Test two categorical column.
 
     sample question: does the proportion of male and female differ across age groups?
 
-    :param data:variable
+    :param data: variable
 
-    :param categorical_column:string
+    :param categorical_column: string
 
-    :param categorical_col:string
+    :param categorical_col: string
 
     :return: p-value
     """
 
     df_cont = pd.crosstab(data[categorical_column], data[categorical_col])
     observed_values = df_cont.values
     val = chi2_contingency(df_cont)
@@ -98,72 +98,72 @@
 
 def oneway_anova_test(data, numerical_column: str, categories_column: str) -> float:
     """
     Oneway anova test.
 
     sample question: is there difference in height between age group?
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_column:string
+    :param numerical_column: string
 
-    :param categories_column:string
+    :param categories_column: string
 
     :return: p_value
     """
     category_group_list = data.groupby(categories_column)[numerical_column].apply(list)
     fvalue, p_value = stats.f_oneway(*category_group_list)
     print(f"P-value of: {p_value}")
     return p_value
 
 
 def wilcoxon_rank_test(data, numerical_colum_before: str, numerical_column_after: str) -> float:
     """
     Wilcoxon test for dependent column.
 
-    :param data:variable
+    :param data: variable
 
-    :param numerical_colum_before:string
+    :param numerical_colum_before: string
 
-    :param numerical_column_after:string
+    :param numerical_column_after: string
 
-    :return:float p_value
+    :return: float p_value
     """
     w, p_value = wilcoxon(data[numerical_colum_before], data[numerical_column_after])
     print(f"P-value of: {p_value}")
     return p_value
 
 
-def test_relationship_between_numerical_columns(data, numeric_column: str, second_numerical_column: str) -> float:
+def test_relationship_between_two_numerical_columns(data, first_column: str, second_column: str) -> float:
     """
-    Perform a test to find the relationship of two numerical columns.
+    Relationship of two numerical column.
     
     sample question: is there relationship between height and weight?
     
-    :param data:variable
+    :param data: variable
     
-    :param numeric_column:str
+    :param first_column: str
     
-    :param second_numerical_column: str 
+    :param second_column: str 
     
     :return: float p_value
     """
-    pearson_coef, p_value = stats.pearsonr(data[numeric_column], data[second_numerical_column])
+    pearson_coef, p_value = stats.pearsonr(data[first_column], data[second_column])
     print(f"Pearson Correlation Coefficient {pearson_coef}, and a P-value of{p_value}")
     return p_value
 
 
 def compare_the_means_of_two_numerical_columns(data, first_numerical_col: str, second_numerical_col: str) -> float:
     """
     Perform a t_test to compare the means of two numeric column.
     
-    :param data:variable
+    :param data: variable
     
-    :param first_numerical_col:string with numerical column name
+    :param first_numerical_col: str
     
-    :param second_numerical_col:string with numerical column name
+    :param second_numerical_col: str
     
     :return: float p-value
     """
     t, p_value = ttest_ind(data[first_numerical_col], data[second_numerical_col])
     print(t, p_value)
     return p_value
```

### Comparing `pydataanalysis-0.0.3/predictive/pypredictive.py` & `pydataanalysis-0.0.4/predictive/pypredictive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from scipy.stats import chi2
 import statsmodels.api as sm
+from statsmodels.tsa.stattools import adfuller
 import matplotlib.pyplot as plt
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 from sklearn.feature_selection import chi2, mutual_info_regression
 import numpy as np
 import seaborn as sns
 from sklearn.linear_model import LinearRegression
@@ -37,19 +38,19 @@
 #                   ---------------  REGRESSION     ---------------
 
 
 def calculate_slope(data, independent_column: str, predicted_column: str) -> float:
     """
     Calculate slope.
 
-    :param data:variable
+    :param data: variable
 
-    :param independent_column:string
+    :param independent_column: string
 
-    :param predicted_column:string
+    :param predicted_column: string
 
     :return: slope value
     """
     if len(data[independent_column]) != len(data[predicted_column]):
         raise ValueError(f"length of {data[independent_column]} is not equal to length of{data[predicted_column]}")
     data[independent_column] = np.array(data[independent_column])
     data[predicted_column] = np.array(data[predicted_column])
@@ -63,19 +64,19 @@
     return np.round(slope, 4)
 
 
 def calculate_intercept_of_y(data, independent_column: str, predicted_column: str) -> float:
     """
     Calculate y - intercept.
 
-    :param data:variable
+    :param data: variable
 
-    :param independent_column:string
+    :param independent_column: string
 
-    :param predicted_column:string
+    :param predicted_column: string
 
     :return: y_intercept value
     """
     if len(data[independent_column]) != len(data[predicted_column]):
         raise ValueError(f"length of {data[independent_column]} is not equal to length of{data[predicted_column]}")
 
     n, slope = len(data[independent_column]), calculate_slope(data, independent_column, predicted_column)
@@ -86,19 +87,19 @@
     return np.round(y_intercept, 4)
 
 
 def plot_linear_equation(data, independent_column: str, predicted_column: str):
     """
     Visualize a linear equation.
 
-    :param data:variable
+    :param data: variable
 
-    :param independent_column:string
+    :param independent_column: string
 
-    :param predicted_column:string
+    :param predicted_column: string
 
     :return: scatter plot
 
     """
     slope = calculate_slope(data, independent_column, predicted_column)
     y_intercept = calculate_intercept_of_y(data, independent_column, predicted_column)
     data["predicted"] = data[independent_column].map(lambda x: slope * x + y_intercept)
@@ -107,40 +108,40 @@
     plt.show()
 
 
 def split_data_into_training_and_test(data, independent_colum: list, dependent_column: str):
     """
     Split data to training and test 80 % train and 20 % test.
 
-    :param data:variable
+    :param data: variable
 
-    :param independent_colum:list
+    :param independent_colum: list
 
-    :param dependent_column:string
+    :param dependent_column: string
 
     :return: dataframe
 
     """
     x = data[independent_colum]
     y = data[dependent_column]
     x_train, x_test, y_train, y_test = train_test_split(x, y, train_size=0.80, test_size=0.20, random_state=0)
     return x_train, x_test, y_train, y_test
 
 
 def plot_polynomial_regression(data, independent_colum, dependent_column, degree: int):
     """
     Visualize and display polynomial regression.
 
-    :param data:variable
+    :param data: variable
 
-    :param independent_colum:string
+    :param independent_colum: string
 
-    :param dependent_column:list
+    :param dependent_column: list
 
-    :param degree:integer
+    :param degree: integer
 
     :return: model
 
     """
     series = pd.Series(data[independent_colum])
     arr = series.values
     x = arr.reshape((-1, 1))
@@ -160,17 +161,17 @@
 
 def multi_linear_regression(data, independent_colum: list, dependent_column: str):
     """
     Implementing MLR, implement independent column as a list.
 
     :param data: variable
 
-    :param independent_colum:list
+    :param independent_colum: list
 
-    :param dependent_column:string
+    :param dependent_column: string
 
     :return: MLR & printing out the intercept_, coef_, R2(coefficient of determination)
 
     """
     x = data[independent_colum]
     y = data[dependent_column]
     model = LinearRegression().fit(x, y)
@@ -251,116 +252,163 @@
 
     """
     data = data.set_index(date_column)
     set_index_data = pd.to_datetime(data.index, infer_datetime_format=True)
     return set_index_data
 
 
-def create_date_range(start_date: str, end_date: str):
+def test_stationarity(timeseries):
+    """
+
+    Plot rolling statistics.
+
+    Perform dickey-fuller test.
+
+    :param timeseries: variable
+    :return: dickey-fuller test
+
+    """
+    moving_average = timeseries.rolling(window=12).mean()
+    moving_std = timeseries.rolling(window=12).std()
+
+    plt.plot(timeseries, color="blue", label="Original")
+    plt.plot(moving_average, color="red", label="Rolling Mean")
+    plt.plot(moving_std, color="black", label="Rolling STD")
+    plt.legend(loc="best")
+    plt.title("Rolling Mean & Standard Deviation")
+    plt.show()
+
+    print("Results of Dickey-Fuller Test:")
+    dftest = adfuller(timeseries.values, autolag="AIC")
+    dfoutput = pd.Series(dftest[0:4], index=["Test Statistic", "p-value", "#Lags Used", "Number of Observations Used"])
+    for key, value in dftest[4].items():
+        dfoutput["Critical Value (%s)" % key] = value
+    print(dfoutput)
+
+
+def create_date_range(start_date: str, end_date: str, freq: str):
     """
     Create date range.
 
     :param start_date: str
 
     :param end_date: str
 
+    :param freq: str
+
     :return: dataframe
     """
-    data_sequence = pd.date_range(start=start_date, end=end_date)
+    data_sequence = pd.date_range(start=start_date, end=end_date, freq=freq)
     return data_sequence
 
 
 def create_date_features(data, date_column: str):
     """
     Create date features.
 
-    :param data: data variable
+    :param data: variable
 
     :param date_column: string
 
     :return: dataframe with date features
     """
-    df = data.set_index[date_column]
-    df[date_column] = pd.to_datetime(df[date_column], format="%Y-%m-%d", errors="coerce", infer_datetime_format=True)
-    df["dayOfWeek"] = df.index.dayofweek
-    df["Quarter"] = df.index.quarter
-    df["Month"] = df.index.month
-    df["Year"] = df.index.year
-    df["dayOfYear"] = df.index.dayofyear
-    return df
+    data[date_column] = pd.to_datetime(data[date_column], format="%Y-%m-%d", errors="coerce",
+                                       infer_datetime_format=True)
+    data["dayOfWeek"] = data[date_column].dt.dayofweek
+    data["Quarter"] = data[date_column].dt.quarter
+    data["Month"] = data[date_column].dt.month
+    data["Year"] = data[date_column].dt.year
+    data["dayOfYear"] = data[date_column].dt.dayofyear
+    return data
 
 
 def create_hourly_feature(data, date_column: str):
     """
     Create hourly feature.
 
     :param data: data variable
 
     :param date_column: string
 
     :return: dataframe
     """
-    df = data.set_index[date_column]
-    df[date_column] = pd.to_datetime(df[date_column], format="%Y-%m-%d %H:%M:%S", errors="coerce",
-                                     infer_datetime_format=True)
-    df["hour"] = df.index.hour
-    return df
-
-
-def seasonal_plot(x, y, period, freq, ax=None):
-    """
-    X = tunnel.copy()
-
-    # days within a week
-    X["day"] = X.index.dayofweek  # the x-axis (freq)
-    X["week"] = X.index.week  # the seasonal period (period)
-
-    # days within a year
-    X["dayofyear"] = X.index.dayofyear
-    X["year"] = X.index.year
-    fig, (ax0, ax1) = plt.subplots(2, 1, figsize=(11, 6))
-    seasonal_plot(X, y="NumVehicles", period="week", freq="day", ax=ax0)
-    seasonal_plot(X, y="NumVehicles", period="year", freq="dayofyear", ax=ax1);
+    data[date_column] = pd.to_datetime(data[date_column], format="%Y-%m-%d %H:%M:%S", errors="coerce",
+                                       infer_datetime_format=True)
+    data["hour"] = data[date_column].dt.hour
+    return data
+
+
+def seasonal_plot(data, column_name: str, period_column: str, freq: str, ax=None):
+    """
+    Seasonal plot.
+
+    example:
+    seasonal_plot(data, "passengers_column", period_column="Year", freq="dayOfYear")
+
+    :param data: variable
+
+    :param column_name: str
+
+    :param period_column: str
+
+    :param freq: str
+
+    :param ax: None
+
+    :return: chart
     """
     if ax is None:
         _, ax = plt.subplots()
-    palette = sns.color_palette("husl", n_colors=x[period].nunique(), )
+    palette = sns.color_palette("husl", n_colors=data[period_column].nunique())
     ax = sns.lineplot(
         x=freq,
-        y=y,
-        hue=period,
-        data=x,
-        ci=False,
+        y=column_name,
+        hue=period_column,
+        data=data,
+        errorbar=("ci", False),
         ax=ax,
         palette=palette,
         legend=False,
     )
-    ax.set_title(f"Seasonal Plot ({period}/{freq})")
-    for line, name in zip(ax.lines, x[period].unique()):
+    ax.set_title(f"Seasonal Plot ({period_column}/{freq})")
+    for line, name in zip(ax.lines, data[period_column].unique()):
         y_ = line.get_ydata()[-1]
         ax.annotate(
             name,
             xy=(1, y_),
             xytext=(6, 0),
             color=line.get_color(),
             xycoords=ax.get_yaxis_transform(),
             textcoords="offset points",
             size=14,
             va="center",
         )
-    return ax
+    plt.show()
 
 
-def plot_periodogram(ts, detrend='linear', ax=None):
+def plot_periodogram(data, column_name: str, detrend='linear', ax=None):
     """
-    Plot_periodogram(tunnel.NumVehicles)
+    Periodogram plot.
+
+    example:
+    plot_periodogram(data, "column_name")
+
+    :param data: variable
+
+    :param column_name: str
+
+    :param detrend: 'linear'
+
+    :param ax: None
+
+    :return: chart
     """
     fs = pd.Timedelta("1Y") / pd.Timedelta("1D")
     freqencies, spectrum = periodogram(
-        ts,
+        data[column_name],
         fs=fs,
         detrend=detrend,
         window="boxcar",
         scaling='spectrum',
     )
     if ax is None:
         _, ax = plt.subplots()
@@ -379,15 +427,15 @@
             "Semiweekly (104)",
         ],
         rotation=30,
     )
     ax.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
     ax.set_ylabel("Variance")
     ax.set_title("Periodogram")
-    return ax
+    plt.show()
 
 
 #                   ---------------  Classification     ---------------
 def chi_value_plot(data):
     """
     Plot the variable importance by ch2 for binary classification.
```

### Comparing `pydataanalysis-0.0.3/prescriptive/pyprescriptive.py` & `pydataanalysis-0.0.4/prescriptive/pyprescriptive.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from sklearn.metrics import precision_score, recall_score, f1_score
 
 
 def visualize_confusion_matrix(y_test, y_predict):
     """
     Visualization.
     
-    :param y_test:variable 
+    :param y_test: variable
     
-    :param y_predict:variable 
+    :param y_predict: variable
     
     :return:chart 
     
     """
     confusion_matrix_ = confusion_matrix(y_test, y_predict)
     cm_display = ConfusionMatrixDisplay(confusion_matrix=confusion_matrix_, display_labels=[False, True])
     cm_display.plot()
@@ -30,15 +30,15 @@
     """
     Plot roc curve.
 
     :param true_y: variable
 
     :param y_prob: variable
 
-    :return:AUC score and chart
+    :return: AUC score and chart
     """
     fpr, tpr, thresholds = roc_curve(true_y, y_prob)
     plt.plot(fpr, tpr)
     plt.xlabel("False Positive Rate")
     plt.ylabel("True Positive Rate")
     plt.show()
     print(f"AUC score: {roc_auc_score(true_y, y_prob)}")
```

### Comparing `pydataanalysis-0.0.3/pydataanalysis.egg-info/PKG-INFO` & `pydataanalysis-0.0.4/pydataanalysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydataanalysis
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Analysis and  Visualization Functions
 Home-page: UNKNOWN
 Author: Tamer Samara
 Author-email: tamer.samara@gmail.com
 License: MIT
 Description: <h1>Data Analysis CheatSheet (everything you might need )</h1>
         <p>
```

### Comparing `pydataanalysis-0.0.3/setup.py` & `pydataanalysis-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Data Analysis and  Visualization Functions'
 LONG_DESCRIPTION = 'The modules include functions that might be useful in general cases for data analysis ' \
                    'and data visualization. '
 
 # Setting up
 setup(
     name="pydataanalysis",
```

