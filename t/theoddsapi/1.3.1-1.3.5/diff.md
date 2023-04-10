# Comparing `tmp/theoddsapi-1.3.1.tar.gz` & `tmp/theoddsapi-1.3.5.tar.gz`

## Comparing `theoddsapi-1.3.1.tar` & `theoddsapi-1.3.5.tar`

### file list

```diff
@@ -1,119 +1,14 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/.travis.yml
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/Makefile
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/api_key.env
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/requirements.txt
--rw-r--r--   0        0        0    60658 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/docs/index.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/pyvenv.cfg
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/requirements.txt
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/Activate.ps1
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/activate
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/activate.csh
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/activate.fish
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/autopep8
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/cygdb
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/cython
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/cythonize
--rwxr-xr-x   0        0        0    10170 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/dl
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/docutils
--rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/dotenv
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/epylint
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/f2py
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/f2py3
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/f2py3.10
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/flake8
--rwxr-xr-x   0        0        0     1719 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/get_objgraph
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/ipython
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/ipython3
--rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/isort
--rwxr-xr-x   0        0        0      311 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/isort-identify-imports
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/isympy
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/jupyter
--rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/jupyter-kernel
--rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/jupyter-kernelspec
--rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/jupyter-migrate
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/jupyter-run
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/jupyter-troubleshoot
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/keyring
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/markdown-it
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/normalizer
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pip
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pip3
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pip3.10
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pipreqs
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pkginfo
--rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pox
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/py.test
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pybabel
--rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pycodestyle
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pydocstyle
--rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pyflakes
--rwxr-xr-x   0        0        0      280 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pygmentize
--rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pylama
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pylint
--rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pylint-config
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pyproject-build
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pyreverse
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/python3 -> /Library/Frameworks/Python.framework/Versions/3.10/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/python3.10 -> python3
--rwxr-xr-x   0        0        0      657 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2html.py
--rwxr-xr-x   0        0        0      779 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1124 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2html5.py
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2latex.py
--rwxr-xr-x   0        0        0      679 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2man.py
--rwxr-xr-x   0        0        0      845 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2odt.py
--rwxr-xr-x   0        0        0     1783 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      700 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2s5.py
--rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rst2xml.py
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/sphinx-apidoc
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/sphinx-autogen
--rwxr-xr-x   0        0        0      280 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/sphinx-build
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/sphinx-quickstart
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/symilar
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/twine
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/undill
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/bin/wheel
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/etc/jupyter/nbconfig/notebook.d/widgetsnbextension.json
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/kernels/python3/kernel.json
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/kernels/python3/logo-32x32.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/kernels/python3/logo-64x64.png
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/kernels/python3/logo-svg.svg
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/install.json
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/package.json
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/schemas/@jupyter-widgets/jupyterlab-manager/package.json.orig
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/schemas/@jupyter-widgets/jupyterlab-manager/plugin.json
--rw-r--r--   0        0        0   154302 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/113.dd66397047ecb9a605cf.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/113.dd66397047ecb9a605cf.js.LICENSE.txt
--rw-r--r--   0        0        0    85597 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/134.40eaa5b8e976096d50b2.js
--rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/150.b0e841b75317744a7595.js
--rw-r--r--   0        0        0    90076 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/291.f707f721e4b3a5489ee0.js
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/291.f707f721e4b3a5489ee0.js.LICENSE.txt
--rw-r--r--   0        0        0    38441 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/345.03be96cd091aac4797a5.js
--rw-r--r--   0        0        0   111264 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/495.5805e8bf9dd8851289a1.js
--rw-r--r--   0        0        0    23918 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/595.e3c9c115ecf5763f080b.js
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/596.5d35bd634ac768ff6d16.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/61.21f571face17e35076c2.js
--rw-r--r--   0        0        0    57036 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/644.11f638668109f1562dd1.js
--rw-r--r--   0        0        0    32641 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/699.563670613eea7b633a22.js
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/965.7ea93aa594250a988d2a.js
--rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/remoteEntry.d6df56cd69f4640706bc.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/style.js
--rw-r--r--   0        0        0    36297 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/labextensions/@jupyter-widgets/jupyterlab-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0   967056 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/nbextensions/jupyter-js-widgets/extension.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/nbextensions/jupyter-js-widgets/extension.js.LICENSE.txt
--rw-r--r--   0        0        0  3466519 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/jupyter/nbextensions/jupyter-js-widgets/extension.js.map
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/man/man1/ipython.1
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/oddsapienv/share/man/man1/isympy.1
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/src/theoddsapi/__init__.py
--rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/src/theoddsapi/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0    11000 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/tests/test.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/LICENSE
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/README.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 theoddsapi-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/.travis.yml
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/Makefile
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/api_key.env
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/requirements.txt
+-rw-r--r--   0        0        0    26200 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/docs/index.html
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/src/theoddsapi/__init__.py
+-rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/src/theoddsapi/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/tests/__init__.py
+-rw-r--r--   0        0        0    11000 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/tests/test.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/LICENSE
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/README.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 theoddsapi-1.3.5/PKG-INFO
```

### Comparing `theoddsapi-1.3.1/Makefile` & `theoddsapi-1.3.5/Makefile`

 * *Files identical despite different names*

### Comparing `theoddsapi-1.3.1/src/theoddsapi/api.py` & `theoddsapi-1.3.5/src/theoddsapi/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import requests
 import pandas as pd
+from bs4 import BeautifulSoup
 
 
 class TheOddsAPI(object):
     """
     This module provides functions to get historical snapshots of sports odds 
     data back to 2020 as well as game scores and results for past and live games.
     """
 
     HOST = "https://api.the-odds-api.com"
+    # List of bookmaker regions to scrape from the-odds-api.com
+    # NOTE: Index of bookmaker regions reflects the index of the table on the website to scrape
+    BOOKMAKER_REGIONS = ['all', 'us', 'uk', 'eu', 'au']
 
     def _get(self, host, endpoint, params):
         """Helper function for GET requests to The Odds API server
 
         Parameters
         ----------
         host : str
@@ -26,17 +30,17 @@
             endpoints. See https://app.swaggerhub.com/apis-docs/the-odds-api/odds-api/4
             for a comprehensive list.
         Returns
         -------
         dict or None
             Returns response from server if successful; otherwise, returns None
         """
-        print(host+endpoint)
+
         params['apiKey'] = self.api_key
-        print(params)
+
         response = requests.get(host + endpoint, params=params)
 
         if response.status_code != 200:
             print(
                 f'Failed to get {endpoint}: status_code {response.status_code}, response body {response.text}')
             return None
         else:
@@ -228,16 +232,16 @@
         del params['eventId']
         # Create the endpoint from the kwargs
         endpoint = f'/v4/sports/{sport}/events/{event_id}/odds/'
         event_odds_response = self._get(
             TheOddsAPI.HOST, endpoint, params)
         return event_odds_response
 
-    @classmethod
-    def get_featured_betting_markets(cls):
+    @staticmethod
+    def get_featured_betting_markets():
         """Get the most common markets that are featured by bookmakers.
         Terminology for betting markets can vary by country, sport and even
         amongst bookmakers.
 
         Returns
         -------
         pd.DataFrame
@@ -256,16 +260,16 @@
                 'Bet on a final outcome of a tournament or competition',
                 'Bet against a h2h outcome. This market is only applicable to betting exchanges',
                 'Bet against an outrights outcome. This market is only applicable to betting exchanges'
             ]
         }
         return pd.DataFrame(featured_betting_markets_dict)
 
-    @classmethod
-    def get_additional_markets(cls):
+    @staticmethod
+    def get_additional_markets():
         """Get information on additional markets limited to US sports and selected
         bookmakers. Additional markets update at 5 minute intervals.
         Additional markets need to be accessed one event at a time using the
         /event/{eventId}/odds endpoint.
 
         Returns
         -------
@@ -283,16 +287,16 @@
                 'Odds that both teams will score during the game. Outcomes are "Yes" or "No". Available for soccer.',
                 'Odds for the match winner, excluding the draw outcome. A draw will result in a returned bet. Available for soccer',
                 'Match winner including draw'
             ]
         }
         return pd.DataFrame(additional_markets_dict)
 
-    @classmethod
-    def get_player_props(cls, sport: str):
+    @staticmethod
+    def get_player_props(sport: str):
         """Get information on player props limited to US sports and selected US
         bookmakers, starting with FanDuel, DraftKings, Caesars, Bovada and more.
         Player props update at 5 minute intervals. Player props need to be accessed
         one event at a time using the /event/{eventId}/odds endpoint.
 
         Parameters
         ----------
@@ -355,7 +359,82 @@
                 'market_name': market_name_arr
             }
         elif sport == 'NHL':
             market_key_arr = [
                 'player_points'
             ]
         return pd.DataFrame(player_props_dict)
+    import requests
+
+    @staticmethod
+    def _get_bookmakers_helper(region_index: int):
+        """Helper function to get a list of bookmakers and their keys from the-odds-api.com website for a given region by index.
+
+        Parameters
+        ----------
+        region_index : int
+            Index of the region which reflects the ordering of regions on the website
+
+        Returns
+        -------
+        bookmakers : list[dict]
+            list of bookmakers and their keys for the a region
+        """
+        url = "https://the-odds-api.com/sports-odds-data/bookmaker-apis.html"
+        response = requests.get(url)
+        soup = BeautifulSoup(response.content, 'html.parser')
+        bookmakers = []
+
+        # Find the list of bookmakers
+        bookmakers_section = soup.find_all('table')
+        region_table = bookmakers_section[region_index]
+        rows = region_table.find_all('tr')
+
+        for row in rows:
+            tds = row.find_all('td')
+            d = dict()
+            for i, td in enumerate(tds):
+                if td.text.strip() != '':
+                    if i == 0:
+                        d['region'] = td.text.strip()
+                    elif i == 1:
+                        d['key'] = td.text.strip()
+                    elif i == 2:
+                        # Bookmaker name is the first element of the split list
+                        d['title'] = td.text.strip().split('\n')[0]
+            # Append the dictionary to the list of bookmakers if it is not empty
+            if d != {}:
+                bookmakers.append(d)
+        return bookmakers
+
+    @classmethod
+    def get_bookmakers(cls, region: str = 'all'):
+        """Get a list of bookmakers and their keys from the-odds-api.com website for a given region (or all regions if no region is specified).
+
+        Parameters
+        ----------
+        region : str, optional
+            region to get all bookmakers for, by default 'all', options are 'all', 'us', 'uk', 'au', 'eu'
+
+        Returns
+        -------
+        bookmakers_all : list[dict]
+            list of bookmakers and their keys for the given region
+        """
+
+        if region == 'all':
+            for i in range(len(TheOddsAPI.BOOKMAKER_REGIONS)-1):
+                bookmakers = TheOddsAPI._get_bookmakers_helper(i)
+                if i == 0:
+                    bookmakers_all = bookmakers
+                else:
+                    bookmakers_all.extend(bookmakers)
+        else:
+            if region not in TheOddsAPI.BOOKMAKER_REGIONS:
+                raise ValueError(
+                    f'Invalid region: {region}. Valid regions are: {TheOddsAPI.BOOKMAKER_REGIONS}')
+            else:
+                bookmaker_index = TheOddsAPI.BOOKMAKER_REGIONS.index(
+                    region) - 1
+                bookmakers_all = TheOddsAPI._get_bookmakers_helper(
+                    bookmaker_index)
+        return bookmakers_all
```

### Comparing `theoddsapi-1.3.1/tests/test.py` & `theoddsapi-1.3.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `theoddsapi-1.3.1/.gitignore` & `theoddsapi-1.3.5/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
+oddsapienv
 .env
 tests/.env
 .venv
 env/
 venv/
 ENV/
 env.bak/
```

### Comparing `theoddsapi-1.3.1/LICENSE` & `theoddsapi-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `theoddsapi-1.3.1/README.md` & `theoddsapi-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `theoddsapi-1.3.1/pyproject.toml` & `theoddsapi-1.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "theoddsapi"
-version = "1.3.1"
+version = "1.3.5"
 authors = [
   { name="MidpriceDog"},
 ]
 description = "A Python wrapper around The Odds-Api V4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `theoddsapi-1.3.1/PKG-INFO` & `theoddsapi-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theoddsapi
-Version: 1.3.1
+Version: 1.3.5
 Summary: A Python wrapper around The Odds-Api V4
 Project-URL: Homepage, https://github.com/MidpriceDog/the-odds-api-client
 Project-URL: Bug Tracker, https://github.com/MidpriceDog/the-odds-api-client/issues
 Author: MidpriceDog
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

