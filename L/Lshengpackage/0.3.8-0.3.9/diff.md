# Comparing `tmp/Lshengpackage-0.3.8.tar.gz` & `tmp/Lshengpackage-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lshengpackage-0.3.8.tar", last modified: Sun May 14 08:46:08 2023, max compression
+gzip compressed data, was "Lshengpackage-0.3.9.tar", last modified: Wed May 17 14:04:55 2023, max compression
```

## Comparing `Lshengpackage-0.3.8.tar` & `Lshengpackage-0.3.9.tar`

### file list

```diff
@@ -1,43 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.227055 Lshengpackage-0.3.8/
--rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.3.8/LICENSE
--rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.3.8/License.md
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.191886 Lshengpackage-0.3.8/Lshengpackage/
--rw-rw-rw-   0        0        0       49 2023-05-14 01:06:32.000000 Lshengpackage-0.3.8/Lshengpackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.201396 Lshengpackage-0.3.8/Lshengpackage/simulate/
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.203396 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/
--rw-rw-rw-   0        0        0     2689 2023-05-14 07:49:17.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/Command_adb.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.204901 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/__pycache__/
--rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.210918 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/
--rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Pac_dm.py
--rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Reg.py
--rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Win_dm.py
--rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.217048 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/
--rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
--rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
--rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/mock_findFr.py
--rw-rw-rw-   0        0        0     2364 2023-05-14 04:20:16.000000 Lshengpackage-0.3.8/Lshengpackage/simulate/mock_findPic.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.225052 Lshengpackage-0.3.8/Lshengpackage/tools/
--rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.3.8/Lshengpackage/tools/ChaoJiYing.py
--rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.3.8/Lshengpackage/tools/General.py
--rw-rw-rw-   0        0        0      900 2023-05-14 04:31:40.000000 Lshengpackage-0.3.8/Lshengpackage/tools/Loading.py
--rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.3.8/Lshengpackage/tools/OperateFile.py
--rw-rw-rw-   0        0        0     2059 2023-05-14 04:52:50.000000 Lshengpackage-0.3.8/Lshengpackage/tools/SearchFile.py
--rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.8/Lshengpackage/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:46:08.197885 Lshengpackage-0.3.8/Lshengpackage.egg-info/
--rw-rw-rw-   0        0        0      858 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1121 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-14 08:46:08.000000 Lshengpackage-0.3.8/Lshengpackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      242 2023-05-14 03:32:07.000000 Lshengpackage-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2023-05-14 08:46:08.227055 Lshengpackage-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.3.8/README.md
--rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.3.8/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-14 08:46:08.228053 Lshengpackage-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2056 2023-05-14 08:46:01.000000 Lshengpackage-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.227382 Lshengpackage-0.3.9/
+-rw-rw-rw-   0        0        0     1079 2022-05-04 09:06:22.000000 Lshengpackage-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0     1077 2022-05-04 09:06:22.000000 Lshengpackage-0.3.9/License.md
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.186549 Lshengpackage-0.3.9/Lshengpackage/
+-rw-rw-rw-   0        0        0      719 2023-05-17 13:46:03.000000 Lshengpackage-0.3.9/Lshengpackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.195159 Lshengpackage-0.3.9/Lshengpackage/simulate/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:17:48.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.198858 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/
+-rw-rw-rw-   0        0        0     3318 2023-05-17 13:41:00.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/Command_adb.py
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.199862 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/__pycache__/
+-rw-rw-rw-   0        0        0      162 2022-10-10 08:45:14.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.202858 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/dingtalk/
+-rw-rw-rw-   0        0        0       51 2022-10-10 06:18:05.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/dingtalk/__init__.py
+-rw-rw-rw-   0        0        0     7181 2023-05-17 13:41:00.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
+-rw-rw-rw-   0        0        0  3646951 2023-05-17 12:12:22.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/dingtalk/image_data.py
+-rw-rw-rw-   0        0        0     1629 2023-05-17 13:41:00.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/adb/re_Pic.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.212863 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/
+-rw-rw-rw-   0        0        0     4677 2022-05-04 09:06:22.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/Pac_dm.py
+-rw-rw-rw-   0        0        0      314 2023-05-14 01:06:32.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/Reg.py
+-rw-rw-rw-   0        0        0     9334 2022-05-04 09:06:22.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/Win_dm.py
+-rw-rw-rw-   0        0        0       49 2022-10-10 06:18:05.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.218866 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__pycache__/
+-rw-rw-rw-   0        0        0     4816 2022-10-10 08:45:14.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      565 2022-10-10 08:45:14.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1262 2022-10-10 08:45:14.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      161 2022-10-10 08:45:14.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      286 2022-06-29 01:11:38.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/mock_findFr.py
+-rw-rw-rw-   0        0        0     2371 2023-05-14 10:04:42.000000 Lshengpackage-0.3.9/Lshengpackage/simulate/mock_findPic.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.226382 Lshengpackage-0.3.9/Lshengpackage/tools/
+-rw-rw-rw-   0        0        0     1988 2022-05-26 11:29:53.000000 Lshengpackage-0.3.9/Lshengpackage/tools/ChaoJiYing.py
+-rw-rw-rw-   0        0        0      759 2023-05-14 04:52:50.000000 Lshengpackage-0.3.9/Lshengpackage/tools/General.py
+-rw-rw-rw-   0        0        0     1724 2023-05-17 12:59:31.000000 Lshengpackage-0.3.9/Lshengpackage/tools/Loading.py
+-rw-rw-rw-   0        0        0     3305 2023-05-14 01:56:09.000000 Lshengpackage-0.3.9/Lshengpackage/tools/OperateFile.py
+-rw-rw-rw-   0        0        0     2059 2023-05-14 04:52:50.000000 Lshengpackage-0.3.9/Lshengpackage/tools/SearchFile.py
+-rw-rw-rw-   0        0        0       49 2023-05-14 09:58:14.000000 Lshengpackage-0.3.9/Lshengpackage/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 14:04:55.192503 Lshengpackage-0.3.9/Lshengpackage.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-05-17 14:04:55.000000 Lshengpackage-0.3.9/Lshengpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-17 14:04:55.000000 Lshengpackage-0.3.9/Lshengpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 14:04:55.000000 Lshengpackage-0.3.9/Lshengpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-17 14:04:55.000000 Lshengpackage-0.3.9/Lshengpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-17 14:04:55.000000 Lshengpackage-0.3.9/Lshengpackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      242 2023-05-14 03:32:07.000000 Lshengpackage-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2023-05-17 14:04:55.227382 Lshengpackage-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3975 2023-05-14 07:50:08.000000 Lshengpackage-0.3.9/README.md
+-rw-rw-rw-   0        0        0      350 2023-05-14 03:44:13.000000 Lshengpackage-0.3.9/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-17 14:04:55.229381 Lshengpackage-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1987 2023-05-17 13:34:10.000000 Lshengpackage-0.3.9/setup.py
```

### Comparing `Lshengpackage-0.3.8/LICENSE` & `Lshengpackage-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/License.md` & `Lshengpackage-0.3.9/License.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/simulate/adb/Command_adb.py` & `Lshengpackage-0.3.9/Lshengpackage/simulate/adb/Command_adb.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,22 +5,39 @@
 from PIL import Image
 import os
 
 
 class command:
     def dev(self):
         # 查看当前链接设备
-        com = os.system('adb devices')
+        com = os.popen('adb devices').read()
+        return com
+
+    #
+    def state(self):
+        # 返回连接状态
+        com = os.popen('adb get-state').read()
+        return com
+
+    #
+    def connect(self, ip):
+        # 连接ip+端口号
+        com = os.popen('adb connect {}'.format(ip)).read()
+        return com
+
+    #
+    def insert(self, text):
+        com = os.system('adb shell input text {}'.format(text))  # 输入文本
         return com
 
     def log(self):
         # 查看日志
-        com = os.system('adb logcat')
+        com = os.popen('adb logcat').read()
         return com
-    
+
     def kill(self):
         # 结束adb服务
         com = os.system('adb kill-server')
         return com
 
     def star(self):
         # 开始adb服务
@@ -33,53 +50,53 @@
         return com
 
     def uninstall(self, apk_name):
         # 卸载
         com = os.system('adb uninstall {}.apk'.format(apk_name))
         return com
 
-    def up(self, file_name, path_phone):
+    def update(self, file_name, path_phone):
         # 上传SDCard/../..手机端路径
         com = os.system('adb push {} {}'.format(file_name, path_phone))
         return com
 
-    def down(self, file_name):
+    def download(self, file_name):
         # 下载
         com = os.system('adb uninstall {}'.format(file_name))
         return com
 
     def scr(self, path_pic_name):
         # 屏幕截图到手机根目录
         com = os.system('adb shell screencap -p /sdcard/{}.png'.format(path_pic_name))
         return com
 
     def video_scr(self, video_name):
         # 录屏，默认mp4格式
         com = os.system('adb shell screenrecord /sdcard/{}.mp4'.format(video_name))
         return com
 
-    def cut_scr(self, path_pic_name, path):
+    def cut_scr(self, fol_path):
         # 屏幕截图到本地
         # pic_name:屏幕截图生成地址+名称，默认为手机的根目录,默认的来
         # path为文件夹目录下
-        self.scr(path_pic_name)
-        com = os.system("adb pull /sdcard/{} {}{}.png".format(path_pic_name, path, path_pic_name))
+        self.scr(fol_path.split('\\')[-1])
+        com = os.system("adb pull /sdcard/{}.png {}".format(fol_path.split('\\')[-1], fol_path))
         ImageFile.LOAD_TRUNCATED_IMAGES = True
         return com
 
-    def spec_scr(self, pic_name, path, int_x1, int_y1, int_x2, int_y2):
+    def spec_scr(self, pic_path, int_x1, int_y1, int_x2, int_y2):
         """
         指定截图保存
         左上角的点到右下角的点
         """
-        self.cut_scr(pic_name, path)
-        img = Image.open(path + pic_name)
+        self.cut_scr(pic_path)
+        img = Image.open(pic_path)
         # (4)将图片验证码截取
         code_image = img.crop((int_x1, int_y1, int_x2, int_y2))
-        code_image.save(path + pic_name)  # 原地址重写
+        code_image.save(pic_path)  # 原地址重写
         return True
 
     def tap_work(self, x, y):
         """
         模拟点击操作
         """
         com = os.system('adb shell input tap {} {}'.format(x, y))
@@ -87,7 +104,12 @@
 
     def swip_work(self, x, y, x2, y2):
         """
         模拟滑动操作
         """
         com = os.system('adb shell input swipe {} {} {} {}'.format(x, y, x2, y2))
         return com
+
+    def get_ui(self, path):
+        re = os.popen('adb shell uiautomator dump /sdcard/ui.xml')  # 获得屏幕控件信息
+        re = os.popen(r'adb pull /sdcard/ui.xml {}+ui.xml'.format(path))  # 获得屏幕控件信息
+        return re
```

### Comparing `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Pac_dm.py` & `Lshengpackage-0.3.9/Lshengpackage/simulate/dm/Pac_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/Win_dm.py` & `Lshengpackage-0.3.9/Lshengpackage/simulate/dm/Win_dm.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc` & `Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc` & `Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc` & `Lshengpackage-0.3.9/Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/simulate/mock_findPic.py` & `Lshengpackage-0.3.9/Lshengpackage/simulate/mock_findPic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from time import sleep
 import os
 import sys
 import cv2
 import pyautogui
-from adb.Command_adb import command
+from .adb.Command_adb import command
 from PIL import Image
 
 
 # 截图
-def screen_shot(fol_path,scr_name):
+def screen_shot(fol_path):
     sleep(0.1)
-    pyautogui.screenshot('{}{}.png'.format(fol_path,scr_name))
+    pyautogui.screenshot(fol_path)
 
 
 # 当前页面找图,找到匹配对象位置中心点
-def find_image(fol_path, target_path, target,src_name='src', _system=None, int_x1=0, int_y1=None, int_x2=None, int_y2=None):
+def find_image(fol_path, target_path, _system=None, int_x1=0, int_y1=None, int_x2=None, int_y2=None):
     """
     在当前页面上找目标图片坐在坐标，返回中心坐标 (x,y)
     :param path:
     :param target: 例：../img/test.png
     :return:
     """
     if _system == 'hwnd':  # hwnd暂时没更新进来
         pass
     elif _system == 'adb':  # android adb 截图
         cut = command()
-        cut.cut_scr(target, fol_path)
+        # print(fol_path.split('\\')[-1])
+        cut.cut_scr(fol_path)
     elif _system is None:  # pyautogui 截图
-        screen_shot(fol_path,src_name)
+        screen_shot(fol_path)
     # 获取当前页面的截图
-    source_path = os.path.join('{}{}.png'.format(fol_path,src_name))
+    source_path = os.path.join(fol_path)
     if int_x1 == 0:
+        pass
+    else:
         img = Image.open(source_path)
         code_image = img.crop((int_x1, int_y1, int_x2, int_y2))
         code_image.save(source_path)  # 原地址重写
 
     # 获取目标图片的存放路径
-    target_path = os.path.join(target_path + target)
+    target_path = os.path.join(target_path)
+    # print(source_path)
+    # print(target_path)
 
     source_image = cv2.imread(source_path)
     target_image = cv2.imread(target_path)
 
     # 使用 TM_CCOEFF_NORMED 获取目标图片与原图片的每个点的匹配度
     result = cv2.matchTemplate(source_image, target_image, cv2.TM_CCOEFF_NORMED)
```

### Comparing `Lshengpackage-0.3.8/Lshengpackage/tools/ChaoJiYing.py` & `Lshengpackage-0.3.9/Lshengpackage/tools/ChaoJiYing.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/tools/General.py` & `Lshengpackage-0.3.9/Lshengpackage/tools/General.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/tools/OperateFile.py` & `Lshengpackage-0.3.9/Lshengpackage/tools/OperateFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage/tools/SearchFile.py` & `Lshengpackage-0.3.9/Lshengpackage/tools/SearchFile.py`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/Lshengpackage.egg-info/PKG-INFO` & `Lshengpackage-0.3.9/Lshengpackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.3.8
+Version: 0.3.9
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.3.8/Lshengpackage.egg-info/SOURCES.txt` & `Lshengpackage-0.3.9/Lshengpackage.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 Lshengpackage.egg-info/requires.txt
 Lshengpackage.egg-info/top_level.txt
 Lshengpackage/simulate/__init__.py
 Lshengpackage/simulate/mock_findFr.py
 Lshengpackage/simulate/mock_findPic.py
 Lshengpackage/simulate/adb/Command_adb.py
 Lshengpackage/simulate/adb/__init__.py
+Lshengpackage/simulate/adb/re_Pic.py
 Lshengpackage/simulate/adb/__pycache__/__init__.cpython-39.pyc
+Lshengpackage/simulate/adb/dingtalk/__init__.py
+Lshengpackage/simulate/adb/dingtalk/dingtalk_api.py
+Lshengpackage/simulate/adb/dingtalk/image_data.py
 Lshengpackage/simulate/dm/Pac_dm.py
 Lshengpackage/simulate/dm/Reg.py
 Lshengpackage/simulate/dm/Win_dm.py
 Lshengpackage/simulate/dm/__init__.py
 Lshengpackage/simulate/dm/__pycache__/Pac_dm.cpython-39.pyc
 Lshengpackage/simulate/dm/__pycache__/Reg.cpython-39.pyc
 Lshengpackage/simulate/dm/__pycache__/Win_dm.cpython-39.pyc
```

### Comparing `Lshengpackage-0.3.8/PKG-INFO` & `Lshengpackage-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lshengpackage
-Version: 0.3.8
+Version: 0.3.9
 Summary: 个人自动化爬虫开源学习
 Home-page: https://lsheng0-0.github.io/
 Download-URL: https://github.com/Lsheng0-0/package
 Author: Lsheng0-0
 Author-email: 1522833718@qq.com
 License: MIT
 Keywords: 游戏,办公,自动化,爬虫
```

### Comparing `Lshengpackage-0.3.8/README.md` & `Lshengpackage-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `Lshengpackage-0.3.8/setup.py` & `Lshengpackage-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from distutils.core import setup
 
 setup(
     name='Lshengpackage',  # How you named your package folder (MyLib)
     packages=['Lshengpackage'],  # Chose the same as "name"
-    version='0.3.8',  # Start with a small number and increase it with every change you make
+    version='0.3.9',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='个人自动化爬虫开源学习',  # Give a short description about your library
     # long_description=open('README.md', 'r', encoding='utf-8').read(),
     author='Lsheng0-0',  # Type in your name
     author_email='1522833718@qq.com',  # Type in your E-Mail
     url='https://lsheng0-0.github.io/',  # Provide either the link to your github or to your website
     download_url='https://github.com/Lsheng0-0/package',  # I explain this later on
     include_package_data=True,
     install_requires=[  # I get to this in a second
-        'openpyxl~=3.0.9',
-        'pandas~=1.4.3',
-        'PyAutoGUI~=0.9.53',
-        'pyperclip~=1.8.2',
-        'opencv-python~=4.5.1.48',
-        'Pillow~=9.1.1',
-        'aircv~=1.4.6',
-        'numpy~=1.22.4',
-        'requests~=2.27.1'
+        'openpyxl',
+        'pandas',
+        'PyAutoGUI',
+        'pyperclip',
+        'opencv-python',
+        'Pillow',
+        'aircv',
+        'numpy',
+        'requests'
     ],
     keywords=['游戏', '办公', '自动化', '爬虫'],  # Keywords that define your package best
     classifiers=[
         'Development Status :: 3 - Alpha',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
```

