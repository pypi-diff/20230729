# Comparing `tmp/videoslides-0.0.9.tar.gz` & `tmp/videoslides-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\videoslides-0.0.9.tar", last modified: Thu Jun 15 03:30:08 2023, max compression
+gzip compressed data, was "dist\videoslides-1.0.0.tar", last modified: Sat Jul 29 05:04:42 2023, max compression
```

## Comparing `videoslides-0.0.9.tar` & `videoslides-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 03:30:08.000000 videoslides-0.0.9/
--rw-rw-rw-   0        0        0    42900 2023-06-09 22:00:49.000000 videoslides-0.0.9/esquema.drawio
--rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1398 2023-06-15 03:30:08.000000 videoslides-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 03:30:08.000000 videoslides-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2179 2023-06-15 03:29:59.000000 videoslides-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:30:08.000000 videoslides-0.0.9/src/
--rw-rw-rw-   0        0        0    45609 2023-06-15 03:12:29.000000 videoslides-0.0.9/src/functions.py
-drwxrwxrwx   0        0        0        0 2023-06-15 03:30:08.000000 videoslides-0.0.9/src/videoslides.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1398 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2023-06-15 03:30:07.000000 videoslides-0.0.9/src/videoslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13523 2023-06-15 03:29:54.000000 videoslides-0.0.9/src/videoslides.py
--rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:04:42.000000 videoslides-1.0.0/
+-rw-rw-rw-   0        0        0    42900 2023-06-09 22:00:49.000000 videoslides-1.0.0/esquema.drawio
+-rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1398 2023-07-29 05:04:42.000000 videoslides-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-29 05:04:42.000000 videoslides-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2179 2023-07-29 05:04:11.000000 videoslides-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:04:42.000000 videoslides-1.0.0/src/
+-rw-rw-rw-   0        0        0    46210 2023-07-29 01:45:43.000000 videoslides-1.0.0/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-29 05:04:42.000000 videoslides-1.0.0/src/videoslides.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-29 05:04:41.000000 videoslides-1.0.0/src/videoslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1398 2023-07-29 05:04:41.000000 videoslides-1.0.0/src/videoslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-07-29 05:04:41.000000 videoslides-1.0.0/src/videoslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-07-29 05:04:41.000000 videoslides-1.0.0/src/videoslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2023-07-29 05:04:41.000000 videoslides-1.0.0/src/videoslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13304 2023-07-28 21:40:08.000000 videoslides-1.0.0/src/videoslides.py
+-rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-1.0.0/src/__init__.py
```

### Comparing `videoslides-0.0.9/esquema.drawio` & `videoslides-1.0.0/esquema.drawio`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.9/LICENSE.txt` & `videoslides-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.9/PKG-INFO` & `videoslides-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.9
+Version: 1.0.0
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.9/README.md` & `videoslides-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.9/setup.py` & `videoslides-1.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="videoslides",
-    version='0.0.9',
+    version='1.0.0',
     description='Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file ',
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["videoslides", "functions"],
     package_dir={'':'src'},
     install_requires=[
         "easyocr >= 1.4.1",
```

### Comparing `videoslides-0.0.9/src/functions.py` & `videoslides-1.0.0/src/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
 def download_video(url): 
     """ Descarga un video de youtube 
     -------------------------------------------------------
     Input:
         url (str): link del video de youtube
     Output:
-        No aplica
+        (boolean): True para descarga exitosa y en caso contrario False 
+        (str): string con el nombre del video descargado, en caso fallido string vacio
     """
     ''' 
     CAMBIOS QUE REQUIERE EN CIPHER.PY (DOCUMENTOS DE LA LIBRERIA)
     lineas 272 y 273
     r'a\.[a-zA-Z]\s*&&\s*\([a-z]\s*=\s*a\.get\("n"\)\)\s*&&\s*'
     r'\([a-z]\s*=\s*([a-zA-Z0-9$]{2,3})(\[\d+\])?\([a-z]\)'
     cambiar linea  288
@@ -59,24 +60,24 @@
     try:
         video = YouTube(url)
         title = video.title
         video = video.streams.get_highest_resolution()
         video.download()
         return True, title
     except Exception as e:
-        print(str(e))
+        warnings.warn(f"Warning ........... [Problema en descarga video: {str(e)}]")
         return False, ""
 
 def getqua(frame1, frame2, rgb = False, me = 4): 
     """ Funcion que compara dos frames con la metrica que indica el parametro "me"
     1:SSIM, 2:dif, 3:mse, 4:psnr, 5:uqi
     -------------------------------------------------------
     Input:
-        frame1 (str): ruta frames
-        frame2 (str): ruta frames
+        frame1 (stro o numpy.ndarray): ruta o informacion frame
+        frame2 (str o numpy.ndarray): ruta o informacion frame
         rgb (boolean): indicador de uso de 3 bandas de color (RGB, True) o solo una (B/W, False)
         me (int): metrica a usar para comparar los frames
     Output:
         (float): valor de evaluacion obtenido con metrica elegida
     """
     color = 0 # B/W
     multich = False
@@ -118,20 +119,21 @@
     elif(me == 4):
         psnrV = psnr(im1F, im2F, data_range=im2F.max() - im2F.min())
         return psnrV
     elif(me == 5):
         uqiV = uqi(im1F, im2F)
         return uqiV
     
-
 def getdata(frames, me, rgb = False): 
-    """ Funcion que usando getqua() en frames ordenados entrega un array con los valores evaluados de frames contiguos
+    """ Funcion que usando getqua() en frames ordenados entrega un array con los valores de similitud de cada par de frames contiguos
     -------------------------------------------------------
     Input:
         frames (str): ruta de carpeta de frames o (list): array de imagenes cv2
+        me (int): metrica a usar para comparar los frames
+        rgb (boolean): indicador de uso de 3 bandas de color (RGB, True) o solo una (B/W, False)
     Output:
         data (list): array ordenado con numeros enteros obtenidos evaluando frames contiguos
     """
     # data = list() ruta
     data = np.array([])
 
     if(isinstance(frames, list)):
@@ -166,14 +168,15 @@
     return data
 
 def localmin(data, coef = 3):
     """ Funcion que obtiene los minimos locales de la data entregada
     -------------------------------------------------------
     Input:
         data (list): array ordenado con numeros enteros 1D
+        coef (int): factor limitador sobre el numero de minimos considerados
     Output:
         counts[1] (int): numero de minimos locales encontrados
         pos (list): posiciones correspondiente a los minimos locales dentro del array data
     """
     # coef = 0.98 # TODO definir respecto a la metrica elegida y descomentar
     a_min =  np.r_[True, data[1:] < data[:-1]] & np.r_[data[:-1] < data[1:], True] & np.r_[data < coef]
     # a_min =  np.r_[True, data[1:] < data[:-1]] & np.r_[data[:-1] < data[1:], True] 
@@ -244,15 +247,15 @@
     - Con las distancias estructura las transcripciones en orden de lectura occidental (arriba hacia abajo e izquierda a derecha)
     -------------------------------------------------------
     Input:
         reader (class): clase easyocr.easyocr.Reader usada para la transcripcion de frames
         frames (str): ruta a carpeta de frames o imagen (numpy array)
         detail (str): nombre de la extension de la carpeta de bloques
         rgb (boolean): indicador de uso de 3 bandas de color (RGB, True) o solo una (B/W, False)
-        gpu_use (boolean): indicador para activar o no el uso de la GPU 
+        ocr (int): indicador de que OCR es usado para obtner la transcripcion, 1 = easyOCR o 2 = teseract 
         debugg (boolean): True -> grafica sobre la imagen los bloques de texto reconocidos
     Output:
         order (list): lista con la transcripcion estructurada 
     """
     # ocr = 1 # 1 EasyOCR y 2 Tesse
     lim_acc = 0.5
     if(ocr == 1):
@@ -378,15 +381,15 @@
                             aux_elem = trans_l[j[0]]
                             order[index][jndex][0] = aux_elem
                         except:
                             try:
                                 aux_elem = trans_l[j]
                                 order[index][jndex][0] = aux_elem
                             except:
-                                print("trans_l[j] > vacio")
+                                warnings.warn(f"Warning ........... [trans_l[j] vacio]")
             else:
                 if(isinstance(i[0], list)):
                     for jndex, j in enumerate(i[0]):
                         order[index][0][jndex] = trans_l[j]
                 else:
                     order[index][0] = trans_l[i[0]]
 
@@ -401,15 +404,15 @@
         if(debugg):
             plt.show()
         return order        
     else:
         return (" ").join(result)
 
 def deep_index(distance, word):
-    """ Funcion que entrega los indices de puntos a los cuales corresponde la distancia indicada en w, dentro de la lista triangular distance (no flatten)
+    """ Funcion que entrega los indices de puntos a los cuales corresponde la distancia indicada en word, dentro de la lista triangular distance (no flatten)
     -------------------------------------------------------
     Input:
         distance (list(lists(int))): lista de listas con distancias entre bloques de texto, (estructura triangular: [a distancia con b, c, d, e] [b distancia con c, d, e] ...)
         word (str): palabra/numero a indexar en las lista distance
     Output:
         l[0] (tuple(int, int)): indices de puntos a los cuales corresponde la distancia indicada en word
     """
@@ -434,15 +437,14 @@
     fla_sort = sorted(flatten)
     media = fla_sort[floor(tot_flat/2)]
     metrica = media# average o media
     while ( len(list(num for sublist in ret_array2 for num in sublist)) < tot*2): 
         minim = min(flatten)
         if (minim > metrica):
             # "existen aislados"
-            # TODO(?) :Agregar solos los que no alcanzaron en ret_array2 
             break
         ind = flatten.index(minim) 
         indx, indy = deep_index(array2, minim)        
 
         flatten[ind] = maxim + 1
         array2[indx][indy] = maxim + 1
         ret_array2[indx] = ret_array2[indx] + [indy+indx+1]
@@ -461,66 +463,63 @@
                 ret_array2[i] = list(set(ret_array2[i] + ret_array2[j]))
                 ret_array2[j] = []
 
     ret_array2 = [i for i in ret_array2 if len(i)>0]
     return(ret_array2)
 
 def select(array, frames, types = 0, rgb = False, gpu_use = False): 
-    """ Obtiene un frame por cada sub lista dentro de "array"
+    """ selecciona un frame por cada sub lista dentro de "array", obteniendo una lista de posiciones de los frames seleccionados
     types
     0 : Obtiene los ultimos elementos 
     1 : Obtiene los que posean mas informacion (get_trans_slide).
     -------------------------------------------------------
     Input:
-        array (list): lista de listas
+        array (list): lista de listas, agrupacion de frames por diapositiva
         frames (str): ruta de carpeta de frames o (list): array de imagenes cv2
         types (int): indicador del tipo de selector a usar; 0 para el ultimo de cada lista, 1 para usar get_trans_slide
         rgb (boolean): indicador de uso de 3 bandas de color (RGB, True) o solo una (B/W, False)
         gpu_use (boolean): indicador para activar o no el uso de la GPU 
     Output:
-        retorno (list) 
+        retorno (list): lista del nombre de los frames seleccionados
     """
     largo = len(array)
     retorno =  []
     if(types == 0):
         for i in range(largo):
             retorno.append(array[i][-1])
     else:
         gc.collect()
         torch.cuda.empty_cache()
         reader = easyocr.Reader(['en'], gpu=gpu_use) # this needs to run only once to load the model into memory
         retorno = get_trans_slide(reader, array, frames, rgb)
     return retorno
 
 def get_trans_slide(reader, array, frames, rgb = False):
-    """ Obtiene una lista de string, con las transcripciones de los frames indicados en array
+    """ Obtiene una lista de posiciones, con las transcripciones de los frames indicados en array compara para seleccionar
     -------------------------------------------------------
     Input:
         reader (class): clase easyocr.easyocr.Reader usada para la transcripcion de frames
         array (list): array con las posiciones de los frames de una slide
         frames (str): ruta a carpeta de frames o imagen (numpy array)
         rgb (boolean): indicador de uso de 3 bandas de color (RGB, True) o solo una (B/W, False)
     Output:
-        list_ret (list) 
+        list_ret (list): lista de posiciones de los frames seleccionados
     """
     debugg = False
     color = 0 # B/W
     remote = True
     if(rgb):
         color = 1 # RGB
     if(isinstance(frames, str)):
         f_ruta = frames
         Frames = ls(ruta = frames)
         Frames.sort()
         frames = list(map(addJ ,Frames))
-        # frames = Frames
         remote = False
 
-        # print("Leer data de frames -> dejarla en una lista de transcripciones -> cual tenga mayor numero de palabas es el seleccionado (comparar el numero de palabras coinidentes)")
-    # else:
     list_ret = []
     for index, i in enumerate(array):
         bigger = []
         pos = 0
         c_aux = 0
         for jndex, j in enumerate(frames):
             if(jndex in i):
@@ -542,15 +541,15 @@
     return(list_ret)
 
 def write_json(data, filename= "default"): 
     """ Funcion que escribe data en un archivo formato json
     -------------------------------------------------------
     Input:
         data (list o dict): data estructurada en listas o diccionarios 
-        filename (str): nombre del archivo incluyendo la extension
+        filename (str): ruta del archivo con el nombre del mismo, excluyendo la extension 
     Output:
         No aplica
     """
     filename = f"{filename}.json"
     with  open(filename, "w") as f:
         json.dump(data, f, indent=4)
 
@@ -560,19 +559,20 @@
     2 = teseract 
     -------------------------------------------------------
     Input:
         vname (str): nombre del video procesado
         frames (str): ruta de carpeta de frames o (list): array de imagenes cv2
         data (list): array con posiciones, usadas como filtro en la seleccion de imagenes
         rgb (boolean): indicador de uso de 3 bandas de color (RGB, True) o solo una (B/W, False)
-        runtime (boolean):
+        runtime (boolean): indicador de modo de manejo de frames (True: en numpy.array, False: en rutas de los frames)
         gpu_use (boolean): indicador para activar o no el uso de la GPU 
+        path (str): ruta destino del archivo json con la transcripcion (necesario solo para caso runtime=False)
         ocr (int): indicador de que OCR es usado para obtner la transcripcion, 1 = easyOCR o 2 = teseract 
     Output:
-        transcription (str o list): texto recopilado de cada frame unido en una sola estuctura
+        transcription (str o list): texto recopilado de cada frame unido en una sola estuctura, ya sea en formato de array o string de la ruta del archivo
     """
     if(isinstance(frames, list)):
         Frames = frames
     else:
         Frames = ls(ruta = frames)
         Frames.sort()
         Frames = list(map(addJ ,Frames))
@@ -586,18 +586,17 @@
                 i = int(frame.split(".")[0]) 
                 rute = frames+ str(i)+'.jpg'
             else:
                 rute = frame
             if (ocr == 1):
                 gc.collect()
                 torch.cuda.empty_cache()
-                reader = easyocr.Reader(['en'], gpu=gpu_use) # this needs to run only once to load the model into memory
+                reader = easyocr.Reader(['en'], gpu=gpu_use) 
                 json.append(easy(reader, rute, 1, rgb, 1))
             elif (ocr == 2):
-                # transcription = transcription + tese(rute, False) + "\n\n"
                 reader = 1
                 json.append(easy(reader, rute, 1, rgb, 2))
                 # TODO: agregar coeficiente para tomar para caso de TESE porcentaje de confianza mayor a 0.8 aprox
 
     if (ocr == 1):
         filename = vname
         transcription = json
@@ -613,16 +612,16 @@
 
     return transcription
 
 def isame(frame1, frame2, rgb = False, pix_lim = 0.001, ssimv_lim = 0.999, dbugg = False):  
     """ Compara dos frames usando el porcentaje de pixeles que difieren como tambien el valor para SSIM entre ellos
     -------------------------------------------------------
     Input:
-        frame1 (str): ruta de primer frame
-        frame2 (str): ruta de segundo frame
+        frame1 (str): ruta del primer frame
+        frame2 (str): ruta del segundo frame
         rgb (boolean): indicador de uso de 3 bandas de color (RGB, True) o solo una (B/W, False)
         pix_lim (float): indicador de limite para filtrar imagenes segun metrica de porcentaje de pixeles cambiantes
         ssimv_lim (float): indicador de limite para filtrar imagenes segun metrica SSIM
         dbugg (boolean): True en caso de querer visualizar los frames
     Output:
         state (boolean): indicador que indica si son considerados suficientemente similares 
     """
@@ -652,35 +651,35 @@
     pix_num = height * width * 3
 
     state = False
     # pix_lim = 0.001
     if ( dif/pix_num < pix_lim):
         #  Son escencial- la misma
         if (dbugg):
-            print(" ----------------- dif %f ----------------- " % float(dif/pix_num))		
+            print(f" ----------------- dif {float(dif/pix_num)} ----------------- ")		
         state  = True
     elif(ssimV>ssimv_lim):	
         # Son escencial- la misma
         if (dbugg):
-            print(" ----------------- ssimV %f ----------------- " % ssimV)		
+            print(f" ----------------- ssimV {ssimV} ----------------- ")		
         state  = True
 
     if (dbugg):
         f = plt.figure()
         f.add_subplot(1,2, 1)
         plt.imshow(im1)
         f.add_subplot(1,2, 2)
         plt.imshow(im2)
         plt.title("SAME ? :" + str(state) )
         plt.show(block=True)
     return state
 
 def clean(frames, rgb = False, pix_lim = 0.001, ssimv_lim = 0.999): 
     """ Funcion que usando isame() filtra las imagenes que son consideradas iguales (dejando solo una de ellas)
-    para el caso de no estar runtime : se elimina el frame de la ruta 
+    para el caso de runtime falso : se elimina el frame de la ruta 
     caso runtime: se crea una nueva lista con los frames correspondientes y se retorna   
     -------------------------------------------------------
     Input:
         frames (str): ruta de carpeta de frames o (list): array de imagenes cv2
         rgb (boolean): indicador de uso de 3 bandas de color (RGB, True) o solo una (B/W, False)
         pix_lim (float): indicador de limite para filtrar imagenes segun metrica de porcentaje de pixeles cambiantes
         ssimv_lim (float): indicador de limite para filtrar imagenes segun metrica SSIM
@@ -719,54 +718,66 @@
                 rute2 = frames+ str(i)+'.jpg'
                 if(isame(rute1, rute2, rgb, pix_lim, ssimv_lim)):  # si son iguales se elimina el primero, si son distintos no se hace nada
                     os.remove(rute1)
             anterior = i
         Frames = frames
     return Frames
 
-def ploteo(nombre, data): 
+def ploteo(nombre, data, coef = 1 ,debugg = False): 
     """ Funcion que grafica data 1D, y en caso de no entregarla la obtiene usando getdata(f_ruta)
     -------------------------------------------------------
     Input:
         nombre (str): nombre de la data (video)
         data (list): lista con valores obtenidos de la comparacion de frames contiguos
+        coef (int): factor limitador sobre el numero de minimos considerados
+        dbugg (boolean): True en caso de querer visualizar el nombre entregado
     Output:
         "OK" (str)
     """
-    print(f" -------- {nombre} -------- ")
+    if (debugg) :
+        print(f" -------- {nombre} -------- ")
     # min, minl = localmin(data)
-    classic(data, nombre)
+    classic(data, nombre, coef)
     return "OK"
 
-def classic(data, nombre): 
+def classic(data, nombre, coef): 
     """ Grafica data 1D, indicando el nombre, minimo y maximo de la data
     -------------------------------------------------------
     Input:
         data (list): array ordenado con numeros enteros 1D
         nombre (str): nombre de la data (video)
+        coef (int): factor limitador sobre el numero de minimos considerados
     Output:
         no aplica
     """
     minim = np.amin(data)
     maxim = np.amax(data)
-    plt.plot(data, label='data', color='b')
-    plt.legend(bbox_to_anchor=(1.05, 1),loc='upper left', borderaxespad=0.)
+    plt.plot(data, label='SIMM', color='b')#, label='SIMM')
+
+    if (coef != 1):
+        x = [0, len(data)]
+        y2 = [coef, coef]
+        plt.plot(x, y2, '-.', color='red', label='COEF')
+
+    plt.legend()
+    # plt.legend( ['SIMM','COEFF'], bbox_to_anchor=(1.05, 1),loc='upper left') #, borderaxespad=0.)
     plt.xlabel("Par de frames")
     plt.ylabel("SIMM par de frames")
-    number_of_diapos, pos = localmin(data)
+    number_of_diapos, pos = localmin(data, coef) 
     plt.title(f"{nombre} ({number_of_diapos})")
     plt.show()
 
 def clean_transc(transc):
     """ Desde una transcripcion en formato de lista se eliminan redundancias y se retorna la nueva lista
     -------------------------------------------------------
     Input:
-        transc (list):  lista de listas con texto transcrito
+        transc (list o str): lista de listas con texto transcrito o ruta de archivo json
     Output:
-        transc 
+        transc (list o str): lista de listas con texto transcrito filtrado o ruta de archivo json filtrado
+        del (list): lista binaria con 1 en la posicion de un frame eliminado
     """
     debugg = False
     limite = 0.9
     runtime = True
     path = ""
     if(isinstance(transc, str)):
         runtime = False
@@ -846,15 +857,15 @@
     """ Desde una transcripcion en formato de lista se eliminan redundancias y se retorna la nueva lista
     -------------------------------------------------------
     Input:
         frames (str): ruta de carpeta de frames o (list): array de imagenes cv2
         lt_delet (list):  lista ordenada de frames a ser eliminados (1 en posicion de frames a eliminar, 0 sino se elimina) o (numero de las posiciones a mantenerse, ej: [0,3,7])
         tipo (int): indicador si se usara la primera o segunda estructura para la lista lt_delet
     Output:
-        frames (str): ruta de carpeta de frames o (list): array de imagenes cv2
+        Frames (str): ruta de carpeta de frames o (list): array de imagenes cv2
     """
     if(isinstance(frames, list)):
         Frames = frames.copy()
     else:
         Frames = ls(ruta = frames)
         Frames.sort()
         Frames = list(map(addJ ,Frames))
@@ -891,79 +902,60 @@
                 if(a not in lt_delet):
                     os.remove(rute)
             Frames = frames
 
     return Frames
 
 def lemat(text, gpu_use = False):
-    """ Funcion que lematiza el texto recibido
+    """ Funcion que lematiza el texto recibido, inicialdo internamente el pipeline de stanza
     -------------------------------------------------------
     Input:
         text (str): string con oración o parrafo a ser lematizado
         gpu_use (boolean): indicador para activar o no el uso de la GPU 
     Output:
         ret (str): string con texto lematizado
     """
-    # stanza.download('es')
     gc.collect()
     torch.cuda.empty_cache()
     nlp = stanza.Pipeline('es', verbose= False,  use_gpu = gpu_use) # pos_batch_size=3000
     doc = nlp(text)
     ret = ""
     for sent in doc.sentences:
         for word in sent.words:
             ret = ret + " " + word.lemma    
-            # print(f'word: {word.text} \tlemma: {word.lemma}') 
     return ret
 
-def lemat2(nlp, text):
+def lemat2(nlp, text, complete = False):
     """ Funcion que lematiza el texto recibido
     -------------------------------------------------------
     Input:
-        nlp: stanza.Pipeline
+        nlp (class): stanza.Pipeline
         text (str): string con oración o parrafo a ser lematizado
         gpu_use (boolean): indicador para activar o no el uso de la GPU 
     Output:
         ret (str): string con texto lematizado
     """
     doc = nlp(text)
     ret = ""
     for sent in doc.sentences:
         for word in sent.words:
             ret = ret + " " + word.lemma    
+            # if complete:
+            #     ret += '\n'
+        if complete:
+            ret += '\n'
     return ret
 
-def pos(nlp, text): # PEND
-    """ Funcion pend
-    -------------------------------------------------------
-    Input:
-        nlp: stanza.Pipeline
-        text (str): string con oración o parrafo a ser 
-        gpu_use (boolean): indicador para activar o no el uso de la GPU 
-    Output:
-        ret (str): string con texto procesado
-    """
-    doc = nlp(text)
-    ret = ""
-    for sent in doc.sentences:
-        for word in sent.words:
-            # ret = ret + " " + word.lemma  
-            if ( word.feats != None and "NumForm=Digit" in word.feats ):
-                print( type(word.feats), "DIGITO", word.text )
-            # print(f'word: {word.text} \tlemma: {word.lemma} \tpos: {word.pos} \tfeats: {word.feats}  ')  
-            # if():
-    return ret
-
-
-def lematize(transcription, gpu_use = False):
+def lematize(transcription, gpu_use = False, dest_file = 'default.json'):
     """ Funcion que lematiza transcripcion desde un array o una carpeta
     -------------------------------------------------------
     Input:
-        transcription (str): string con oración o parrafo a ser lematizado
+        transcription (str): string con oración/parrafo a ser lematizado o ruta del archivo json
         gpu_use (boolean): indicador para activar o no el uso de la GPU 
+        dest_file (str): ruta de archivo de salida, incluyendo nombre y extension archivo
     Output:
         transcription (str o list): string con ruta al json o lista de listas con la transcripcion
     """
 
     if(isinstance(transcription, list)):
         slides = transcription.copy()
     else:
@@ -986,88 +978,77 @@
                         slides[index][jndex][kndex] = lemat2(nlp, slides[index][jndex][kndex])
             else:
                 slides[index][jndex] = lemat2(nlp, slides[index][jndex])
 
     if(isinstance(transcription, list)):
         return slides
     else:
-        filename = transcription.replace(".json", "")
+        filename = dest_file.replace(".json", "")
         write_json(slides, filename)
-        return transcription
+        return dest_file
 
 def tese(ruta, lim_acc, debug = False): 
-    """ Funcion que desde un frame/imagene obtiene una transcripcion usando OCR tesseract
+    """ Funcion que desde un frame/imagen obtiene una transcripcion usando OCR tesseract, 
+    entregandolo en un formato estandar usado por el sistema EasyOCR
     -------------------------------------------------------
     Input:
         ruta (str): ruta de frame/imagen a transcribir
+        lim_acc (int): factor minimo de confianza usado para filtrar las palabras extraidas con el sistema OCR
         debug (boolean): indicador si se quiere o no mostrar la imagen a transcribir
     Output:
         data (str): transcripcion de la imagen a texto
     """
     # inicio = time.time()
     pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
     image = cv2.imread(ruta, 0)
     conf = f'--psm 6'
     coefic = lim_acc*100
-    # conf = f'--psm 6 -c tessedit_char_whitelist=0123456789.%,/+-*'
-    # rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-    # results = pytesseract.image_to_data(rgb, output_type=Output.DICT)
     results = pytesseract.image_to_data(image, lang='eng', config=conf, output_type=Output.DICT)
     data = pytesseract.image_to_string(image, lang='eng', config=conf)
-    # print(data)
-    # [print(i, results[i]) for i in results ]
-    # exit(1)
-    # [print(i) for i in results ]
-
 
     conf = [results[i] for i in results if i == 'conf'][0]
     conf = [float(i) for i in conf]
     left = [j for jndex, j in enumerate([results[i] for i in results if i == 'left'][0]) if float(conf[jndex]) > coefic]
     top = [j for jndex, j in enumerate([results[i] for i in results if i == 'top'][0]) if float(conf[jndex]) > coefic]
     width = [j for jndex, j in enumerate([results[i] for i in results if i == 'width'][0]) if float(conf[jndex]) > coefic]
     height = [j for jndex, j in enumerate([results[i] for i in results if i == 'height'][0]) if float(conf[jndex]) > coefic]
     text = [j for jndex, j in enumerate([results[i] for i in results if i == 'text'][0]) if float(conf[jndex]) > coefic]
     conf = [i for i in conf if i > coefic]
 
-    # [print(f"{i} --> {conf[index]}") for index, i in enumerate(text)]  
     compilado = [([[left[index], top[index]], [left[index]+width[index],top[index]], [left[index]+width[index], top[index]+height[index]], [left[index], top[index]+height[index]]], i, conf[index]) for index, i in enumerate(text)]
     return compilado
-    # [print(i) for i in compilado ]
-
-    [print(f"{conf[index]} --> {i}") for index, i in enumerate(text) if float(conf[index]) > 70] 
-    # print(results)
-    return data
 
 def upscale_img(img, pb_path, model, ratio, runtime, gpu):
     """ funcion que mejora imagen segun modelo y escala entregada
-    Args:
+    Input:
         img (str): ruta hacia de imagen a mejorar
+        pb_path (str): ruta del archivo pb del modelo a usar
         model (str): nombre del modelo a usar ('edsr', 'espcn', 'fsrcnn' o 'lapsrn')
         ratio (int): escala a aplicar a la imagen (2, 3 o 4)
-        replace (boolean): indicador para reemplazo de img mejorada 
         runtime (boolean): indicador de modo de manejo de imagenes (True: imagen en numpy.array, False: entonces img es ruta de la imagen)
         gpu (boolean): indicador de uso de gpu
+    Output:
+        imagen en array cv2 para runtime True y 'ok' para caso contrario
     """
     sr = dnn_superres.DnnSuperResImpl_create()
     if not runtime:
         image = img
         img = cv2.imread(img)
     # Read the desired model
-    # path = f"./models/{model}_x{ratio}.pb"
     path = f"{pb_path}{model}_x{ratio}.pb"
     sr.readModel(path)
     if (gpu):
         # Set CUDA backend and target to enable GPU inference
         sr.setPreferableBackend(cv2.dnn.DNN_BACKEND_CUDA)
         sr.setPreferableTarget(cv2.dnn.DNN_TARGET_CUDA)
     # Set the desired model and scale to get correct pre- and post-processing
     sr.setModel(model.lower(), ratio)
     result = sr.upsample(img)
     # Save the image
-    # if replace:
+    # if replace: # replace (boolean): indicador para reemplazo de img mejorada 
     if not runtime:
         cv2.imwrite(image, result)
         return 'ok'
     else:
         return img
         # img = result
     # else:
@@ -1098,20 +1079,23 @@
     lt_real = [i for i in f_real.split(' ') if len(i) > 0]
     dif_wused = word_perc(lt_process, lt_real)
     # **************************************************************
 
     return dif_tf, dif_wused
 
 def word_perc(lt_process, lt_real):
+    """ Funcion obtiene el porcentaje de palabras del texto en lt_process dentro de lt_real
+    
+    """
     total = len(lt_real)
     lt_inner = []
 
     for i in lt_process:
         if len(lt_real) == 0:
-            print('vacio')
+            warnings.warn(f"Warning ........... [lista con texto real vacia]")
         if i in lt_real:
             lt_inner.append(i)
             lt_real.remove(i)
 
     dif = (len(lt_inner)/total)
     return dif
 
@@ -1123,9 +1107,8 @@
     # from nltk.corpus import stopwords
 
     st_words = stopwords.words('spanish')
     vect = TfidfVectorizer(min_df=1, stop_words= st_words)                                                                                                                                                                                                   
     tfidf = vect.fit_transform(corpus)                                                                                                                                                                                                                       
     pairwise_similarity = tfidf * tfidf.T
 
-    # print(pairwise_similarity.mean(axis=0))
-    return((pairwise_similarity.A)[0,1])
+    return((pairwise_similarity.A)[0,1])
```

### Comparing `videoslides-0.0.9/src/videoslides.egg-info/PKG-INFO` & `videoslides-1.0.0/src/videoslides.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.9
+Version: 1.0.0
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.9/src/videoslides.py` & `videoslides-1.0.0/src/videoslides.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,40 @@
 import cv2
 import validators
 from pathlib import Path
 import functions as fc
 
 
 class Video:
-    def __init__(self, path, scale = 100 , saltos = 1, rgb = False, runtime = True, lematiz = False, gpu_use = False, pix_lim = 0.001, ssimv_lim = 0.999): # scale:percent of original size
+    def __init__(self, path, scale = 100 , jumps = 1, rgb = False, runtime = True, gpu_use = False, pix_lim = 0.001, ssimv_lim = 0.999, re_run = False): # scale:percent of original size
         """ Clase para manejar el video, frames y transcripcion 
         path (str): link del video o a la ruta local del archivo mp4
         scale (int): numero que indica de que escala del tamaño real de los frames se desean extraer [0,100]
-        saltos (int): numero de saltos periodicos entre lecturas de frames
+        jumps (int): numero de saltos periodicos entre lecturas de frames
+        rgb (boolean): indicador booleano si se da uso de banda RGB (True) o solo banda blanco y negro (False)
         runtime (boolean): False -> para usar la data de frames de forma persistente (archivos) o True -> en ejecucion (objetos y listas) 
+        gpu_use (boolean): indicador para activar o no el uso de la GPU 
+        re_run (False or string): indicador si la ejecucion actual es reproceso o no, y en caso de serlo desde que tipo de informacion se inicia, 
+                frame-> path asigna ruta de frames y trans-> asigna path a atributo transcription
         """
         link = True
         self.rgb = rgb
         self.runtime = runtime
-        self.lematiz = lematiz
         self.gpu_use = gpu_use
         self.pix_lim, self.ssimv_lim = pix_lim, ssimv_lim
+        if (re_run != False):
+            if (re_run == 'frame'):
+                self.frames_path = path
+                self.video_name = path.split('/')[-1]
+                return
+            elif (re_run == 'trans'):
+                self.transcription = path
+                self.video_name = path.split('/')[-1]
+                return
+
         # ------------ Video de Youtube ------------
         extension = "mp4"
         if (validators.url(path)):
             status, real_VideoName = fc.download_video(path)
             real_VideoName = real_VideoName.replace("|", "")
             if(not status):
                 print(status)
@@ -88,15 +101,15 @@
         count = 0
         if(runtime):
             frames = []
         else:
             frames = self.frames_path
         
         while (count < self.num_frames-1):
-            if(count%(self.fps*saltos) == 0):
+            if(count%(self.fps*jumps) == 0):
                 # resize image
                 resized = cv2.resize(image, dim, interpolation = cv2.INTER_AREA)
                 if(runtime):
                     frames.append(resized)
                 else:
                     # cv2.imwrite(Path(self.frames_path+f"{count}.jpg"), resized)     # save frame as JPEG file  
                     cv2.imwrite(self.frames_path+f"{count}.jpg", resized)     # save frame as JPEG file  
@@ -108,30 +121,43 @@
         self.frames = frames
         # -------------------------------------------------------------------------
 
         self.data = []
         self.slides = []
 
     # --------------- GETTERS ---------------
-    def get_number_frames(self):  # numero de frames
+    def get_num_frames(self):  # numero de frames
         return self.num_frames
     def get_fps(self):            # fotogramas por segundo del video
         return self.fps
     def get_path(self):           # ruta del video
         return self.path
     def get_video_name(self):     # nombre del video
         return self.video_name
     def get_frames_path(self):    # ruta de los frames
         return self.frames_path
     def get_video_cap(self):      # captura del video 
         return self.video_cap
     def get_frames(self):
         return self.frames
+    def get_dim(self):
+        return self.dim
+    def get_data(self):
+        return self.data
+    def get_slides(self):
+        return self.slides
     # --------------- SETTERS ---------------
     def set_frames_path(self, frames_path):
+        """ Funcion de seteo de atributo frames_path
+        -------------------------------------------------------
+        Input:
+            No aplica
+        Output:
+            No aplica
+        """
         self.frames_path = frames_path
 
     def set_data(self, me): # se setea la data segun este usandose de forma runtime o no
         """ Funcion que usando getqua() sobre frames ordenados entrega un array con los valores evaluados de frames contiguos
         -------------------------------------------------------
         Input:
             No aplica
@@ -140,15 +166,17 @@
         """
         self.data = fc.getdata(self.frames, me, self.rgb) # ambos casos cubiertos (runtime TRUE/FALSE)
 
     def set_slides(self, me = 1, posiciones = None, coef = 3):
         """ divide y obtiene los frames que contienen la mayor parte de la informacion de cada slide
         -------------------------------------------------------
         Input:
-            posiciones (array): lista con posiciones de los frames elegios para conformar el conjunto final de diapositivas (opcional)
+            me (int): metrica a usar para comparar los frames en la obtencion de minimos -> diapositivas
+            posiciones (array): (opcional) lista con posiciones de los frames elegidos para conformar el conjunto final de diapositivas, sin utilizar el proceso de seleecion automatica.
+            coef (int): factor limitador sobre el numero de minimos considerados
         Output:
             No aplica
         """
         if(posiciones != None):
             self.frames = [i for index, i in enumerate(self.frames) if index in posiciones]
         else:
             if (len(self.data) == 0):
@@ -216,73 +244,47 @@
             No aplica
         Output:
             No aplica
         """
         self.transcription, lt_delet = fc.clean_transc(self.transcription)
         self.frames = fc.delete_frames(self.frames, lt_delet)
 
-    def lematize(self):
+    def lematize(self, dest_file = 'default.json' ):
         """  Funcion aplica lematizacion sobre la transcripcion almacenada en self.transcription, reemplazando la original
         -------------------------------------------------------
         Input:
             No aplica
         Output:
             No aplica
         """
-        self.transcription = fc.lematize(self.transcription, self.gpu_use)
-
-    def improve_num(self):
-        """  Funcion corrige digitos de la transcripcion inicial, utilizando el OCR de Tesseract 
-        -------------------------------------------------------
-        Input:
-            No aplica
-        Output:
-            No aplica
-        """
-        # tomar frames finales
-        print("ENTRO")
-        transcription_tesse = fc.get_transcription(self.video_name, self.frames, [], self.rgb, self.runtime, self.gpu_use, 2) # los dos casos cubiertos 
-        print(transcription_tesse)
+        self.transcription = fc.lematize(self.transcription, self.gpu_use, dest_file)
 
     def improve_quality(self, path, model, ratio):
         """  Funcion mejora calidad de imagenes, ya sea la lista de frames o frames guardados localmente
         -------------------------------------------------------
         Input:
             No aplica
             model
             ratio
         Output:
             No aplica
         """
-        # self.frames
         if(self.runtime):
             for index, frame in enumerate(self.frames):
                 self.frames[index] = fc.upscale_img(frame, path, model, ratio, self.runtime, self.gpu_use)
         else:
             Frames = fc.ls(ruta = self.frames)
             Frames.sort()
             Frames = list(map(fc.addJ ,Frames))
             for index, frame in enumerate(Frames):
                 fc.upscale_img(self.frames+frame, path, model, ratio, self.runtime, self.gpu_use)
 
-
-
-        # TODO: aplicar tesseract en los casos que se encuentre un digito o cifra en self.transcription (puede ir despues de lematization)
-        # TODO: REVISAR SI EXISTE ALGUNA FORMA DE ENTREGAR MAYOR VALOR A LA ESTRUCTURACION ( ETIQUETAS ? : TITTLE, COMMENT, NAMES, NUMBER OR DATES)
-
-
-        # TODO: REVISAR FORMAS DE OBTENER CONTEXTO DE INFO EN UNA LAMINA (QUIZAS FILTRAR Y OMITIR INFORMACION NO RELEVANTE)
-        # TODO: N-GRAMA PARA LA CORRECCION -> REVISAR QUE PALABRAS SE REPITEN MAS Y QUIZAR HACER UNA ANALISIS ESTADISTICO CON ESTO (UN PLUS (?))
-        # TODO: MENCIONAR QUE SE PUEDE MEJORAR EL CALCULO DE DISTANCIA ENTRE CUADRADOS DE TEXTO -> MEJORAR ESTRUCTURACION EN CASO DE TEXTO EN DIAGONAL
-        # TODO: quizas quitar parametros desde la definicion de la clase y dejaros seteables luego de su creacion
-        # TODO : dejar como parametro editable el limite para la limpieza por texto
-
-
-
-
-        # DONE: Dejar con el formato de result de EASYOCR el resultado obtenido con tesseract 
-        # DONE: MEJORAR FUNCION PARA ELEGIR FRAMES DESDE SLIDE (actual es last_one) -> AGREGAR A DOCUMENTO
-        # DONE: REVISAR QUE TAN UTIL SERIA EL RTF (no mucho, se puede agregar formato, y quizas imagenes, -> buscar valor o uso de los RTF)
-        
-        # DONE: eleccion de lematizar
-        # DONE dar libertad de los rangos a los cuales se desea filtrar
-        # DONE revisar cambios necesarios para implementar solo escala de grises ( o dar la opcion de elegir) -> agregar comparacion al documento
+    # def improve_num(self):
+        # """  Funcion corrige digitos de la transcripcion inicial, utilizando el OCR de Tesseract 
+        # -------------------------------------------------------
+        # Input:
+        #     No aplica
+        # Output:
+        #     No aplica
+        # """
+        # # tomar frames finales
+        # transcription_tesse = fc.get_transcription(self.video_name, self.frames, [], self.rgb, self.runtime, self.gpu_use, 2) # los dos casos cubiertos
```

