# Comparing `tmp/prodiapy-2.4.tar.gz` & `tmp/prodiapy-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-2.4.tar", last modified: Sat May 13 16:16:42 2023, max compression
+gzip compressed data, was "prodiapy-2.5.tar", last modified: Wed May 17 08:02:23 2023, max compression
```

## Comparing `prodiapy-2.4.tar` & `prodiapy-2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 16:16:42.840177 prodiapy-2.4/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-2.4/LICENSE
--rw-rw-rw-   0        0        0     2668 2023-05-13 16:16:42.840177 prodiapy-2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2447 2023-05-13 16:16:26.000000 prodiapy-2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 16:16:42.832175 prodiapy-2.4/prodia/
--rw-rw-rw-   0        0        0      111 2023-05-10 09:58:54.000000 prodiapy-2.4/prodia/__init__.py
--rw-rw-rw-   0        0        0     2225 2023-05-05 10:09:12.000000 prodiapy-2.4/prodia/data.py
--rw-rw-rw-   0        0        0    10126 2023-05-13 16:13:31.000000 prodiapy-2.4/prodia/main.py
-drwxrwxrwx   0        0        0        0 2023-05-13 16:16:42.838176 prodiapy-2.4/prodiapy.egg-info/
--rw-rw-rw-   0        0        0     2668 2023-05-13 16:16:42.000000 prodiapy-2.4/prodiapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-05-13 16:16:42.000000 prodiapy-2.4/prodiapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 16:16:42.000000 prodiapy-2.4/prodiapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-13 16:16:42.000000 prodiapy-2.4/prodiapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 16:16:42.000000 prodiapy-2.4/prodiapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 16:16:42.840177 prodiapy-2.4/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-05-13 16:15:32.000000 prodiapy-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:02:23.230169 prodiapy-2.5/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-2.5/LICENSE
+-rw-rw-rw-   0        0        0     1039 2023-05-17 08:02:23.229170 prodiapy-2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-05-17 08:01:08.000000 prodiapy-2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 08:02:23.209890 prodiapy-2.5/prodia/
+-rw-rw-rw-   0        0        0      132 2023-05-17 08:01:33.000000 prodiapy-2.5/prodia/__init__.py
+-rw-rw-rw-   0        0        0     2290 2023-05-16 11:51:42.000000 prodiapy-2.5/prodia/data.py
+-rw-rw-rw-   0        0        0    15010 2023-05-17 07:59:57.000000 prodiapy-2.5/prodia/main.py
+drwxrwxrwx   0        0        0        0 2023-05-17 08:02:23.228170 prodiapy-2.5/prodiapy.egg-info/
+-rw-rw-rw-   0        0        0     1039 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 08:02:23.000000 prodiapy-2.5/prodiapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 08:02:23.230169 prodiapy-2.5/setup.cfg
+-rw-rw-rw-   0        0        0      396 2023-05-16 11:04:01.000000 prodiapy-2.5/setup.py
```

### Comparing `prodiapy-2.4/LICENSE` & `prodiapy-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-2.4/prodia/data.py` & `prodiapy-2.5/prodia/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,26 @@
     sd14 = "sdv1_4.ckpt [7460a6fa]"
     sd15 = "v1-5-pruned-emaonly.ckpt [81761151]"
     anyv3 = "anythingv3_0-pruned.ckpt [2700c435]"
     anyv4 = "anything-v4.5-pruned.ckpt [65745d25]"
     analog = "analog-diffusion-1.0.ckpt [9ca13f02]"
     theallys = "theallys-mix-ii-churned.safetensors [5d9225a4]"
     elldreths = "elldreths-vivid-mix.safetensors [342d9d26]"
-    delibrate = "deliberate_v2.safetensors [10ec4b29]"
+    deliberate = "deliberate_v2.safetensors [10ec4b29]"
     openjourney = "openjourney_V4.ckpt [ca2f377f]"
     dreaml1 = "dreamlike-diffusion-1.0.safetensors [5c9fd6e0]"
     dreaml2 = "dreamlike-diffusion-2.0.safetensors [fdcf65e7]"
     portrait = "portrait+1.0.safetensors [1400e684]"
     riffusion = "riffusion-model-v1.ckpt [3aafa6fe]"
     timeless = "timeless-1.0.ckpt [7c4971d4]"
     dreamsh = "dreamshaper_5BakedVae.safetensors [a3fbf318]"
     revA = "revAnimated_v122.safetensors [3f4fefd9]"
     meina = "meinamix_meinaV9.safetensors [2ec66ab0]"
     lyriel = "lyriel_v15.safetensors [65d547c5]"
+    realistic = "Realistic_Vision_V2.0.safetensors [79587710]"
     mlist = [
         "sdv1_4.ckpt [7460a6fa]",
         "v1-5-pruned-emaonly.ckpt [81761151]",
         "anythingv3_0-pruned.ckpt [2700c435]",
         "anything-v4.5-pruned.ckpt [65745d25]",
         "analog-diffusion-1.0.ckpt [9ca13f02]",
         "theallys-mix-ii-churned.safetensors [5d9225a4]",
```

### Comparing `prodiapy-2.4/prodia/main.py` & `prodiapy-2.5/prodia/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,30 +10,43 @@
     if api_key is None:
         print("No API key provided")
         return
     else:
         global key
         key = api_key
 
+def models():
+    print('Available models:')
+    print(Models.mlist)
+
+def samplers():
+    print('Available samplers:')
+    print(Samplers.slist)
+
+def aspect_ratios():
+    print('Available ratios:')
+    print(ar.alist)
+
 
 def txt2img(
-        prompt:str="kittens on cloud",
-        negative_prompt:str="bad drawn, low quality, low detailed, ugly, mutated, blurry, watermark",
-        model:str="deliberate_v2.safetensors [10ec4b29]",
+        prompt:str=None,
+        negative_prompt:str="badly draw",
+        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
         sampler:str="Heun",
         aspect_ratio:str="square",
         steps:int=25,
         cfg_scale:int=7,
         seed:int=-1,
         upscale:bool=False):
     if key is None:
         print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
     else:
-        if prompt == "kittens on cloud":
+        if prompt == None:
             print("LOG: Prompt was not defined, used default (kittens on cloud)")
+            prompt = "kittens on cloud"
         url = "https://api.prodia.com/v1/job"
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
@@ -43,59 +56,59 @@
             "aspect_ratio": aspect_ratio
         }
         headers = {
             "accept": "application/json",
             "content-type": "application/json",
             "X-Prodia-Key": key
         }
-        headersrecieve = {
+        headers2 = {
             "accept": "application/json",
             "X-Prodia-Key": key
         }
         print(f"LOG: txt2img image with params:\n{payload}")
         response = requests.post(url, json=payload, headers=headers)
         job_id = response.json()['job']
         time.sleep(3)
 
-        rec_url = f'https://api.prodia.com/v1/job/{job_id}'
+        retrieve_url = f'https://api.prodia.com/v1/job/{job_id}'
         stt = True
         while stt is True:
-            rec = requests.get(rec_url, headers=headersrecieve)
+            rec = requests.get(retrieve_url, headers=headersr2)
             status = rec.json()['status']
             if status == "succeeded":
                 print(f"Image {job_id} generated!")
                 image_url = rec.json()['imageUrl']
                 stt = False
                 return image_url
             elif status == "queued":
                 print("Still working...")
-                time.sleep(1)
+                time.sleep(2)
             elif status == "generating":
                 print("Still working...")
-                time.sleep(1)
+                time.sleep(2)
             else:
                 print(f"ERROR: Something went wrong! Please try later, error: {status}")
                 stt = False
                 return status
 
 
 def img2img(
         imageUrl:str=None,
-        model:str="deliberate_v2.safetensors [10ec4b29]",
+        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
         prompt:str=None,
         denoising_strength:float=0.7,
-        negative_prompt:str="badly drawn, low detailed, ugly, mutated, unralistic",
+        negative_prompt:str="badly drawn",
         steps:int=25,
         cfg_scale:int=7,
         seed:int=-1,
         upscale:bool=False,
         sampler:str="Heun"):
 
     if key is None:
-        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
+        print("ERROR: API key is corrupted or not defined, get your API key at https://app.prodia.com/api\nto define api key use:\nprodia.Client(api_key='your-key')")
     elif imageUrl is None:
         print("ERROR: Image URL is required and cannot be empty")
     elif prompt is None:
         print("ERROR: Prompt is required and cannot be empty")
     else:
         url = "https://api.prodia.com/v1/transform"
 
@@ -133,38 +146,102 @@
             if status == "succeeded":
                 print(f"LOG: Image {job_id} generated!")
                 image_url = rec.json()['imageUrl']
                 stt = False
                 return image_url
             elif status == "queued":
                 print("Still working...")
-                time.sleep(5)
+                time.sleep(3)
+            elif status == "generating":
+                print("Still working...")
+                time.sleep(3)
+            else:
+                print(f"ERROR: Something went wrong! Please try later, error: {status}")
+                stt = False
+                return status
+
+def control_net_scribble(
+        imageUrl:str=None,
+        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
+        prompt:str=None,
+        negative_prompt:str="badly drawn",
+        steps:int=25,
+        cfg_scale:int=7,
+        seed:int=-1,
+        sampler:str="Heun"):
+
+    if key is None:
+        print("ERROR: API key is corrupted or not defined, get your API key at https://app.prodia.com/api\nto define api key use:\nprodia.Client(api_key='your-key')")
+    elif imageUrl is None:
+        print("ERROR: Image URL is required and cannot be empty")
+    elif prompt is None:
+        print("ERROR: Prompt is required and cannot be empty")
+    else:
+        url = "https://api.prodia.com/v1/controlnet/scribble"
+
+        payload = {
+            "steps": steps,
+            "sampler": sampler,
+            "imageUrl": imageUrl,
+            "model": model,
+            "prompt": prompt,
+            "negative_prompt": negative_prompt,
+            "cfg_scale": cfg_scale,
+            "seed": seed
+        }
+        headers = {
+            "accept": "application/json",
+            "content-type": "application/json",
+            "X-Prodia-Key": key
+        }
+        headersrecieve = {
+            "accept": "application/json",
+            "X-Prodia-Key": key
+        }
+        print(f"LOG: control_net image with params:\n{payload}")
+        response = requests.post(url, json=payload, headers=headers)
+        job_id = response.json()['job']
+        time.sleep(5)
+
+        rec_url = f'https://api.prodia.com/v1/job/{job_id}'
+        stt = True
+        while stt is True:
+            rec = requests.get(rec_url, headers=headersrecieve)
+            status = rec.json()['status']
+            if status == "succeeded":
+                print(f"LOG: Image {job_id} generated!")
+                image_url = rec.json()['imageUrl']
+                stt = False
+                return image_url
+            elif status == "queued":
+                print("Still working...")
+                time.sleep(3)
             elif status == "generating":
                 print("Still working...")
-                time.sleep(5)
+                time.sleep(3)
             else:
                 print(f"ERROR: Something went wrong! Please try later, error: {status}")
                 stt = False
                 return status
 
 async def arunv1(
         prompt:str="kittens on cloud",
-        negative_prompt:str="bad drawn, low quality, low detailed, ugly, mutated, blurry, watermark",
-        model:str="deliberate_v2.safetensors [10ec4b29]",
+        negative_prompt:str="badly drawn",
+        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
         sampler:str="Heun",
         aspect_ratio:str="square",
         steps:int=25,
         cfg_scale:int=7,
         seed:int=-1,
         upscale:bool=False):
     if key is None:
-        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
+        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.Client(api_key='your-key')")
     else:
         if prompt == "kittens on cloud" or prompt == "" or prompt == " ":
-            print("LOG: Prompt was not defined, used default (kittens on cloud)")
+            print("LOG: Prompt was not defined or empty, used default (kittens on cloud)")
         url = "https://api.prodia.com/v1/job"
         payload = {
             "prompt": prompt,
             "model": model,
             "sampler": sampler,
             "negative_prompt": negative_prompt,
             "steps": steps,
@@ -195,27 +272,27 @@
             if status == "succeeded":
                 print(f"Image {job_id} generated!")
                 image_url = rec.json()['imageUrl']
                 stt = False
                 return image_url
             elif status == "queued":
                 print("Still working...")
-                await asyncio.sleep(1)
+                await asyncio.sleep(2)
             elif status == "generating":
                 print("Still working...")
-                await asyncio.sleep(1)
+                await asyncio.sleep(2)
             else:
                 print(f"ERROR: Something went wrong! Please try later, error: {status}")
                 stt = False
                 return status
 
 
 async def arunv2(
         imageUrl:str=None,
-        model:str="deliberate_v2.safetensors [10ec4b29]",
+        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
         prompt:str=None,
         denoising_strength:float=0.7,
         negative_prompt:str="badly drawn, low detailed, ugly, mutated, unralistic",
         steps:int=25,
         cfg_scale:int=7,
         seed:int=-1,
         upscale:bool=False,
@@ -273,9 +350,74 @@
                 print("Still working...")
                 await asyncio.sleep(2)
             else:
                 print(f"ERROR: Something went wrong! Please try later, error: {status}")
                 stt = False
                 return status
 
+async def arunv3(
+        imageUrl:str=None,
+        model:str="Realistic_Vision_V2.0.safetensors [79587710]",
+        prompt:str=None,
+        negative_prompt:str="badly drawn, low detailed, ugly, mutated, unralistic",
+        steps:int=25,
+        cfg_scale:int=7,
+        seed:int=-1,
+        sampler:str="Heun"):
+
+    if key is None:
+        print("ERROR: API key is corrupted or not defined, get your API kay at https://app.prodia.com/api\nto define api key use:\nprodia.api_key = 'your-key'")
+    elif imageUrl is None:
+        print("ERROR: Image URL is required and cannot be empty")
+    elif prompt is None:
+        print("ERROR: Prompt is required and cannot be empty")
+    else:
+        url = "https://api.prodia.com/v1/controlnet/scribble"
+
+        payload = {
+            "steps": steps,
+            "sampler": sampler,
+            "imageUrl": imageUrl,
+            "model": model,
+            "prompt": prompt,
+            "negative_prompt": negative_prompt,
+            "cfg_scale": cfg_scale,
+            "seed": seed
+        }
+        headers = {
+            "accept": "application/json",
+            "content-type": "application/json",
+            "X-Prodia-Key": key
+        }
+        headersrecieve = {
+            "accept": "application/json",
+            "X-Prodia-Key": key
+        }
+        print(f"LOG: img2img image with params:\n{payload}")
+        response = requests.post(url, json=payload, headers=headers)
+        job_id = response.json()['job']
+        await asyncio.sleep(4)
+
+        rec_url = f'https://api.prodia.com/v1/job/{job_id}'
+        stt = True
+        while stt is True:
+            rec = requests.get(rec_url, headers=headersrecieve)
+            status = rec.json()['status']
+            if status == "succeeded":
+                print(f"LOG: Image {job_id} generated!")
+                image_url = rec.json()['imageUrl']
+                stt = False
+                return image_url
+            elif status == "queued":
+                print("Still working...")
+                await asyncio.sleep(2)
+            elif status == "generating":
+                print("Still working...")
+                await asyncio.sleep(2)
+            else:
+                print(f"ERROR: Something went wrong! Please try later, error: {status}")
+                stt = False
+                return status
+
+
```

