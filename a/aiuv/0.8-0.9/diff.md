# Comparing `tmp/aiuv-0.8.tar.gz` & `tmp/aiuv-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiuv-0.8.tar", last modified: Wed May 17 05:19:33 2023, max compression
+gzip compressed data, was "aiuv-0.9.tar", last modified: Wed May 17 07:41:02 2023, max compression
```

## Comparing `aiuv-0.8.tar` & `aiuv-0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 05:19:33.857010 aiuv-0.8/
--rw-rw-rw-   0        0        0        0 2023-05-11 10:25:19.000000 aiuv-0.8/Licence.txt
--rw-rw-rw-   0        0        0      144 2023-05-17 05:19:33.856012 aiuv-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 05:19:33.853011 aiuv-0.8/aiuv.egg-info/
--rw-rw-rw-   0        0        0      144 2023-05-17 05:19:33.000000 aiuv-0.8/aiuv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      148 2023-05-17 05:19:33.000000 aiuv-0.8/aiuv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 05:19:33.000000 aiuv-0.8/aiuv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-17 05:19:33.000000 aiuv-0.8/aiuv.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 05:19:33.855012 aiuv-0.8/pkg/
--rw-rw-rw-   0        0        0    37268 2023-05-17 05:18:17.000000 aiuv-0.8/pkg/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-17 05:19:33.858010 aiuv-0.8/setup.cfg
--rw-rw-rw-   0        0        0      183 2023-05-17 05:17:25.000000 aiuv-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:41:02.978955 aiuv-0.9/
+-rw-rw-rw-   0        0        0        0 2023-05-11 10:25:19.000000 aiuv-0.9/Licence.txt
+-rw-rw-rw-   0        0        0      144 2023-05-17 07:41:02.970954 aiuv-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 07:41:02.946882 aiuv-0.9/aiuv.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-05-17 07:41:02.000000 aiuv-0.9/aiuv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      148 2023-05-17 07:41:02.000000 aiuv-0.9/aiuv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:41:02.000000 aiuv-0.9/aiuv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-17 07:41:02.000000 aiuv-0.9/aiuv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 07:41:02.970954 aiuv-0.9/pkg/
+-rw-rw-rw-   0        0        0    39885 2023-05-17 07:40:32.000000 aiuv-0.9/pkg/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:41:02.978955 aiuv-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      183 2023-05-17 07:40:57.000000 aiuv-0.9/setup.py
```

### Comparing `aiuv-0.8/pkg/__init__.py` & `aiuv-0.9/pkg/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1379,9 +1379,100 @@
 """
     return s
 
 def deep_learning_10():
     s = """https://github.com/shubhamprabhu10/18CSC305J-AI-All-Lab-Exps"""
     return s
 
+def naivebyees():
+    s = """from sklearn.datasets import load_breast_cancer
+from sklearn.model_selection import train_test_split
+from sklearn.naive_bayes import GaussianNB
+
+# Load the breast cancer dataset
+cancer = load_breast_cancer()
+
+# Split the dataset into training and testing sets
+X_train, X_test, y_train, y_test = train_test_split(
+    cancer.data, cancer.target, test_size=0.2, random_state=42)
+
+# Create a Naive Bayes model
+nb_model = GaussianNB()
+
+# Train the model on the training data
+nb_model.fit(X_train, y_train)
+
+# Predict the target values for the test data
+y_pred = nb_model.predict(X_test)
+
+# Calculate the accuracy of the model
+accuracy = nb_model.score(X_test, y_test)
+
+# Print the accuracy as a percentage
+print("Naive Bayes Accuracy: {:.2f}%".format(accuracy*100))"""
+
+    return s
+
+def SVM():
+    s = """from sklearn.datasets import load_breast_cancer
+from sklearn.model_selection import train_test_split
+from sklearn.svm import SVC
+from sklearn.metrics import accuracy_score
+
+# Load the breast cancer dataset
+cancer = load_breast_cancer()
+
+# Split the dataset into training and testing sets
+X_train, X_test, y_train, y_test = train_test_split(
+    cancer.data, cancer.target, test_size=0.2, random_state=42)
+
+# Create an SVM classifier
+svm_model = SVC()
+
+# Train the classifier on the training data
+svm_model.fit(X_train, y_train)
+
+# Predict the target values for the test data
+y_pred = svm_model.predict(X_test)
+
+# Calculate the accuracy of the model
+accuracy = accuracy_score(y_test, y_pred)
+
+# Print the accuracy as a percentage
+print("SVM Accuracy: {:.2f}%".format(accuracy * 100))"""
+
+    return s
+
+def linearreg():
+    s= """from sklearn.datasets import load_breast_cancer
+from sklearn.model_selection import train_test_split
+from sklearn.linear_model import LinearRegression
+from sklearn.metrics import mean_squared_error, r2_score
+
+# Load the breast cancer dataset
+cancer = load_breast_cancer()
+
+# Split the dataset into training and testing sets
+X_train, X_test, y_train, y_test = train_test_split(
+    cancer.data, cancer.target, test_size=0.2, random_state=42)
+
+# Create a linear regression model
+lr_model = LinearRegression()
+
+# Train the model on the training data
+lr_model.fit(X_train, y_train)
+
+# Predict the target values for the test data
+y_pred = lr_model.predict(X_test)
+
+# Evaluate the model
+mse = mean_squared_error(y_test, y_pred)
+r2 = r2_score(y_test, y_pred)
+
+# Print the evaluation metrics
+print("Mean Squared Error:", mse)
+print("R-squared Score:", r2)"""
+
+    return s 
+
```

