# Comparing `tmp/neon_gui-1.1.2a1-py3-none-any.whl.zip` & `tmp/neon_gui-1.1.3a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9626 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1831 b- defN 23-Feb-23 17:08 neon_gui/__init__.py
--rw-r--r--  2.0 unx     2371 b- defN 23-Feb-23 17:08 neon_gui/__main__.py
--rw-r--r--  2.0 unx     3888 b- defN 23-Feb-23 17:08 neon_gui/service.py
--rw-r--r--  2.0 unx     5575 b- defN 23-Feb-23 17:08 neon_gui/utils.py
--rw-r--r--  2.0 unx     1635 b- defN 23-Feb-23 17:08 neon_gui-1.1.2a1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1344 b- defN 23-Feb-23 17:08 neon_gui-1.1.2a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-23 17:08 neon_gui-1.1.2a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Feb-23 17:08 neon_gui-1.1.2a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Feb-23 17:08 neon_gui-1.1.2a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      805 b- defN 23-Feb-23 17:08 neon_gui-1.1.2a1.dist-info/RECORD
-10 files, 17610 bytes uncompressed, 8252 bytes compressed:  53.1%
+Zip file size: 9621 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-17 21:04 neon_gui/__init__.py
+-rw-r--r--  2.0 unx     2405 b- defN 23-May-17 21:04 neon_gui/__main__.py
+-rw-r--r--  2.0 unx     3885 b- defN 23-May-17 21:04 neon_gui/service.py
+-rw-r--r--  2.0 unx     5572 b- defN 23-May-17 21:04 neon_gui/utils.py
+-rw-r--r--  2.0 unx     1635 b- defN 23-May-17 21:04 neon_gui-1.1.3a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1344 b- defN 23-May-17 21:04 neon_gui-1.1.3a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 21:04 neon_gui-1.1.3a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-May-17 21:04 neon_gui-1.1.3a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-17 21:04 neon_gui-1.1.3a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      805 b- defN 23-May-17 21:04 neon_gui-1.1.3a1.dist-info/RECORD
+10 files, 17638 bytes uncompressed, 8247 bytes compressed:  53.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: neon_gui/service.py
 Comment: 
 
 Filename: neon_gui/utils.py
 Comment: 
 
-Filename: neon_gui-1.1.2a1.dist-info/LICENSE.md
+Filename: neon_gui-1.1.3a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_gui-1.1.2a1.dist-info/METADATA
+Filename: neon_gui-1.1.3a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_gui-1.1.2a1.dist-info/WHEEL
+Filename: neon_gui-1.1.3a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_gui-1.1.2a1.dist-info/entry_points.txt
+Filename: neon_gui-1.1.3a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_gui-1.1.2a1.dist-info/top_level.txt
+Filename: neon_gui-1.1.3a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_gui-1.1.2a1.dist-info/RECORD
+Filename: neon_gui-1.1.3a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_gui/__main__.py

```diff
@@ -26,23 +26,22 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ovos_utils import wait_for_exit_signal
 from neon_gui.service import NeonGUIService
 from neon_utils.configuration_utils import init_config_dir
 from neon_utils.log_utils import init_log
-
-from mycroft.lock import Lock
+from ovos_utils.process_utils import PIDLock as Lock
 
 
 def main(*args, **kwargs):
     init_config_dir()
     init_log(log_name="gui")
 
-    from mycroft.util import reset_sigint_handler
+    from ovos_utils.process_utils import reset_sigint_handler
     reset_sigint_handler()
     Lock("gui")
 
     gui = NeonGUIService(*args, **kwargs)
     gui.start()
     wait_for_exit_signal()
     gui.shutdown()
```

## neon_gui/service.py

```diff
@@ -26,16 +26,15 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from time import sleep
 from tornado import ioloop
 from threading import Thread, Event
 from ovos_utils.log import LOG
-
-from mycroft.gui.service import GUIService
+from ovos_gui.service import GUIService
 
 from neon_gui.utils import update_gui_ip_address
 
 
 def on_ready():
     LOG.info("GUI Service Ready")
 
@@ -64,15 +63,15 @@
 def on_started():
     LOG.debug("Messagebus client started")
 
 
 class NeonGUIService(Thread, GUIService):
     def __init__(self, ready_hook=on_ready, error_hook=on_error,
                  stopping_hook=on_stopping, alive_hook=on_alive,
-                 started_hook=on_started, gui_config=None, daemonic=False):
+                 started_hook=on_started, gui_config=None, daemonic=False,):
         if gui_config:
             from neon_gui.utils import patch_config
             patch_config(gui_config)
         Thread.__init__(self)
         self.setDaemon(daemonic)
         self.setName('GUI')
         self.started = Event()
```

## neon_gui/utils.py

```diff
@@ -22,15 +22,15 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from mycroft_bus_client import Message
+from ovos_bus_client import Message
 from ovos_utils.log import LOG
 from ovos_utils.gui import extend_about_data
 
 
 def patch_config(config: dict = None):
     """
     Write the specified speech configuration to the global config file
```

## Comparing `neon_gui-1.1.2a1.dist-info/LICENSE.md` & `neon_gui-1.1.3a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_gui-1.1.2a1.dist-info/METADATA` & `neon_gui-1.1.3a1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: neon-gui
-Version: 1.1.2a1
+Version: 1.1.3a1
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: neon-utils[network] (~=1.1)
 Requires-Dist: ovos-utils (>=0.0.25,~=0.0)
 Requires-Dist: tornado (~=6.0)
-Requires-Dist: mycroft-messagebus-client (~=0.10)
-Requires-Dist: ovos-core (~=0.0.4)
+Requires-Dist: ovos-bus-client (~=0.0.3)
+Requires-Dist: ovos-gui (>=0.0.3a2,~=0.0.2)
 Requires-Dist: ovos-config (~=0.0.4)
 Provides-Extra: docker
 
 # Neon GUI
 GUI Module for Neon Core. This module extracts the GUI components from the 
 [Mycroft Mark 2 Skill](https://github.com/MycroftAI/skill-mark-2) and the `enclosure` module
 from [mycroft-core](https://github.com/MycroftAI/mycroft-core/tree/dev/mycroft/enclosure).
```

## Comparing `neon_gui-1.1.2a1.dist-info/RECORD` & `neon_gui-1.1.3a1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 neon_gui/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
-neon_gui/__main__.py,sha256=GWxJ8aZJXMs5Q5k0oL92_y7pLjk9NuOEGyfa2tq-nzQ,2371
-neon_gui/service.py,sha256=o0fek2o8Z2dEYkZ3Vvw7Qf3oh4OZ0ei6LiiOPmaN6ps,3888
-neon_gui/utils.py,sha256=Bl2fyV0dP5xFAkIljIZ7YQgEGs6RAwMRP4bD2meySkw,5575
-neon_gui-1.1.2a1.dist-info/LICENSE.md,sha256=KxXbLh0XZkaLbNrj5ksC1Hl04EeiMbY-I0pGhKTPBRc,1635
-neon_gui-1.1.2a1.dist-info/METADATA,sha256=RDciNFeUPp0H3dRjNgR_CxSTIOCASHcfw7vUlVH4How,1344
-neon_gui-1.1.2a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-neon_gui-1.1.2a1.dist-info/entry_points.txt,sha256=hE3Ku5E4jTRtW7KRRDBIFVMozBF8CoWL5a5pOEWIRcM,60
-neon_gui-1.1.2a1.dist-info/top_level.txt,sha256=TYzHMKJMmDxoVOZENwOOqnXQZpcaWbmngtOUOXgDDpY,9
-neon_gui-1.1.2a1.dist-info/RECORD,,
+neon_gui/__main__.py,sha256=bAYBEqEbgPppzKgnN_UXtC7ZjFYXVJARIO7xwN1YMoU,2405
+neon_gui/service.py,sha256=EtiGdmlu9RelwwOkeMeKBm2VMG7AE8jKmdmFuSSobRg,3885
+neon_gui/utils.py,sha256=I-9bDQRY7dD_3d-65KGCHtdPExroatiRpwvpYpfk8BM,5572
+neon_gui-1.1.3a1.dist-info/LICENSE.md,sha256=KxXbLh0XZkaLbNrj5ksC1Hl04EeiMbY-I0pGhKTPBRc,1635
+neon_gui-1.1.3a1.dist-info/METADATA,sha256=S6aLwO_4k-Vz4jFCXynVVHvuqaaiMQOF6Px8RazUDgA,1344
+neon_gui-1.1.3a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_gui-1.1.3a1.dist-info/entry_points.txt,sha256=hE3Ku5E4jTRtW7KRRDBIFVMozBF8CoWL5a5pOEWIRcM,60
+neon_gui-1.1.3a1.dist-info/top_level.txt,sha256=TYzHMKJMmDxoVOZENwOOqnXQZpcaWbmngtOUOXgDDpY,9
+neon_gui-1.1.3a1.dist-info/RECORD,,
```

