# Comparing `tmp/aireq-0.4.tar.gz` & `tmp/aireq-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aireq-0.4.tar", last modified: Wed May 17 06:42:09 2023, max compression
+gzip compressed data, was "aireq-0.5.tar", last modified: Wed May 17 07:00:04 2023, max compression
```

## Comparing `aireq-0.4.tar` & `aireq-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 06:42:09.662215 aireq-0.4/
--rw-rw-rw-   0        0        0      106 2023-05-17 06:42:09.659708 aireq-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 06:42:09.488480 aireq-0.4/ai/
--rw-rw-rw-   0        0        0    15240 2023-05-14 06:59:07.000000 aireq-0.4/ai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 06:42:09.632116 aireq-0.4/aireq.egg-info/
--rw-rw-rw-   0        0        0      106 2023-05-17 06:42:09.000000 aireq-0.4/aireq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-17 06:42:09.000000 aireq-0.4/aireq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 06:42:09.000000 aireq-0.4/aireq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-17 06:42:09.000000 aireq-0.4/aireq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 06:42:09.635053 aireq-0.4/ippr/
--rw-rw-rw-   0        0        0     8186 2023-05-14 07:08:54.000000 aireq-0.4/ippr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 06:42:09.643316 aireq-0.4/mwa/
--rw-rw-rw-   0        0        0     3230 2023-05-17 06:37:34.000000 aireq-0.4/mwa/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-17 06:42:09.662215 aireq-0.4/setup.cfg
--rw-rw-rw-   0        0        0      212 2023-05-17 06:42:04.000000 aireq-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:00:04.057430 aireq-0.5/
+-rw-rw-rw-   0        0        0      106 2023-05-17 07:00:04.055401 aireq-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 07:00:03.656699 aireq-0.5/ai/
+-rw-rw-rw-   0        0        0    15240 2023-05-14 06:59:07.000000 aireq-0.5/ai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:00:04.017305 aireq-0.5/aireq.egg-info/
+-rw-rw-rw-   0        0        0      106 2023-05-17 07:00:03.000000 aireq-0.5/aireq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-05-17 07:00:03.000000 aireq-0.5/aireq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:00:03.000000 aireq-0.5/aireq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-17 07:00:03.000000 aireq-0.5/aireq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 07:00:04.024373 aireq-0.5/ippr/
+-rw-rw-rw-   0        0        0     8186 2023-05-14 07:08:54.000000 aireq-0.5/ippr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:00:04.033550 aireq-0.5/mwa/
+-rw-rw-rw-   0        0        0     4826 2023-05-17 06:58:34.000000 aireq-0.5/mwa/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:00:04.057430 aireq-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      212 2023-05-17 06:58:41.000000 aireq-0.5/setup.py
```

### Comparing `aireq-0.4/ai/__init__.py` & `aireq-0.5/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `aireq-0.4/ippr/__init__.py` & `aireq-0.5/ippr/__init__.py`

 * *Files identical despite different names*

### Comparing `aireq-0.4/mwa/__init__.py` & `aireq-0.5/mwa/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -92,8 +92,66 @@
       default:
         result = 'Invalid operator';
     }
     alert(`Result: ${result}`);
   });
 </script>
 """
-    return s
+    return s
+
+def val():
+  s="""<!DOCTYPE html>
+<html>
+<head>
+  <title>Email and Password Validation</title>
+</head>
+<body>
+  <h1>Email and Password Validation</h1>
+  <form id="myForm">
+    <label for="email">Email:</label>
+    <input type="email" id="email" name="email" required><br><br>
+    <label for="password">Password:</label>
+    <input type="password" id="password" name="password" required><br><br>
+    <input type="submit" value="Submit">
+  </form>
+
+  <script>
+    const form = document.getElementById("myForm");
+    const email = document.getElementById("email");
+    const password = document.getElementById("password");
+
+    form.addEventListener("submit", function(event) {
+      // Prevent form submission
+      event.preventDefault();
+
+      // Validate email
+      if (!isValidEmail(email.value)) {
+        alert("Please enter a valid email address");
+        return;
+      }
+
+      // Validate password
+      if (!isValidPassword(password.value)) {
+        alert("Password must be at least 8 characters long");
+        return;
+      }
+
+      // If both email and password are valid, submit form
+      alert("Form submitted successfully");
+      form.submit();
+    });
+
+    function isValidEmail(email) {
+      // Regular expression for email validation
+      const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
+      return emailRegex.test(email);
+    }
+
+    function isValidPassword(password) {
+      // Password must be at least 8 characters long
+      return password.length >= 8;
+    }
+  </script>
+</body>
+</html>
+"""
+  return s
```

#### html2text {}

```diff
@@ -2,8 +2,15 @@
 ****** Palindrome Checker ******
 Enter a word or phrase to check if it's a palindrome:
 [                    ] Check
 """ return s def fib(): s="""
 Generate Fibonacci sequence up to: [Unknown INPUT type] Generate
  """ return s def cal(): s="""
 [Unknown INPUT type] [One of: +/-/*//] [Unknown INPUT type] Calculate
- """ return s
+ """ return s def val(): s="""
+****** Email and Password Validation ******
+Email: [Unknown INPUT type]
+
+Password: [********************]
+
+[Submit]
+""" return s
```

