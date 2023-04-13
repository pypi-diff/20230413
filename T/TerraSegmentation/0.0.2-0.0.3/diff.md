# Comparing `tmp/TerraSegmentation-0.0.2.tar.gz` & `tmp/TerraSegmentation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentation-0.0.1\TerraSegmentation-0.0.1\dist\.tmp-iqjvfrmx\TerraSegmentation-0.0.2.tar", last modified: Thu Apr 13 06:30:01 2023, max compression
+gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentation-0.0.1\TerraSegmentation-0.0.1\dist\.tmp-4i0uezf1\TerraSegmentation-0.0.3.tar", last modified: Thu Apr 13 06:53:28 2023, max compression
```

## Comparing `TerraSegmentation-0.0.2.tar` & `TerraSegmentation-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/
--rw-rw-rw-   0        0        0      134 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation/
--rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentation-0.0.2/TerraSegmentation/TerraMaskrcnnDemo.py
--rw-rw-rw-   0        0        0    50401 2023-04-13 06:29:20.000000 TerraSegmentation-0.0.2/TerraSegmentation/TerraSegmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/
--rw-rw-rw-   0        0        0      134 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      235 2023-04-13 06:29:30.000000 TerraSegmentation-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/
+-rw-rw-rw-   0        0        0      134 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation/
+-rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentation-0.0.3/TerraSegmentation/TerraMaskrcnnDemo.py
+-rw-rw-rw-   0        0        0    50300 2023-04-13 06:52:53.000000 TerraSegmentation-0.0.3/TerraSegmentation/TerraSegmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/TerraSegmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:53:28.000000 TerraSegmentation-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      235 2023-04-13 06:53:04.000000 TerraSegmentation-0.0.3/setup.py
```

### Comparing `TerraSegmentation-0.0.2/TerraSegmentation/TerraMaskrcnnDemo.py` & `TerraSegmentation-0.0.3/TerraSegmentation/TerraMaskrcnnDemo.py`

 * *Files identical despite different names*

### Comparing `TerraSegmentation-0.0.2/TerraSegmentation/TerraSegmentation.py` & `TerraSegmentation-0.0.3/TerraSegmentation/TerraSegmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -818,29 +818,29 @@
   # обучаем                                
   history = model.fit(x_train, y_train,
                         epochs=epochs, batch_size=batch_size,
                          validation_data=(x_val, y_val),callbacks=reduce_lr) 
 
   # выводим график обучения                                          
   plt.figure(figsize=(10, 5))
-  plt.plot(history.history['sparse_categorical_accuracy'])                                                              
-  plt.plot(history.history['val_sparse_categorical_accuracy'])
+  plt.plot(history.history['dice_coef'])                                                              
+  plt.plot(history.history['val_dice_coef'])
   plt.show()
 
   # оцениваем на тестовой выборке
-  accuracy = model.evaluate(x_test,y_test, verbose=0)[1]                                                                
+  acc = model.evaluate(x_test,y_test, verbose=0)[1]                                                                
  
-  print(f'Средняя точность модели на тестовой выборке: {accuracy}')
+  print(f'Средняя точность модели на тестовой выборке: {  }')
 
   # рисуем случайные картинки из предикта
   process_images(model, class_list,x_test, y_test,3)                                                                     
   
   # сохраняем параметры модели и обучения для итоговой статистики
-  parameters_list = ['filters', 'kernel','pool_size','num_layers','batch_size', 'accuracy']                              
-  values_list = [(parameters[0]),(parameters[1]),(parameters[2]), (parameters[3]),(batch_size),accuracy]
+  parameters_list = ['filters', 'kernel','pool_size','num_layers','batch_size', 'dice_coef']                              
+  values_list = [(parameters[0]),(parameters[1]),(parameters[2]), (parameters[3]),(batch_size),  ]
   model_list = [model.name]
 
   result_table = pd.DataFrame(values_list).T
   result_table.columns = parameters_list
   result_table.index = model_list
   result_table[['filters', 'pool_size','num_layers','batch_size']] = result_table[['filters', 'pool_size','num_layers','batch_size']].astype(int)
   
@@ -859,15 +859,15 @@
   best = np.argsort(accuracy_list)[-5:].tolist()
   process_images_1(model, class_list, 3,x_test, y_test, best, bad)
 # финальная таблица результатов после обучения нескольких вариантов архитектур модели
 def final_result(*result_tabels):    
   print('Итоговая таблица результатов')
   df = pd.concat([*result_tabels])
   
-  return df.style.background_gradient(subset='accuracy')
+  return df.style.background_gradient(subset='dice_coef')
   
 def enter_parameters_PSP(x_data, y_data, class_list):
 
   '''Получение списка параметров модели PSPnet '''                
   
   filters = int(input('Число фильтров в каждом слое сверточного блока (filters):  '.ljust(62)))
   kernel = input('Размер ядра свертки(kernel):  '.ljust(62)) 
@@ -1028,28 +1028,28 @@
   # обучаем
   history = model.fit(x_train, y_train,                                                                                
                         epochs=epochs, batch_size=batch_size,
                          validation_data=(x_val, y_val),callbacks=reduce_lr)
   
   # выводим график обучения
   plt.figure(figsize=(10, 5))                                                                
-  plt.plot(history.history['sparse_categorical_accuracy'])
-  plt.plot(history.history['val_sparse_categorical_accuracy'])
+  plt.plot(history.history['dice_coef'])
+  plt.plot(history.history['val_dice_coef'])
   plt.show()                                                                                                            
  
   # оцениваем на тестовой выборке
-  accuracy = model.evaluate(x_test,y_test, verbose=0)[1]                                                               
+  acc = model.evaluate(x_test,y_test, verbose=0)[1]                                                               
  
-  print(f'Средняя точность модели на тестовой выборке: {accuracy}')
+  print(f'Средняя точность модели на тестовой выборке: {acc}')
 
   # рисуем случайные картитнки
   process_images(model, class_list,x_test, y_test,3)                                                                   
   
-  parameters_list = ['filters', 'kernel', 'pool_number','conv_number','batch_size', 'accuracy']
-  values_list = [parameters[0],parameters[1],parameters[2], parameters[3],batch_size,accuracy]
+  parameters_list = ['filters', 'kernel', 'pool_number','conv_number','batch_size', 'dice_coef']
+  values_list = [parameters[0],parameters[1],parameters[2], parameters[3],batch_size,acc]
   model_list = [model.name]
   
   # сохраняем параметры модели и обучения в таблицу
   result_table = pd.DataFrame(values_list).T                                                                            
   result_table.columns = parameters_list
   result_table.index = model_list
   result_table[['filters', 'pool_number','conv_number','batch_size']] = result_table[['filters','pool_number','conv_number','batch_size']].astype(int)
```

