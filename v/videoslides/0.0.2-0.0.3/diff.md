# Comparing `tmp/videoslides-0.0.2.tar.gz` & `tmp/videoslides-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\videoslides-0.0.2.tar", last modified: Fri Jul 15 23:36:53 2022, max compression
+gzip compressed data, was "dist\videoslides-0.0.3.tar", last modified: Wed May 17 02:30:36 2023, max compression
```

## Comparing `videoslides-0.0.2.tar` & `videoslides-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-07-15 23:36:53.000000 videoslides-0.0.2/
--rw-rw-rw-   0        0        0     6011 2022-07-09 02:09:54.000000 videoslides-0.0.2/esquema.drawio
--rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1398 2022-07-15 23:36:53.000000 videoslides-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2022-07-15 23:36:53.000000 videoslides-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2023 2022-07-15 23:36:46.000000 videoslides-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-15 23:36:53.000000 videoslides-0.0.2/src/
--rw-rw-rw-   0        0        0    25005 2022-07-14 04:48:00.000000 videoslides-0.0.2/src/functions.py
-drwxrwxrwx   0        0        0        0 2022-07-15 23:36:53.000000 videoslides-0.0.2/src/videoslides.egg-info/
--rw-rw-rw-   0        0        0        1 2022-07-15 23:36:53.000000 videoslides-0.0.2/src/videoslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1398 2022-07-15 23:36:53.000000 videoslides-0.0.2/src/videoslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2022-07-15 23:36:53.000000 videoslides-0.0.2/src/videoslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2022-07-15 23:36:53.000000 videoslides-0.0.2/src/videoslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2022-07-15 23:36:53.000000 videoslides-0.0.2/src/videoslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8154 2022-07-15 23:18:13.000000 videoslides-0.0.2/src/videoslides.py
--rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:30:36.000000 videoslides-0.0.3/
+-rw-rw-rw-   0        0        0     6063 2022-07-20 03:36:12.000000 videoslides-0.0.3/esquema.drawio
+-rw-rw-rw-   0        0        0     1103 2022-07-12 04:02:52.000000 videoslides-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       46 2022-07-12 05:01:15.000000 videoslides-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1398 2023-05-17 02:30:36.000000 videoslides-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2022-07-14 02:45:05.000000 videoslides-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-17 02:30:36.000000 videoslides-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2023 2023-05-17 02:30:31.000000 videoslides-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:30:36.000000 videoslides-0.0.3/src/
+-rw-rw-rw-   0        0        0    45516 2023-05-11 02:57:14.000000 videoslides-0.0.3/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-17 02:30:36.000000 videoslides-0.0.3/src/videoslides.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-17 02:30:36.000000 videoslides-0.0.3/src/videoslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1398 2023-05-17 02:30:36.000000 videoslides-0.0.3/src/videoslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-05-17 02:30:36.000000 videoslides-0.0.3/src/videoslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-05-17 02:30:36.000000 videoslides-0.0.3/src/videoslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2023-05-17 02:30:36.000000 videoslides-0.0.3/src/videoslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13048 2023-05-11 03:10:08.000000 videoslides-0.0.3/src/videoslides.py
+-rw-rw-rw-   0        0        0        0 2022-07-12 02:31:10.000000 videoslides-0.0.3/src/__init__.py
```

### Comparing `videoslides-0.0.2/LICENSE.txt` & `videoslides-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.2/PKG-INFO` & `videoslides-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.2/README.md` & `videoslides-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `videoslides-0.0.2/setup.py` & `videoslides-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="videoslides",
-    version='0.0.2',
+    version='0.0.3',
     description='Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file ',
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["videoslides", "functions"],
     package_dir={'':'src'},
     install_requires=[
         "easyocr ~= 1.4.1",
-        "opencv-python-headless ~= 4.1.2.30",
+        "opencv-python-headless <= 4.1.2.30",
         "stanza ~= 1.4.0",
         "numpy ~= 1.19.5",
         "matplotlib ~= 3.3.4",
         "pytube ~= 12.0.0",
         "scikit-image ~= 0.17.2",
         "validators ~= 0.20.0",
         "nltk ~= 3.6.7"
```

### Comparing `videoslides-0.0.2/src/videoslides.egg-info/PKG-INFO` & `videoslides-0.0.3/src/videoslides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videoslides
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package made to obtain a text transcription from a video, with a flow from video to frames to structured frames to transcription in a json file 
 Home-page: https://github.com/Zes7one/VideoSlides
 Author: Franco Palma
 Author-email: franco.pm10@gmail.com 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `videoslides-0.0.2/src/videoslides.py` & `videoslides-0.0.3/src/videoslides.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,106 @@
-import validators
-import warnings
 import os
+import warnings
+
 import cv2
+import validators
+
 import functions as fc
 
+
 class Video:
-    def __init__(self, path, scale = 100 , saltos = 1, local = True): # scale:percent of original size
+    def __init__(self, path, scale = 100 , saltos = 1, rgb = False, runtime = True, lematiz = False, gpu_use = False, pix_lim = 0.001, ssimv_lim = 0.999): # scale:percent of original size
         """ Clase para manejar el video, frames y transcripcion 
         path (str): link del video o a la ruta local del archivo mp4
         scale (int): numero que indica de que escala del tamaño real de los frames se desean extraer [0,100]
         saltos (int): numero de saltos periodicos entre lecturas de frames
-        local (boolean): indicador para usar la data de frames de forma persistente (archivos) o en ejecucion (objetos y listas)
+        runtime (boolean): False -> para usar la data de frames de forma persistente (archivos) o True -> en ejecucion (objetos y listas) 
         """
         link = True
-        self.local = local
+        self.rgb = rgb
+        self.runtime = runtime
+        self.lematiz = lematiz
+        self.gpu_use = gpu_use
+        self.pix_lim, self.ssimv_lim = pix_lim, ssimv_lim
         # ------------ Video de Youtube ------------
+        extension = "mp4"
         if (validators.url(path)):
             status, real_VideoName = fc.download_video(path)
             real_VideoName = real_VideoName.replace("|", "")
             if(not status):
                 raise Exception("El link entregado no es un video")
-            RutaFolder = os.path.dirname(os.path.abspath(__file__))+"\\"
-            self.path = RutaFolder+real_VideoName+".mp4"
+            # RutaFolder = os.path.dirname(os.path.abspath(__file__))+"\\"
+            RutaFolder = os.path.abspath(os.getcwd())+"\\"
+            self.path = RutaFolder+real_VideoName+f".{extension}"
             self.video_name = real_VideoName
         # ------------------------------------------
         # ------------ Video desde directorio ------------
         else:
             link = False
             real_VideoName = path.split("/")[-1] 
+            extension = real_VideoName.split(".")[-1]
             RutaFolder = path.replace(real_VideoName, '')
             self.path = path
-            self.video_name = real_VideoName.replace(".mp4", "") #.replace("y2mate.com", "").replace(" ", "").replace(".", "").replace("-", "")
+            self.video_name = real_VideoName.replace(f".{extension}", "") #.replace("y2mate.com", "").replace(" ", "").replace(".", "").replace("-", "")
         # ------------------------------------------------
             
         # ------------ Se crea carpeta y se captura el video ------------
         self.frames_path = ""
-        if(not local):
+        if(not runtime):
             self.frames_path = RutaFolder+"F_"+self.video_name+"\\"
             if (not os.path.isdir(self.frames_path)):
                 os.mkdir(self.frames_path)
-        vidcap = cv2.VideoCapture(RutaFolder+self.video_name+".mp4")
+        vidcap = cv2.VideoCapture(RutaFolder+self.video_name+f".{extension}")
         self.video_cap = vidcap
         # ---------------------------------------------------------------
         
-        # ------------ Se elimina el video en caso de local y link ------------
-        if(local and link): 
-            # TODO Se borra la carpeta con los frames -> solo se puede cuando se deje de usar el vidcap
-            string = """
-            se mantiene una lista de imagenes = frames
-            se mantiene una vidcap = video
-            """ 
-            # os.remove(self.path)
-            warnings.warn(string)
+        # ------------ Se elimina el video en caso de runtime y link ------------
+        # if(runtime and link): 
+        #     # TODO Se borra la carpeta con los frames -> solo se puede cuando se deje de usar el vidcap
+        #     string = """
+        #     Manejo de data en Runtime
+        #     se mantiene una lista de imagenes = frames
+        #     se mantiene una vidcap = video
+        #     """ 
+        #     # os.remove(self.path)
+        #     warnings.warn(string)
         # ---------------------------------------------------------------------
 
         self.num_frames = int(vidcap.get(cv2.CAP_PROP_FRAME_COUNT))
         self.fps    = int(vidcap.get(cv2.CAP_PROP_FPS))
         # ------------ Se lee un frame y se obtiene las dimensiones ------------
         success,image = vidcap.read()	
-        image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) # TODO revisar cambios necesarios para implementar solo escala de grises ( o dar la opcion de elegir)
+        if(not rgb):
+            image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) 
         if(not success):
-            raise Exception("Problemas en la captura del video: video corrompido o formato incorrecto")
+            raise Exception("Problemas en la captura del video: video corrupto o formato incorrecto")
         width = int(image.shape[1] * scale / 100)
         height = int(image.shape[0] * scale / 100)
         dim = (width, height)
         self.dim = dim
         # ----------------------------------------------------------------------
 
         # ------------ Se guardan los frames o se crea lista de frames ------------
         count = 0
-        if(local):
+        if(runtime):
             frames = []
         else:
             frames = self.frames_path
         
         while (count < self.num_frames-1):
             if(count%(self.fps*saltos) == 0):
                 # resize image
                 resized = cv2.resize(image, dim, interpolation = cv2.INTER_AREA)
-                if(local):
+                if(runtime):
                     frames.append(resized)
                 else:
                     cv2.imwrite(self.frames_path+"%d.jpg" % count, resized)     # save frame as JPEG file  
             success,image = vidcap.read()
-            image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) # TODO revisar cambios necesarios para implementar solo escala de grises ( o dar la opcion de elegir)
+            if(not rgb):
+                image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) 
             count += 1
 
         self.frames = frames
         # -------------------------------------------------------------------------
 
         self.data = []
         self.slides = []
@@ -107,45 +120,42 @@
         return self.video_cap
     def get_frames(self):
         return self.frames
     # --------------- SETTERS ---------------
     def set_frames_path(self, frames_path):
         self.frames_path = frames_path
 
-    def set_data(self): # se setea la data segun este usandose de forma local o no
+    def set_data(self, me): # se setea la data segun este usandose de forma runtime o no
         """ Funcion que usando getqua() sobre frames ordenados entrega un array con los valores evaluados de frames contiguos
         -------------------------------------------------------
-        Input: TODO
-            posiciones (array): lista con posiciones de los frames elegios para conformar el conjunto final de diapositivas
+        Input:
+            No aplica
         Output:
             No aplica
         """
-        if(self.local):
-            self.data = fc.getdata(self.frames) # caso local 
-        else:
-            self.data = fc.getdata(self.frames_path) # caso NO local
+        self.data = fc.getdata(self.frames, me, self.rgb) # ambos casos cubiertos (runtime TRUE/FALSE)
 
-    def set_slides(self, posiciones = None):
+    def set_slides(self, me = 1, posiciones = None, coef = 3):
         """ divide y obtiene los frames que contienen la mayor parte de la informacion de cada slide
         -------------------------------------------------------
         Input:
-            posiciones (array): lista con posiciones de los frames elegios para conformar el conjunto final de diapositivas
+            posiciones (array): lista con posiciones de los frames elegios para conformar el conjunto final de diapositivas (opcional)
         Output:
             No aplica
         """
         if(posiciones != None):
             self.frames = [i for index, i in enumerate(self.frames) if index in posiciones]
         else:
             if (len(self.data) == 0):
-                self.set_data()
+                self.set_data(me)
                 msg = "No se tiene data, se ejecuta automaticamente el metodo set_data() para setearla en el atributo data"
                 warnings.warn(f"Warning........... {msg}")
 
             N = len(self.data) + 1
-            num_slides, pos_division = fc.localmin(self.data)
+            num_slides, pos_division = fc.localmin(self.data, coef)
             sets = []
             pos_division.append(N)
 
             j = 0
             array = []
             for i in range(N):
                 if (i <= pos_division[j]):
@@ -153,28 +163,120 @@
                 else:
                     sets.append(array)
                     j += 1
                     array = []
                     array.append(i)
                     
             sets.append(array)
-            self.slides = fc.last_ones(sets) # Se seleccionan los ultimos frames de cada conjunto 
+            self.slides = fc.select(sets, self.frames, 1, self.rgb, self.gpu_use) # 0 -> Se seleccionan los ultimos frames de cada conjunto 
 
-    def set_transcription(self):
+        self.frames = fc.delete_frames(self.frames, self.slides, 1)
+
+    def set_transcription(self, path = '', ocr = 1):
+        """ Transcribe las imagenes  contenidas en self.frames, ordena la data y la deja almacenada en un array o json (dependiendo de self.runtime)
+        -------------------------------------------------------
+        Input:
+            No aplica
+        Output:
+            No aplica
+        """
         if (len(self.slides) == 0):
             self.set_slides()
             msg = "No se tienen las slides, se ejecuta automaticamente el metodo set_slides() para setearla en el atributo slides"
             warnings.warn(f"Warning........... {msg}")
 
-        if(self.local):
-            self.transcription = fc.get_transcription(self.frames, self.slides, self.local) # caso local 
+        self.transcription = fc.get_transcription(self.video_name, self.frames, self.slides, self.rgb, self.runtime, self.gpu_use, path, ocr) # los dos casos cubiertos 
+
+    def clean_frames(self): 
+        """ Itera sobre los frames comparando usando metricas de calidad de imagen para eliminar las que sean consideradas suficientemente similares
+        para el caso de no estar runtime : se elimina el frame de la ruta 
+        caso runtime: se crea una nueva lista con los frames correspondientes y se retorna  
+        -------------------------------------------------------
+        Input:
+            No aplica
+        Output:
+            No aplica
+        """
+        if(self.runtime):
+            self.frames = fc.clean(self.frames, self.rgb, self.pix_lim, self.ssimv_lim)
         else:
-            self.transcription = fc.get_transcription(self.frames_path, self.slides, self.local) # caso NO local
+            fc.clean(self.frames, self.rgb, self.pix_lim, self.ssimv_lim)
+
+    def clean_transc(self):
+        """  Desde una transcripcion formateada se eliminan redundancias y luego se eliminan los frames:
+        runtime: se filtran sobre el array 
+        no runtime: se eliminan los archivos de la ruta de los frames
+        -------------------------------------------------------
+        Input:
+            No aplica
+        Output:
+            No aplica
+        """
+        self.transcription, lt_delet = fc.clean_transc(self.transcription)
+        self.frames = fc.delete_frames(self.frames, lt_delet)
 
-    def clean_frames(self): # TODO dar libertad de los rangos a los cuales se desea filtrar
-        if(self.local):
-            self.frames = fc.clean(self.frames)
+    def lematize(self):
+        """  Funcion aplica lematizacion sobre la transcripcion almacenada en self.transcription, reemplazando la original
+        -------------------------------------------------------
+        Input:
+            No aplica
+        Output:
+            No aplica
+        """
+        self.transcription = fc.lematize(self.transcription, self.gpu_use)
+
+    def improve_num(self):
+        """  Funcion corrige digitos de la transcripcion inicial, utilizando el OCR de Tesseract 
+        -------------------------------------------------------
+        Input:
+            No aplica
+        Output:
+            No aplica
+        """
+        # tomar frames finales
+        print("ENTRO")
+        transcription_tesse = fc.get_transcription(self.video_name, self.frames, [], self.rgb, self.runtime, self.gpu_use, 2) # los dos casos cubiertos 
+        print(transcription_tesse)
+
+    def improve_quality(self, model, ratio):
+        """  Funcion mejora calidad de imagenes, ya sea la lista de frames o frames guardados localmente
+        -------------------------------------------------------
+        Input:
+            No aplica
+            model
+            ratio
+        Output:
+            No aplica
+        """
+        # self.frames
+        if(self.runtime):
+            for index, frame in enumerate(self.frames):
+                self.frames[index] = fc.upscale_img(frame, model, ratio, self.runtime, self.gpu_use)
         else:
-            fc.clean(self.frames_path)
+            Frames = fc.ls(ruta = self.frames)
+            Frames.sort()
+            Frames = list(map(fc.addJ ,Frames))
+            for index, frame in enumerate(Frames):
+                fc.upscale_img(self.frames+frame, model, ratio, self.runtime, self.gpu_use)
 
 
 
+        # TODO: aplicar tesseract en los casos que se encuentre un digito o cifra en self.transcription (puede ir despues de lematization)
+        # TODO: REVISAR SI EXISTE ALGUNA FORMA DE ENTREGAR MAYOR VALOR A LA ESTRUCTURACION ( ETIQUETAS ? : TITTLE, COMMENT, NAMES, NUMBER OR DATES)
+
+
+        # TODO: REVISAR FORMAS DE OBTENER CONTEXTO DE INFO EN UNA LAMINA (QUIZAS FILTRAR Y OMITIR INFORMACION NO RELEVANTE)
+        # TODO: N-GRAMA PARA LA CORRECCION -> REVISAR QUE PALABRAS SE REPITEN MAS Y QUIZAR HACER UNA ANALISIS ESTADISTICO CON ESTO (UN PLUS (?))
+        # TODO: MENCIONAR QUE SE PUEDE MEJORAR EL CALCULO DE DISTANCIA ENTRE CUADRADOS DE TEXTO -> MEJORAR ESTRUCTURACION EN CASO DE TEXTO EN DIAGONAL
+        # TODO: quizas quitar parametros desde la definicion de la clase y dejaros seteables luego de su creacion
+        # TODO : dejar como parametro editable el limite para la limpieza por texto
+
+
+
+
+        # DONE: Dejar con el formato de result de EASYOCR el resultado obtenido con tesseract 
+        # DONE: MEJORAR FUNCION PARA ELEGIR FRAMES DESDE SLIDE (actual es last_one) -> AGREGAR A DOCUMENTO
+        # DONE: REVISAR QUE TAN UTIL SERIA EL RTF (no mucho, se puede agregar formato, y quizas imagenes, -> buscar valor o uso de los RTF)
+        
+        # DONE: eleccion de lematizar
+        # DONE dar libertad de los rangos a los cuales se desea filtrar
+        # DONE revisar cambios necesarios para implementar solo escala de grises ( o dar la opcion de elegir) -> agregar comparacion al documento
```

