# Comparing `tmp/torch_simple_timing-0.1.4.tar.gz` & `tmp/torch_simple_timing-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_simple_timing-0.1.4.tar", max compression
+gzip compressed data, was "torch_simple_timing-0.1.5.tar", max compression
```

## Comparing `torch_simple_timing-0.1.4.tar` & `torch_simple_timing-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-05 19:37:48.767196 torch_simple_timing-0.1.4/LICENSE
--rw-r--r--   0        0        0     4468 2023-05-01 19:11:11.141712 torch_simple_timing-0.1.4/README.md
--rw-r--r--   0        0        0      686 2023-05-17 13:39:03.727837 torch_simple_timing-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4434 2023-05-17 13:38:17.341399 torch_simple_timing-0.1.4/torch_simple_timing/__init__.py
--rw-r--r--   0        0        0     8857 2023-05-01 19:11:11.142954 torch_simple_timing-0.1.4/torch_simple_timing/clock.py
--rw-r--r--   0        0        0    13141 2023-05-01 18:44:28.717396 torch_simple_timing-0.1.4/torch_simple_timing/timer.py
--rw-r--r--   0        0        0      988 2023-04-12 22:55:21.560200 torch_simple_timing-0.1.4/torch_simple_timing/utils.py
--rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.4/setup.py
--rw-r--r--   0        0        0     4998 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-05 19:37:48.767196 torch_simple_timing-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4468 2023-05-01 19:11:11.141712 torch_simple_timing-0.1.5/README.md
+-rw-r--r--   0        0        0      686 2023-05-17 13:42:05.286475 torch_simple_timing-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4450 2023-05-17 13:41:54.208007 torch_simple_timing-0.1.5/torch_simple_timing/__init__.py
+-rw-r--r--   0        0        0     8857 2023-05-01 19:11:11.142954 torch_simple_timing-0.1.5/torch_simple_timing/clock.py
+-rw-r--r--   0        0        0    13141 2023-05-01 18:44:28.717396 torch_simple_timing-0.1.5/torch_simple_timing/timer.py
+-rw-r--r--   0        0        0      988 2023-04-12 22:55:21.560200 torch_simple_timing-0.1.5/torch_simple_timing/utils.py
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.5/setup.py
+-rw-r--r--   0        0        0     4998 1970-01-01 00:00:00.000000 torch_simple_timing-0.1.5/PKG-INFO
```

### Comparing `torch_simple_timing-0.1.4/LICENSE` & `torch_simple_timing-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.4/README.md` & `torch_simple_timing-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.4/pyproject.toml` & `torch_simple_timing-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-simple-timing"
-version = "0.1.4"
+version = "0.1.5"
 description = "A simple package to time CPU/GPU/Multi-GPU ops"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "torch_simple_timing"}]
 
 [tool.poetry.dependencies]
```

### Comparing `torch_simple_timing-0.1.4/torch_simple_timing/__init__.py` & `torch_simple_timing-0.1.5/torch_simple_timing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         logger.log(timer.stats())
 """
 import importlib.metadata as met
 
 from .clock import Clock  # noqa: F401
 from .timer import Timer
 
-___version__ = met.version("gfn")
+___version__ = met.version("torch_simple_timing")
 """The package version string."""
 
 TIMER = Timer()
 """
 The global :class:`~torch_simple_timing.timer.Timer` instance
 used by :func:`~torch_simple_timing.timeit` to time functions.
 """
```

### Comparing `torch_simple_timing-0.1.4/torch_simple_timing/clock.py` & `torch_simple_timing-0.1.5/torch_simple_timing/clock.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.4/torch_simple_timing/timer.py` & `torch_simple_timing-0.1.5/torch_simple_timing/timer.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.4/torch_simple_timing/utils.py` & `torch_simple_timing-0.1.5/torch_simple_timing/utils.py`

 * *Files identical despite different names*

### Comparing `torch_simple_timing-0.1.4/setup.py` & `torch_simple_timing-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=1.11']
 
 setup_kwargs = {
     'name': 'torch-simple-timing',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'A simple package to time CPU/GPU/Multi-GPU ops',
     'long_description': '<p align="center">\n<strong><a href="https://github.com/vict0rsch/torch_simple_timing" target="_blank">💻&nbsp;&nbsp;Code</a></strong>\n<strong>&nbsp;&nbsp;•&nbsp;&nbsp;</strong>\n<strong><a href="https://torch-simple-timing.readthedocs.io/" target="_blank">Docs&nbsp;&nbsp;📑</a></strong>\n</p>\n\n<p align="center">\n    <a>\n\t    <img src=\'https://img.shields.io/badge/python-3.8%2B-blue\' alt=\'Python\' />\n\t</a>\n\t<a href=\'https://torch-simple-timing.readthedocs.io/en/latest/?badge=latest\'>\n    \t<img src=\'https://readthedocs.org/projects/torch-simple-timing/badge/?version=latest\' alt=\'Documentation Status\' />\n\t</a>\n    <a href="https://github.com/psf/black">\n\t    <img src=\'https://img.shields.io/badge/code%20style-black-black\' />\n\t</a>\n    <a href="https://pytorch.org">\n        <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white"/>\n    </a>\n    <a href="https://pypi.org/project/torch-simple-timing/">\n        <img src="https://badge.fury.io/py/torch_simple_timing.svg" alt="PyPI version" height="20">\n    </a>\n</p>\n<br/>\n\n\n# Torch Simple Timing\n\nA simple yet versatile package to time CPU/GPU/Multi-GPU ops.\n\n1. "*I want to time operations once*"\n   1. That\'s what a `Clock` is for\n2. "*I want to time the same operations multiple times*"\n   1. That\'s what a `Timer` is for\n\nIn simple terms:\n\n* A `Clock` is an object (and context-manager) that will compute the ellapsed time between its `start()` (or `__enter__`) and `stop()` (or `__exit__`)\n* A `Timer` will internally manage clocks so that you can focus on readability and not data structures\n\n## Installation\n\n```\npip install torch_simple_timing\n```\n\n## How to use\n\n### A `Clock`\n\n```python\nfrom torch_simple_parsing import Clock\nimport torch\n\nt = torch.rand(2000, 2000)\ngpu = torch.cuda.is_available()\n\nwith Clock(gpu=gpu) as context_clock:\n    torch.inverse(t @ t.T)\n\nclock = Clock(gpu=gpu).start()\ntorch.inverse(t @ t.T)\nclock.stop()\n\nprint(context_clock.duration) # 0.29688501358032227\nprint(clock.duration)         # 0.292896032333374\n```\n\nMore examples, including bout how to easily share data structures using a `store` can be found in the [documentation](https://torch-simple-timing.readthedocs.io/en/latest/autoapi/torch_simple_timing/clock/index.html).\n\n### A `Timer`\n\n```python\nfrom torch_simple_timing import Timer\nimport torch\n\ndevice = torch.device("cuda" if torch.cuda.is_available() else "cpu")\n\nX = torch.rand(5000, 5000, device=device)\nY = torch.rand(5000, 100, device=device)\nmodel = torch.nn.Linear(5000, 100).to(device)\noptimizer = torch.optim.Adam(model.parameters())\n\ngpu = device.type == "cuda"\ntimer = Timer(gpu=gpu)\n\nfor epoch in range(10):\n    timer.clock("epoch").start()\n    for b in range(50):\n        x = X[b*100: (b+1)*100]\n        y = Y[b*100: (b+1)*100]\n        optimizer.zero_grad()\n        with timer.clock("forward", ignore=epoch>0):\n            p = model(x)\n        loss = torch.nn.functional.cross_entropy(p, y)\n        with timer.clock("backward", ignore=epoch>0):\n            loss.backward()\n        optimizer.step()\n    timer.clock("epoch").stop()\n\nstats = timer.stats()\n# use stats for display and/or logging\n# wandb.summary.update(stats)\nprint(timer.display(stats=stats, precision=5))\n```\n\n```\nepoch    : 0.25064 ± 0.02728 (n=10)\nforward  : 0.00226 ± 0.00526 (n=50)\nbackward : 0.00209 ± 0.00387 (n=50)\n```\n\n### A decorator\n\nYou can also use a decorator to time functions without much overhead in your code:\n\n```python\nfrom torch_simple_timing import timeit, get_global_timer, reset_global_timer\nimport torch\n\n# Use the function name as the timer name\n@timeit(gpu=True)\ndef train():\n    x = torch.rand(1000, 1000, device="cuda" if torch.cuda.is_available() else "cpu")\n    return torch.inverse(x @ x)\n\n# Use a custom name\n@timeit("test")\ndef test_cpu():\n    return torch.inverse(torch.rand(1000, 1000) @ torch.rand(1000, 1000))\n\nif __name__ == "__main__":\n    for _ in range((epochs := 10)):\n        train()\n\n    test_cpu()\n\n    timer = get_global_timer()\n    print(timer.display())\n\n    reset_global_timer()\n```\n\nPrints:\n\n```text\ntrain : 0.045 ± 0.007 (n=10)\ntest  : 0.046         (n= 1)\n```\n\nBy default the `@timeit` decodrator takes at least a `name`, will use `gpu=False` and use the global timer (`torch_simple_timing.TIMER`). You can pass your own timer with `@timeit(name, timer=timer)`.\n\nSee [in the docs]([https://](https://torch-simple-timing.readthedocs.io/en/latest/autoapi/torch_simple_timing/index.html)).\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['torch_simple_timing'] package_data = \ {'': ['*']} install_requires = \
 ['torch>=1.11'] setup_kwargs = { 'name': 'torch-simple-timing', 'version':
-'0.1.4', 'description': 'A simple package to time CPU/GPU/Multi-GPU ops',
+'0.1.5', 'description': 'A simple package to time CPU/GPU/Multi-GPU ops',
 'long_description': '
                       \nð»  Code\n  â¢  \nDocs  ð\n
 \n\n
   \n \n\t [\'Python\']\n\t\n\t\n_\t'_/>\n\t\n \n\t_[\'https://img.shields.io/
    badge/code%20style-black-black\']\n\t\n \n_[https://img.shields.io/badge/
  PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white]\n\n \n_[PyPI_version]\n\n
 \n
```

### Comparing `torch_simple_timing-0.1.4/PKG-INFO` & `torch_simple_timing-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-simple-timing
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple package to time CPU/GPU/Multi-GPU ops
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

