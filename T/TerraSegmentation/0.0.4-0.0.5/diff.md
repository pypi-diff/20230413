# Comparing `tmp/TerraSegmentation-0.0.4.tar.gz` & `tmp/TerraSegmentation-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentation-0.0.1\TerraSegmentation-0.0.1\dist\.tmp-673aezm4\TerraSegmentation-0.0.4.tar", last modified: Thu Apr 13 07:03:00 2023, max compression
+gzip compressed data, was "C:\Users\Serega\Downloads\TerraSegmentation-0.0.1\TerraSegmentation-0.0.1\dist\.tmp-582vir3v\TerraSegmentation-0.0.5.tar", last modified: Thu Apr 13 11:03:21 2023, max compression
```

## Comparing `TerraSegmentation-0.0.4.tar` & `TerraSegmentation-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/
--rw-rw-rw-   0        0        0      134 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation/
--rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentation-0.0.4/TerraSegmentation/TerraMaskrcnnDemo.py
--rw-rw-rw-   0        0        0    50302 2023-04-13 07:02:23.000000 TerraSegmentation-0.0.4/TerraSegmentation/TerraSegmentation.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/
--rw-rw-rw-   0        0        0      134 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/TerraSegmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 07:03:00.000000 TerraSegmentation-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      235 2023-04-13 07:02:34.000000 TerraSegmentation-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/
+-rw-rw-rw-   0        0        0      134 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/TerraSegmentation/
+-rw-rw-rw-   0        0        0    12420 2023-02-06 17:46:17.000000 TerraSegmentation-0.0.5/TerraSegmentation/TerraMaskrcnnDemo.py
+-rw-rw-rw-   0        0        0    50336 2023-04-13 11:01:49.000000 TerraSegmentation-0.0.5/TerraSegmentation/TerraSegmentation.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/TerraSegmentation.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/TerraSegmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/TerraSegmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/TerraSegmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/TerraSegmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:03:21.000000 TerraSegmentation-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      235 2023-04-13 11:02:49.000000 TerraSegmentation-0.0.5/setup.py
```

### Comparing `TerraSegmentation-0.0.4/TerraSegmentation/TerraMaskrcnnDemo.py` & `TerraSegmentation-0.0.5/TerraSegmentation/TerraMaskrcnnDemo.py`

 * *Files identical despite different names*

### Comparing `TerraSegmentation-0.0.4/TerraSegmentation/TerraSegmentation.py` & `TerraSegmentation-0.0.5/TerraSegmentation/TerraSegmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
 # игнорировать предупреждения
 import warnings
 warnings.filterwarnings('ignore')
 
 def dice_coef(y_true, y_pred):
     return (2. * K.sum(y_true * y_pred) + 1.) / (K.sum(y_true) + K.sum(y_pred) + 1.) # Возвращаем площадь пересечения деленную на площадь объединения двух областей
+
+
+
 	
 def load_images(folder, subset1, subset2, IMG_WIDTH, IMG_HEIGHT):
   ''' Функция загрузки изображений.
   
   folder, subset1, subset2 - каталог и подкаталоги с файлами оригинальных 
   
   и сегментированных изображений
@@ -84,15 +87,15 @@
   for filename in sorted(os.listdir(f'{folder}/{subset2}')):
     mask_format_list.append(os.path.splitext(filename)[1] )
     mask = image.load_img(os.path.join(f'{folder}/{subset2}', filename),target_size= (IMG_HEIGHT,IMG_WIDTH))
     mask_list.append(mask)
   
   if len(set(mask_format_list)) > 1:
     
-    print(f'NB!В каталоге{subset2} есть файлы с разными расширениями!')
+    print(f'NB!В каталоге {subset2} есть файлы с разными расширениями!')
   
   print(f'Выборка {subset2} загружена, количество изображений: {len(mask_list)}')
  
   
   return image_list, mask_list 
 
 
@@ -331,14 +334,15 @@
   for img in data_list:
     x = np.array(img)                
     x_data.append(x)
   x_data = np.array(x_data)
 
   #в сегментированных сначала меняем значения на метки и тоже преаращаем в массив
   y_data = rgb_to_label(mask_list, new_color_list, extra_color_list,pixel_problem, IMG_HEIGHT, IMG_WIDTH) 
+  y_data = utils.to_categorical(y_data, len(new_color_list))
 
   return x_data, y_data
 # Функция для просмотра изображений из набора
 
 def show_imageset(image_list, mask_list, n):
                   
     '''Функция для просмотра изображений из набора.
@@ -472,15 +476,15 @@
           # если значение равно какому либо из вложенных, меняем на новый индекс этой смеси
           y[np.where(np.all(sample == mix_list_idx[j][k], axis = -1))] = joint_list_idx.index(mix_list_idx[j]) 
 
       
       
       y_data_mix.append(y)
   
-  return np.array(y_data_mix), joint_color_list
+  return utils.to_categorical(np.array(y_data_mix), len(joint_color_list)), joint_color_list
 def split_images(x_data, y_data, num_tiles):
   '''Разбиение изображений на части и формирование новых выборок x_data, y_data.
 
   x_data, y_data - исходные выборки
 
   num_tiles - необходимое количество частей каждой картинки (4, 16 ...
 
@@ -512,15 +516,14 @@
     color_list - список цветов
 
     y_test, x_test - тестовые выборки
 
     Возвращает массив трехканальных изображений, где на месте метки стоят значения пикселей этого цвета
 
     '''
-
     result = []
 
     # Для всех картинок в списке:
     for y in mask_list:
         # Создание пустой цветной картики
         temp = np.zeros(( x_test.shape[1],x_test.shape[2], 3), dtype='uint8')
         
@@ -643,15 +646,15 @@
         
         output = Conv2D(class_count, (3, 3), activation='softmax', padding='same')(x)
       
               
         model = Model(input_image, output,
                       name = model_name)
         model.compile(optimizer=Adam(learning_rate=1e-4),
-                  loss='sparse_categorical_crossentropy',
+                  loss='categorical_crossentropy',
                   metrics=[dice_coef])
 
         return model
 def get_model_Unet(x_data, y_data, class_list, parameters_dict = None):
   
   '''Создание модели и фиксация ее параметров ''' 
 
@@ -716,15 +719,15 @@
         # Отображение на графике в первой линии предсказания модели
         axs[0, 0].set_title('Результат работы модели - случайные изображения:')
         axs[0, i].imshow(orig[i])
         axs[0, i].axis('off')
 
         # Отображение на графике во второй линии сегментированного изображения из y_test
         axs[1, 0].set_title('Оригинальное сегментированное')
-        axs[1, i].imshow(labels_to_rgb(y_test[indexes], color_list,x_test, y_test)[i])
+        axs[1, i].imshow(labels_to_rgb(np.argmax(y_test[indexes], axis=-1)[..., None], color_list, x_test, y_test)[i])       
         axs[1 ,i].axis('off')
 
         # Отображение на графике в третьей линии оригинального изображения
         axs[2, 0].set_title('Оригинальное изображение')
         axs[2, i].imshow(x_test[indexes[i]])
         axs[2 ,i].axis('off')
 
@@ -766,52 +769,48 @@
     for i in range(count):
         # Отображение на графике в первой линии предсказания модели
         axs[0, 0].set_title('Результат работы модели - лучшие изображения:')
         axs[0, i].imshow(orig_best[i])
         axs[0, i].axis('off')
 
         axs[1, 0].set_title('Оригинальное сегментированное')
-        axs[1, i].imshow(labels_to_rgb(y_test[indexes_best], color_list, x_test, y_test)[i])
+        axs[1, i].imshow(labels_to_rgb(np.argmax(y_test[indexes_best], axis=-1)[..., None], color_list, x_test, y_test)[i])
         axs[1 ,i].axis('off')
 
         axs[2, 0].set_title('Оригинальное изображение')
         axs[2, i].imshow(x_test[indexes_best[i]])
         axs[2 ,i].axis('off')
 
         axs[3, 0].set_title('Результат работы модели -худшие изображения:')
         axs[3, i].imshow(orig_bad[i])
         axs[3, i].axis('off')
 
         # Отображение на графике во второй линии сегментированного изображения из y_test
         axs[4, 0].set_title('Оригинальное сегментированное')
-        axs[4, i].imshow(labels_to_rgb(y_test[indexes_bad], color_list, x_test, y_test)[i])
+        axs[4, i].imshow(labels_to_rgb(np.argmax(y_test[indexes_bad], axis=-1)[..., None], color_list, x_test, y_test)[i])
         axs[4 ,i].axis('off')
 
         # Отображение на графике в третьей линии оригинального изображения
         axs[5, 0].set_title('Оригинальное изображение')
         axs[5, i].imshow(x_test[indexes_bad[i]])
         axs[5 ,i].axis('off')
 
     plt.show() 
-def train_eval_modelUnet(model, parameters, x_data, y_data, class_list): # обучение и оценка модели
+def train_eval_modelUnet(model, parameters, x_data, y_data, batch_size, epochs, class_list): # обучение и оценка модели
 
   '''Обучение и оценка модели
 
   model, parameters - модель с заданными параметрами
 
   x_data, y_data - выборки для обучения
 
   class_list - список классов(цветов)
 
   '''
                            
-                
-  # вводим параметры обучения           
-  batch_size = int(input('Размер батча: '))                             
-  epochs = int(input('Количество эпох: '))
 
   # формируем тренировочную, валидационную и тестовую выборки
   x_train,x_val, y_train, y_val = train_test_split(x_data, y_data, test_size = 0.2, shuffle = True, random_state = 6) 
   x_train,x_test, y_train, y_test = train_test_split(x_train, y_train, test_size = 0.1, shuffle = True, random_state = 6)
 
   reduce_lr = ReduceLROnPlateau(monitor='val_loss', factor=0.6, patience=5, verbose=0) 
 
@@ -854,18 +853,25 @@
   x_train,x_test, y_train, y_test = train_test_split(x_train, y_train, test_size = 0.1, shuffle = True, random_state = 6)
   accuracy_list = np.array([model.evaluate(x_test[i:i+1], 
                                          y_test[i:i+1],
                                          verbose=0)[1] for i in range(x_test.shape[0])])
   bad = np.argsort(accuracy_list)[:5].tolist()
   best = np.argsort(accuracy_list)[-5:].tolist()
   process_images_1(model, class_list, 3,x_test, y_test, best, bad)
-# финальная таблица результатов после обучения нескольких вариантов архитектур модели
+
+  # финальная таблица результатов после обучения нескольких вариантов архитектур модели
 def final_result(*result_tabels):    
   print('Итоговая таблица результатов')
   df = pd.concat([*result_tabels])
+  df.fillna(0, inplace=True)
+  dtype_dict = {col: int for col in df.columns if col not in ['kernel', 'dice_coef']}
+
+  # преобразуем типы данных в DataFrame
+  df = df.astype(dtype_dict)
+
   
   return df.style.background_gradient(subset='dice_coef')
   
 def enter_parameters_PSP(x_data, y_data, class_list):
 
   '''Получение списка параметров модели PSPnet '''                
   
@@ -966,15 +972,15 @@
   x, _ = conv_block_PSP(x,filters, kernel)                   
 
   output = Conv2D(class_count, (3, 3), activation='softmax', padding='same')(x)
   
           
   model = Model(img_input, output, name = model_name)
   model.compile(optimizer=Adam(learning_rate=1e-4),
-                  loss='sparse_categorical_crossentropy',
+                  loss='categorical_crossentropy',
                   metrics=[dice_coef])
   return model
 
   
   
 
 def get_model_PSP(x_data, y_data,class_list, parameters_dict = None):
@@ -1007,22 +1013,18 @@
     # выполняется функция enter_parameters_PSP
     parameters = enter_parameters_PSP(x_data, y_data, class_list)
 
   # создаем модель
   model = create_PSPnet(*parameters)
 
   return model, parameters
-def train_eval_modelPSP(model, parameters, x_data, y_data, class_list): 
+def train_eval_modelPSP(model, parameters, x_data, y_data, batch_size, epochs, class_list): 
   '''Обучение и оценка модели '''
                 
                 
-  # вводим параметры обучения                         
-  batch_size = int(input('Размер батча: '))
-  epochs = int(input('Количество эпох: '))
-
   # делим данные на тренировочную, проверочную и тестовую выборки
   x_train,x_val, y_train, y_val = train_test_split(x_data, y_data, test_size = 0.2, shuffle = True, random_state = 6)  
   x_train,x_test, y_train, y_test = train_test_split(x_train, y_train, test_size = 0.1, shuffle = True, random_state = 6)
 
   reduce_lr = ReduceLROnPlateau(monitor='val_loss', factor=0.6, patience=5)
 
   # обучаем
```

