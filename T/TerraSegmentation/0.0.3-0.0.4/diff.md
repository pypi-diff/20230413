# Comparing `tmp/TerraSegmentation-0.0.3.tar.gz` & `tmp/TerraSegmentation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentation-0.0.1\TerraSegmentation-0.0.1\dist\.tmp-4i0uezf1\TerraSegmentation-0.0.3.tar", last modified: Thu Apr 13 06:53:28 2023, max compression
+gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentation-0.0.1\TerraSegmentation-0.0.1\dist\.tmp-673aezm4\TerraSegmentation-0.0.4.tar", last modified: Thu Apr 13 07:03:00 2023, max compression
```

## Comparing `TerraSegmentation-0.0.3.tar` & `TerraSegmentation-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/
--rw-rw-rw-   0        0        0      134 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation/
--rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentation-0.0.3/TerraSegmentation/TerraMaskrcnnDemo.py
--rw-rw-rw-   0        0        0    50300 2023-04-13 06:52:53.000000 TerraSegmentation-0.0.3/TerraSegmentation/TerraSegmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/
--rw-rw-rw-   0        0        0      134 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      235 2023-04-13 06:53:04.000000 TerraSegmentation-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/
+-rw-rw-rw-   0        0        0      134 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation/
+-rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentation-0.0.4/TerraSegmentation/TerraMaskrcnnDemo.py
+-rw-rw-rw-   0        0        0    50302 2023-04-13 07:02:23.000000 TerraSegmentation-0.0.4/TerraSegmentation/TerraSegmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      235 2023-04-13 07:02:34.000000 TerraSegmentation-0.0.4/setup.py
```

### Comparing `TerraSegmentation-0.0.3/TerraSegmentation/TerraMaskrcnnDemo.py` & `TerraSegmentation-0.0.4/TerraSegmentation/TerraMaskrcnnDemo.py`

 * *Files identical despite different names*

### Comparing `TerraSegmentation-0.0.3/TerraSegmentation/TerraSegmentation.py` & `TerraSegmentation-0.0.4/TerraSegmentation/TerraSegmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -825,22 +825,22 @@
   plt.plot(history.history['dice_coef'])                                                              
   plt.plot(history.history['val_dice_coef'])
   plt.show()
 
   # оцениваем на тестовой выборке
   acc = model.evaluate(x_test,y_test, verbose=0)[1]                                                                
  
-  print(f'Средняя точность модели на тестовой выборке: {  }')
+  print(f'Средняя точность модели на тестовой выборке: {acc}')
 
   # рисуем случайные картинки из предикта
   process_images(model, class_list,x_test, y_test,3)                                                                     
   
   # сохраняем параметры модели и обучения для итоговой статистики
   parameters_list = ['filters', 'kernel','pool_size','num_layers','batch_size', 'dice_coef']                              
-  values_list = [(parameters[0]),(parameters[1]),(parameters[2]), (parameters[3]),(batch_size),  ]
+  values_list = [(parameters[0]),(parameters[1]),(parameters[2]), (parameters[3]),(batch_size),acc]
   model_list = [model.name]
 
   result_table = pd.DataFrame(values_list).T
   result_table.columns = parameters_list
   result_table.index = model_list
   result_table[['filters', 'pool_size','num_layers','batch_size']] = result_table[['filters', 'pool_size','num_layers','batch_size']].astype(int)
```

