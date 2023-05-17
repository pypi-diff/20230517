# Comparing `tmp/pypipr-0.1.90.tar.gz` & `tmp/pypipr-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-0.1.90.tar", max compression
+gzip compressed data, was "pypipr-0.1.91.tar", max compression
```

## Comparing `pypipr-0.1.90.tar` & `pypipr-0.1.91.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2022-10-24 06:22:00.291550 pypipr-0.1.90/pypipr/__init__.py
--rw-r--r--   0        0        0    34411 2023-05-17 11:40:01.977129 pypipr-0.1.90/pypipr/pypipr.py
--rw-r--r--   0        0        0      615 2023-05-17 11:40:29.767386 pypipr-0.1.90/pyproject.toml
--rw-r--r--   0        0        0    14981 2023-05-17 11:40:11.143420 pypipr-0.1.90/README.md
--rw-r--r--   0        0        0    15893 1970-01-01 00:00:00.000000 pypipr-0.1.90/setup.py
--rw-r--r--   0        0        0    14873 1970-01-01 00:00:00.000000 pypipr-0.1.90/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-24 06:22:00.291550 pypipr-0.1.91/pypipr/__init__.py
+-rw-r--r--   0        0        0    34611 2023-05-17 12:17:45.699620 pypipr-0.1.91/pypipr/pypipr.py
+-rw-r--r--   0        0        0      615 2023-05-17 12:18:26.826931 pypipr-0.1.91/pyproject.toml
+-rw-r--r--   0        0        0    15120 2023-05-17 12:17:49.111037 pypipr-0.1.91/README.md
+-rw-r--r--   0        0        0    16032 1970-01-01 00:00:00.000000 pypipr-0.1.91/setup.py
+-rw-r--r--   0        0        0    15008 1970-01-01 00:00:00.000000 pypipr-0.1.91/PKG-INFO
```

### Comparing `pypipr-0.1.90/pypipr/pypipr.py` & `pypipr-0.1.91/pypipr/pypipr.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,16 +238,18 @@
                 f"[{start} - {finish}] tidak dapat diidentifikasi kesamaannya"
             )
 
         counter_class, converter_class = casting_class()
         start = counter_class(start)
         finish = counter_class(finish)
 
+        step = 1 if is_empty(step) else int(step)
+
         faktor = 1 if finish > start else -1
-        step = int(step) * faktor
+        step *= faktor
         finish += faktor
 
         for i in range(start, finish, step):
             yield converter_class(i)
 
     def sets_ordered(iterator):
         """
@@ -1184,40 +1186,43 @@
     """
     return os.path.dirname(path)
 
 
 class Batchmaker:
     """
     Alat Bantu untuk membuat teks yang berulang.
-    Gunakan {...-...}.
+    Gunakan {[start]-[finish][-[step]]}.
+    ```
+    [start] dan [finish]    -> bisa berupa huruf maupun angka
+    [-[step]]               -> bersifat optional
+    ```
 
     ```python
-    s = "Urutan {1-3} dan {3-1} dan {a-d} dan {D-A} saja."
+    s = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."
     print(Batchmaker(s).result())
     ```
     """
 
-    regex_pattern = r"\{([0-9a-zA-Z]+)\-([0-9a-zA-Z]+)\}"
+    regex_pattern = r"\{([0-9a-zA-Z]+)\-([0-9a-zA-Z]+)(?:\-(\d+))?\}"
     regex_compile = re.compile(regex_pattern)
 
     def __init__(self, pattern) -> None:
         self.text: str = pattern
 
     def result(self):
         s = self.regex_compile.search(self.text)
 
         if s is None:
             return [self.text]
 
         find = s.group()
-        start = s.group(1)
-        finish = s.group(2)
+        start, finish, step = s.groups()
 
         result = list()
-        for i in generator.irange(start, finish):
+        for i in generator.irange(start, finish, step):
             r = self.text.replace(find, i)
             result += Batchmaker(r).result()
 
         return result
 
 
 def filter_empty(iterable, zero_is_empty=True, str_strip=True):
```

### Comparing `pypipr-0.1.90/pyproject.toml` & `pypipr-0.1.91/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypipr"
-version = "0.1.90"
+version = "0.1.91"
 description = "The Python Package Index Project"
 authors = ["ufiapjj <ufiapjj@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 getch = { version = "*", markers = "platform_system == 'Linux'" }
```

### Comparing `pypipr-0.1.90/README.md` & `pypipr-0.1.91/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -601,18 +601,22 @@
 
 # CLASS
 
 ## Batchmaker
 `Batchmaker`
 
 Alat Bantu untuk membuat teks yang berulang.
-Gunakan {...-...}.
+Gunakan {[start]-[finish][-[step]]}.
+```
+[start] dan [finish]    -> bisa berupa huruf maupun angka
+[-[step]]               -> bersifat optional
+```
 
 ```python
-s = "Urutan {1-3} dan {3-1} dan {a-d} dan {D-A} saja."
+s = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."
 print(Batchmaker(s).result())
 ```
 
 
 ## ComparePerformance
 `ComparePerformance`
```

### Comparing `pypipr-0.1.90/setup.py` & `pypipr-0.1.91/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'tzdata']
 
 extras_require = \
 {':platform_system == "Linux"': ['getch']}
 
 setup_kwargs = {
     'name': 'pypipr',
-    'version': '0.1.90',
+    'version': '0.1.91',
     'description': 'The Python Package Index Project',
-    'long_description': '\n# About\nThe Python Package Index Project (pypipr)\n\npypi : https://pypi.org/project/pypipr\n\n\n# Setup\nInstall with pip\n```\npython -m pip install pypipr\n```\n\nImport with * for fastest access\n```python\nfrom pypipr.pypipr import *\n```\n\n# CONSTANT\n\n`LINUX`\n\n`WINDOWS`\n\n# FUNCTION\n\n## avg\n`avg`\n\nSimple Average Function karena tidak disediakan oleh python\n\n```python\nn = [1, 22, 2, 3, 13, 2, 123, 12, 31, 2, 2, 12, 2, 1]\nprint(avg(n))\n```\n\n\n## basename\n`basename`\n\nMengembalikan nama file dari path\n\n```python\nprint(basename("/ini/nama/folder/ke/file.py"))\n```\n\n\n## chunck_array\n`chunck_array`\n\nMembagi array menjadi potongan-potongan dengan besaran yg diinginkan\n\n```python\narray = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]\nprint(generator.chunck_array(array, 5))\nprint(chunck_array(array, 5))\n```\n\n\n## console_run\n`console_run`\n\nMenjalankan command seperti menjalankan command di Command Terminal\n\n\n## create_folder\n`create_folder`\n\nMembuat folder.\nMembuat folder secara recursive dengan permission.\n\n```py\ncreate_folder("contoh_membuat_folder")\ncreate_folder("contoh/membuat/folder/recursive")\ncreate_folder("./contoh_membuat_folder/secara/recursive")\n```\n\n\n## datetime_from_string\n`datetime_from_string`\n\nParse iso_string menjadi datetime object\n\n```python\nprint(datetime_from_string("2022-12-12 15:40:13").isoformat())\nprint(datetime_from_string("2022-12-12 15:40:13", timezone="Asia/Jakarta").isoformat())\n```\n\n\n## datetime_now\n`datetime_now`\n\nMemudahkan dalam membuat Datetime untuk suatu timezone tertentu\n\n```python\nprint(datetime_now("Asia/Jakarta"))\nprint(datetime_now("GMT"))\nprint(datetime_now("Etc/GMT+7"))\n```\n\n\n## dict_first\n`dict_first`\n\nMengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple\n\n```python\nd = {\n    "key1": "value1",\n    "key2": "value2",\n    "key3": "value3",\n}\nprint(dict_first(d))\n```\n\n\n## dirname\n`dirname`\n\nMengembalikan nama folder dari path.\nTanpa trailing slash di akhir.\n\n```python\nprint(dirname("/ini/nama/folder/ke/file.py"))\n```\n\n\n## exit_if_empty\n`exit_if_empty`\n\nKeluar dari program apabila seluruh variabel\nsetara dengan empty\n\n```python\nvar1 = None\nvar2 = \'0\'\nexit_if_empty(var1, var2)\n```\n\n\n## explode\n`explode`\n\nMemecah text menjadi list berdasarkan separator.\n\n```python\nt = \'/ini/contoh/path/\'\nprint(explode(t, separator=\'/\'))\n```\n\n\n## file_get_contents\n`file_get_contents`\n\nMembaca seluruh isi file ke memory.\nApabila file tidak ada maka akan return None.\nApabila file ada tetapi kosong, maka akan return empty string\n\n```py\nprint(file_get_contents("ifile_test.txt"))\n```\n\n\n## file_put_contents\n`file_put_contents`\n\nMenuliskan content ke file.\nApabila file tidak ada maka file akan dibuat.\nApabila file sudah memiliki content maka akan di overwrite.\n\n```py\nfile_put_contents("ifile_test.txt", "Contoh menulis content")\n```\n\n\n## filter_empty\n`filter_empty`\n\n\n## get_class_method\n`get_class_method`\n\nMengembalikan berupa tuple yg berisi list dari method dalam class\n\n```python\nclass ExampleGetClassMethod:\n    def a():\n        return [x for x in range(10)]\n\n    def b():\n        return [x for x in range(10)]\n\n    def c():\n        return [x for x in range(10)]\n\n    def d():\n        return [x for x in range(10)]\n\nif __name__ == "__main__":\n    print(get_class_method(ExampleGetClassMethod))\n```\n\n\n## get_filemtime\n`get_filemtime`\n\nMengambil informasi last modification time file dalam nano seconds\n\n```python\nprint(get_filemtime(__file__))\n```\n\n\n## get_filesize\n`get_filesize`\n\nMengambil informasi file size dalam bytes\n\n```python\nprint(get_filesize(__file__))\n```\n\n\n## github_pull\n`github_pull`\n\nMenjalankan command `git pull`\n\n```py\ngithub_pull()\n```\n\n\n## github_push\n`github_push`\n\nMenjalankan command status, add, commit dan push\n\n```py\ngithub_push(\'Commit Message\')\n```\n\n\n## html_get_contents\n`html_get_contents`\n\nMengambil content html dari url.\n\nRETURN:\n- String: Apabila hanya url saja yg diberikan\n- List of etree: Apabila xpath diberikan\n- False: Apabila terjadi error\n\n```py\nprint(html_get_contents("https://arbadzukhron.deta.dev/"))\n```\n```python\n# Using XPATH\na = html_get_contents("https://www.google.com/", xpath="//a")\nfor i in a:\n    print(i.text)\n    print(i.attrib.get(\'href\'))\n\n# Using REGEX\na = html_get_contents("https://www.google.com/", regex=r"(<a.[^>]+>(?:(?:\\s+)?(.[^<]+)(?:\\s+)?)<\\/a>)")\nfor i in a:\n    print(i)\n\n# Using cssselect\na = html_get_contents("https://www.google.com/", css_select="a")\nfor i in a:\n    print(i.text)\n    print(i.attrib.get("href"))\n```\n\n\n## html_put_contents\n`html_put_contents`\n\nFungsi untuk mengirim data ke URL dengan method POST dan mengembalikan\nrespon dari server sebagai string.\n\nParameters:\n    url (str): URL tujuan.\n    data (dict): Data yang akan dikirim.\n\nReturns:\n- str: Respon dari server dalam bentuk string.\n\n```python\ndata = dict(pengirim="saya", penerima="kamu")\nprint(html_put_contents("https://arbadzukhron.deta.dev/", data))\n```\n\n\n## implode\n`implode`\n\nSimplify Python join functions like PHP function.\nIterable bisa berupa sets, tuple, list, dictionary.\n\n```python\narr = {\'asd\',\'dfs\',\'weq\',\'qweqw\'}\nprint(implode(arr, \', \'))\n\narr = \'/ini/path/seperti/url/\'.split(\'/\')\nprint(implode(arr, \',\'))\nprint(implode(arr, \',\', remove_empty=True))\n\narr = {\'a\':\'satu\', \'b\':(12, 34, 56), \'c\':\'tiga\', \'d\':\'empat\'}\nprint(implode(arr, separator=\'</li>\\n<li>\', start=\'<li>\', end=\'</li>\', recursive_flat=True))\nprint(implode(arr, separator=\'</div>\\n<div>\', start=\'<div>\', end=\'</div>\'))\nprint(implode(10, \' \'))\n```\n\n\n## input_char\n`input_char`\n\nMeminta masukan satu huruf tanpa menekan Enter.\n\n```py\ninput_char("Input char : ")\ninput_char("Input char : ", default=\'Y\')\ninput_char("Input Char without print : ", echo_char=False)\n```\n\n\n## irange\n`irange`\n\nImprove python range() function untuk pengulangan menggunakan huruf\n\n```python\nprint(generator.irange(\'a\', \'z\'))\nprint(irange(\'H\', \'a\'))\nprint(irange(\'1\', \'5\', 3))\nprint(irange(\'1\', 5, 3))\n# print(irange(\'a\', 5, 3))\nprint(irange(-10, 4, 3))\nprint(irange(1, 5))\n```\n\n\n## is_empty\n`is_empty`\n\nMengecek apakah variable setara dengan nilai kosong pada empty.\n\nPengecekan nilai yang setara menggunakan simbol \'==\', sedangkan untuk\npengecekan lokasi memory yang sama menggunakan keyword \'is\'\n\n```python\nprint(is_empty("teks"))\nprint(is_empty(True))\nprint(is_empty(False))\nprint(is_empty(None))\nprint(is_empty(0))\nprint(is_empty([]))\n```\n\n\n## is_iterable\n`is_iterable`\n\nMengecek apakah suatu variabel bisa dilakukan forloop atau tidak\n\n```python\ns = \'ini string\'\nprint(is_iterable(s))\n\nl = [12,21,2,1]\nprint(is_iterable(l))\n\nr = range(100)\nprint(is_iterable(r))\n\nd = {\'a\':1, \'b\':2}\nprint(is_iterable(d.values()))\n```\n\n\n## iscandir\n`iscandir`\n\nMempermudah scandir untuk mengumpulkan folder, subfolder dan file\n\n```py\nfor i in generator.iscandir():\n    print(i)\n\nfor i in iscandir():\n    print(i)\n```\n\n\n## log\n`log`\n\nDecorator untuk mempermudah pembuatan log karena tidak perlu mengubah fungsi yg sudah ada.\nMelakukan print ke console untuk menginformasikan proses yg sedang berjalan didalam program.\n\n```python\n@log\ndef some_function():\n    pass\n\n@log()\ndef some_function_again():\n    pass\n\n@log("Calling some function")\ndef some_function_more():\n    pass\n\nif __name__ == "__main__":\n    some_function()\n    some_function_again()\n    some_function_more()\n```\n\n\n## print_colorize\n`print_colorize`\n\nPrint text dengan warna untuk menunjukan text penting\n\n```python\nprint_colorize("Print some text")\nprint_colorize("Print some text", color=colorama.Fore.RED)\n```\n\n\n## print_dir\n`print_dir`\n\nPrint property dan method yang tersedia pada variabel\n\n```python\np = pathlib.Path("c:/arba/dzukhron.dz")\nprint_dir(p)\n```\n\n\n## print_log\n`print_log`\n\nAkan melakukan print ke console.\nBerguna untuk memberikan informasi proses program yg sedang berjalan.\n\n```python\nprint_log("Standalone Log")\n```\n\n\n## random_bool\n`random_bool`\n\nMenghasilkan nilai random True atau False.\nFungsi ini merupakan fungsi tercepat untuk mendapatkan random bool.\n\n```python\nprint(random_bool())\n```\n\n\n## scan_file\n`scan_file`\n\nMengumpulkan nama-nama file dalam folder dan subfolder.\n\n```py\nfor i in generator.scan_file():\n    print(i)\n\nfor i in scan_file():\n    print(i)\n```\n\n\n## scan_folder\n`scan_folder`\n\nMengumpulkan nama-nama folder dan subfolder.\nTidak termasuk [".", ".."] dan file.\n\n```python\nfor i in generator.scan_folder(recursive=False):\n    print(i)\n\nfor i in scan_folder(recursive=False):\n    print(i)\n```\n\n\n## serialize\n`serialize`\n\nMengubah variabel data menjadi string untuk yang dapat dibaca untuk disimpan.\nString yang dihasilkan berbentuk syntax YAML.\n\n```python\ndata = {\n    \'a\': 123,\n    \'t\': [\'disini\', \'senang\', \'disana\', \'senang\'],\n    \'l\': (12, 23, [12, 42])\n}\nprint(serialize(data))\n```\n\n\n## set_timeout\n`set_timeout`\n\nMenjalankan fungsi ketika sudah sekian detik.\nApabila timeout masih berjalan tapi kode sudah selesai dieksekusi semua, maka\nprogram tidak akan berhenti sampai timeout selesai, kemudian fungsi dijalankan,\nkemudian program dihentikan.\n\n```python\nset_timeout(3, lambda: print("Timeout 3"))\nx = set_timeout(7, lambda: print("Timeout 7"))\nprint(x)\nprint("menghentikan timeout 7")\nx.cancel()\n```\n\n\n## sets_ordered\n`sets_ordered`\n\nHanya mengambil nilai unik dari suatu list\n\n```python\narray = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]\nprint(generator.sets_ordered(array))\nprint(sets_ordered(array))\n```\n\n\n## strtr\n`strtr`\n\nSTRing TRanslate, mengubah string menggunakan kamus dari dict.\n\n```python\ntext = \'aku disini mau kemana saja\'\nreplacements = {\n    "disini": "disitu",\n    "kemana": "kesini",\n}\nprint(strtr(text, replacements))\n```\n\n\n## strtr_regex\n`strtr_regex`\n\nSTRing TRanslate metode Regex, mengubah string menggunakan kamus dari dict.\n\n```python\ntext = \'aku {{ ini }} mau ke {{ sini }} mau kemana saja\'\nreplacements = {\n    r"\\{\\{\\s*(ini)\\s*\\}\\}": r"itu dan \\1",\n    r"\\{\\{\\s*sini\\s*\\}\\}": r"situ",\n}\nprint(strtr_regex(text, replacements))\n```\n\n\n## to_str\n`to_str`\n\nMengubah value menjadi string literal\n\n```python\nprint(to_str(5))\nprint(to_str([]))\nprint(to_str(False))\nprint(to_str(True))\nprint(to_str(None))\n```\n\n\n## unserialize\n`unserialize`\n\nMengubah string data hasil dari serialize menjadi variabel.\nString data adalah berupa syntax YAML.\n\n```python\ndata = {\n    \'a\': 123,\n    \'t\': [\'disini\', \'senang\', \'disana\', \'senang\'],\n    \'l\': (12, 23, [12, 42])\n}\ns = serialize(data)\nprint(unserialize(s))\n```\n\n\n# CLASS\n\n## Batchmaker\n`Batchmaker`\n\nAlat Bantu untuk membuat teks yang berulang.\nGunakan {...-...}.\n\n```python\ns = "Urutan {1-3} dan {3-1} dan {a-d} dan {D-A} saja."\nprint(Batchmaker(s).result())\n```\n\n\n## ComparePerformance\n`ComparePerformance`\n\nMenjalankan seluruh method dalam class,\nkemudian membandingkan waktu yg diperlukan.\n\n```python\nclass ExampleComparePerformance(ComparePerformance):\n    # number = 1\n    z = 10\n\n    def a(self):\n        return (x for x in range(self.z))\n\n    def b(self):\n        return tuple(x for x in range(self.z))\n\n    def c(self):\n        return [x for x in range(self.z)]\n\n    def d(self):\n        return list(x for x in range(self.z))\n\nif __name__ == "__main__":\n    print(ExampleComparePerformance().compare_result())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n```\n\n\n## RunParallel\n`RunParallel`\n\nMenjalankan program secara bersamaan.\n\nStructure:\n- Semua methods akan dijalankan secara paralel kecuali method dengan nama yg diawali underscore `_`\n- Method untuk multithreading/multiprocessing harus memiliki 2 parameter, yaitu: `result: dict` dan `q: queue.Queue`. Parameter `result` digunaan untuk memberikan return value dari method, dan Parameter `q` digunakan untuk mengirim data antar proses.\n- Method untuk asyncio harus menggunakan keyword `async def`, dan untuk perpindahan antar kode menggunakan `await asyncio.sleep(0)`, dan keyword `return` untuk memberikan return value.\n- Return Value berupa dictionary dengan key adalah nama function, dan value adalah return value dari setiap fungsi\n\nNote:\n- `class RunParallel` didesain hanya untuk pemrosesan data saja.\n- Penggunaannya `class RunParallel` dengan cara membuat instance sub class beserta data yg akan diproses, kemudian panggil fungsi yg dipilih `run_asyncio / run_multi_threading / run_multi_processing`, kemudian dapatkan hasilnya.\n- `class RunParallel` tidak didesain untuk menyimpan data, karena setiap module terutama module `multiprocessing` tidak dapat mengakses data kelas dari proses yg berbeda.\n\n```python\nclass ExampleRunParallel(RunParallel):\n    z = "ini"\n\n    def __init__(self) -> None:\n        self.pop = random.randint(0, 100)\n\n    def _set_property_here(self, v):\n        self.prop = v\n\n    def a(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["a"] = "a"\n        q.put("from a 1")\n        q.put("from a 2")\n\n    def b(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["b"] = "b"\n        result["q_get"] = q.get()\n\n    def c(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["c"] = "c"\n        result["q_get"] = q.get()\n\n    async def d(self):\n        print("hello")\n        await asyncio.sleep(0)\n        print("hello")\n\n        result = {}\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["d"] = "d"\n        return result\n\n    async def e(self):\n        print("world")\n        await asyncio.sleep(0)\n        print("world")\n\n        result = {}\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["e"] = "e"\n        return result\n\nif __name__ == "__main__":\n    print(ExampleRunParallel().run_asyncio())\n    print(ExampleRunParallel().run_multi_threading())\n    print(ExampleRunParallel().run_multi_processing())\n```\n\n\n## generator\n`generator`\n\nClass ini menyediakan beberapa fungsi yang bisa mengembalikan generator.\nDigunakan untuk mengoptimalkan program.\n\nClass ini dibuat karena python generator yang disimpan dalam variabel\nhanya dapat diakses satu kali.\n\n',
+    'long_description': '\n# About\nThe Python Package Index Project (pypipr)\n\npypi : https://pypi.org/project/pypipr\n\n\n# Setup\nInstall with pip\n```\npython -m pip install pypipr\n```\n\nImport with * for fastest access\n```python\nfrom pypipr.pypipr import *\n```\n\n# CONSTANT\n\n`LINUX`\n\n`WINDOWS`\n\n# FUNCTION\n\n## avg\n`avg`\n\nSimple Average Function karena tidak disediakan oleh python\n\n```python\nn = [1, 22, 2, 3, 13, 2, 123, 12, 31, 2, 2, 12, 2, 1]\nprint(avg(n))\n```\n\n\n## basename\n`basename`\n\nMengembalikan nama file dari path\n\n```python\nprint(basename("/ini/nama/folder/ke/file.py"))\n```\n\n\n## chunck_array\n`chunck_array`\n\nMembagi array menjadi potongan-potongan dengan besaran yg diinginkan\n\n```python\narray = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]\nprint(generator.chunck_array(array, 5))\nprint(chunck_array(array, 5))\n```\n\n\n## console_run\n`console_run`\n\nMenjalankan command seperti menjalankan command di Command Terminal\n\n\n## create_folder\n`create_folder`\n\nMembuat folder.\nMembuat folder secara recursive dengan permission.\n\n```py\ncreate_folder("contoh_membuat_folder")\ncreate_folder("contoh/membuat/folder/recursive")\ncreate_folder("./contoh_membuat_folder/secara/recursive")\n```\n\n\n## datetime_from_string\n`datetime_from_string`\n\nParse iso_string menjadi datetime object\n\n```python\nprint(datetime_from_string("2022-12-12 15:40:13").isoformat())\nprint(datetime_from_string("2022-12-12 15:40:13", timezone="Asia/Jakarta").isoformat())\n```\n\n\n## datetime_now\n`datetime_now`\n\nMemudahkan dalam membuat Datetime untuk suatu timezone tertentu\n\n```python\nprint(datetime_now("Asia/Jakarta"))\nprint(datetime_now("GMT"))\nprint(datetime_now("Etc/GMT+7"))\n```\n\n\n## dict_first\n`dict_first`\n\nMengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple\n\n```python\nd = {\n    "key1": "value1",\n    "key2": "value2",\n    "key3": "value3",\n}\nprint(dict_first(d))\n```\n\n\n## dirname\n`dirname`\n\nMengembalikan nama folder dari path.\nTanpa trailing slash di akhir.\n\n```python\nprint(dirname("/ini/nama/folder/ke/file.py"))\n```\n\n\n## exit_if_empty\n`exit_if_empty`\n\nKeluar dari program apabila seluruh variabel\nsetara dengan empty\n\n```python\nvar1 = None\nvar2 = \'0\'\nexit_if_empty(var1, var2)\n```\n\n\n## explode\n`explode`\n\nMemecah text menjadi list berdasarkan separator.\n\n```python\nt = \'/ini/contoh/path/\'\nprint(explode(t, separator=\'/\'))\n```\n\n\n## file_get_contents\n`file_get_contents`\n\nMembaca seluruh isi file ke memory.\nApabila file tidak ada maka akan return None.\nApabila file ada tetapi kosong, maka akan return empty string\n\n```py\nprint(file_get_contents("ifile_test.txt"))\n```\n\n\n## file_put_contents\n`file_put_contents`\n\nMenuliskan content ke file.\nApabila file tidak ada maka file akan dibuat.\nApabila file sudah memiliki content maka akan di overwrite.\n\n```py\nfile_put_contents("ifile_test.txt", "Contoh menulis content")\n```\n\n\n## filter_empty\n`filter_empty`\n\n\n## get_class_method\n`get_class_method`\n\nMengembalikan berupa tuple yg berisi list dari method dalam class\n\n```python\nclass ExampleGetClassMethod:\n    def a():\n        return [x for x in range(10)]\n\n    def b():\n        return [x for x in range(10)]\n\n    def c():\n        return [x for x in range(10)]\n\n    def d():\n        return [x for x in range(10)]\n\nif __name__ == "__main__":\n    print(get_class_method(ExampleGetClassMethod))\n```\n\n\n## get_filemtime\n`get_filemtime`\n\nMengambil informasi last modification time file dalam nano seconds\n\n```python\nprint(get_filemtime(__file__))\n```\n\n\n## get_filesize\n`get_filesize`\n\nMengambil informasi file size dalam bytes\n\n```python\nprint(get_filesize(__file__))\n```\n\n\n## github_pull\n`github_pull`\n\nMenjalankan command `git pull`\n\n```py\ngithub_pull()\n```\n\n\n## github_push\n`github_push`\n\nMenjalankan command status, add, commit dan push\n\n```py\ngithub_push(\'Commit Message\')\n```\n\n\n## html_get_contents\n`html_get_contents`\n\nMengambil content html dari url.\n\nRETURN:\n- String: Apabila hanya url saja yg diberikan\n- List of etree: Apabila xpath diberikan\n- False: Apabila terjadi error\n\n```py\nprint(html_get_contents("https://arbadzukhron.deta.dev/"))\n```\n```python\n# Using XPATH\na = html_get_contents("https://www.google.com/", xpath="//a")\nfor i in a:\n    print(i.text)\n    print(i.attrib.get(\'href\'))\n\n# Using REGEX\na = html_get_contents("https://www.google.com/", regex=r"(<a.[^>]+>(?:(?:\\s+)?(.[^<]+)(?:\\s+)?)<\\/a>)")\nfor i in a:\n    print(i)\n\n# Using cssselect\na = html_get_contents("https://www.google.com/", css_select="a")\nfor i in a:\n    print(i.text)\n    print(i.attrib.get("href"))\n```\n\n\n## html_put_contents\n`html_put_contents`\n\nFungsi untuk mengirim data ke URL dengan method POST dan mengembalikan\nrespon dari server sebagai string.\n\nParameters:\n    url (str): URL tujuan.\n    data (dict): Data yang akan dikirim.\n\nReturns:\n- str: Respon dari server dalam bentuk string.\n\n```python\ndata = dict(pengirim="saya", penerima="kamu")\nprint(html_put_contents("https://arbadzukhron.deta.dev/", data))\n```\n\n\n## implode\n`implode`\n\nSimplify Python join functions like PHP function.\nIterable bisa berupa sets, tuple, list, dictionary.\n\n```python\narr = {\'asd\',\'dfs\',\'weq\',\'qweqw\'}\nprint(implode(arr, \', \'))\n\narr = \'/ini/path/seperti/url/\'.split(\'/\')\nprint(implode(arr, \',\'))\nprint(implode(arr, \',\', remove_empty=True))\n\narr = {\'a\':\'satu\', \'b\':(12, 34, 56), \'c\':\'tiga\', \'d\':\'empat\'}\nprint(implode(arr, separator=\'</li>\\n<li>\', start=\'<li>\', end=\'</li>\', recursive_flat=True))\nprint(implode(arr, separator=\'</div>\\n<div>\', start=\'<div>\', end=\'</div>\'))\nprint(implode(10, \' \'))\n```\n\n\n## input_char\n`input_char`\n\nMeminta masukan satu huruf tanpa menekan Enter.\n\n```py\ninput_char("Input char : ")\ninput_char("Input char : ", default=\'Y\')\ninput_char("Input Char without print : ", echo_char=False)\n```\n\n\n## irange\n`irange`\n\nImprove python range() function untuk pengulangan menggunakan huruf\n\n```python\nprint(generator.irange(\'a\', \'z\'))\nprint(irange(\'H\', \'a\'))\nprint(irange(\'1\', \'5\', 3))\nprint(irange(\'1\', 5, 3))\n# print(irange(\'a\', 5, 3))\nprint(irange(-10, 4, 3))\nprint(irange(1, 5))\n```\n\n\n## is_empty\n`is_empty`\n\nMengecek apakah variable setara dengan nilai kosong pada empty.\n\nPengecekan nilai yang setara menggunakan simbol \'==\', sedangkan untuk\npengecekan lokasi memory yang sama menggunakan keyword \'is\'\n\n```python\nprint(is_empty("teks"))\nprint(is_empty(True))\nprint(is_empty(False))\nprint(is_empty(None))\nprint(is_empty(0))\nprint(is_empty([]))\n```\n\n\n## is_iterable\n`is_iterable`\n\nMengecek apakah suatu variabel bisa dilakukan forloop atau tidak\n\n```python\ns = \'ini string\'\nprint(is_iterable(s))\n\nl = [12,21,2,1]\nprint(is_iterable(l))\n\nr = range(100)\nprint(is_iterable(r))\n\nd = {\'a\':1, \'b\':2}\nprint(is_iterable(d.values()))\n```\n\n\n## iscandir\n`iscandir`\n\nMempermudah scandir untuk mengumpulkan folder, subfolder dan file\n\n```py\nfor i in generator.iscandir():\n    print(i)\n\nfor i in iscandir():\n    print(i)\n```\n\n\n## log\n`log`\n\nDecorator untuk mempermudah pembuatan log karena tidak perlu mengubah fungsi yg sudah ada.\nMelakukan print ke console untuk menginformasikan proses yg sedang berjalan didalam program.\n\n```python\n@log\ndef some_function():\n    pass\n\n@log()\ndef some_function_again():\n    pass\n\n@log("Calling some function")\ndef some_function_more():\n    pass\n\nif __name__ == "__main__":\n    some_function()\n    some_function_again()\n    some_function_more()\n```\n\n\n## print_colorize\n`print_colorize`\n\nPrint text dengan warna untuk menunjukan text penting\n\n```python\nprint_colorize("Print some text")\nprint_colorize("Print some text", color=colorama.Fore.RED)\n```\n\n\n## print_dir\n`print_dir`\n\nPrint property dan method yang tersedia pada variabel\n\n```python\np = pathlib.Path("c:/arba/dzukhron.dz")\nprint_dir(p)\n```\n\n\n## print_log\n`print_log`\n\nAkan melakukan print ke console.\nBerguna untuk memberikan informasi proses program yg sedang berjalan.\n\n```python\nprint_log("Standalone Log")\n```\n\n\n## random_bool\n`random_bool`\n\nMenghasilkan nilai random True atau False.\nFungsi ini merupakan fungsi tercepat untuk mendapatkan random bool.\n\n```python\nprint(random_bool())\n```\n\n\n## scan_file\n`scan_file`\n\nMengumpulkan nama-nama file dalam folder dan subfolder.\n\n```py\nfor i in generator.scan_file():\n    print(i)\n\nfor i in scan_file():\n    print(i)\n```\n\n\n## scan_folder\n`scan_folder`\n\nMengumpulkan nama-nama folder dan subfolder.\nTidak termasuk [".", ".."] dan file.\n\n```python\nfor i in generator.scan_folder(recursive=False):\n    print(i)\n\nfor i in scan_folder(recursive=False):\n    print(i)\n```\n\n\n## serialize\n`serialize`\n\nMengubah variabel data menjadi string untuk yang dapat dibaca untuk disimpan.\nString yang dihasilkan berbentuk syntax YAML.\n\n```python\ndata = {\n    \'a\': 123,\n    \'t\': [\'disini\', \'senang\', \'disana\', \'senang\'],\n    \'l\': (12, 23, [12, 42])\n}\nprint(serialize(data))\n```\n\n\n## set_timeout\n`set_timeout`\n\nMenjalankan fungsi ketika sudah sekian detik.\nApabila timeout masih berjalan tapi kode sudah selesai dieksekusi semua, maka\nprogram tidak akan berhenti sampai timeout selesai, kemudian fungsi dijalankan,\nkemudian program dihentikan.\n\n```python\nset_timeout(3, lambda: print("Timeout 3"))\nx = set_timeout(7, lambda: print("Timeout 7"))\nprint(x)\nprint("menghentikan timeout 7")\nx.cancel()\n```\n\n\n## sets_ordered\n`sets_ordered`\n\nHanya mengambil nilai unik dari suatu list\n\n```python\narray = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]\nprint(generator.sets_ordered(array))\nprint(sets_ordered(array))\n```\n\n\n## strtr\n`strtr`\n\nSTRing TRanslate, mengubah string menggunakan kamus dari dict.\n\n```python\ntext = \'aku disini mau kemana saja\'\nreplacements = {\n    "disini": "disitu",\n    "kemana": "kesini",\n}\nprint(strtr(text, replacements))\n```\n\n\n## strtr_regex\n`strtr_regex`\n\nSTRing TRanslate metode Regex, mengubah string menggunakan kamus dari dict.\n\n```python\ntext = \'aku {{ ini }} mau ke {{ sini }} mau kemana saja\'\nreplacements = {\n    r"\\{\\{\\s*(ini)\\s*\\}\\}": r"itu dan \\1",\n    r"\\{\\{\\s*sini\\s*\\}\\}": r"situ",\n}\nprint(strtr_regex(text, replacements))\n```\n\n\n## to_str\n`to_str`\n\nMengubah value menjadi string literal\n\n```python\nprint(to_str(5))\nprint(to_str([]))\nprint(to_str(False))\nprint(to_str(True))\nprint(to_str(None))\n```\n\n\n## unserialize\n`unserialize`\n\nMengubah string data hasil dari serialize menjadi variabel.\nString data adalah berupa syntax YAML.\n\n```python\ndata = {\n    \'a\': 123,\n    \'t\': [\'disini\', \'senang\', \'disana\', \'senang\'],\n    \'l\': (12, 23, [12, 42])\n}\ns = serialize(data)\nprint(unserialize(s))\n```\n\n\n# CLASS\n\n## Batchmaker\n`Batchmaker`\n\nAlat Bantu untuk membuat teks yang berulang.\nGunakan {[start]-[finish][-[step]]}.\n```\n[start] dan [finish]    -> bisa berupa huruf maupun angka\n[-[step]]               -> bersifat optional\n```\n\n```python\ns = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."\nprint(Batchmaker(s).result())\n```\n\n\n## ComparePerformance\n`ComparePerformance`\n\nMenjalankan seluruh method dalam class,\nkemudian membandingkan waktu yg diperlukan.\n\n```python\nclass ExampleComparePerformance(ComparePerformance):\n    # number = 1\n    z = 10\n\n    def a(self):\n        return (x for x in range(self.z))\n\n    def b(self):\n        return tuple(x for x in range(self.z))\n\n    def c(self):\n        return [x for x in range(self.z)]\n\n    def d(self):\n        return list(x for x in range(self.z))\n\nif __name__ == "__main__":\n    print(ExampleComparePerformance().compare_result())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n    print(ExampleComparePerformance().compare_performance())\n```\n\n\n## RunParallel\n`RunParallel`\n\nMenjalankan program secara bersamaan.\n\nStructure:\n- Semua methods akan dijalankan secara paralel kecuali method dengan nama yg diawali underscore `_`\n- Method untuk multithreading/multiprocessing harus memiliki 2 parameter, yaitu: `result: dict` dan `q: queue.Queue`. Parameter `result` digunaan untuk memberikan return value dari method, dan Parameter `q` digunakan untuk mengirim data antar proses.\n- Method untuk asyncio harus menggunakan keyword `async def`, dan untuk perpindahan antar kode menggunakan `await asyncio.sleep(0)`, dan keyword `return` untuk memberikan return value.\n- Return Value berupa dictionary dengan key adalah nama function, dan value adalah return value dari setiap fungsi\n\nNote:\n- `class RunParallel` didesain hanya untuk pemrosesan data saja.\n- Penggunaannya `class RunParallel` dengan cara membuat instance sub class beserta data yg akan diproses, kemudian panggil fungsi yg dipilih `run_asyncio / run_multi_threading / run_multi_processing`, kemudian dapatkan hasilnya.\n- `class RunParallel` tidak didesain untuk menyimpan data, karena setiap module terutama module `multiprocessing` tidak dapat mengakses data kelas dari proses yg berbeda.\n\n```python\nclass ExampleRunParallel(RunParallel):\n    z = "ini"\n\n    def __init__(self) -> None:\n        self.pop = random.randint(0, 100)\n\n    def _set_property_here(self, v):\n        self.prop = v\n\n    def a(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["a"] = "a"\n        q.put("from a 1")\n        q.put("from a 2")\n\n    def b(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["b"] = "b"\n        result["q_get"] = q.get()\n\n    def c(self, result: dict, q: queue.Queue):\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["c"] = "c"\n        result["q_get"] = q.get()\n\n    async def d(self):\n        print("hello")\n        await asyncio.sleep(0)\n        print("hello")\n\n        result = {}\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["d"] = "d"\n        return result\n\n    async def e(self):\n        print("world")\n        await asyncio.sleep(0)\n        print("world")\n\n        result = {}\n        result["z"] = self.z\n        result["pop"] = self.pop\n        result["e"] = "e"\n        return result\n\nif __name__ == "__main__":\n    print(ExampleRunParallel().run_asyncio())\n    print(ExampleRunParallel().run_multi_threading())\n    print(ExampleRunParallel().run_multi_processing())\n```\n\n\n## generator\n`generator`\n\nClass ini menyediakan beberapa fungsi yang bisa mengembalikan generator.\nDigunakan untuk mengoptimalkan program.\n\nClass ini dibuat karena python generator yang disimpan dalam variabel\nhanya dapat diakses satu kali.\n\n',
     'author': 'ufiapjj',
     'author_email': 'ufiapjj@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pypipr-0.1.90/PKG-INFO` & `pypipr-0.1.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipr
-Version: 0.1.90
+Version: 0.1.91
 Summary: The Python Package Index Project
 Author: ufiapjj
 Author-email: ufiapjj@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -621,18 +621,22 @@
 
 # CLASS
 
 ## Batchmaker
 `Batchmaker`
 
 Alat Bantu untuk membuat teks yang berulang.
-Gunakan {...-...}.
+Gunakan {[start]-[finish][-[step]]}.
+```
+[start] dan [finish]    -> bisa berupa huruf maupun angka
+[-[step]]               -> bersifat optional
+```
 
 ```python
-s = "Urutan {1-3} dan {3-1} dan {a-d} dan {D-A} saja."
+s = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."
 print(Batchmaker(s).result())
 ```
 
 
 ## ComparePerformance
 `ComparePerformance`
```

