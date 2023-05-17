# Comparing `tmp/opensourceleg-1.1.0.tar.gz` & `tmp/opensourceleg-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.1.0.tar", max compression
+gzip compressed data, was "opensourceleg-1.1.1.tar", max compression
```

## Comparing `opensourceleg-1.1.0.tar` & `opensourceleg-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.1.0/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.1.0/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.1.0/opensourceleg/__init__.py
--rw-r--r--   0        0        0    17769 2023-05-11 19:00:34.462414 opensourceleg-1.1.0/opensourceleg/actuators.py
--rw-r--r--   0        0        0     1554 2023-05-11 18:11:48.610119 opensourceleg-1.1.0/opensourceleg/constants.py
--rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.1.0/opensourceleg/control.py
--rw-r--r--   0        0        0     3628 2023-05-15 19:07:24.503566 opensourceleg-1.1.0/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.1.0/opensourceleg/example.py
--rw-r--r--   0        0        0    10266 2023-05-11 18:11:48.618013 opensourceleg-1.1.0/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.1.0/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8887 2023-05-11 18:11:49.772102 opensourceleg-1.1.0/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3713 2023-05-11 18:11:48.609099 opensourceleg-1.1.0/opensourceleg/logger.py
--rw-r--r--   0        0        0    31248 2023-05-15 18:56:33.702009 opensourceleg-1.1.0/opensourceleg/osl.py
--rw-r--r--   0        0        0     6705 2023-05-15 18:56:33.342899 opensourceleg-1.1.0/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     3470 2023-05-11 18:11:49.648892 opensourceleg-1.1.0/opensourceleg/thermal.py
--rw-r--r--   0        0        0    18739 2023-04-13 17:07:02.837138 opensourceleg-1.1.0/opensourceleg/tui.py
--rw-r--r--   0        0        0     3529 2023-05-11 18:11:47.533081 opensourceleg-1.1.0/opensourceleg/units.py
--rw-r--r--   0        0        0    11463 2023-05-11 15:28:34.400165 opensourceleg-1.1.0/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-05-15 19:21:12.714425 opensourceleg-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 opensourceleg-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.1.1/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.1.1/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    17769 2023-05-11 19:00:34.462414 opensourceleg-1.1.1/opensourceleg/actuators.py
+-rw-r--r--   0        0        0     1554 2023-05-11 18:11:48.610119 opensourceleg-1.1.1/opensourceleg/constants.py
+-rw-r--r--   0        0        0      811 2023-05-11 18:11:48.616184 opensourceleg-1.1.1/opensourceleg/control.py
+-rw-r--r--   0        0        0     2948 2023-05-17 19:38:43.254806 opensourceleg-1.1.1/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.1.1/opensourceleg/example.py
+-rw-r--r--   0        0        0    10266 2023-05-11 18:11:48.618013 opensourceleg-1.1.1/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.1.1/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8887 2023-05-11 18:11:49.772102 opensourceleg-1.1.1/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3713 2023-05-11 18:11:48.609099 opensourceleg-1.1.1/opensourceleg/logger.py
+-rw-r--r--   0        0        0    10898 2023-05-17 19:52:06.579669 opensourceleg-1.1.1/opensourceleg/osl.py
+-rw-r--r--   0        0        0     6986 2023-05-17 19:39:38.540874 opensourceleg-1.1.1/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     3470 2023-05-11 18:11:49.648892 opensourceleg-1.1.1/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21103 2023-05-17 17:39:09.073251 opensourceleg-1.1.1/opensourceleg/tui.py
+-rw-r--r--   0        0        0     3529 2023-05-11 18:11:47.533081 opensourceleg-1.1.1/opensourceleg/units.py
+-rw-r--r--   0        0        0    11525 2023-05-17 19:52:02.930040 opensourceleg-1.1.1/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-05-17 19:52:10.381282 opensourceleg-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 opensourceleg-1.1.1/PKG-INFO
```

### Comparing `opensourceleg-1.1.0/LICENSE` & `opensourceleg-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/README.md` & `opensourceleg-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/actuators.py` & `opensourceleg-1.1.1/opensourceleg/actuators.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/constants.py` & `opensourceleg-1.1.1/opensourceleg/constants.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/control.py` & `opensourceleg-1.1.1/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/demo.py` & `opensourceleg-1.1.1/opensourceleg/demo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from osl import OpenSourceLeg
-from state_machine import Event, State
+from opensourceleg.osl import OpenSourceLeg
+from opensourceleg.state_machine import Event, State
 
 BODY_WEIGHT = 60.0  # kg
 FZ_LSTANCE = -0.0167 * BODY_WEIGHT
 FZ_ESWING = -0.00167 * BODY_WEIGHT
 FZ_ESTANCE = -0.02 * BODY_WEIGHT
 VELOCITY_LSWING = 0.135  # rad/sec
 POSITION_LSWING = 60  # deg
@@ -62,41 +62,18 @@
 
     osl.add_loadcell(
         dephy_mode=False,
     )
 
     osl.add_state_machine()
 
-    early_stance = State(
-        "EStance",
-        5,
-        130,
-        100,
-    )
-
-    late_stance = State(
-        "LStance",
-        5,
-        175,
-        0,
-    )
-
-    early_swing = State(
-        "ESwing",
-        62,
-        40,
-        40,
-    )
-
-    late_swing = State(
-        "LSwing",
-        30,
-        60,
-        200,
-    )
+    early_stance = State("e_stance", 5, 130, 100)
+    late_stance = State("l_stance", 5, 175, 0)
+    early_swing = State("e_swing", 62, 40, 40)
+    late_swing = State("l_swing", 30, 60, 200)
 
     foot_flat = Event("foot_flat")
     heel_off = Event("heel_off")
     toe_off = Event("toe_off")
     pre_heel_strike = Event("pre_heel_strike")
     heel_strike = Event("heel_strike")
     misc = Event("misc")
@@ -138,28 +115,12 @@
         late_swing,
         early_stance,
         heel_strike,
         lswing_to_estance,
     )
 
     with osl:
-        osl.state_machine.start()
-        osl.knee.set_mode("impedance")
-        osl.knee.set_impedance_gains()
-
-        for t in osl.clock:
-            osl.update(current_limit=8000)
-            osl.state_machine.update()
-            osl.log.info(f"[OSL] State: {osl.state_machine.current_state.name}")
-
-            osl.knee.set_impedance_gains(
-                K=osl.state_machine.current_state.stiffness,
-                B=osl.state_machine.current_state.damping,
-            )
-
-            osl.knee.set_output_position(
-                osl.state_machine.current_state.equilibrium_angle
-            )
+        osl.run(set_state_machine_parameters=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `opensourceleg-1.1.0/opensourceleg/joints.py` & `opensourceleg-1.1.1/opensourceleg/joints.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/loadcell.py` & `opensourceleg-1.1.1/opensourceleg/loadcell.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/logger.py` & `opensourceleg-1.1.1/opensourceleg/logger.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/state_machine.py` & `opensourceleg-1.1.1/opensourceleg/state_machine.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 
     @property
     def damping(self):
         return self._b
 
 
 class Idle(State):
-    def __init__(self, status="Idle") -> None:
-        self._name = status
+    def __init__(self) -> None:
+        self._name = "idle"
         super().__init__(self._name)
 
     @property
     def status(self):
         return self._name
 
 
@@ -178,25 +178,26 @@
         self._events: list[Event] = []
         self._transitions: list[Transition] = []
         self._initial_state: Optional[State] = None
         self._current_state: Optional[State] = None
         self._exit_callback: Optional[Callable[[Idle, Any], None]] = None
         self._exit_state = Idle()
         self.add_state(self._exit_state)
-        self._exited = True
+        self._initial_state = self._exit_state
 
+        self._exited = True
         self._osl = osl
 
     def add_state(self, state: State, initial_state: bool = False):
         if state in self._states:
             raise ValueError("State already exists.")
 
         self._states.append(state)
 
-        if not self._initial_state and initial_state:
+        if initial_state:
             self._initial_state = state
 
     def add_event(self, event: Event):
         self._events.append(event)
 
     def add_transition(
         self,
@@ -233,15 +234,15 @@
                     if self._exit_callback:
                         self._exit_callback(self._current_state, data)
 
                 validity = True
                 break
 
         if not validity:
-            self._osl.log.warn(f"Event isn't valid at {self._current_state.name}")
+            self._osl.log.debug(f"Event isn't valid at {self._current_state.name}")
 
     def start(self, data: Any = None):
         if not self._initial_state:
             raise ValueError("Initial state not set.")
 
         self._current_state = self._initial_state
         self._exited = False
@@ -259,8 +260,19 @@
         if self._current_state and self._current_state != self._exit_state:
             return True
         else:
             return False
 
     @property
     def current_state(self):
-        return self._current_state
+        if self._current_state is None:
+            return self._initial_state
+        else:
+            return self._current_state
+
+    @property
+    def states(self):
+        return [state.name for state in self._states]
+
+    @property
+    def current_state_name(self):
+        return self.current_state.name
```

### Comparing `opensourceleg-1.1.0/opensourceleg/thermal.py` & `opensourceleg-1.1.1/opensourceleg/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/tui.py` & `opensourceleg-1.1.1/opensourceleg/tui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from typing import Callable
+from typing import Any, Callable
+
+import threading
+import time
 
 import TermTk as ttk
 from attr import dataclass
+from TermTk.TTkCore.string import TTkString
 
 
 # create a dataclass for various colors (str: hex codes)
 @dataclass
 class Colors:
     red: str = "#ff0000"
     green: str = "#00ff00"
@@ -18,46 +22,30 @@
     turquoise: str = "#00dddd"
     orange: str = "#ff8800"
     grey: str = "#888888"
     mblue: str = "#00274C"
     maize: str = "#FBEC5D"
 
 
-# create a tree data structure class
-class Group:
-    def __init__(self, name: str, parent: "Group" = None):
-        self._name = name
-        self._parent = parent
-        self._children = []
-
-    def add_child(self, child: "Group" = None):
-        self._children.append(child)
-
-    @property
-    def children(self):
-        return self._children
-
-    @property
-    def parent(self):
-        return self._parent
-
-    @property
-    def name(self):
-        return self._name
-
-    @property
-    def is_root(self):
-        return self.parent is None
+@dataclass
+class Plot:
+    title: str = "plot"
+    parent: ttk.TTkFrame = None
+    object: Any = None
+    attribute: str = None
+    graph: ttk.TTkGraph = None
 
-    @property
-    def is_leaf(self):
-        return len(self.children) == 0
 
-    def __str__(self):
-        return f"{self.name} -> {self.children}"
+@dataclass
+class StateVisualizer:
+    frame: ttk.TTkFrame = None
+    object: Any = None
+    attribute: str = None
+    states: dict[ttk.TTkButton] = None
+    previous_state: str = None
 
 
 COLORS = Colors()
 
 
 class TUI:
     """
@@ -78,97 +66,80 @@
 
         self._layouts = {
             "horizontal": ttk.TTkHBoxLayout,
             "vertical": ttk.TTkVBoxLayout,
             "grid": ttk.TTkGridLayout,
         }
 
-        self._modes = {
-            0: "voltage",
-            1: "position",
-            2: "current",
-            3: "impedance",
-        }
-
         self.root_ttk.setLayout(self._layouts["grid"]())
-        self._groups = {}
-
-        self._knee = None
-        self._ankle = None
-
-        self._joint = None
-        self._loadcell = None
-        self._attribute = "motor_position"
 
+        self._panels = {}
+        self._plots = {}
         self._buttons = {}
         self._radio_buttons = {}
         self._checkboxes = {}
         self._categories = {}
         self._dropdowns = {}
         self._values = {}
-
-        self._knee_values = {}
-        self._ankle_values = {}
-        self._other_values = {}
-
         self._texts = {}
 
+        self._state_vizualisers = {}
+
         self.frame = ttk.TTkFrame(
             parent=self.root_ttk,
             border=True,
             title=title,
             titleColor=ttk.TTkColor.BOLD + ttk.TTkColor.fg(COLORS.maize),
         )
-        self.frame.setLayout(self._layouts[layout]())
-        self._groups["root"] = self.frame
 
-        self._plot_parent: ttk.TTkFrame = None
-        self._plot: ttk.TTkGraph = None
-        self._pvalue = [0.0]
-        self._pcounter: int = 0
-
-        self._kmode: int = 0
-        self._amode: int = 0
-
-        self._plot_title: str = "Plot"
+        self.frame.setLayout(self._layouts[layout]())
+        self._panels["root"] = self.frame
 
         self._update_callbacks: list[callable] = []
 
         self.timer.timeout.connect(self.update)
         self.timer.start(1)
 
     @ttk.pyTTkSlot()
     def update(self):
-        if self._plot is not None:
-
-            if "loadcell" in self._attribute:
-                if self.loadcell is not None:
-                    if "fx" in self._attribute:
-                        self.set_plot_value(getattr(self.loadcell, "fx"))
-                    elif "fy" in self._attribute:
-                        self.set_plot_value(getattr(self.loadcell, "fy"))
-                    else:
-                        self.set_plot_value(getattr(self.loadcell, "fz"))
-
-            else:
-                if self.joint is not None:
-                    self.set_plot_value(getattr(self.joint, self._attribute))
+        if self._plots:
+            for _plot in self._plots.keys():
+                if self._plots[_plot].object is not None:
+                    self._plots[_plot].graph.addValue(
+                        [
+                            getattr(
+                                self._plots[_plot].object, self._plots[_plot].attribute
+                            )
+                        ]
+                    )
+                else:
+                    self._plots[_plot].graph.addValue([0.0])
+
+        if self._state_vizualisers:
+            for _sv in self._state_vizualisers.keys():
+                if self._state_vizualisers[_sv].object is not None:
+                    _current_state = getattr(
+                        self._state_vizualisers[_sv].object,
+                        self._state_vizualisers[_sv].attribute,
+                    )
+
+                    self._state_vizualisers[_sv].states[_current_state].setDisabled(
+                        False
+                    )
+
+                    if (
+                        self._state_vizualisers[_sv].previous_state
+                        and self._state_vizualisers[_sv].previous_state
+                        != _current_state
+                    ):
+                        self._state_vizualisers[_sv].states[
+                            self._state_vizualisers[_sv].previous_state
+                        ].setDisabled(True)
 
-            self._plot.addValue(self._pvalue)
-
-            if "attributes" in self._categories:
-                _plot_name = self.attribute.replace("_", " ").title()
-
-            else:
-                _plot_name = self._plot_title
-
-            self._plot_parent.setTitle(
-                ttk.TTkString(f"{_plot_name}: {self._pvalue[0]:0.2f}")
-            )
-            self._pcounter += 1
+                    self._state_vizualisers[_sv].previous_state = _current_state
 
         for callback in self._update_callbacks:
             callback()
 
         self.timer.start(self.dt)
 
     def add_update_callback(self, callback: callable):
@@ -176,140 +147,212 @@
 
     def set_active_attribute(self, attribute: str):
         self._attribute = attribute
 
     def set_plot_value(self, value: float):
         self._pvalue = [value]
 
-    def add_knee(self, knee):
-        self._knee = knee
-
-    def add_ankle(self, ankle):
-        self._ankle = ankle
+    def set_plot_title(self, title: str):
+        self._plot_title = title
 
     def run(self):
         self._is_running = True
         self.root_ttk.mainloop()
 
     def quit(self):
         self._is_running = False
         self.root_ttk.quit()
 
-    def add_group(
+    def add_panel(
         self,
-        name: str = "Group",
+        name: str = "Panel",
         parent: str = "root",
         layout: str = "horizontal",
         title_color: str = COLORS.white,
         border_color: str = COLORS.white,
         border: bool = True,
         show_title: bool = False,
         row: int = 0,
         col: int = 0,
     ):
         """
-        Adds a group to the TUI
+        Adds a panel to the TUI
 
         Args:
-            name (str): Name of the group. Defaults to "Group".
-            parent (str): Parent of the group. Defaults to "root".
-            layout (str): Layout of the group. Defaults to "horizontal".
-            title_color (str): Title color of the group. Defaults to COLORS.white.
+            name (str): Name of the panel. Defaults to "Panel".
+            parent (str): Parent of the panel. Defaults to "root".
+            layout (str): Layout of the panel. Defaults to "horizontal".
+            title_color (str): Title color of the panel. Defaults to COLORS.white.
             border_color (str): _description_. Defaults to COLORS.white.
             border (bool): _description_. Defaults to True.
             show_title (bool): _description_. Defaults to False.
             row (int): _description_. Defaults to 0.
             col (int): _description_. Defaults to 0.
 
         Raises:
             ValueError: _description_
         """
 
-        self._groups[name] = ttk.TTkFrame(
+        self._panels[name] = ttk.TTkFrame(
             border=border,
             titleColor=ttk.TTkColor.fg(title_color),
             borderColor=ttk.TTkColor.fg(border_color),
         )
 
         _name = " ".join(name.split("_")).title()
 
         if show_title:
-            self._groups[name].setTitle(ttk.TTkString(" " + _name + " "))
+            self._panels[name].setTitle(ttk.TTkString(" " + _name + " "))
 
-        self._groups[name].setLayout(self._layouts[layout]())
+        self._panels[name].setLayout(self._layouts[layout]())
 
-        if parent in self._groups:
+        if parent in self._panels:
 
             if (
-                self._groups[parent].layout().__class__.__name__
+                self._panels[parent].layout().__class__.__name__
                 == ttk.TTkGridLayout.__name__
             ):
-                self._groups[parent].layout().addWidget(
-                    self._groups[name],
+                self._panels[parent].layout().addWidget(
+                    self._panels[name],
                     row,
                     col,
                 )
 
             else:
-                self._groups[parent].layout().addWidget(self._groups[name])
+                self._panels[parent].layout().addWidget(self._panels[name])
         else:
-            raise ValueError(f"Parent group: {parent} does not exist.")
+            raise ValueError(f"Parent panel: {parent} does not exist.")
 
-    def add_plot(
+    def set_panel_color(self, name: str, color: str):
+        self._panels[name].setBorderColor(ttk.TTkColor.fg(color))
+
+    def add_state_visualizer(
         self,
+        name: str = "state_visualizer",
         parent: str = "root",
-        color: str = COLORS.white,
+        states: list[str] = [],
+        object: Any = None,
+        attribute: str = None,
+        layout: str = "horizontal",
+        title_color: str = COLORS.white,
+        border_color: str = COLORS.white,
+        border: bool = True,
+        show_title: bool = True,
         row: int = 0,
         col: int = 0,
     ):
-        self._plot = ttk.TTkGraph(
-            color=ttk.TTkColor.fg(
-                color,
+        _sv_frame = ttk.TTkFrame(
+            border=border,
+            titleColor=ttk.TTkColor.fg(title_color),
+            borderColor=ttk.TTkColor.fg(border_color),
+        )
+
+        _sv_title = " ".join(name.split("_")).title()
+
+        if show_title:
+            _sv_frame.setTitle(ttk.TTkString(" " + _sv_title + " "))
+
+        _sv_frame.setLayout(self._layouts[layout]())
+
+        if (
+            self._panels[parent].layout().__class__.__name__
+            == ttk.TTkGridLayout.__name__
+        ):
+            self._panels[parent].layout().addWidget(
+                _sv_frame,
+                row,
+                col,
             )
+
+        else:
+            self._panels[parent].layout().addWidget(
+                _sv_frame,
+            )
+
+        _state_displays = {}
+
+        for state in states:
+            _sv_frame.layout().addWidget(
+                _button := ttk.TTkButton(
+                    text=" ".join(state.split("_")).title(),
+                    color=ttk.TTkColor.fg(title_color),
+                    border=border,
+                )
+            )
+
+            _button.setDisabled(True)
+            _button.setBorderColor(ttk.TTkColor.fg(COLORS.green))
+            _state_displays[state] = _button
+
+        self._state_vizualisers[name] = StateVisualizer(
+            frame=_sv_frame,
+            object=object,
+            attribute=attribute,
+            states=_state_displays,
         )
 
-        self._plot_parent = self._groups[parent]
+    def add_plot(
+        self,
+        name: str = "plot",
+        parent: str = "root",
+        object=None,
+        attribute: str = None,
+        color: str = COLORS.white,
+        row: int = 0,
+        col: int = 0,
+    ):
+        self._plots[name] = Plot(
+            title=" ".join(name.split("_")).title(),
+            parent=self._panels[parent],
+            object=object,
+            attribute=attribute,
+            graph=ttk.TTkGraph(
+                color=ttk.TTkColor.fg(
+                    color,
+                )
+            ),
+        )
 
         if (
-            self._groups[parent].layout().__class__.__name__
+            self._panels[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
         ):
-            self._groups[parent].layout().addWidget(
-                self._plot,
+            self._panels[parent].layout().addWidget(
+                self._plots[name].graph,
                 row,
                 col,
             )
 
         else:
-            self._groups[parent].layout().addWidget(self._plot)
+            self._panels[parent].layout().addWidget(self._plots[name].graph)
 
     def add_dropdown(
         self,
         name: str = "dropdown",
         parent: str = "root",
         options: list[str] = [],
         callback: callable = None,
         callback_args: list = [],
         row: int = 0,
         col: int = 0,
     ):
         if (
-            self._groups[parent].layout().__class__.__name__
+            self._panels[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
         ):
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _dropdown := ttk.TTkComboBox(
                     list=options,
                 ),
                 row,
                 col,
             )
 
         else:
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _dropdown := ttk.TTkComboBox(
                     list=options,
                 )
             )
 
         self._dropdowns[parent + "_" + name] = _dropdown
 
@@ -327,53 +370,57 @@
         parent: str = "root",
         color: str = COLORS.white,
         row: int = 0,
         col: int = 0,
     ):
 
         if (
-            self._groups[parent].layout().__class__.__name__
+            self._panels[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
         ):
-            self._groups[parent].layout().addWidget(
-                ttk.TTkLabel(text=name, color=ttk.TTkColor.fg(color)),
+            self._panels[parent].layout().addWidget(
+                ttk.TTkLabel(
+                    text=" ".join(name.split("_")).title(), color=ttk.TTkColor.fg(color)
+                ),
                 row,
                 col,
             )
 
         else:
-            self._groups[parent].layout().addWidget(
-                ttk.TTkLabel(text=name, color=ttk.TTkColor.fg(color)),
+            self._panels[parent].layout().addWidget(
+                ttk.TTkLabel(
+                    text=" ".join(name.split("_")).title(), color=ttk.TTkColor.fg(color)
+                ),
             )
 
     def add_value(
         self,
         name: str = "value",
         parent: str = "root",
         default: int = 0,
         callback: callable = None,
         callback_args: list = [],
         row: int = 0,
         col: int = 0,
     ):
 
         if (
-            self._groups[parent].layout().__class__.__name__
+            self._panels[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
         ):
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _value := ttk.TTkLineEdit(
                     text=default, inputType=ttk.TTkK.Input_Number
                 ),
                 row,
                 col,
             )
 
         else:
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _value := ttk.TTkLineEdit(
                     text=default, inputType=ttk.TTkK.Input_Number
                 ),
             )
 
         self._values[parent + "_" + name] = _value
 
@@ -395,29 +442,29 @@
         border: bool = True,
         row: int = 0,
         col: int = 0,
     ):
         _name = " ".join(name.split("_")).title()
 
         if (
-            self._groups[parent].layout().__class__.__name__
+            self._panels[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
         ):
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _button := ttk.TTkButton(
                     text=_name,
                     color=ttk.TTkColor.BOLD + ttk.TTkColor.bg(color),
                     border=border,
                 ),
                 row,
                 col,
             )
 
         else:
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _button := ttk.TTkButton(
                     text=_name, color=ttk.TTkColor.fg(color), border=border
                 )
             )
 
         self._buttons[parent + "_" + name] = _button
 
@@ -456,30 +503,30 @@
             row (int): Row of the radio button. Defaults to 0.
             col (int): Column of the radio button. Defaults to 0.
         """
 
         _name = " ".join(name.split("_")).title()
 
         if (
-            self._groups[parent].layout().__class__.__name__
+            self._panels[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
         ):
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _radio_button := ttk.TTkRadioButton(
                     text=" " + _name,
                     name=category,
                     color=ttk.TTkColor.fg(color),
                     checked=is_checked,
                 ),
                 row,
                 col,
             )
 
         else:
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _radio_button := ttk.TTkRadioButton(
                     text=" " + _name,
                     name=category,
                     color=ttk.TTkColor.fg(color),
                     checked=is_checked,
                 )
             )
@@ -508,29 +555,29 @@
         is_checked: bool = False,
         row: int = 0,
         col: int = 0,
     ):
         _name = " ".join(name.split("_")).title()
 
         if (
-            self._groups[parent].layout().__class__.__name__
+            self._panels[parent].layout().__class__.__name__
             == ttk.TTkGridLayout.__name__
         ):
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _checkbox := ttk.TTkCheckbox(
                     text=_name,
                     color=ttk.TTkColor.fg(color),
                     checked=is_checked,
                 ),
                 row,
                 col,
             )
 
         else:
-            self._groups[parent].layout().addWidget(
+            self._panels[parent].layout().addWidget(
                 _checkbox := ttk.TTkCheckbox(
                     text=_name,
                     color=ttk.TTkColor.fg(color),
                     checked=is_checked,
                 )
             )
 
@@ -588,51 +635,24 @@
     ):
         callback_args.insert(0, self._dropdowns[parent + "_" + name].currentIndex())
 
         self._dropdowns[parent + "_" + name].currentIndexChanged.connect(
             lambda x: callback(name=name, parent=parent, args=callback_args)
         )
 
-    def set_joint_mode(self, **kwargs):
-        name = kwargs["name"]
-        parent = kwargs["parent"]
-        mode_id = int(self._dropdowns[parent + "_" + name].currentIndex())
-
-        if "knee" in name.lower():
-            self._kmode = mode_id
-        elif "ankle" in name.lower():
-            self._amode = mode_id
-
     def set_category(
         self,
         **kwargs,
     ):
         name = kwargs["name"]
         args = kwargs["args"]
         category = args[0]
 
         self._categories[category] = name
 
-    def set_active_joint(self, **kwargs):
-        name = kwargs["name"]
-        parent = kwargs["parent"]
-
-        _name = (name + parent).lower()
-
-        if "knee" in _name:
-            self._joint = self._knee
-        elif "ankle" in _name:
-            self._joint = self._ankle
-
-    def set_loadcell(
-        self,
-        loadcell,
-    ):
-        self._loadcell = loadcell
-
     def set_value(
         self,
         **kwargs,
     ):
 
         name = kwargs["name"]
         parent = kwargs["parent"]
@@ -651,45 +671,98 @@
         self,
         **kwargs,
     ):
         name = kwargs["name"]
         parent = kwargs["parent"]
         args = kwargs["args"]
 
-        print(f"Button {name} in group {parent} was clicked.")
+        print(f"Button {name} in panel {parent} was clicked.")
+
+    @property
+    def panels(self):
+        return self._panels
+
+    @property
+    def plots(self):
+        return self._plots
 
     @property
-    def joint(self):
-        return self._joint
+    def buttons(self):
+        return self._buttons
 
     @property
-    def loadcell(self):
-        return self._loadcell
+    def radio_buttons(self):
+        return self._radio_buttons
 
     @property
-    def attribute(self):
-        return self._attribute
+    def checkboxes(self):
+        return self._checkboxes
 
     @property
     def categories(self):
         return self._categories
 
     @property
     def values(self):
         return self._values
 
     @property
-    def dropdowns(self):
-        return self._dropdowns
+    def texts(self):
+        return self._texts
 
     @property
-    def control_modes(self):
-        return self._modes
+    def dropdowns(self):
+        return self._dropdowns
 
     @property
     def is_running(self):
         return self._is_running
 
 
+def quit(**kwargs):
+    tui.quit()
+
+
+def other_thread(loop, a):
+    for t in loop:
+        a.value += 1
+        a.t = t
+
+
+class V:
+    def __init__(self, value, loop, states) -> None:
+        self.value = value
+        self.states = states
+        self.loop = loop
+        self.state = states[0]
+
+    def run(self):
+        for t in self.loop:
+            self.value += 1
+
+            if self.value % 100 == 0:
+                self.state = self.states[
+                    (self.states.index(self.state) + 1) % len(self.states)
+                ]
+
+
 if __name__ == "__main__":
-    tui = TUI()
+    from opensourceleg.utilities import SoftRealtimeLoop
+
+    tui = TUI(frequency=200)
+    loop = SoftRealtimeLoop(dt=1 / 200)
+
+    states = ["early_stance", "late_stance", "early_swing", "late_swing"]
+
+    a = V(0, loop, states)
+
+    tui.add_state_visualizer(
+        name="state_machine",
+        parent="root",
+        states=states,
+        object=a,
+        attribute="state",
+    )
+
+    threading.Thread(target=a.run).start()
+
     tui.run()
```

### Comparing `opensourceleg-1.1.0/opensourceleg/units.py` & `opensourceleg-1.1.1/opensourceleg/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.1.0/opensourceleg/utilities.py` & `opensourceleg-1.1.1/opensourceleg/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,21 +313,20 @@
         else:
             delta = -1 * self.delta_per_update
         self.value += delta
 
         self.value = min(max(self.value, 0), 1)
         return self.value
 
-
 def get_active_ports():
     """
     Lists active serial ports.
     """
     if sys.platform.startswith("linux") or sys.platform.startswith("cygwin"):
-        ports = glob.glob("/dev/tty[A-Za-z]*")
+        ports = glob.glob("/dev/tty[A-Za-z]C*")
     elif sys.platform.startswith("darwin"):
         ports = glob.glob("/dev/tty.*")
     elif sys.platform.startswith("win"):
         ports = ["COM%s" % (i + 1) for i in range(256)]
     else:
         raise OSError("Unsupported platform.")
 
@@ -337,7 +336,11 @@
             s = serial.Serial(port)
             s.close()
             serial_ports.append(port)
         except (OSError, serial.SerialException):
             pass
 
     return serial_ports
+
+
+if __name__ == "__main__":
+    print(get_active_ports()[0])
```

### Comparing `opensourceleg-1.1.0/pyproject.toml` & `opensourceleg-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.1.0"
+version = "1.1.1"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.1.0/PKG-INFO` & `opensourceleg-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.1.0
+Version: 1.1.1
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

