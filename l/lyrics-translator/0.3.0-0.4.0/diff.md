# Comparing `tmp/lyrics-translator-0.3.0.tar.gz` & `tmp/lyrics_translator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics-translator-0.3.0.tar", max compression
+gzip compressed data, was "lyrics_translator-0.4.0.tar", max compression
```

## Comparing `lyrics-translator-0.3.0.tar` & `lyrics_translator-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     4207 2023-01-08 16:15:14.410000 lyrics-translator-0.3.0/README.md
--rw-r--r--   0        0        0      491 2022-11-05 17:42:46.060000 lyrics-translator-0.3.0/lyrics_translator/__init__.py
--rw-r--r--   0        0        0      901 2023-01-08 15:29:11.530000 lyrics-translator-0.3.0/lyrics_translator/console.py
--rw-r--r--   0        0        0     2867 2023-01-08 15:29:22.190000 lyrics-translator-0.3.0/lyrics_translator/core/lyrics.py
--rw-r--r--   0        0        0     2701 2023-01-08 15:29:28.840000 lyrics-translator-0.3.0/lyrics_translator/core/lyrics_translator.py
--rw-r--r--   0        0        0     1523 2023-01-08 15:20:34.620000 lyrics-translator-0.3.0/lyrics_translator/core/saver.py
--rw-r--r--   0        0        0     5494 2023-01-08 15:49:56.240000 lyrics-translator-0.3.0/lyrics_translator/core/translator.py
--rw-r--r--   0        0        0      758 2022-06-10 18:57:12.137042 lyrics-translator-0.3.0/lyrics_translator/core/utils.py
--rw-r--r--   0        0        0     1206 2023-01-08 15:34:56.900000 lyrics-translator-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5307 2023-01-08 16:15:49.397293 lyrics-translator-0.3.0/setup.py
--rw-r--r--   0        0        0     5087 2023-01-08 16:15:49.397952 lyrics-translator-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5277 2023-03-26 18:03:01.860000 lyrics_translator-0.4.0/README.md
+-rw-r--r--   0        0        0      491 2023-01-17 19:24:47.628153 lyrics_translator-0.4.0/lyrics_translator/__init__.py
+-rw-r--r--   0        0        0      846 2023-01-17 19:23:55.388153 lyrics_translator-0.4.0/lyrics_translator/console.py
+-rw-r--r--   0        0        0     3035 2023-05-17 15:28:25.270254 lyrics_translator-0.4.0/lyrics_translator/core/lyrics.py
+-rw-r--r--   0        0        0     3058 2023-05-17 15:35:15.950255 lyrics_translator-0.4.0/lyrics_translator/core/lyrics_translator.py
+-rw-r--r--   0        0        0     1523 2023-01-08 15:20:34.620000 lyrics_translator-0.4.0/lyrics_translator/core/saver.py
+-rw-r--r--   0        0        0     5745 2023-05-17 15:13:00.950255 lyrics_translator-0.4.0/lyrics_translator/core/translator.py
+-rw-r--r--   0        0        0      758 2022-06-10 18:57:12.137042 lyrics_translator-0.4.0/lyrics_translator/core/utils.py
+-rw-r--r--   0        0        0     1978 2023-05-17 15:46:41.420255 lyrics_translator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6199 1970-01-01 00:00:00.000000 lyrics_translator-0.4.0/PKG-INFO
```

### Comparing `lyrics-translator-0.3.0/README.md` & `lyrics_translator-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,34 +15,46 @@
 
 <a href="https://pypi.org/project/lyrics-translator" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/lyrics-translator.svg" alt="Supported versions">
 </a>
 
 <a href="https://github.com/ambv/black" target="_blank">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="Code style: black">
+</a>
+
 
 <a href="https://pycqa.github.io/isort/" target="_blank">
     <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="Imports: isort">
+</a>
 
 
+<a href="https://github.com/MauroLuzzatto/lyrics-translator/actions?workflow=Tests" target="_blank">
+    <img src="https://github.com/MauroLuzzatto/lyrics-translator/workflows/Tests/badge.svg" alt="Tests">
+</a>
+
 </p>
 
+
 ---
 
 **Documentation**: <a href="https://mauroluzzatto.github.io/lyrics-translator" target="_blank">https://mauroluzzatto.github.io/lyrics-translator</a>
 
 **Source Code**: <a href="https://github.com/MauroLuzzatto/lyrics-translator" target="_blank">https://github.com/MauroLuzzatto/lyrics-translator</a>
 
 ---
 
 
-The `LyricsTranslator` downloads lyrics from [genius](https://genius.com/) and uses 🤗[hugging face](https://huggingface.co/) to translate the lyrics into a target language.
+`LyricsTranslator` is a Python module that allows you to download lyrics from the popular music lyrics website [genius](https://genius.com/) and translate them into a target language of your choice. The module uses the powerful 🤗[hugging face](https://huggingface.co/) library for translation, which provides state-of-the-art performance in natural language processing tasks.
+
+With `LyricsTranslator`, you can easily translate the lyrics of your favorite songs into different languages, allowing you to appreciate the beauty and meaning of the lyrics in a language that you're comfortable with. This can be particularly helpful if you're learning a new language or if you want to explore the cultural nuances of a different language.
+
+The module supports all languages that are available on the [OPUS-MT](https://github.com/Helsinki-NLP/Opus-MT) platform, which includes languages from all around the world. Whether you're interested in German, Spanish, Chinese, Japanese, or any other language, LyricsTranslator has got you covered. The full list of list of languages can be found on 🤗[hugging face](https://huggingface.co/models?other=marian).
 
 
-All languages that are supported by [OPUS-MT](https://github.com/Helsinki-NLP/Opus-MT) are available for translation.The full list of list of languages can be found on 🤗[hugging face](https://huggingface.co/models?other=marian).
+All languages that are supported by [OPUS-MT](https://github.com/Helsinki-NLP/Opus-MT) are available for translation.
 
 - German: `de`
 - Swedish: `sv`
 - French: `fr`
 - Spanish: `es` 
 - Chinese: `zh`
 - Japanese: `ja`
@@ -65,17 +77,14 @@
 ## Setup
 To use the `LyricsTranslator` you will have to [get an API token](https://docs.genius.com/#/getting-started-h1) from `genius` add the API token to the `.env` file:
 
 ```txt
 GENIUS_ACCESS_TOKEN=<replace-me-with-your-genius-api-token>
 ```
 
-## Supported Languages
-
-
 
 ## Usage
 <!--
 📚 A comprehensive example of the `explainy` API can be found in this ![Jupyter Notebook](https://github.com/MauroLuzzatto/explainy/blob/main/examples/01-explainy-intro.ipynb)
 
 📖 Or in the [example section](https://explainy.readthedocs.io/en/latest/examples/01-explainy-intro.html) of the documentation -->
```

#### html2text {}

```diff
@@ -1,24 +1,36 @@
 
       ****** ðµ LyricsTranslator - automated lyrics translation ******
-   [pypi_version] [Supported_versions] [Code_style:_black]_[Imports:_isort]
+   [pypi_version] [Supported_versions] [Code_style:_black] [Imports:_isort]
+                                    [Tests]
 --- **Documentation**: https://mauroluzzatto.github.io/lyrics-translator
-**Source Code**: https://github.com/MauroLuzzatto/lyrics-translator --- The
-`LyricsTranslator` downloads lyrics from [genius](https://genius.com/) and uses
-ð¤[hugging face](https://huggingface.co/) to translate the lyrics into a
-target language. All languages that are supported by [OPUS-MT](https://
-github.com/Helsinki-NLP/Opus-MT) are available for translation.The full list of
-list of languages can be found on ð¤[hugging face](https://huggingface.co/
-models?other=marian). - German: `de` - Swedish: `sv` - French: `fr` - Spanish:
-`es` - Chinese: `zh` - Japanese: `ja` - Portuguese: `pt` - Arabic: `ar` -
-Italian: `it` and many more ... ## Install ``` pip install lyrics-translator
-``` ## Setup To use the `LyricsTranslator` you will have to [get an API token]
-(https://docs.genius.com/#/getting-started-h1) from `genius` add the API token
-to the `.env` file: ```txt GENIUS_ACCESS_TOKEN= ``` ## Supported Languages ##
-Usage  ```python from lyrics_translator import LyricsTranslator song = "Surfin'
+**Source Code**: https://github.com/MauroLuzzatto/lyrics-translator --
+- `LyricsTranslator` is a Python module that allows you to download lyrics from
+the popular music lyrics website [genius](https://genius.com/) and translate
+them into a target language of your choice. The module uses the powerful ð¤
+[hugging face](https://huggingface.co/) library for translation, which provides
+state-of-the-art performance in natural language processing tasks. With
+`LyricsTranslator`, you can easily translate the lyrics of your favorite songs
+into different languages, allowing you to appreciate the beauty and meaning of
+the lyrics in a language that you're comfortable with. This can be particularly
+helpful if you're learning a new language or if you want to explore the
+cultural nuances of a different language. The module supports all languages
+that are available on the [OPUS-MT](https://github.com/Helsinki-NLP/Opus-MT)
+platform, which includes languages from all around the world. Whether you're
+interested in German, Spanish, Chinese, Japanese, or any other language,
+LyricsTranslator has got you covered. The full list of list of languages can be
+found on ð¤[hugging face](https://huggingface.co/models?other=marian). All
+languages that are supported by [OPUS-MT](https://github.com/Helsinki-NLP/Opus-
+MT) are available for translation. - German: `de` - Swedish: `sv` - French:
+`fr` - Spanish: `es` - Chinese: `zh` - Japanese: `ja` - Portuguese: `pt` -
+Arabic: `ar` - Italian: `it` and many more ... ## Install ``` pip install
+lyrics-translator ``` ## Setup To use the `LyricsTranslator` you will have to
+[get an API token](https://docs.genius.com/#/getting-started-h1) from `genius`
+add the API token to the `.env` file: ```txt GENIUS_ACCESS_TOKEN= ``` ## Usage
+```python from lyrics_translator import LyricsTranslator song = "Surfin'
 U.S.A." artist = "The Beach Boys" language = "de" translator = LyricsTranslator
 (language) lyrics = translator.get_song_translation(song, artist) print(lyrics)
 ``` Output: ``` Surfinâ USA Lyrics[Verse 1] Wenn jeder einen Ozean hÃ¤tte
 Ãberall in den USA Dann wÃ¼rde jeder surfen Wie Californi-a Sie wÃ¼rden ihre
 Taschen tragen. Auch Huarache Sandalen Ein stumpfes stumpfes blond Haar Surfin'
 U.S.A [Korus] Sie wÃ¼rden sie surfen in Del Mar (Innen, AuÃen, USA) Ventura
 County Line (Innen, AuÃen, USA) Santa Cruz und Trestles (Innen, AuÃen, USA)
```

### Comparing `lyrics-translator-0.3.0/lyrics_translator/console.py` & `lyrics_translator-0.4.0/lyrics_translator/console.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import textwrap
-
 import click
 
 from lyrics_translator import LyricsTranslator
 
 from . import __version__
 
 
@@ -14,20 +12,17 @@
 @click.option("--artist", default="The Beach Boys", help="Name of the artist.")
 @click.option(
     "--language", default="de", help="Language to song lyrics to translate to."
 )
 @click.option(
     "--testing",
     default=False,
-    help=('Mode of developement, if testing is set to "True" only dummy data is used'),
+    help='Mode of developement, if testing is set to "True" only dummy data is used',
 )
 @click.version_option(version=__version__)
 def main(song, artist, language, testing):
-
     translator = LyricsTranslator(language)
     lyrics = translator.get_song_translation(song, artist, testing)
-    lyrics.get_song_translation()
-
     title = f"'{song}' by '{artist}' translated into '{language}'"
 
     click.secho(title, fg="green")
     click.echo(lyrics)
```

### Comparing `lyrics-translator-0.3.0/lyrics_translator/core/lyrics.py` & `lyrics_translator-0.4.0/lyrics_translator/core/lyrics_translator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,83 @@
-from pathlib import Path
-from typing import Optional
+import lyricsgenius
+from dotenv import dotenv_values
 
-from lyrics_translator.core.saver import Saver
-from lyrics_translator.core.utils import MockGeniusSong
+from lyrics_translator.core.lyrics import Lyrics
+from lyrics_translator.core.translator import Translator
 
+MANDATORY_ENV_VARS = ["GENIUS_ACCESS_TOKEN"]
 
-class Lyrics(object):
-    def __init__(self, song: str, artist: str, testing: bool = None) -> None:
-        self.song = song
-        self.artist = artist
-        self.testing = testing
 
-        self.text: str = None
-        self.translation: str = None
-        self.language: str = None
-
-    def download_lyrics(self, genius, get_full_info: Optional[bool] = False) -> None:
-        """Download the lyrics of the song using the `genius` API.
+class LyricsTranslator(object):
+    def __init__(
+        self,
+        language: str = "de",
+        origin_language="en",
+        config: dict = None,
+        model_name: str = None,
+    ) -> None:
+        """LyricsTranslator main class, which uses the Lyrics class to fetch
+        lyrics and translates them into the target language.
 
         Args:
-            get_full_info (bool): _description_. Defaults to False.
+            language (str): target language that the lyrics should be transalted into. Defaults to "de".
+            origin_language (str, optional): set optional current language of the lyrics for more advanced traslations. Defaults to "en".
+            config (dict): config file to pass in environment variables
+            model_name (str, optional): model name to use for the translation. Defaults to None (uses the default model for the language pair)
 
-        Returns:
-            str: _description_
-        """
-        if self.testing:
-            genius_song = MockGeniusSong(lyrics="<test lyrics>")
-        else:
-            genius_song = genius.search_song(
-                self.song, self.artist, get_full_info=get_full_info
-            )
-
-        if not genius_song:
-            message = f"not found - song: {self.song}, artist: {self.artist}"
-            raise ValueError(message)
-
-        self.text = genius_song.lyrics
-
-    def translate(self, translator, language: str) -> None:
-        """Translate the lyrics into the target language.
-
-        Returns:
-            str: _description_
+        Raises:
+            EnvironmentError: _description_
         """
         self.language = language
+        self.origin_language = origin_language
 
-        if self.testing:
-            self.translation = "<test translation>"
+        if config is None:
+            self.config = dotenv_values(".env")
         else:
-            self.translation = translator.translate(self.text)
-
-    def get_translation(self, translator, language) -> str:
-        self.translate(translator, language)
-        return self.translation
-
-    def get_lyrics(self, genius) -> str:
-        self.download_lyrics(genius)
-        return self.text
+            self.config = config
 
-    def save(self, folder: str = "lyrics", kind: str = "txt") -> None:
-        """Save the translated lyrics to a file.
+        for env_var in MANDATORY_ENV_VARS:
+            if env_var not in self.config:
+                message = (
+                    f"Failed because the envrionment variable '{env_var}' is not set."
+                    f" Add '{env_var}' to the '.env' file and try it again!"
+                )
+                raise EnvironmentError(message)
 
-        Args:
-            folder (Path): _description_
-            kind (str, optional): _description_. Defaults to "txt".
-        """
+        if not model_name:
+            model_name = self.config.get("MODEL_NAME", None)
 
-        if not folder:
-            folder_path = Path().resolve()
-        else:
-            folder_path = Path(folder).resolve()
-            folder_path.mkdir(parents=True, exist_ok=True)
-
-        saver = Saver(
-            song=self.song,
-            artist=self.artist,
-            translation=self.translation,
+        self.translator = Translator(
             language=self.language,
+            origin_language=self.origin_language,
+            model_name=model_name,
         )
-        saver.save(folder=folder_path, kind=kind)
+        self.translator.get_translator_pipeline()
 
-    def __str__(self) -> str:
-        """string version of the Lyrics instance, returns the translated lyrics
+        self.genius = lyricsgenius.Genius(
+            self.config["GENIUS_ACCESS_TOKEN"], timeout=10, retries=3
+        )
 
-        Returns:
-            str: _description_
-        """
-        return self.translation
+    def get_song_lyrics(self, song, artist, testing: bool = False):
+        """retrun only the lyrics of the song"""
+        lyrics = Lyrics(genius=self.genius, song=song, artist=artist, testing=testing)
+        text = lyrics.get_lyrics_text()
+        return text
+
+    def get_song_translation(self, song, artist, testing: bool = False) -> None:
+        """Download the song lyrics from the API and translate them using the Lyrics class."""
+        lyrics = Lyrics(genius=self.genius, song=song, artist=artist, testing=testing)
+        translation = lyrics.get_translation(
+            translator=self.translator, language=self.language
+        )
+        return translation
 
     def __repr__(self) -> str:
-        """Lyrics representation
+        """LyricsTranslator representation
 
         Returns:
             str: returns the string to create the same instance
         """
-        return f"Lyrics(song={self.song}, artist={self.artist})"
+        return (
+            "LyricsTranslator("
+            f" language={self.language}, origin_language={self.origin_language})"
+        )
```

### Comparing `lyrics-translator-0.3.0/lyrics_translator/core/saver.py` & `lyrics_translator-0.4.0/lyrics_translator/core/saver.py`

 * *Files identical despite different names*

### Comparing `lyrics-translator-0.3.0/lyrics_translator/core/translator.py` & `lyrics_translator-0.4.0/lyrics_translator/core/translator.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,55 +6,64 @@
 torch.multiprocessing.freeze_support()
 
 
 cache = {}
 
 
 class Translator(object):
-    def __init__(self, language: str, origin_language: str = "en"):
+    def __init__(self, language: str, origin_language: str = "en", model_name=None):
         self.language = language
         self.origin_language = origin_language
 
+        if model_name:
+            self.model_name = model_name
+        else:
+            self.model_name = self.get_model_name()
+
+    def get_model_name(self) -> str:
+        if self.language == "de" and self.origin_language == "en":
+            model_name = "t5-small"
+        else:
+            print("trying to find the model....")
+            model_name = f"Helsinki-NLP/opus-mt-{self.origin_language}-{self.language}"
+
+        return model_name
+
     @lru_cache(maxsize=5)
     def get_translator_pipeline(self) -> None:
         """[summary]
 
         Raises:
             ValueError: [description]
 
         """
-        if self.language == "de" and self.origin_language == "en":
-            model_name = "t5-small"
-        else:
-            print("trying to find the model....")
-            model_name = f"Helsinki-NLP/opus-mt-{self.origin_language}-{self.language}"
 
-        if model_name in cache:
-            self.translator = cache[model_name]
+        if self.model_name in cache:
+            self.translator = cache[self.model_name]
         else:
             try:
                 tokenizer = AutoTokenizer.from_pretrained(
-                    model_name, model_max_length=512, skip_special_tokens=True
+                    self.model_name, model_max_length=512, skip_special_tokens=True
                 )
-                model = AutoModelForSeq2SeqLM.from_pretrained(model_name)
+                model = AutoModelForSeq2SeqLM.from_pretrained(self.model_name)
 
             except OSError as err:
                 message = f'{err} -- language "{self.language}" is not supported!'
                 raise ValueError(message)
 
             self.translator = pipeline(
                 f"translation_{self.origin_language}_to_{self.language}",
                 model=model,
                 tokenizer=tokenizer,
             )
-            cache[model_name] = self.translator
+            cache[self.model_name] = self.translator
 
         print(
             f'Setup translator_pipeline to translate from "{self.origin_language}" to'
-            f' "{self.language}" using "{model_name}"!'
+            f' "{self.language}" using "{self.model_name}"!'
         )
 
     def translate(self, text: str) -> str:
         """[summary]
 
         Args:
             text (str): [description]
@@ -79,15 +88,14 @@
 
     def load_config():
         """to be implemented"""
         pass
 
 
 if __name__ == "__main__":
-
     language = "de"  # "de"
     short_text = "Hello my friends! How are you doing today?"
 
     long_text = """
         Importing AutoTokenizer and AutoModelForSeq2SeqLM from transformers. Note that you need to import TFAutoModelForSeq2SeqLM if you want the TensorFlow equivalent.
         Initializing the Tokenizer. We’ll be using the Helsinki-NLP pretrained/finetuned OpusMT English to Dutch model for initializing the tokenizer. Using a tokenizer, we can convert textual inputs into tokens.
         Initializing the model. Using the same pretrained/finetuned model, we can generate translations.
@@ -162,14 +170,15 @@
 
         Yeah everybody's gone surfin'
         Surfin' U.S.A
 
         Yeah everybody's gone surfin'
         Surfin' U.S.A12Embed
         """
+
     translator = Translator(language)
-    translator.get_translator_pipeline()
-    # translation = translator.translate(long_text)
-    translation = translator.translate_fast(lyrics)
+    for input in [short_text, long_text, lyrics]:
+        translator.get_translator_pipeline()
+        translation = translator.translate(input)
 
-    print("----" * 10)
-    print(translation)
+        print("----" * 10)
+        print(translation)
```

### Comparing `lyrics-translator-0.3.0/lyrics_translator/core/utils.py` & `lyrics_translator-0.4.0/lyrics_translator/core/utils.py`

 * *Files identical despite different names*

### Comparing `lyrics-translator-0.3.0/PKG-INFO` & `lyrics_translator-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: lyrics-translator
-Version: 0.3.0
+Version: 0.4.0
 Summary: 🎵 LyricsTranslator - automated lyrics translation
 Home-page: https://mauroluzzatto.github.io/lyrics-translator
 License: MIT
 Keywords: lyrics,translation
 Author: Mauro Luzzatto
 Author-email: mauroluzzatto@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: lyricsgenius (>=3.0.1,<4.0.0)
 Requires-Dist: python-docx (>=0.8.11,<0.9.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: sacremoses (>=0.0.53,<0.0.54)
 Requires-Dist: sentencepiece (>=0.1.96,<0.2.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
@@ -41,34 +42,46 @@
 
 <a href="https://pypi.org/project/lyrics-translator" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/lyrics-translator.svg" alt="Supported versions">
 </a>
 
 <a href="https://github.com/ambv/black" target="_blank">
     <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="Code style: black">
+</a>
+
 
 <a href="https://pycqa.github.io/isort/" target="_blank">
     <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="Imports: isort">
+</a>
+
 
+<a href="https://github.com/MauroLuzzatto/lyrics-translator/actions?workflow=Tests" target="_blank">
+    <img src="https://github.com/MauroLuzzatto/lyrics-translator/workflows/Tests/badge.svg" alt="Tests">
+</a>
 
 </p>
 
+
 ---
 
 **Documentation**: <a href="https://mauroluzzatto.github.io/lyrics-translator" target="_blank">https://mauroluzzatto.github.io/lyrics-translator</a>
 
 **Source Code**: <a href="https://github.com/MauroLuzzatto/lyrics-translator" target="_blank">https://github.com/MauroLuzzatto/lyrics-translator</a>
 
 ---
 
 
-The `LyricsTranslator` downloads lyrics from [genius](https://genius.com/) and uses 🤗[hugging face](https://huggingface.co/) to translate the lyrics into a target language.
+`LyricsTranslator` is a Python module that allows you to download lyrics from the popular music lyrics website [genius](https://genius.com/) and translate them into a target language of your choice. The module uses the powerful 🤗[hugging face](https://huggingface.co/) library for translation, which provides state-of-the-art performance in natural language processing tasks.
+
+With `LyricsTranslator`, you can easily translate the lyrics of your favorite songs into different languages, allowing you to appreciate the beauty and meaning of the lyrics in a language that you're comfortable with. This can be particularly helpful if you're learning a new language or if you want to explore the cultural nuances of a different language.
 
+The module supports all languages that are available on the [OPUS-MT](https://github.com/Helsinki-NLP/Opus-MT) platform, which includes languages from all around the world. Whether you're interested in German, Spanish, Chinese, Japanese, or any other language, LyricsTranslator has got you covered. The full list of list of languages can be found on 🤗[hugging face](https://huggingface.co/models?other=marian).
 
-All languages that are supported by [OPUS-MT](https://github.com/Helsinki-NLP/Opus-MT) are available for translation.The full list of list of languages can be found on 🤗[hugging face](https://huggingface.co/models?other=marian).
+
+All languages that are supported by [OPUS-MT](https://github.com/Helsinki-NLP/Opus-MT) are available for translation.
 
 - German: `de`
 - Swedish: `sv`
 - French: `fr`
 - Spanish: `es` 
 - Chinese: `zh`
 - Japanese: `ja`
@@ -91,17 +104,14 @@
 ## Setup
 To use the `LyricsTranslator` you will have to [get an API token](https://docs.genius.com/#/getting-started-h1) from `genius` add the API token to the `.env` file:
 
 ```txt
 GENIUS_ACCESS_TOKEN=<replace-me-with-your-genius-api-token>
 ```
 
-## Supported Languages
-
-
 
 ## Usage
 <!--
 📚 A comprehensive example of the `explainy` API can be found in this ![Jupyter Notebook](https://github.com/MauroLuzzatto/explainy/blob/main/examples/01-explainy-intro.ipynb)
 
 📖 Or in the [example section](https://explainy.readthedocs.io/en/latest/examples/01-explainy-intro.html) of the documentation -->
```

#### html2text {}

```diff
@@ -1,38 +1,51 @@
-Metadata-Version: 2.1 Name: lyrics-translator Version: 0.3.0 Summary: ðµ
+Metadata-Version: 2.1 Name: lyrics-translator Version: 0.4.0 Summary: ðµ
 LyricsTranslator - automated lyrics translation Home-page: https://
 mauroluzzatto.github.io/lyrics-translator License: MIT Keywords:
 lyrics,translation Author: Mauro Luzzatto Author-email:
 mauroluzzatto@hotmail.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: lyricsgenius
-(>=3.0.1,<4.0.0) Requires-Dist: python-docx (>=0.8.11,<0.9.0) Requires-Dist:
-python-dotenv (>=0.20.0,<0.21.0) Requires-Dist: sacremoses (>=0.0.53,<0.0.54)
-Requires-Dist: sentencepiece (>=0.1.96,<0.2.0) Requires-Dist: tqdm
-(>=4.64.1,<5.0.0) Requires-Dist: transformers[torch] (>=4.20.1,<5.0.0) Project-
-URL: Repository, https://github.com/MauroLuzzatto/lyrics-translator
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
+(>=8.1.3,<9.0.0) Requires-Dist: lyricsgenius (>=3.0.1,<4.0.0) Requires-Dist:
+python-docx (>=0.8.11,<0.9.0) Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: sacremoses (>=0.0.53,<0.0.54) Requires-Dist: sentencepiece
+(>=0.1.96,<0.2.0) Requires-Dist: tqdm (>=4.64.1,<5.0.0) Requires-Dist:
+transformers[torch] (>=4.20.1,<5.0.0) Project-URL: Repository, https://
+github.com/MauroLuzzatto/lyrics-translator Description-Content-Type: text/
+markdown
       ****** ðµ LyricsTranslator - automated lyrics translation ******
-   [pypi_version] [Supported_versions] [Code_style:_black]_[Imports:_isort]
+   [pypi_version] [Supported_versions] [Code_style:_black] [Imports:_isort]
+                                    [Tests]
 --- **Documentation**: https://mauroluzzatto.github.io/lyrics-translator
-**Source Code**: https://github.com/MauroLuzzatto/lyrics-translator --- The
-`LyricsTranslator` downloads lyrics from [genius](https://genius.com/) and uses
-ð¤[hugging face](https://huggingface.co/) to translate the lyrics into a
-target language. All languages that are supported by [OPUS-MT](https://
-github.com/Helsinki-NLP/Opus-MT) are available for translation.The full list of
-list of languages can be found on ð¤[hugging face](https://huggingface.co/
-models?other=marian). - German: `de` - Swedish: `sv` - French: `fr` - Spanish:
-`es` - Chinese: `zh` - Japanese: `ja` - Portuguese: `pt` - Arabic: `ar` -
-Italian: `it` and many more ... ## Install ``` pip install lyrics-translator
-``` ## Setup To use the `LyricsTranslator` you will have to [get an API token]
-(https://docs.genius.com/#/getting-started-h1) from `genius` add the API token
-to the `.env` file: ```txt GENIUS_ACCESS_TOKEN= ``` ## Supported Languages ##
-Usage  ```python from lyrics_translator import LyricsTranslator song = "Surfin'
+**Source Code**: https://github.com/MauroLuzzatto/lyrics-translator --
+- `LyricsTranslator` is a Python module that allows you to download lyrics from
+the popular music lyrics website [genius](https://genius.com/) and translate
+them into a target language of your choice. The module uses the powerful ð¤
+[hugging face](https://huggingface.co/) library for translation, which provides
+state-of-the-art performance in natural language processing tasks. With
+`LyricsTranslator`, you can easily translate the lyrics of your favorite songs
+into different languages, allowing you to appreciate the beauty and meaning of
+the lyrics in a language that you're comfortable with. This can be particularly
+helpful if you're learning a new language or if you want to explore the
+cultural nuances of a different language. The module supports all languages
+that are available on the [OPUS-MT](https://github.com/Helsinki-NLP/Opus-MT)
+platform, which includes languages from all around the world. Whether you're
+interested in German, Spanish, Chinese, Japanese, or any other language,
+LyricsTranslator has got you covered. The full list of list of languages can be
+found on ð¤[hugging face](https://huggingface.co/models?other=marian). All
+languages that are supported by [OPUS-MT](https://github.com/Helsinki-NLP/Opus-
+MT) are available for translation. - German: `de` - Swedish: `sv` - French:
+`fr` - Spanish: `es` - Chinese: `zh` - Japanese: `ja` - Portuguese: `pt` -
+Arabic: `ar` - Italian: `it` and many more ... ## Install ``` pip install
+lyrics-translator ``` ## Setup To use the `LyricsTranslator` you will have to
+[get an API token](https://docs.genius.com/#/getting-started-h1) from `genius`
+add the API token to the `.env` file: ```txt GENIUS_ACCESS_TOKEN= ``` ## Usage
+```python from lyrics_translator import LyricsTranslator song = "Surfin'
 U.S.A." artist = "The Beach Boys" language = "de" translator = LyricsTranslator
 (language) lyrics = translator.get_song_translation(song, artist) print(lyrics)
 ``` Output: ``` Surfinâ USA Lyrics[Verse 1] Wenn jeder einen Ozean hÃ¤tte
 Ãberall in den USA Dann wÃ¼rde jeder surfen Wie Californi-a Sie wÃ¼rden ihre
 Taschen tragen. Auch Huarache Sandalen Ein stumpfes stumpfes blond Haar Surfin'
 U.S.A [Korus] Sie wÃ¼rden sie surfen in Del Mar (Innen, AuÃen, USA) Ventura
 County Line (Innen, AuÃen, USA) Santa Cruz und Trestles (Innen, AuÃen, USA)
```

