# Comparing `tmp/panml-0.0.10.tar.gz` & `tmp/panml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.10.tar", last modified: Wed May 17 11:35:21 2023, max compression
+gzip compressed data, was "panml-0.0.9.tar", last modified: Wed May 17 08:39:10 2023, max compression
```

## Comparing `panml-0.0.10.tar` & `panml-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 11:35:21.287263 panml-0.0.10/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1424 2023-05-17 11:35:21.287378 panml-0.0.10/PKG-INFO
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 11:35:21.287212 panml-0.0.10/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.10/panml/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    23754 2023-05-17 11:25:28.807370 panml-0.0.10/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     7024 2023-05-16 08:12:47.828416 panml-0.0.10/panml/search.py
--rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.10/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2407 2023-05-17 11:32:56.774669 panml-0.0.10/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 08:39:10.304084 panml-0.0.9/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1501 2023-05-17 08:39:10.304230 panml-0.0.9/PKG-INFO
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-17 08:39:10.303995 panml-0.0.9/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.248295 panml-0.0.9/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    22590 2023-05-16 08:12:47.827759 panml-0.0.9/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     7024 2023-05-16 08:12:47.828416 panml-0.0.9/panml/search.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)       39 2023-05-15 13:51:34.871217 panml-0.0.9/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2404 2023-05-17 08:38:54.989634 panml-0.0.9/setup.py
```

### Comparing `panml-0.0.10/PKG-INFO` & `panml-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: panml
-Version: 0.0.10
+Version: 0.0.9
 Summary: PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: williamxn.z@gmail.com
 License: MIT
+Download-URL: https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.9.tar.gz
 Description: PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers.                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others.                       
         
         Quick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide                       
         
         Documentation/Wiki: https://github.com/Pan-ML/panml/wiki
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.10/panml/models.py` & `panml-0.0.9/panml/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -322,54 +322,39 @@
         
         if keep_last:
             return history[-1] # returns last prediction output
         else:
             return history # returns all historical prediction output
         
     # Generate and execute code using (LM powered function)
-    def predict_code(self, text: str, x: Union[int, float, str, pd.DataFrame], variable_names: dict[str, str]={'input': 'x', 'output': 'y'}, 
+    def predict_code(self, text: str, x: Union[int, float, str], variable_names: dict[str, str]={'input': 'x', 'output': 'y'}, 
                      language: str='python', max_tokens: int=500) -> str:
         '''
         Generates code output by prompting a language model from OpenAI with a constrained command that is specific for code generation.
-        Input variables can be a value, or a pandas dataframe
         Variable names are passed into the prompt context to allow the generated code to contain the specified variable names.
-        Returns: text of generated code
+        Returns: generated text of the code
         '''
         # Catch input exceptions
-        if self.model != 'text-davinci-002' and self.model != 'text-davinci-003':
-            raise ValueError(f"The specified model is '{self.model}'. Only 'text-davinci-002' and 'text-davinci-002' are supported in this package for code generation")
+        if self.model != 'text-davinci-002':
+            raise ValueError(f"The specified model is '{self.model}'. Only 'text-davinci-002' is supported in this package for code generation")
         if not isinstance(text, str):
             raise TypeError('Input text needs to be of type: string')
-        if not isinstance(x, int) and not isinstance(x, float) and \
-            not isinstance(x, str) and not isinstance(x, pd.DataFrame):
-            raise TypeError('Input x needs to be of type: int, float, str or pandas dataframe')
         if not isinstance(variable_names, dict):
             raise TypeError('Input variable names needs to be of type: dict')
             
         if 'input' not in variable_names:
             variable_names['input'] = 'x'
         if 'output' not in variable_names:
             variable_names['output'] = 'y'
         
-        # Prompt logic for code generation
-        input_dataframe_col_names = ''
-        if isinstance(x, pd.DataFrame):
-            input_dataframe_col_names = f" dataframe has columns: {', '.join(x.columns.tolist())}"
-            input_arg_context = f"{variable_names['output']} = None" # Set input and output variables
-        else:
-            input_arg_context = f"{variable_names['input']}, {variable_names['output']} = {x}, None" # Set output variables (if input is dataframe)
-
-        prompt_prepend = f"Write {language} code to only produce function and input variable {variable_names['input']}" # Set instruction context
-        prompt_append = f"of variable {variable_names['input']} and return in variable. {input_dataframe_col_names} \
-                         Lastly, call function beginning with '{variable_names['output']} = .., and input of {variable_names['input']}'." # Set prompt details
-        prompt_append = f"{prompt_append} do not show print, do not show enter input." # Set instruction to prevent code showing print or input functions
-        prompt_append = f"{prompt_append} format the code with relevant indentation." # Set instruction to maintain code layout
+        input_vars = f"{variable_names['input']}, {variable_names['output']} = {x}, None" # Set input and output variables
+        prompt_prepend = f'Write {language} code to only produce function and input variable x, then call the function without print, without enter input:'
+        prompt_append = f"of variable {variable_names['input']} and return output in {variable_names['output']}" # Set prompt
         output_context = self.predict(f'{prompt_prepend} {text} {prompt_append}', max_tokens=max_tokens) # Get predicted code snippet
-        code_context = f"{input_arg_context}\n{output_context['text']}" # Create code context
-
+        code_context = f"{input_vars}\n{output_context['text']}" # Create code context
         return code_context
         
     # Embed text
     def embedding(self, text: str, model: str=None) -> list[float]:
         text = text.replace("\n", " ")
         if model is None:
             model = self.model_embedding
```

### Comparing `panml-0.0.10/panml/search.py` & `panml-0.0.9/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.10/setup.py` & `panml-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 from distutils.core import setup
 setup(
   name = 'panml', # package name     
   packages = ['panml'], # package name
-  version = '0.0.10', # version
+  version = '0.0.9', # version
   license = 'MIT', # license
   description = 'PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.', # short description about the package
   long_description = 'PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. \
                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others. \
                       \n\nQuick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide \
                       \n\nDocumentation/Wiki: https://github.com/Pan-ML/panml/wiki', # long description
   author = 'PanML team', # team name
   author_email = 'williamxn.z@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
-  # download_url = 'https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.9.tar.gz', # set a release on GitHub (with release tag) -> Assets -> right click and copy the link
+  download_url = 'https://github.com/Pan-ML/panml/archive/refs/tags/v0.0.9.tar.gz', # set a release on GitHub (with release tag) -> Assets -> right click and copy the link
   keywords = ['generative AI', 'generative model', 'machine learning', 'large language model', # keywords
               'LLM', 'prompt engineering', 'fine tuning', 'prompt tuning', 'retrieval augmentation', 
               'AI safety', 'AI alignment'], 
   install_requires=[  # dependencies
         'huggingface-hub>=0.14.1',
         'numpy>=1.24.3',
         'openai>=0.27.6',
```

