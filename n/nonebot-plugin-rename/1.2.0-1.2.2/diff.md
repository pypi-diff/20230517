# Comparing `tmp/nonebot_plugin_rename-1.2.0.tar.gz` & `tmp/nonebot_plugin_rename-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.2.2.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.2.0.tar` & `nonebot_plugin_rename-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1066 2023-04-22 03:22:02.175737 nonebot_plugin_rename-1.2.0/LICENSE
--rw-r--r--   0        0        0     5066 2023-04-22 03:22:02.175737 nonebot_plugin_rename-1.2.0/README.md
--rw-r--r--   0        0        0      363 2023-04-22 03:22:02.195737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      244 2023-04-22 03:22:02.195737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      789 2023-04-22 03:22:02.195737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0      885 2023-04-22 03:22:02.195737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      408 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      466 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      603 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      300 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0     9113 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      186 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      478 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      749 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0      507 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/utils/download.py
--rw-r--r--   0        0        0     1535 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      423 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      663 2023-04-22 03:22:02.199737 nonebot_plugin_rename-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-17 04:29:53.316762 nonebot_plugin_rename-1.2.2/LICENSE
+-rw-r--r--   0        0        0     5230 2023-05-17 04:29:53.316762 nonebot_plugin_rename-1.2.2/README.md
+-rw-r--r--   0        0        0      363 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      293 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      789 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0     1020 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      408 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      607 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      604 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      338 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0     9234 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      187 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      479 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      838 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0      643 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/download.py
+-rw-r--r--   0        0        0     1534 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      423 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      663 2023-05-17 04:29:53.348762 nonebot_plugin_rename-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6135 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.2.2/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.2.0/LICENSE` & `nonebot_plugin_rename-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.0/README.md` & `nonebot_plugin_rename-1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -76,21 +76,22 @@
 | 查看当前群名片    | 查看当前群名片的设置                       |
 | 立即更改群名片 序号 | 立即更改当前群组bot名片，后面仅可跟一个序号（bot无返回值） |
 | 删除群名片      | 删除当前群组群名片                        |
 | 设置所有群名片    | 为当前机器人所在所有群设置群名片，仅限超管私聊          |
 
 ## ⚙️插件配置项
 
-| 配置项                           | 描述                  | 类型   |
-|-------------------------------|---------------------|------|
-| set_group_card_hour           | 间隔时间(小时)            | int  |
-| set_group_card_minute         | 间隔时间(分钟)            | int  |
-| use_nickname_front            | 是否在群名片前加上bot名称      | bool |
-| self_name                     | 自定义前缀(需开启上一个配置)     | str  |
-| is_one_bot_set_all_group_card | 是否允许与bot会话可以设置所有群名片 | bool |
+| 配置项                           | 描述                          | 类型   |
+|-------------------------------|-----------------------------|------|
+| set_group_card_hour           | 间隔时间(小时)                    | int  |
+| set_group_card_minute         | 间隔时间(分钟)                    | int  |
+| use_nickname_front            | 是否在群名片前加上bot名称              | bool |
+| self_name                     | 自定义前缀(需开启上一个配置)             | str  |
+| is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool |
+ | is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool |
 
 **请注意不要将两个间隔时间都设为0!!!!!!**
 
 **由于qq群名片特殊性,间隔太短可能意义并不大反而容易导致风控,建议在30分钟以上**
 
 ## 🎉目前已实现的群名片功能
 <details>
```

#### html2text {}

```diff
@@ -22,20 +22,21 @@
 æ¥çç¾¤åçåè¡¨ | æ¥çå½åæ¯æçææç¾¤åçåè¡¨çå¾ç | |
 æ¥çå½åç¾¤åç | æ¥çå½åç¾¤åççè®¾ç½® | |
 ç«å³æ´æ¹ç¾¤åç åºå· |
 ç«å³æ´æ¹å½åç¾¤ç»botåçï¼åé¢ä»å¯è·ä¸ä¸ªåºå·ï¼botæ è¿åå¼ï¼
 | | å é¤ç¾¤åç | å é¤å½åç¾¤ç»ç¾¤åç | | è®¾ç½®ææç¾¤åç |
 ä¸ºå½åæºå¨äººæå¨ææç¾¤è®¾ç½®ç¾¤åçï¼ä»éè¶ç®¡ç§è | ##
 âï¸æä»¶éç½®é¡¹ | éç½®é¡¹ | æè¿° | ç±»å | |------------------------
--------|---------------------|------| | set_group_card_hour | é´éæ¶é´
-(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) | int | |
-use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | | self_name
-| èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
+-------|-----------------------------|------| | set_group_card_hour |
+é´éæ¶é´(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) |
+int | | use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | |
+self_name | èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
 is_one_bot_set_all_group_card |
-æ¯å¦åè®¸ä¸botä¼è¯å¯ä»¥è®¾ç½®ææç¾¤åç | bool |
+æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
+| is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool |
 **è¯·æ³¨æä¸è¦å°ä¸¤ä¸ªé´éæ¶é´é½è®¾ä¸º0!!!!!!**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- åç¥çæ¬å©ä½æ¶é´
 -- åäº¬æ¶é´
 -- å¤ä»£è®¡æ¶å¶æ¶é´
```

### Comparing `nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/gaokao_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/genshin_time.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # Description: 获取原神版本剩余时间
 from datetime import datetime
 
 
 def genshin_version_time() -> str:
-    # 基准版本
-    Version = 3.5
-    baseTime = (
-        datetime.strptime("2023-3-1 11:00:00", "%Y-%m-%d %H:%M:%S").timestamp() * 1000
-    )
-    nowTime = datetime.now().timestamp() * 1000
+    # 原神版本号
+    Versions = [36, 37, 38, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50]
+    Index = 0
     # 获取持续时间
-    duringTime = baseTime - nowTime
+    baseTime = datetime.strptime('2023-4-12 11:00:00', '%Y-%m-%d %H:%M:%S')
+    nowTime = datetime.now()
+    duringTime = (baseTime - nowTime).total_seconds() * 1000
+    # 推算版本
     while duringTime <= 0:
-        # 版本+0.1 同时时间+42天
         duringTime += 42 * 24 * 60 * 60 * 1000
-        Version += 0.1
+        Index += 1
+    # 计算版本号并取到小数点后一位
+    Version = (Versions[Index] / 10).__round__(1)
     # 获取天数并取整
     days = int(duringTime / (24 * 3600 * 1000))
     leave1 = duringTime % (24 * 3600 * 1000)
     # 获取小时数并取整
     hours = int(leave1 / (3600 * 1000))
     leave2 = leave1 % (3600 * 1000)
     # 获取分钟数并取整
     minutes = int(leave2 / (60 * 1000))
-    return f"离原神{Version:.1f}还有{days}天{hours}小时{minutes}分钟"
+    # 字符串处理
+    return f'离原神{Version}还有{days}天{hours}小时{minutes}分钟'
```

### Comparing `nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/hot_search.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Description: 获取热搜
 
 import random
-import httpx
+from typing import Optional
 
+import httpx
 from nonebot import logger
-from typing import Optional
 
 URL = {
     "1": "https://tenapi.cn/v2/bilihot/",  # B站
     "2": "https://tenapi.cn/v2/weibohot",  # 微博
     "3": "https://tenapi.cn/v2/douyinhot",  # 抖音
     "4": "https://tenapi.cn/v2/baiduhot/",  # 百度
     "5": "https://tenapi.cn/v2/zhihuhot",  # 知乎
```

### Comparing `nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/card/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Description: 获取机器人所在系统状态
 
 import asyncio
+
 import psutil
 
 
 async def system_status():
     mem = psutil.virtual_memory()
     # 系统总计内存
     zj = float(mem.total) / 1024 / 1024 / 1024
```

### Comparing `nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import asyncio
 import random
 from pathlib import Path
 from typing import List
 
-from nonebot import get_driver, on_command, require, logger, get_bots
+from nonebot import get_bots, get_driver, logger, on_command, require
 from nonebot.adapters.onebot.v11 import (
+    GROUP_ADMIN,
+    GROUP_OWNER,
+    ActionFailed,
     Bot,
     GroupMessageEvent,
     Message,
-    GROUP_ADMIN,
-    GROUP_OWNER,
     MessageSegment,
-    ActionFailed, PrivateMessageEvent,
+    PrivateMessageEvent,
 )
 from nonebot.drivers import Driver
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
 from .config import Config
 from .utils import (
+    card_list,
     choice_card,
+    download_file,
     generate_card_image,
-    card_list,
     read_yaml,
     write_yaml,
-    download_file,
 )
 
 require("nonebot_plugin_apscheduler")
-from nonebot_plugin_apscheduler import scheduler
+from nonebot_plugin_apscheduler import scheduler # noqa
 
 driver: Driver = get_driver()
 env_config = Config.parse_obj(get_driver().config.dict())
 hour, minute = env_config.set_group_card_hour, env_config.set_group_card_minute
 if driver.config.nickname:
     NICKNAME = (
         env_config.self_name
@@ -160,15 +161,15 @@
 
 # on_command "立即更改群名片"
 @set_card_now.handle()
 async def _(bot: Bot, event: GroupMessageEvent, arg: Message = CommandArg()):
     card_number = arg.extract_plain_text().strip()
     if not card_number:
         await set_card_now.finish("请输入序号或序号输入错误")
-    elif card_number not in map(str, range(1, 14)):
+    elif card_number not in map(str, range(1, len(card_list)+1)):
         await set_card_now.finish("没有这种类型的群名片哦，可以发送[查看群名片列表]命令查看吧")
     card_names = await choice_card(card_number)
     if env_config.use_nickname_front:
         card_names = f"{NICKNAME}|{card_names}"
     try:
         await bot.set_group_card(
             group_id=event.group_id, user_id=int(bot.self_id), card=card_names
@@ -223,22 +224,24 @@
             tasks.append(
                 bot_case.set_group_card(
                     group_id=group_id,
                     user_id=int(bot_id),
                     card=card_names,
                 )
             )
-            logger.info(f"即将为群{group_id}的bot设置群名片后缀{card_names}")
+            if env_config.is_show_aps_info_log:
+                logger.info(f"即将为群{group_id}的bot设置群名片后缀{card_names}")
     return tasks
 
 
 # 定时任务入口
 @scheduler.scheduled_job("interval", hours=hour, minutes=minute, id="rename_group_card")
 async def _():
-    logger.info("开始为列表中的群更改bot群名片")
+    if env_config.is_show_aps_info_log:
+        logger.info("开始为列表中的群更改bot群名片")
     await set_group_card()
 
 
 # bot启动时执行
 @driver.on_startup
 async def init_group_card():
     if not (yml_file / "group_card.yaml").exists():
```

### Comparing `nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/card_name.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     get_msg,
     get_one_speak,
     gk,
     hot,
     now_time,
     old_time,
     system_status,
+    starrail_version_time
 )
 
 card_list = {
     "1": ("原神版本剩余时间", genshin_version_time),
     "2": ("北京时间(小时)", now_time),
     "3": ("当前时间(古代计时制)", old_time),
     "4": ("B站热搜", hot),
@@ -20,8 +21,9 @@
     "7": ("百度热搜", hot),
     "8": ("知乎热搜", hot),
     "9": ("今日头条热搜", hot),
     "10": ("每日一言", get_one_speak),
     "11": ("距离高考剩余时间", gk),
     "12": ("bot系统运行状态", system_status),
     "13": ("bot收发消息统计", get_msg),
+    "14": ("崩铁版本剩余时间", starrail_version_time),
 }
```

### Comparing `nonebot_plugin_rename-1.2.0/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.2.2/nonebot_plugin_rename/utils/draw.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from io import BytesIO
+from pathlib import Path
 
 from PIL import Image, ImageDraw, ImageFont
-from pathlib import Path
 
 from .card_name import card_list
 
-
 font_path = Path.cwd() / "data" / "group_card" / "fonts" / "draw.ttf"
 
 
 def generate_card_image(
     font: Path = font_path,
     font_size: int = 20,
     title_left: str = "群名片序号",
```

### Comparing `nonebot_plugin_rename-1.2.0/pyproject.toml` & `nonebot_plugin_rename-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.2.0"
+version = "1.2.2"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
 
 [[tool.poetry.source]]
```

### Comparing `nonebot_plugin_rename-1.2.0/PKG-INFO` & `nonebot_plugin_rename-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.2.0
+Version: 1.2.2
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -99,21 +99,22 @@
 | 查看当前群名片    | 查看当前群名片的设置                       |
 | 立即更改群名片 序号 | 立即更改当前群组bot名片，后面仅可跟一个序号（bot无返回值） |
 | 删除群名片      | 删除当前群组群名片                        |
 | 设置所有群名片    | 为当前机器人所在所有群设置群名片，仅限超管私聊          |
 
 ## ⚙️插件配置项
 
-| 配置项                           | 描述                  | 类型   |
-|-------------------------------|---------------------|------|
-| set_group_card_hour           | 间隔时间(小时)            | int  |
-| set_group_card_minute         | 间隔时间(分钟)            | int  |
-| use_nickname_front            | 是否在群名片前加上bot名称      | bool |
-| self_name                     | 自定义前缀(需开启上一个配置)     | str  |
-| is_one_bot_set_all_group_card | 是否允许与bot会话可以设置所有群名片 | bool |
+| 配置项                           | 描述                          | 类型   |
+|-------------------------------|-----------------------------|------|
+| set_group_card_hour           | 间隔时间(小时)                    | int  |
+| set_group_card_minute         | 间隔时间(分钟)                    | int  |
+| use_nickname_front            | 是否在群名片前加上bot名称              | bool |
+| self_name                     | 自定义前缀(需开启上一个配置)             | str  |
+| is_one_bot_set_all_group_card | 是否允许与单个bot会话可以设置所有bot所在的群名片 | bool |
+ | is_show_aps_info_log          | 是否显示定时任务的info级别日志           | bool |
 
 **请注意不要将两个间隔时间都设为0!!!!!!**
 
 **由于qq群名片特殊性,间隔太短可能意义并不大反而容易导致风控,建议在30分钟以上**
 
 ## 🎉目前已实现的群名片功能
 <details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.2.2 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
@@ -34,20 +34,21 @@
 æ¥çç¾¤åçåè¡¨ | æ¥çå½åæ¯æçææç¾¤åçåè¡¨çå¾ç | |
 æ¥çå½åç¾¤åç | æ¥çå½åç¾¤åççè®¾ç½® | |
 ç«å³æ´æ¹ç¾¤åç åºå· |
 ç«å³æ´æ¹å½åç¾¤ç»botåçï¼åé¢ä»å¯è·ä¸ä¸ªåºå·ï¼botæ è¿åå¼ï¼
 | | å é¤ç¾¤åç | å é¤å½åç¾¤ç»ç¾¤åç | | è®¾ç½®ææç¾¤åç |
 ä¸ºå½åæºå¨äººæå¨ææç¾¤è®¾ç½®ç¾¤åçï¼ä»éè¶ç®¡ç§è | ##
 âï¸æä»¶éç½®é¡¹ | éç½®é¡¹ | æè¿° | ç±»å | |------------------------
--------|---------------------|------| | set_group_card_hour | é´éæ¶é´
-(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) | int | |
-use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | | self_name
-| èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
+-------|-----------------------------|------| | set_group_card_hour |
+é´éæ¶é´(å°æ¶) | int | | set_group_card_minute | é´éæ¶é´(åé) |
+int | | use_nickname_front | æ¯å¦å¨ç¾¤åçåå ä¸botåç§° | bool | |
+self_name | èªå®ä¹åç¼(éå¼å¯ä¸ä¸ä¸ªéç½®) | str | |
 is_one_bot_set_all_group_card |
-æ¯å¦åè®¸ä¸botä¼è¯å¯ä»¥è®¾ç½®ææç¾¤åç | bool |
+æ¯å¦åè®¸ä¸åä¸ªbotä¼è¯å¯ä»¥è®¾ç½®ææbotæå¨çç¾¤åç | bool |
+| is_show_aps_info_log | æ¯å¦æ¾ç¤ºå®æ¶ä»»å¡çinfoçº§å«æ¥å¿ | bool |
 **è¯·æ³¨æä¸è¦å°ä¸¤ä¸ªé´éæ¶é´é½è®¾ä¸º0!!!!!!**
 **ç±äºqqç¾¤åçç¹æ®æ§,é´éå¤ªç­å¯è½æä¹å¹¶ä¸å¤§åèå®¹æå¯¼è´é£æ§,å»ºè®®å¨30åéä»¥ä¸**
 ## ðç®åå·²å®ç°çç¾¤åçåè½  ä¸å¾æµ [help]   æ¶é´
 -- é«èæ¶é´
 -- åç¥çæ¬å©ä½æ¶é´
 -- åäº¬æ¶é´
 -- å¤ä»£è®¡æ¶å¶æ¶é´
```

