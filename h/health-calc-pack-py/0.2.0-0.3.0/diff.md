# Comparing `tmp/health_calc_pack_py-0.2.0.tar.gz` & `tmp/health_calc_pack_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "health_calc_pack_py-0.2.0.tar", max compression
+gzip compressed data, was "health_calc_pack_py-0.3.0.tar", max compression
```

## Comparing `health_calc_pack_py-0.2.0.tar` & `health_calc_pack_py-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-17 01:13:19.681769 health_calc_pack_py-0.2.0/health_calc_pack_py/__init__.py
--rw-r--r--   0        0        0     2198 2023-05-17 02:07:50.108989 health_calc_pack_py-0.2.0/health_calc_pack_py/app.py
--rw-r--r--   0        0        0      114 2023-05-17 01:13:20.285768 health_calc_pack_py-0.2.0/health_calc_pack_py/imc.py
--rw-r--r--   0        0        0      869 2023-05-17 01:29:17.749957 health_calc_pack_py-0.2.0/health_calc_pack_py/macronutrientes.py
--rw-r--r--   0        0        0     2988 2023-05-17 01:52:51.016461 health_calc_pack_py-0.2.0/health_calc_pack_py/static/swagger.json
--rw-r--r--   0        0        0      234 2023-05-17 01:13:21.222773 health_calc_pack_py-0.2.0/health_calc_pack_py/test_imc.py
--rw-r--r--   0        0        0      510 2023-05-17 01:48:05.517550 health_calc_pack_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1480 2023-05-17 01:46:36.647277 health_calc_pack_py-0.2.0/README.md
--rw-r--r--   0        0        0     1970 1970-01-01 00:00:00.000000 health_calc_pack_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-17 01:13:19.681769 health_calc_pack_py-0.3.0/health_calc_pack_py/__init__.py
+-rw-r--r--   0        0        0     2198 2023-05-17 02:07:50.108989 health_calc_pack_py-0.3.0/health_calc_pack_py/app.py
+-rw-r--r--   0        0        0      114 2023-05-17 01:13:20.285768 health_calc_pack_py-0.3.0/health_calc_pack_py/imc.py
+-rw-r--r--   0        0        0      869 2023-05-17 01:29:17.749957 health_calc_pack_py-0.3.0/health_calc_pack_py/macronutrientes.py
+-rw-r--r--   0        0        0     2988 2023-05-17 01:52:51.016461 health_calc_pack_py-0.3.0/health_calc_pack_py/static/swagger.json
+-rw-r--r--   0        0        0      234 2023-05-17 01:13:21.222773 health_calc_pack_py-0.3.0/health_calc_pack_py/test_imc.py
+-rw-r--r--   0        0        0      510 2023-05-17 02:31:45.405419 health_calc_pack_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1531 2023-05-17 02:28:40.089458 health_calc_pack_py-0.3.0/README.md
+-rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 health_calc_pack_py-0.3.0/PKG-INFO
```

### Comparing `health_calc_pack_py-0.2.0/health_calc_pack_py/app.py` & `health_calc_pack_py-0.3.0/health_calc_pack_py/app.py`

 * *Files identical despite different names*

### Comparing `health_calc_pack_py-0.2.0/health_calc_pack_py/macronutrientes.py` & `health_calc_pack_py-0.3.0/health_calc_pack_py/macronutrientes.py`

 * *Files identical despite different names*

### Comparing `health_calc_pack_py-0.2.0/health_calc_pack_py/static/swagger.json` & `health_calc_pack_py-0.3.0/health_calc_pack_py/static/swagger.json`

 * *Files identical despite different names*

### Comparing `health_calc_pack_py-0.2.0/README.md` & `health_calc_pack_py-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Health Calc Pack Py
 
 Health Calc Pack Py é uma API para calcular o Índice de Massa Corporal (IMC) e os macronutrientes necessários para um indivíduo de acordo com seu objetivo nutricional.
 
 ## Instalação
 
 1. Clone o repositório:
-git clone https://github.com/seu_usuario/health-calc-pack-py.git
+git clone https://github.com/Angelo-Diniz/health-calc-pack-py
 
 
 2. Entre no diretório do projeto:
 cd health_calc_pack_py
 
 3. Crie um ambiente virtual e ative-o (opcional, mas recomendado):
 python -m venv venv
@@ -23,19 +23,22 @@
 ## Executando localmente
 
 Após instalar as dependências, execute o seguinte comando para iniciar o servidor de desenvolvimento:
 python app.py
 
 A API estará disponível em http://localhost:5000. Envie requisições HTTP para os endpoints disponíveis para interagir com a aplicação.
 
+## Swagger
+Acesse o http://localhost:5000/docs/
+
 ## Testes unitários
 python -m unittest discover tests
 
 Isso executará todos os testes unitários definidos na pasta tests e exibirá os resultados.
 
 ## Testes unitários
 Endpoints
 A API fornece os seguintes endpoints:
 
 /imc: Recebe um JSON contendo altura e peso, e retorna o IMC calculado.
 
-/macronutrientes: Recebe um JSON contendo peso e objetivo nutricional, e retorna os macronutrientes calculados.
+/macronutrientes: Recebe um JSON contendo peso e objetivo nutricional, e retorna os macronutrientes calculados.
```

### Comparing `health_calc_pack_py-0.2.0/PKG-INFO` & `health_calc_pack_py-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: health-calc-pack-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: Uma API para calcular IMC e macronutrientes
 Author: Angelo Diniz
 Author-email: angelo.jose.7l@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -16,15 +16,15 @@
 # Health Calc Pack Py
 
 Health Calc Pack Py é uma API para calcular o Índice de Massa Corporal (IMC) e os macronutrientes necessários para um indivíduo de acordo com seu objetivo nutricional.
 
 ## Instalação
 
 1. Clone o repositório:
-git clone https://github.com/seu_usuario/health-calc-pack-py.git
+git clone https://github.com/Angelo-Diniz/health-calc-pack-py
 
 
 2. Entre no diretório do projeto:
 cd health_calc_pack_py
 
 3. Crie um ambiente virtual e ative-o (opcional, mas recomendado):
 python -m venv venv
@@ -38,19 +38,23 @@
 ## Executando localmente
 
 Após instalar as dependências, execute o seguinte comando para iniciar o servidor de desenvolvimento:
 python app.py
 
 A API estará disponível em http://localhost:5000. Envie requisições HTTP para os endpoints disponíveis para interagir com a aplicação.
 
+## Swagger
+Acesse o http://localhost:5000/docs/
+
 ## Testes unitários
 python -m unittest discover tests
 
 Isso executará todos os testes unitários definidos na pasta tests e exibirá os resultados.
 
 ## Testes unitários
 Endpoints
 A API fornece os seguintes endpoints:
 
 /imc: Recebe um JSON contendo altura e peso, e retorna o IMC calculado.
 
 /macronutrientes: Recebe um JSON contendo peso e objetivo nutricional, e retorna os macronutrientes calculados.
+
```

