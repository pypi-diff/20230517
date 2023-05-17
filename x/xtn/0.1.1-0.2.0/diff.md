# Comparing `tmp/xtn-0.1.1.tar.gz` & `tmp/xtn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtn-0.1.1.tar", max compression
+gzip compressed data, was "xtn-0.2.0.tar", max compression
```

## Comparing `xtn-0.1.1.tar` & `xtn-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      458 2023-05-15 17:48:09.995708 xtn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      575 2023-05-13 04:15:51.322967 xtn-0.1.1/README.md
--rw-r--r--   0        0        0      122 2023-05-12 15:09:11.486768 xtn-0.1.1/xtn/__init__.py
--rw-r--r--   0        0        0    13235 2023-05-15 17:54:47.956116 xtn-0.1.1/xtn/_xtn.py
--rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 xtn-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      458 2023-05-17 17:02:17.559755 xtn-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      575 2023-05-13 04:15:51.322967 xtn-0.2.0/README.md
+-rw-r--r--   0        0        0      122 2023-05-12 15:09:11.486768 xtn-0.2.0/xtn/__init__.py
+-rw-r--r--   0        0        0    15534 2023-05-17 16:59:10.865759 xtn-0.2.0/xtn/_xtn.py
+-rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 xtn-0.2.0/PKG-INFO
```

### Comparing `xtn-0.1.1/README.md` & `xtn-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xtn-0.1.1/xtn/_xtn.py` & `xtn-0.2.0/xtn/_xtn.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 class XtnErrorCode(Enum):
     OBJECT_MUST_BE_ON_NEW_LINE = 1
     ARRAY_MUST_BE_ON_NEW_LINE = 2
     MULTILINE_MUST_BE_ON_NEW_LINE = 3
     LINE_MUST_NOT_START_WITH_COLON = 4
     PLUS_ENCOUNTERED_OUTSIDE_ARRAY = 5
     ARRAY_ELEMENT_MUST_START_WITH_PLUS = 6
-    MULTILINE_MARKER_TOO_SHORT = 7
+    MISSING_COLON = 7
     UNMATCHED_CLOSE_MARKER = 8
     MISSING_CLOSE_MARKER = 9
+    INDENTATION_MUST_BE_SPACE_OR_TAB = 10
+    INDENTATION_MUST_NOT_BE_MIXED = 11
+    INSUFFICIENT_INDENTATION = 12
 
 
 class XtnException(Exception):
     def __init__(self, code: XtnErrorCode, message: str, *args: object) -> None:
         super().__init__(message, *args)
         self.code = code
         self.message = message
@@ -82,60 +85,55 @@
             if len(value) == 0 or value.endswith('\n'):
                 lines.append('')
             for line in lines:
                 line = line.rstrip()
                 if len(line) == 0:
                     write()
                 else:
-                    write(indent, '#', comment.prefix, '' if line[0:1].isspace() else ' ', line)
+                    write(indent, '#', comment.prefix,
+                          '' if line[0:1].isspace() else ' ', line)
 
         def write_comments(comments: list[XtnComment] | None, indent: str):
             if comments is not None and len(comments) > 0:
                 for comment in comments:
                     write_comment(comment, indent)
 
-        def write_pair(name: str, data: XtnDataElement, indent: str, end: bool):
+        def write_pair(name: str, data: XtnDataElement, indent: str):
             write_comments(data.comments, indent)
             if isinstance(data, XtnArray):
                 write(indent, name, '[]:')
                 child_indent = indent + '    '
                 for element in data.elements:
-                    write_pair('+', element, child_indent, False)
+                    write_pair('+', element, child_indent)
                 write_comments(data.trail_comments, child_indent)
-                if end:
-                    write(indent, '----')
+                write(indent, '----')
             elif isinstance(data, XtnObject):
                 write(indent, name, '{}:')
                 child_indent = indent + '    '
                 for child_name, child_value in data.elements.items():
-                    write_pair(child_name, child_value, child_indent, True)
+                    write_pair(child_name, child_value, child_indent)
                 write_comments(data.trail_comments, child_indent)
-                if end:
-                    write(indent, '----')
+                write(indent, '----')
             elif isinstance(data, XtnText):
                 sv = data.value
                 lines = sv.splitlines()
                 if sv.endswith('\n'):
                     lines.append('')
                 if data.force_multiline or len(lines) > 1 or sv[0:1].isspace() or sv[-1:].isspace() or any(m.group(0) != ' ' for m in re.finditer(r'\s', sv)):
-                    marker_len = max((len(m.group(0)) for m in re.finditer(r'`+', sv)), default=0)
-                    marker_len = min(marker_len, 4)
-                    marker = (4 if marker_len < 3 else marker_len + (3 if marker_len % 2 == 1 else 4)) * "'"
                     write(indent, name, "'':")
                     child_indent = indent + '    '
-                    write(child_indent, marker)
                     for line in lines:
                         write(child_indent, line)
-                    write(child_indent, marker)
+                    write(indent, '----')
                 else:
                     write(indent, name, ': ', sv)
 
         write_comments(self.comments, '')
         for name, value in self.elements.items():
-            write_pair(name, value, '', True)
+            write_pair(name, value, '')
         write_comments(self.trail_comments, '')
 
 
 def _make_Xtn(value: dict[str, Any] | list | str):
     if isinstance(value, list):
         return XtnArray(value)
     elif isinstance(value, dict):
@@ -178,32 +176,35 @@
     mode: Literal[_Mode.ARRAY] = _Mode.ARRAY
 
     def set(self, name: str, value: dict[str, Any] | list | str, raise_error: Callable[[XtnErrorCode, str], NoReturn], convert_spaces: bool = True):
         name = _convert_spaces(name, True)
         if convert_spaces and isinstance(value, str):
             value = _convert_spaces(value, False)
         if name != '+':
-            raise_error(XtnErrorCode.ARRAY_ELEMENT_MUST_START_WITH_PLUS, "An array element must start with a plus")
+            raise_error(XtnErrorCode.ARRAY_ELEMENT_MUST_START_WITH_PLUS,
+                        "An array element must start with a plus")
         if self.target is None:
             self.current.append(value)
             return None
         else:
             child = _make_Xtn(value)
             self.current.append(child)
             return child
 
 
 @dataclass
 class _MultilineState:
     start_line: int
     name: str
     parent_state: _ObjectState | _ArrayState
-    marker: str = ''
+    indent: str
+    indent_char: str = ' '
+    exp_indent: str | None = None
+    cur_indent: str = ''
     text: str = ''
-    indent: int = -1
     target = None
     mode: Literal[_Mode.MULTILINE] = _Mode.MULTILINE
 
 
 def _load(f: TextIO, target: XtnObject | None) -> dict[str, Any]:
     top_level = {} if target is None else target.elements
     stack: list[_ObjectState | _ArrayState | _MultilineState] = [
@@ -235,103 +236,137 @@
 
     def attach_trailing_comments(target: XtnDataElement | None):
         if target is not None and comments is not None and len(comments) > 0:
             target.trail_comments = comments.copy()
             comments.clear()
 
     i = -1
-    for i, line in enumerate(f):
+    for i, orig_line in enumerate(f):
+        line = orig_line
         state = stack[-1]
         if state.mode == _Mode.MULTILINE:
-            if len(state.marker) == 0:
-                state.indent = len(line)
-                line = line.lstrip()
-                state.indent -= len(line)
-                if not line.startswith("''''"):
-                    raise_error(XtnErrorCode.MULTILINE_MARKER_TOO_SHORT,
-                                f"A multi-line marker must start with at least 4 single quote characters")
-                state.marker = line.rstrip()
-            else:
-                cur_indent = state.indent
-                prefix = line[0:cur_indent]
-                if not prefix.isspace():
-                    cur_indent = len(prefix)
-                    prefix = prefix.lstrip()
-                    cur_indent -= len(prefix)
-                line = line[cur_indent:]
-                if len(line) == 0:
-                    line = '\n'
-                if line.startswith(state.marker) and line[len(state.marker):].isspace():
-                    child_target = state.parent_state.set(
-                        state.name, state.text[0:-1], raise_error, convert_spaces=False)
-                    if child_target is not None:
-                        child_target.force_multiline = True  # type: ignore
-                    attach_comments(child_target)
-                    stack.pop()
+            if state.exp_indent is None:
+                if len(state.indent) > 0:
+                    state.indent_char = state.indent[0]
+                    state.exp_indent = state.indent + \
+                        state.indent_char * (1 if state.indent_char == '\t' else 4)
+                elif line[:1] == '\t':
+                    state.exp_indent = '\t'
+                    state.indent_char = '\t'
                 else:
-                    state.text = state.text + line
+                    state.exp_indent = '    '
+                    state.indent_char = ' '
+                state.cur_indent = state.exp_indent
+            cur_indent_len = len(state.cur_indent)
+            act_indent_len = 0
+            if cur_indent_len > 0:
+                prefix = line[0:cur_indent_len]
+                act_indent = prefix[:(
+                    len(prefix) - len(prefix.lstrip(state.exp_indent[0])))]
+                act_indent_len = len(act_indent)
+                prefix = prefix[act_indent_len:act_indent_len+1]
+                if act_indent_len < cur_indent_len and prefix.isspace() and prefix != '\n':
+                    raise_error(XtnErrorCode.INDENTATION_MUST_NOT_BE_MIXED,
+                                f"Indentation for a complex text value can use either spaces or tabs but not both")
+                line = line[act_indent_len:]
+                if act_indent_len < cur_indent_len:
+                    state.cur_indent = act_indent
+            if act_indent_len < len(state.exp_indent):
+                close_ind = line.find('--', None, len(state.exp_indent) - act_indent_len)
+                if close_ind >= 0:
+                    prefix = line[:close_ind]
+                    if len(prefix) == 0 or prefix.isspace():
+                        if line[close_ind:(close_ind+4)] == '----' and (len(line) == close_ind + 4 or line[(close_ind+4):].isspace()):
+                            if act_indent_len + close_ind <= len(state.indent):
+                                if len(state.indent) > 0 and len(prefix.lstrip(state.indent_char)) != 0:
+                                    raise_error(XtnErrorCode.INDENTATION_MUST_NOT_BE_MIXED, f"Indentation for a complex text value can use either spaces or tabs but not both")
+                                
+                                child_target = state.parent_state.set(state.name, state.text[0:-1], raise_error, convert_spaces=False)
+                                if child_target is not None:
+                                    child_target.force_multiline = True  # type: ignore
+                                    attach_comments(child_target)
+                                stack.pop()
+                                continue
+                            
+                        raise_error(XtnErrorCode.INSUFFICIENT_INDENTATION, f"Lines starting with two or more dashes must be indented by at least 4 spaces or a tab compared to the key line")
+            
+            state.text = state.text + line
         else:
             line = line.strip()
             if line.startswith('#'):
                 record_comment(line)
                 continue
             if (len(line) == 0):
                 record_comment(line)
                 continue
             left, sep, right = line.partition(':')
-            left = left.strip()
-            right = right.strip()
-            if len(left) == 0:
-                raise_error(XtnErrorCode.LINE_MUST_NOT_START_WITH_COLON,
-                            f"A line cannot start with a colon")
-            elif left.startswith('+') and state.mode == _Mode.OBJECT:
-                if not state.in_array:
+            left = left.rstrip()
+            right = right.lstrip()
+            if sep == ':':
+                if len(left) == 0:
+                    raise_error(XtnErrorCode.LINE_MUST_NOT_START_WITH_COLON,
+                                f"A line cannot start with a colon")
+                elif left.startswith('+') and state.mode == _Mode.OBJECT and not state.in_array:
                     raise_error(XtnErrorCode.PLUS_ENCOUNTERED_OUTSIDE_ARRAY,
                                 f"A line cannot start with a plus outside the context of an array")
-                stack.pop()
-                state = stack[-1]
-                if state.mode != _Mode.ARRAY:
-                    raise RuntimeError('Error in parsing logic. Expected an array mode')
-
-            if left.endswith('{}'):
-                if len(right) > 0:
-                    raise_error(XtnErrorCode.OBJECT_MUST_BE_ON_NEW_LINE,
-                                f"An object must start on a new line")
-                name = left[0:-2].rstrip()
-                obj = {}
-                child_target = state.set(name, obj, raise_error)
-                attach_comments(child_target)
-                stack.append(_ObjectState(start_line=i, current=obj,
-                             target=child_target, in_array=state.mode == _Mode.ARRAY))  # type: ignore
-            elif left.endswith('[]'):
-                if len(right) > 0:
-                    raise_error(XtnErrorCode.ARRAY_MUST_BE_ON_NEW_LINE,
-                                f"An array must start on a new line")
-                name = left[0:-2].rstrip()
-                obj = []
-                child_target = state.set(name, obj, raise_error)
-                attach_comments(child_target)
-                stack.append(_ArrayState(start_line=i, current=obj, target=child_target))  # type: ignore
-            elif left.endswith("''"):
-                name = left[0:-2].rstrip()
-                if len(right) > 0:
-                    raise_error(XtnErrorCode.MULTILINE_MUST_BE_ON_NEW_LINE,
-                                f"A multi-line value must start on a new line")
-                stack.append(_MultilineState(start_line=i, name=name, parent_state=state))
-            elif not left.startswith('-'):
-                child_target = state.set(left, right, raise_error)
-                attach_comments(child_target)
-            else:
-                if state.mode == _Mode.OBJECT and state.in_array:
-                    stack.pop()
+
+                if left.endswith('{}'):
+                    if len(right) > 0:
+                        raise_error(XtnErrorCode.OBJECT_MUST_BE_ON_NEW_LINE,
+                                    f"An object must start on a new line")
+                    name = left[0:-2].rstrip()
+                    obj = {}
+                    child_target = state.set(name, obj, raise_error)
+                    attach_comments(child_target)
+                    stack.append(_ObjectState(start_line=i, current=obj,
+                                              target=child_target, in_array=state.mode == _Mode.ARRAY))  # type: ignore
+                elif left.endswith('[]'):
+                    if len(right) > 0:
+                        raise_error(XtnErrorCode.ARRAY_MUST_BE_ON_NEW_LINE,
+                                    f"An array must start on a new line")
+                    name = left[0:-2].rstrip()
+                    obj = []
+                    child_target = state.set(name, obj, raise_error)
+                    attach_comments(child_target)
+                    # type: ignore
+                    stack.append(_ArrayState(
+                        start_line=i, current=obj, target=child_target))
+                elif left.endswith("''"):
+                    indent = orig_line[:orig_line.find(left[0])]
+                    if len(indent) > 0:
+                        indent_char = indent[0]
+                        if indent_char != ' ' and indent_char != '\t':
+                            raise_error(XtnErrorCode.INDENTATION_MUST_BE_SPACE_OR_TAB,
+                                        f"Indentation for a complex text value must be a space (32) or tab (9) character")
+                        if len(indent.lstrip(indent_char)) > 0:
+                            raise_error(XtnErrorCode.INDENTATION_MUST_NOT_BE_MIXED,
+                                        f"Indentation for a complex text value can use either spaces or tabs but not both")
+
+                    name = left[0:-2].rstrip()
+                    if len(right) > 0:
+                        raise_error(XtnErrorCode.MULTILINE_MUST_BE_ON_NEW_LINE,
+                                    f"A multi-line value must start on a new line")
+                    stack.append(_MultilineState(
+                        start_line=i, name=name, parent_state=state, indent=indent))
+                else:
+                    child_target = state.set(left, right, raise_error)
+                    attach_comments(child_target)
+
+            elif left.startswith('----') and (len(left) == 4 or left[4:].isspace()):
                 attach_trailing_comments(stack[-1].target)
                 stack.pop()
                 if len(stack) == 0:
-                    raise_error(XtnErrorCode.UNMATCHED_CLOSE_MARKER, "The close marker ---- does not match any open object or array")
+                    raise_error(XtnErrorCode.UNMATCHED_CLOSE_MARKER,
+                                "The close marker ---- does not match any open object or array")
+            else:
+                raise_error(XtnErrorCode.MISSING_COLON,
+                            f"A colon was expected")
+
     i += 1
     if len(stack) > 1:
-        raise_error(XtnErrorCode.MISSING_CLOSE_MARKER, "A close marker ---- was expected")
+        raise_error(XtnErrorCode.MISSING_CLOSE_MARKER,
+                    "A close marker ---- was expected")
     return top_level
 
 
 def load(f: TextIO):
     return _load(f, None)
```

### Comparing `xtn-0.1.1/PKG-INFO` & `xtn-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtn
-Version: 0.1.1
+Version: 0.2.0
 Summary: A library for working with the xtn format
 Home-page: https://github.com/koustubhmoharir/xtn
 License: MIT
 Author: Koustubh Moharir
 Author-email: koustubhmoharir@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

