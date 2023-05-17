# Comparing `tmp/CTkColorPicker-0.5.0.tar.gz` & `tmp/CTkColorPicker-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkColorPicker-0.5.0.tar", last modified: Fri Apr 14 11:22:56 2023, max compression
+gzip compressed data, was "CTkColorPicker-0.6.0.tar", last modified: Wed May 17 13:58:11 2023, max compression
```

## Comparing `CTkColorPicker-0.5.0.tar` & `CTkColorPicker-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 11:22:56.306281 CTkColorPicker-0.5.0/
-drwxrwxrwx   0        0        0        0 2023-04-14 11:22:56.286117 CTkColorPicker-0.5.0/CTkColorPicker/
--rw-rw-rw-   0        0        0      221 2023-04-14 10:14:45.000000 CTkColorPicker-0.5.0/CTkColorPicker/__init__.py
--rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 CTkColorPicker-0.5.0/CTkColorPicker/color_wheel.png
--rw-rw-rw-   0        0        0     9078 2023-04-14 11:17:37.000000 CTkColorPicker-0.5.0/CTkColorPicker/ctk_color_picker.py
--rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 CTkColorPicker-0.5.0/CTkColorPicker/target.png
-drwxrwxrwx   0        0        0        0 2023-04-14 11:22:56.306281 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/
--rw-rw-rw-   0        0        0     2601 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkColorPicker-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     2601 2023-04-14 11:22:56.306281 CTkColorPicker-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1922 2023-04-14 11:20:38.000000 CTkColorPicker-0.5.0/README.md
--rw-rw-rw-   0        0        0      607 2023-04-14 11:22:56.318617 CTkColorPicker-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-04-14 11:19:22.000000 CTkColorPicker-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 13:58:11.580203 CTkColorPicker-0.6.0/
+drwxrwxrwx   0        0        0        0 2023-05-17 13:58:11.548954 CTkColorPicker-0.6.0/CTkColorPicker/
+-rw-rw-rw-   0        0        0      272 2023-05-17 13:38:07.000000 CTkColorPicker-0.6.0/CTkColorPicker/__init__.py
+-rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 CTkColorPicker-0.6.0/CTkColorPicker/color_wheel.png
+-rw-rw-rw-   0        0        0     9081 2023-05-17 13:36:46.000000 CTkColorPicker-0.6.0/CTkColorPicker/ctk_color_picker.py
+-rw-rw-rw-   0        0        0     7068 2023-05-17 13:51:56.000000 CTkColorPicker-0.6.0/CTkColorPicker/ctk_color_picker_widget.py
+-rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 CTkColorPicker-0.6.0/CTkColorPicker/target.png
+drwxrwxrwx   0        0        0        0 2023-05-17 13:58:11.564578 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/
+-rw-rw-rw-   0        0        0     3653 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-17 13:58:11.000000 CTkColorPicker-0.6.0/CTkColorPicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkColorPicker-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     3653 2023-05-17 13:58:11.580203 CTkColorPicker-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2974 2023-05-17 13:55:59.000000 CTkColorPicker-0.6.0/README.md
+-rw-rw-rw-   0        0        0      607 2023-05-17 13:58:11.580203 CTkColorPicker-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-05-17 13:54:31.000000 CTkColorPicker-0.6.0/setup.py
```

### Comparing `CTkColorPicker-0.5.0/CTkColorPicker/color_wheel.png` & `CTkColorPicker-0.6.0/CTkColorPicker/color_wheel.png`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.5.0/CTkColorPicker/ctk_color_picker.py` & `CTkColorPicker-0.6.0/CTkColorPicker/ctk_color_picker.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         
         self.bg_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"]) if bg_color is None else bg_color
         self.fg_color = self.fg_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"]) if fg_color is None else fg_color
         self.button_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkButton"]["fg_color"]) if button_color is None else button_color
         self.button_hover_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkButton"]["hover_color"]) if button_hover_color is None else button_hover_color
         self.button_text = text
         self.corner_radius = corner_radius
-        self.slider_width = 10 if slider_border>=10 else slider_border
+        self.slider_border = 10 if slider_border>=10 else slider_border
         
         self.config(bg=self.bg_color)
         
         self.frame = customtkinter.CTkFrame(master=self, fg_color=self.fg_color, bg_color=self.bg_color)
         self.frame.grid(padx=20, pady=20, sticky="nswe")
           
         self.canvas = tkinter.Canvas(self.frame, height=self.image_dimension, width=self.image_dimension, highlightthickness=0, bg=self.fg_color)
@@ -79,21 +79,21 @@
         
         self.canvas.create_image(self.image_dimension/2, self.image_dimension/2, image=self.wheel)
         self.set_initial_color(initial_color)
         
         self.brightness_slider_value = customtkinter.IntVar()
         self.brightness_slider_value.set(255)
         
-        self.slider = customtkinter.CTkSlider(master=self.frame, height=20, border_width=self.slider_width,
+        self.slider = customtkinter.CTkSlider(master=self.frame, height=20, border_width=self.slider_border,
                                               button_length=15, progress_color=self.default_hex_color, from_=0, to=255,
                                               variable=self.brightness_slider_value, number_of_steps=256,
                                               button_corner_radius=self.corner_radius, corner_radius=self.corner_radius,
                                               button_color=self.button_color, button_hover_color=self.button_hover_color,
                                               command=lambda x:self.update_colors())
-        self.slider.pack(fill="both", pady=(0,15), padx=20-self.slider_width)
+        self.slider.pack(fill="both", pady=(0,15), padx=20-self.slider_border)
 
         self.label = customtkinter.CTkLabel(master=self.frame, text_color="#000000", height=50, fg_color=self.default_hex_color,
                                             corner_radius=self.corner_radius, text=self.default_hex_color)
         self.label.pack(fill="both", padx=10)
         
         self.button = customtkinter.CTkButton(master=self.frame, text=self.button_text, height=50, corner_radius=self.corner_radius, fg_color=self.button_color,
                                               hover_color=self.button_hover_color, command=self._ok_event, **button_kwargs)
```

### Comparing `CTkColorPicker-0.5.0/CTkColorPicker/target.png` & `CTkColorPicker-0.6.0/CTkColorPicker/target.png`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.5.0/CTkColorPicker.egg-info/PKG-INFO` & `CTkColorPicker-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: CTkColorPicker
-Version: 0.5.0
-Summary: A modern color picker for customtkinter
-Home-page: https://github.com/Akascape/CTkColorPicker
-Author: Akash Bora
-License: Creative Commons Zero v1.0 Universal
-Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CTkColorPicker
 **A modern color picker made for customtkinter!**
 
 ![Screenshot](https://user-images.githubusercontent.com/89206401/209182773-d76bf05c-610e-4297-aec5-7bb61a11d6d3.jpg)
 
 ## Download
 
@@ -29,38 +14,65 @@
 ## Requirements
 - [customtkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [pillow](https://pypi.org/project/Pillow/)
 
 ### How to use?
 ```python
 import customtkinter as ctk
-from CTkColorPicker import AskColor
+from CTkColorPicker import *
 
 def ask_color():
     pick_color = AskColor() # open the color picker
     color = pick_color.get() # get the color string
     button.configure(fg_color=color)
     
 root = ctk.CTk()
 
 button = ctk.CTkButton(master=root, text="CHOOSE COLOR", text_color="black", command=ask_color)
 button.pack(padx=30, pady=20)
 root.mainloop()
 ```
 
-# Options
+## Options
 | Arguments | Description |
 |---------|-------------|
 | width | set the overall size of the color picker window |
 | title | change the title of color picker window |
 | fg_color | change forground color of the color picker frame |
 | bg_color | change background color of the color picker frame |
 | button_color | change the color of the button and slider |
 | button_hover_color | change the hover color of the buttons |
 | text | change the default text of the 'OK' button |
 | initial_color | set the default color of color picker (currently in beta stage) |
 | slider_border | change the border width of slider |
 | corner_radius | change the corner radius of all the widgets inside color picker |
 | _**other button parameters_ | pass other button arguments if required |
 
+# ColorPickerWidget
+**This is a new color picker widget that can be placed inside a customtkinter frame.**
+
+![Screenshot 2023-05-17 191125](https://github.com/Akascape/CTkColorPicker/assets/89206401/ca03751a-90a3-45e6-8ba4-745a92ab1c12)
+
+### Usage
+```python
+from CTkColorPicker import *
+import customtkinter
+
+root = customtkinter.CTk()
+colorpicker = CTkColorPicker(root, width=500, command=lambda e: print(e))
+colorpicker.pack(padx=10, pady=10)
+root.mainloop()
+```
+
+## Options
+| Arguments | Description |
+|---------|-------------|
+| master | parent widget |
+| width | set the overall size of the color picker frame |
+| fg_color | change forground color of the color picker frame |
+| initial_color | set the default color of color picker (currently in beta stage) |
+| slider_border | change the border width of slider |
+| corner_radius | change the corner radius of all the widgets inside color picker |
+| command | add a command when the color is changed |
+| _**other slider parameters_ | pass other slider arguments if required |
 
 **That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.5.0/LICENSE` & `CTkColorPicker-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.5.0/PKG-INFO` & `CTkColorPicker-0.6.0/CTkColorPicker.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkColorPicker
-Version: 0.5.0
+Version: 0.6.0
 Summary: A modern color picker for customtkinter
 Home-page: https://github.com/Akascape/CTkColorPicker
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -29,38 +29,65 @@
 ## Requirements
 - [customtkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [pillow](https://pypi.org/project/Pillow/)
 
 ### How to use?
 ```python
 import customtkinter as ctk
-from CTkColorPicker import AskColor
+from CTkColorPicker import *
 
 def ask_color():
     pick_color = AskColor() # open the color picker
     color = pick_color.get() # get the color string
     button.configure(fg_color=color)
     
 root = ctk.CTk()
 
 button = ctk.CTkButton(master=root, text="CHOOSE COLOR", text_color="black", command=ask_color)
 button.pack(padx=30, pady=20)
 root.mainloop()
 ```
 
-# Options
+## Options
 | Arguments | Description |
 |---------|-------------|
 | width | set the overall size of the color picker window |
 | title | change the title of color picker window |
 | fg_color | change forground color of the color picker frame |
 | bg_color | change background color of the color picker frame |
 | button_color | change the color of the button and slider |
 | button_hover_color | change the hover color of the buttons |
 | text | change the default text of the 'OK' button |
 | initial_color | set the default color of color picker (currently in beta stage) |
 | slider_border | change the border width of slider |
 | corner_radius | change the corner radius of all the widgets inside color picker |
 | _**other button parameters_ | pass other button arguments if required |
 
+# ColorPickerWidget
+**This is a new color picker widget that can be placed inside a customtkinter frame.**
+
+![Screenshot 2023-05-17 191125](https://github.com/Akascape/CTkColorPicker/assets/89206401/ca03751a-90a3-45e6-8ba4-745a92ab1c12)
+
+### Usage
+```python
+from CTkColorPicker import *
+import customtkinter
+
+root = customtkinter.CTk()
+colorpicker = CTkColorPicker(root, width=500, command=lambda e: print(e))
+colorpicker.pack(padx=10, pady=10)
+root.mainloop()
+```
+
+## Options
+| Arguments | Description |
+|---------|-------------|
+| master | parent widget |
+| width | set the overall size of the color picker frame |
+| fg_color | change forground color of the color picker frame |
+| initial_color | set the default color of color picker (currently in beta stage) |
+| slider_border | change the border width of slider |
+| corner_radius | change the corner radius of all the widgets inside color picker |
+| command | add a command when the color is changed |
+| _**other slider parameters_ | pass other slider arguments if required |
 
 **That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.5.0/README.md` & `CTkColorPicker-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: CTkColorPicker
+Version: 0.6.0
+Summary: A modern color picker for customtkinter
+Home-page: https://github.com/Akascape/CTkColorPicker
+Author: Akash Bora
+License: Creative Commons Zero v1.0 Universal
+Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CTkColorPicker
 **A modern color picker made for customtkinter!**
 
 ![Screenshot](https://user-images.githubusercontent.com/89206401/209182773-d76bf05c-610e-4297-aec5-7bb61a11d6d3.jpg)
 
 ## Download
 
@@ -14,38 +29,65 @@
 ## Requirements
 - [customtkinter](https://github.com/TomSchimansky/CustomTkinter)
 - [pillow](https://pypi.org/project/Pillow/)
 
 ### How to use?
 ```python
 import customtkinter as ctk
-from CTkColorPicker import AskColor
+from CTkColorPicker import *
 
 def ask_color():
     pick_color = AskColor() # open the color picker
     color = pick_color.get() # get the color string
     button.configure(fg_color=color)
     
 root = ctk.CTk()
 
 button = ctk.CTkButton(master=root, text="CHOOSE COLOR", text_color="black", command=ask_color)
 button.pack(padx=30, pady=20)
 root.mainloop()
 ```
 
-# Options
+## Options
 | Arguments | Description |
 |---------|-------------|
 | width | set the overall size of the color picker window |
 | title | change the title of color picker window |
 | fg_color | change forground color of the color picker frame |
 | bg_color | change background color of the color picker frame |
 | button_color | change the color of the button and slider |
 | button_hover_color | change the hover color of the buttons |
 | text | change the default text of the 'OK' button |
 | initial_color | set the default color of color picker (currently in beta stage) |
 | slider_border | change the border width of slider |
 | corner_radius | change the corner radius of all the widgets inside color picker |
 | _**other button parameters_ | pass other button arguments if required |
 
+# ColorPickerWidget
+**This is a new color picker widget that can be placed inside a customtkinter frame.**
+
+![Screenshot 2023-05-17 191125](https://github.com/Akascape/CTkColorPicker/assets/89206401/ca03751a-90a3-45e6-8ba4-745a92ab1c12)
+
+### Usage
+```python
+from CTkColorPicker import *
+import customtkinter
+
+root = customtkinter.CTk()
+colorpicker = CTkColorPicker(root, width=500, command=lambda e: print(e))
+colorpicker.pack(padx=10, pady=10)
+root.mainloop()
+```
+
+## Options
+| Arguments | Description |
+|---------|-------------|
+| master | parent widget |
+| width | set the overall size of the color picker frame |
+| fg_color | change forground color of the color picker frame |
+| initial_color | set the default color of color picker (currently in beta stage) |
+| slider_border | change the border width of slider |
+| corner_radius | change the corner radius of all the widgets inside color picker |
+| command | add a command when the color is changed |
+| _**other slider parameters_ | pass other slider arguments if required |
 
 **That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.5.0/setup.cfg` & `CTkColorPicker-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 436f 6c6f 7250 6963 6b65   = CTkColorPicke
-00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e35  r..version = 0.5
+00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e36  r..version = 0.6
 00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000040: 3d20 4120 6d6f 6465 726e 2063 6f6c 6f72  = A modern color
 00000050: 2070 6963 6b65 7220 666f 7220 6375 7374   picker for cust
 00000060: 6f6d 746b 696e 7465 720d 0a6c 6f6e 675f  omtkinter..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
```

### Comparing `CTkColorPicker-0.5.0/setup.py` & `CTkColorPicker-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkColorPicker',
-    version = '0.5.0',
+    version = '0.6.0',
     description = "A modern color picker for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkColorPicker",
```

