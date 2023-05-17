# Comparing `tmp/irene_pro-0.0.34.tar.gz` & `tmp/irene_pro-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.34.tar", last modified: Mon May 15 13:46:15 2023, max compression
+gzip compressed data, was "irene_pro-0.0.35.tar", last modified: Wed May 17 12:51:36 2023, max compression
```

## Comparing `irene_pro-0.0.34.tar` & `irene_pro-0.0.35.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 13:46:15.676083 irene_pro-0.0.34/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.34/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.34/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-05-15 13:46:15.671095 irene_pro-0.0.34/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-05-11 07:56:46.000000 irene_pro-0.0.34/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 13:46:15.634194 irene_pro-0.0.34/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.34/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.34/irene_pro/logic.py
--rw-rw-rw-   0        0        0    25421 2023-05-15 13:43:48.000000 irene_pro-0.0.34/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-15 13:46:15.663116 irene_pro-0.0.34/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-05-15 13:46:15.000000 irene_pro-0.0.34/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-15 13:46:15.000000 irene_pro-0.0.34/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 13:46:15.000000 irene_pro-0.0.34/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-15 13:46:15.000000 irene_pro-0.0.34/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 13:46:15.000000 irene_pro-0.0.34/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 13:46:15.677079 irene_pro-0.0.34/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-15 13:44:53.000000 irene_pro-0.0.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 12:51:36.016281 irene_pro-0.0.35/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.35/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.35/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-05-17 12:51:36.014288 irene_pro-0.0.35/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-05-11 07:56:46.000000 irene_pro-0.0.35/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 12:51:35.995337 irene_pro-0.0.35/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.35/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-11 09:46:57.000000 irene_pro-0.0.35/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    25403 2023-05-17 12:43:44.000000 irene_pro-0.0.35/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-17 12:51:36.011303 irene_pro-0.0.35/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-05-17 12:51:35.000000 irene_pro-0.0.35/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-17 12:51:35.000000 irene_pro-0.0.35/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 12:51:35.000000 irene_pro-0.0.35/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-17 12:51:35.000000 irene_pro-0.0.35/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 12:51:35.000000 irene_pro-0.0.35/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 12:51:36.016281 irene_pro-0.0.35/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-17 12:50:50.000000 irene_pro-0.0.35/setup.py
```

### Comparing `irene_pro-0.0.34/PKG-INFO` & `irene_pro-0.0.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene_pro
-Version: 0.0.34
+Version: 0.0.35
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.34/README.md` & `irene_pro-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.34/irene_pro/logic.py` & `irene_pro-0.0.35/irene_pro/logic.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.34/irene_pro/widgets.py` & `irene_pro-0.0.35/irene_pro/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,28 @@
         num = re.compile("\d{1,}")
         try:
             found_num = num.findall(master['bg'])
             if found_num:
                 text = master['bg'][:master['bg'].index(found_num[0])]
                 num = int(master['bg'][master['bg'].index(found_num[0]):]) - 3
                 self.config(bg = text+str(num))
-        except (TypeError, ValueError):
+        except Exception:
             pass
 
 class lframe(LabelFrame):
     def __init__(self, master, **kwargs):
         super().__init__(master = master, font = ('arial', w(12)), bd=0, fg = "gray20", labelanchor='ne', **kwargs)
         num = re.compile("\d{1,}")
         try:
             found_num = num.findall(master['bg'])
             if found_num:
                 text = master['bg'][:master['bg'].index(found_num[0])]
                 num = int(master['bg'][master['bg'].index(found_num[0]):]) - 3
                 self.config(bg = text+str(num))
-        except TypeError:
+        except Exception:
             pass
 
 class treeview(ttk.Treeview):
     def __init__(self, master, columns, col_width = w(130), rowheight = h(100),include_index = False, **kwargs) -> None:
         super().__init__(master, **kwargs)
         self.master = master
 
@@ -297,15 +297,15 @@
         num = re.compile("\d{1,}")
         try:
             found_num = num.findall(master['bg'])
             if found_num:
                 text = master['bg'][:master['bg'].index(found_num[0])]
                 num = int(master['bg'][master['bg'].index(found_num[0]):]) - 3
                 self.config(bg = text+str(num))
-        except TypeError:
+        except Exception:
             pass
 
         def remove_txt():
             if default.strip() in str(self.get()).strip():
                 self.delete(0, END)
                 self.config(fg = "#000")
         
@@ -373,15 +373,15 @@
         num = re.compile("\d{1,}")
         try:
             found_num = num.findall(master['bg'])
             if found_num:
                 text = master['bg'][:master['bg'].index(found_num[0])]
                 num = int(master['bg'][master['bg'].index(found_num[0]):]) - 3
                 self.config(bg = text+str(num))
-        except TypeError:
+        except Exception:
             pass
 
     def scr_fr(self):
         return self.Scrol_frame
 
 class label(Label):
     def __init__(self, master, **kwargs):
@@ -409,19 +409,18 @@
         num = re.compile("\d{1,}")
         try:
             found_num = num.findall(master['bg'])
             if found_num:
                 text = master['bg'][:master['bg'].index(found_num[0])]
                 num = int(master['bg'][master['bg'].index(found_num[0]):]) - 3
                 self.config(bg = text+str(num))
-        except TypeError:
+        except Exception:
             pass
 
 
-
 class spinbox(ttk.Spinbox):
     def __init__(self, master, **kwargs):
         super().__init__(master =master, **kwargs)
 
 class calendar(Calendar):
     def __init__(self, master, global_date_holder:Variable, date_holder_widget = None, create_toplevel = False, **kw):
         super().__init__(master = master, **kw)
@@ -605,12 +604,11 @@
     
     def final_data(self):
         # BY NOW, THE DATAFRAME WILL BE BEING DISLPLAY IN THE TERMINAL
         nd = np.array(self.data)
         transposed_data = nd.T
         return transposed_data.tolist()
 
-
 # CONSTANTS
 comb_syle = 'comb.TCombobox'
 check_style = "TCheckbutton"
 radio_style = "Custom.TRadiobutton"
```

### Comparing `irene_pro-0.0.34/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.35/irene_pro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irene-pro
-Version: 0.0.34
+Version: 0.0.35
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.34/setup.py` & `irene_pro-0.0.35/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3334 270d 0a44 4553 4352   '0.0.34'..DESCR
+00000100: 2027 302e 302e 3335 270d 0a44 4553 4352   '0.0.35'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

