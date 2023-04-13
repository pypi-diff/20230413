# Comparing `tmp/TerraSegmentation-0.0.1.tar.gz` & `tmp/TerraSegmentation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerraSegmentation-0.0.1.tar", last modified: Mon Feb  6 17:50:16 2023, max compression
+gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentation-0.0.1\TerraSegmentation-0.0.1\dist\.tmp-iqjvfrmx\TerraSegmentation-0.0.2.tar", last modified: Thu Apr 13 06:30:01 2023, max compression
```

## Comparing `TerraSegmentation-0.0.1.tar` & `TerraSegmentation-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 17:50:16.049198 TerraSegmentation-0.0.1/
--rw-rw-rw-   0        0        0      134 2023-02-06 17:50:16.049198 TerraSegmentation-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-06 17:50:16.011152 TerraSegmentation-0.0.1/TerraSegmentation/
--rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentation-0.0.1/TerraSegmentation/TerraMaskrcnnDemo.py
--rw-rw-rw-   0        0        0    50134 2023-02-06 17:46:16.000000 TerraSegmentation-0.0.1/TerraSegmentation/TerraSegmentation.py
-drwxrwxrwx   0        0        0        0 2023-02-06 17:50:16.048173 TerraSegmentation-0.0.1/TerraSegmentation.egg-info/
--rw-rw-rw-   0        0        0      134 2023-02-06 17:50:15.000000 TerraSegmentation-0.0.1/TerraSegmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-02-06 17:50:15.000000 TerraSegmentation-0.0.1/TerraSegmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 17:50:15.000000 TerraSegmentation-0.0.1/TerraSegmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-02-06 17:50:15.000000 TerraSegmentation-0.0.1/TerraSegmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-06 17:50:16.049198 TerraSegmentation-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      235 2023-02-06 17:48:32.000000 TerraSegmentation-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/
+-rw-rw-rw-   0        0        0      134 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation/
+-rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentation-0.0.2/TerraSegmentation/TerraMaskrcnnDemo.py
+-rw-rw-rw-   0        0        0    50401 2023-04-13 06:29:20.000000 TerraSegmentation-0.0.2/TerraSegmentation/TerraSegmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/TerraSegmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:30:01.000000 TerraSegmentation-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      235 2023-04-13 06:29:30.000000 TerraSegmentation-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `TerraSegmentation-0.0.1/TerraSegmentation/TerraMaskrcnnDemo.py` & `TerraSegmentation-0.0.2/TerraSegmentation/TerraMaskrcnnDemo.py`

 * *Files identical despite different names*

### Comparing `TerraSegmentation-0.0.1/TerraSegmentation/TerraSegmentation.py` & `TerraSegmentation-0.0.2/TerraSegmentation/TerraSegmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 # Инструменты для работы с массивами
 import numpy as np 
 
 #для создания таблиц
 import pandas as pd
 
+from tensorflow.keras import backend as K
+
 # Системные инструменты
 import time, random, gdown, os
 
 # Дополнительные инструменты для работы с изображениями
 from PIL import Image
 
 # работа с регулярными выражениями
@@ -39,15 +41,17 @@
 import seaborn as sns
 sns.set_style('darkgrid')
 
 # игнорировать предупреждения
 import warnings
 warnings.filterwarnings('ignore')
 
-
+def dice_coef(y_true, y_pred):
+    return (2. * K.sum(y_true * y_pred) + 1.) / (K.sum(y_true) + K.sum(y_pred) + 1.) # Возвращаем площадь пересечения деленную на площадь объединения двух областей
+	
 def load_images(folder, subset1, subset2, IMG_WIDTH, IMG_HEIGHT):
   ''' Функция загрузки изображений.
   
   folder, subset1, subset2 - каталог и подкаталоги с файлами оригинальных 
   
   и сегментированных изображений
   
@@ -640,15 +644,15 @@
         output = Conv2D(class_count, (3, 3), activation='softmax', padding='same')(x)
       
               
         model = Model(input_image, output,
                       name = model_name)
         model.compile(optimizer=Adam(learning_rate=1e-4),
                   loss='sparse_categorical_crossentropy',
-                  metrics=['sparse_categorical_accuracy'])
+                  metrics=[dice_coef])
 
         return model
 def get_model_Unet(x_data, y_data, class_list, parameters_dict = None):
   
   '''Создание модели и фиксация ее параметров ''' 
 
   # если берем параметры из словаря
@@ -963,15 +967,15 @@
 
   output = Conv2D(class_count, (3, 3), activation='softmax', padding='same')(x)
   
           
   model = Model(img_input, output, name = model_name)
   model.compile(optimizer=Adam(learning_rate=1e-4),
                   loss='sparse_categorical_crossentropy',
-                  metrics=['sparse_categorical_accuracy'])
+                  metrics=[dice_coef])
   return model
 
   
   
 
 def get_model_PSP(x_data, y_data,class_list, parameters_dict = None):
   ''' Получение модели PSPnet с заданными параметрами '''
```

