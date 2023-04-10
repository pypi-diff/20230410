# Comparing `tmp/base16_colorlib-0.1.0.tar.gz` & `tmp/base16_colorlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base16_colorlib-0.1.0.tar", max compression
+gzip compressed data, was "base16_colorlib-0.2.0.tar", max compression
```

## Comparing `base16_colorlib-0.1.0.tar` & `base16_colorlib-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-05 15:32:23.547921 base16_colorlib-0.1.0/LICENSE
--rw-r--r--   0        0        0    27694 2023-04-09 12:37:10.150719 base16_colorlib-0.1.0/README.md
--rw-r--r--   0        0        0       68 2023-04-07 06:22:52.459780 base16_colorlib-0.1.0/base16_colorlib/__init__.py
--rw-r--r--   0        0        0     8995 2023-04-09 12:37:10.151719 base16_colorlib-0.1.0/base16_colorlib/color.py
--rw-r--r--   0        0        0    21633 2023-04-09 12:37:10.151719 base16_colorlib-0.1.0/base16_colorlib/color_scheme.py
--rw-r--r--   0        0        0      414 2023-04-07 04:43:02.556465 base16_colorlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    28131 1970-01-01 00:00:00.000000 base16_colorlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      301 2023-04-10 11:51:31.844928 base16_colorlib-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-04-10 06:06:54.978352 base16_colorlib-0.2.0/LICENSE
+-rw-r--r--   0        0        0    29776 2023-04-10 11:51:31.844928 base16_colorlib-0.2.0/README.md
+-rw-r--r--   0        0        0      752 2023-04-10 11:51:31.844928 base16_colorlib-0.2.0/base16_colorlib/__init__.py
+-rw-r--r--   0        0        0    21633 2023-04-10 11:51:31.844928 base16_colorlib-0.2.0/base16_colorlib/color_scheme.py
+-rw-r--r--   0        0        0     8995 2023-04-10 11:51:31.844928 base16_colorlib-0.2.0/base16_colorlib/utils.py
+-rw-r--r--   0        0        0       68 2023-04-10 11:51:31.844928 base16_colorlib-0.2.0/base16_colorlib/version.py
+-rw-r--r--   0        0        0      589 2023-04-10 11:51:31.845928 base16_colorlib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    30491 1970-01-01 00:00:00.000000 base16_colorlib-0.2.0/PKG-INFO
```

### Comparing `base16_colorlib-0.1.0/LICENSE` & `base16_colorlib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `base16_colorlib-0.1.0/base16_colorlib/color.py` & `base16_colorlib-0.2.0/base16_colorlib/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 # █▀▄▀█ █▀▀ ▀█▀ ▄▀█ ▀
 # █░▀░█ ██▄ ░█░ █▀█ ▄
 # -------------------
 __author__ = "MOIS3Y"
 __credits__ = ["Stepan Zhukovsky"]
 __license__ = "GPL v3.0"
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __maintainer__ = "Stepan Zhukovsky"
 __email__ = "stepan@zhukovsky.me"
 __status__ = "Production"
 
 
 # █▀▀ █▀█ █░░ █▀█ █▀█ ▀
 # █▄▄ █▄█ █▄▄ █▄█ █▀▄ ▄
```

### Comparing `base16_colorlib-0.1.0/base16_colorlib/color_scheme.py` & `base16_colorlib-0.2.0/base16_colorlib/color_scheme.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 # █▀▄▀█ █▀▀ ▀█▀ ▄▀█ ▀
 # █░▀░█ ██▄ ░█░ █▀█ ▄
 # -------------------
 __author__ = "MOIS3Y"
 __credits__ = ["Stepan Zhukovsky"]
 __license__ = "GPL v3.0"
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __maintainer__ = "Stepan Zhukovsky"
 __email__ = "stepan@zhukovsky.me"
 __status__ = "Production"
 
 
 # █▀ █▀▀ █░█ █▀▀ █▀▄▀█ █▀▀ ▀
 # ▄█ █▄▄ █▀█ ██▄ █░▀░█ ██▄ ▄
```

### Comparing `base16_colorlib-0.1.0/PKG-INFO` & `base16_colorlib-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-Metadata-Version: 2.1
-Name: base16-colorlib
-Version: 0.1.0
-Summary: base16 color schemes for your python projects
-Author: MOIS3Y
-Author-email: stepan@zhukovsky.me
-Requires-Python: >=3.8.1,<4.0.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 # BASE16_COLORLIB
 
 ## COLOR SCHEME:
 
-### Package contains several ready-made color schemes in `base16` format:
+Package contains several ready-made color schemes in `base16` format:
 <br/>
 
-![image info](./assets/onedark_example.png)
+![image info](https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/onedark_example.png)
 
 
 <details>
   <summary>Each color scheme is a dictionary with a common structure:</summary>
     <br>
 
   ```python
@@ -51,15 +38,15 @@
 
 <br/>
 
 <details><summary>Available color schemes:</summary>
   <br/>
   <details><summary>aquarium:</summary>
   <br/>
-  <img src="./assets/aquarium_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/aquarium_example.png">
   <br/>
 
   ```
   {
     "scheme": "aquarium",
     "author": "https://github.com/FrenzyExists/aquarium-vim",
     "base00": "#20202A",
@@ -79,15 +66,15 @@
     "base0E": "#f6bbe7",
     "base0F": "#eAc1c1",
   }
   ```
   </details>
   <details><summary>ashes:</summary>
   <br/>
-  <img src="./assets/ashes_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/ashes_example.png">
   <br/>
 
   ```
   {
     "scheme": "ashes",
     "author": "https://github.com/chriskempson/base16-vim",
     "base00": "#1c2023",
@@ -107,15 +94,15 @@
     "base0E": "#c795ae",
     "base0F": "#c79595",
   }
   ```
   </details>
   <details><summary>ayu_dark:</summary>
   <br/>
-  <img src="./assets/ayu_dark_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/ayu_dark_example.png">
   <br/>
 
   ```
   {
     "scheme": "ayu_dark",
     "author": "https://github.com/ayu-theme/ayu-vim",
     "base00": "#0B0E14",
@@ -135,15 +122,15 @@
     "base0E": "#FFB454",
     "base0F": "#CBA6F7",
   }
   ```
   </details>
   <details><summary>ayu_light:</summary>
   <br/>
-  <img src="./assets/ayu_light_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/ayu_light_example.png">
   <br/>
 
   ```
   {
     "scheme": "ayu_light",
     "author": "https://github.com/ayu-theme/ayu-vim",
     "base00": "#fafafa",
@@ -164,15 +151,15 @@
     "base0F": "#F2AE49",
   }
   ```
   </details>
   <br/>
   <details><summary>bearded_arc:</summary>
   <br/>
-  <img src="./assets/bearded_arc_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/bearded_arc_example.png">
   <br/>
 
   ```
   {
     "scheme": "bearded_arc",
     "author": "https://github.com/BeardedBear/bearded-theme",
     "base00": "#1c2433",
@@ -192,15 +179,15 @@
     "base0E": "#22ECDB",
     "base0F": "#FF738A",
   }
   ```
   </details>
   <details><summary>blossom_light:</summary>
   <br/>
-  <img src="./assets/blossom_light_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/blossom_light_example.png">
   <br/>
 
   ```
   {
     "scheme": "blossom_light",
     "author": "https://github.com/blossom-theme",
     "base00": "#e6dfdc",
@@ -221,15 +208,15 @@
     "base0F": "#976153",
   }
   ```
   </details>
   <br/>
   <details><summary>catppuccin_latte:</summary>
   <br/>
-  <img src="./assets/catppuccin_latte_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/catppuccin_latte_example.png">
   <br/>
 
   ```
   {
     "scheme": "catppuccin_latte",
     "author": "https://github.com/catppuccin/catppuccin",
     "base00": "#eff1f5", # base
@@ -249,15 +236,15 @@
     "base0E": "#8839ef", # mauve
     "base0F": "#dd7878", # flamingo
   }
   ```
   </details>
   <details><summary>catppuccin_frappe:</summary>
   <br/>
-  <img src="./assets/catppuccin_frappe_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/catppuccin_frappe_example.png">
   <br/>
 
   ```
   {
     "scheme": "catppuccin_frappe",
     "author": "https://github.com/catppuccin/catppuccin",
     "base00": "#303446", # base
@@ -277,15 +264,15 @@
     "base0E": "#ca9ee6", # mauve
     "base0F": "#eebebe", # flamingo
   }
   ```
   </details>
   <details><summary>catppuccin_macchiato:</summary>
   <br/>
-  <img src="./assets/catppuccin_macchiato_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/catppuccin_macchiato_example.png">
   <br/>
 
   ```
   {
     "scheme": "catppuccin_macchiato",
     "author": "https://github.com/catppuccin/catppuccin",
     "base00": "#24273a", # base
@@ -305,15 +292,15 @@
     "base0E": "#c6a0f6", # mauve
     "base0F": "#f0c6c6", # flamingo
   }
   ```
   </details>
   <details><summary>catppuccin_mocha:</summary>
   <br/>
-  <img src="./assets/catppuccin_mocha_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/catppuccin_mocha_example.png">
   <br/>
 
   ```
   {
     "scheme": "catppuccin_mocha",
     "author": "https://github.com/catppuccin/catppuccin",
     "base00": "#1e1e2e", # base
@@ -334,15 +321,15 @@
     "base0F": "#f2cdcd", # flamingo
   }
   ```
   </details>
   <br/>
   <details><summary>decay:</summary>
   <br/>
-  <img src="./assets/decay_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/decay_example.png">
   <br/>
 
   ```
   {
     "scheme": "decay",
     "author": "https://github.com/decaycs",
     "base00": "#171B20",
@@ -362,15 +349,15 @@
     "base0E": "#c68aee",
     "base0F": "#9cd1ff",
   }
   ```
   </details>
   <details><summary>dracula:</summary>
   <br/>
-  <img src="./assets/dracula_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/dracula_example.png">
   <br/>
 
   ```
   {
     "scheme": "dracula",
     "author": "https://github.com/dracula",
     "base00": "#282936",
@@ -391,15 +378,15 @@
     "base0F": "#00f769",
 }
   ```
   </details>
   <br/>
   <details><summary>everblush:</summary>
   <br/>
-  <img src="./assets/everblush_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/everblush_example.png">
   <br/>
 
   ```
   {
     "scheme": "everblush",
     "author": "https://github.com/Everblush",
     "base00": "#141b1e",
@@ -419,15 +406,15 @@
     "base0E": "#c47fd5",
     "base0F": "#ef7d7d",
   }
   ```
   </details>
   <details><summary>everforest_dark:</summary>
   <br/>
-  <img src="./assets/everforest_dark_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/everforest_dark_example.png">
   <br/>
 
   ```
   {
     "author": "https://github.com/sainnhe/everforest",
     "base00": "#2b3339",
     "base01": "#323c41",
@@ -446,15 +433,15 @@
     "base0E": "#e67e80",
     "base0F": "#d699b6",
   }
   ```
   </details>
   <details><summary>everforest_light:</summary>
   <br/>
-  <img src="./assets/everforest_light_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/everforest_light_example.png">
   <br/>
 
   ```
   {
     "scheme": "everforest_light",
     "author": "https://github.com/sainnhe/everforest",
     "base00": "#fff9e8",
@@ -475,15 +462,15 @@
     "base0F": "#c85552",
   }
   ```
   </details>
   <br/>
   <details><summary>falcon:</summary>
   <br/>
-  <img src="./assets/falcon_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/falcon_example.png">
   <br/>
 
   ```
   {
     "scheme": "falcon",
     "author": "https://github.com/fenetikm/falcon",
     "base00": "#020222",
@@ -504,15 +491,15 @@
     "base0F": "#DFDFE5",
   }
   ```
   </details>
   <br/>
  <details><summary>gruvbox_dark:</summary>
   <br/>
-  <img src="./assets/gruvbox_dark_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/gruvbox_dark_example.png">
   <br/>
 
   ```
   {
     "scheme": "gruvbox_dark",
     "author": "https://github.com/morhetz/gruvbox",
     "base00": "#282828",
@@ -532,15 +519,15 @@
     "base0E": "#d3869b",
     "base0F": "#d65d0e",
   }
   ```
   </details>
   <details><summary>gruvbox_light:</summary>
   <br/>
-  <img src="./assets/gruvbox_light_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/gruvbox_light_example.png">
   <br/>
 
   ```
   {
     "scheme": "gruvbox_light",
     "author": "https://github.com/morhetz/gruvbox",
     "base00": "#F2E5BC",
@@ -561,15 +548,15 @@
     "base0F": "#d65d0e",
   }
   ```
   </details>
   <br/>
   <details><summary>kanagawa:</summary>
   <br/>
-  <img src="./assets/kanagawa_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/kanagawa_example.png">
   <br/>
 
   ```
   {
     "scheme": "kanagawa",
     "author": "https://github.com/rebelot/kanagawa.nvim",
     "base00": "#1f1f28",
@@ -590,15 +577,15 @@
     "base0F": "#d8616b",
   }
   ```
   </details>
   <br/>
   <details><summary>melange:</summary>
   <br/>
-  <img src="./assets/melange_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/melange_example.png">
   <br/>
 
   ```
   {
     "scheme": "melange",
     "author": "https://github.com/savq/melange",
     "base00": "#2A2520",
@@ -618,15 +605,15 @@
     "base0E": "#E49B5D",
     "base0F": "#8E733F",
   }
   ```
   </details>
   <details><summary>monokai:</summary>
   <br/>
-  <img src="./assets/monokai_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/monokai_example.png">
   <br/>
 
   ```
   {
     "scheme": "monokai",
     "author": "https://monokai.pro",
     "base00": "#272822",
@@ -646,15 +633,15 @@
     "base0E": "#f92672",
     "base0F": "#cc6633",
   }
   ```
   </details>
   <details><summary>monochrome:</summary>
   <br/>
-  <img src="./assets/monochrome_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/monochrome_example.png">
   <br/>
 
   ```
   {
     "scheme": "monochrome",
     "author": "https://github.com/kdheepak/monochrome.nvim",
     "base00": "#101010",
@@ -674,15 +661,15 @@
     "base0E": "#DAD4C3",
     "base0F": "#ced4df",
   }
   ```
   </details>
   <details><summary>mountain:</summary>
   <br/>
-  <img src="./assets/mountain_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/mountain_example.png">
   <br/>
 
   ```
   {
     "scheme": "mountain",
     "author": "https://github.com/mountain-theme/Mountain",
     "base00": "#0f0f0f",
@@ -703,15 +690,15 @@
     "base0F": "#b39193",
   }
   ```
   </details>
    <br/>
   <details><summary>nord:</summary>
   <br/>
-  <img src="./assets/nord_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/nord_example.png">
   <br/>
 
   ```
   {
     "scheme": "nord",
     "author": "https://www.nordtheme.com",
     "base00": "#2E3440",
@@ -732,15 +719,15 @@
     "base0F": "#B48EAD",
   }
   ```
   </details>
    <br/>
   <details><summary>onedark:</summary>
   <br/>
-  <img src="./assets/onedark_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/onedark_example.png">
   <br/>
 
   ```
   {
     "scheme": "onedark",
     "author": "https://github.com/one-dark",
     "base00": "#1e222a",
@@ -760,15 +747,15 @@
     "base0E": "#c678dd",
     "base0F": "#be5046",
   }
   ```
   </details>
   <details><summary>onelight:</summary>
   <br/>
-  <img src="./assets/onelight_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/onelight_example.png">
   <br/>
 
   ```
   {
     "scheme": "onelight",
     "author": "https://github.com/one-dark",
     "base00": "#fafafa",
@@ -789,15 +776,15 @@
     "base0F": "#986801",
   }
   ```
   </details>
   <br/>
   <details><summary>rosepine:</summary>
   <br/>
-  <img src="./assets/rosepine_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/rosepine_example.png">
   <br/>
 
   ```
   {
     "scheme": "rosepine",
     "author": "https://github.com/edunfelt/base16-rose-pine-scheme",
     "base00": "#191724",
@@ -817,15 +804,15 @@
     "base0E": "#f6c177",
     "base0F": "#524f67",
   }
   ```
   </details>
   <details><summary>rosepine_moon:</summary>
   <br/>
-  <img src="./assets/rosepine_moon_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/rosepine_moon_example.png">
   <br/>
 
   ```
   {
     "scheme": "rosepine_moon",
     "author": "https://github.com/edunfelt/base16-rose-pine-scheme",
     "base00": "#232136",
@@ -846,15 +833,15 @@
     "base0E": "#f6c177",
     "base0F": "#56526e",
   }
   ```
   </details>
   <details><summary>rosepine_dawn:</summary>
   <br/>
-  <img src="./assets/rosepine_dawn_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/rosepine_dawn_example.png">
   <br/>
 
   ```
   {
     "scheme": "rosepine_dawn",
     "author": "https://github.com/edunfelt/base16-rose-pine-scheme",
     "base00": "#faf4ed",
@@ -874,15 +861,15 @@
     "base0E": "#ea9d34",
     "base0F": "#cecacd",
   }
   ```
   </details>
   <details><summary>rxyhn:</summary>
   <br/>
-  <img src="./assets/rxyhn_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/rxyhn_example.png">
   <br/>
 
   ```
   {
     "scheme": "rxyhn",
     "author": "https://github.com/rxyhn/yoru",
     "base00": "#061115",
@@ -903,15 +890,15 @@
     "base0F": "#F16269",
   }
   ```
   </details>
   <br/>
   <details><summary>solarized:</summary>
   <br/>
-  <img src="./assets/solarized_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/solarized_example.png">
   <br/>
 
   ```
   {
     "scheme": "solarized",
     "author": "https://github.com/altercation/solarized",
     "base00": "#002b36",
@@ -931,15 +918,15 @@
     "base0E": "#6c71c4",
     "base0F": "#d33682",
   }
   ```
   </details>
   <details><summary>sweetpastel:</summary>
   <br/>
-  <img src="./assets/sweetpastel_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/sweetpastel_example.png">
   <br/>
 
   ```
   {
     "scheme": "sweetpastel",
     "author": "https://github.com/SweetPastel",
     "base00": "#1B1F23",
@@ -960,15 +947,15 @@
     "base0F": "#e5a3a1",
   }
   ```
   </details>
   <br/>
   <details><summary>tokyodark:</summary>
   <br/>
-  <img src="./assets/tokyodark_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/tokyodark_example.png">
   <br/>
 
   ```
   {
     "scheme": "tokyodark",
     "author": "https://github.com/tiagovla/tokyodark.nvim",
     "base00": "#11121d",
@@ -988,15 +975,15 @@
     "base0E": "#a485dd",
     "base0F": "#f3627a",
   }
   ```
   </details>
   <details><summary>tokyonight:</summary>
   <br/>
-  <img src="./assets/tokyonight_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/tokyonight_example.png">
   <br/>
 
   ```
   {
     "scheme": "tokyonight",
     "author": "https://github.com/tiagovla/tokyonight.nvim",
     "base00": "#1a1b26",
@@ -1017,15 +1004,15 @@
     "base0F": "#f7768e",
   }
   ```
   </details>
   <br/>
   <details><summary>yoru:</summary>
   <br/>
-  <img src="./assets/yoru_example.png">
+  <img src="https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/yoru_example.png">
   <br/>
 
   ```
   {
     "scheme": "yoru",
     "author": "https://github.com/rxyhn/yoru",
     "base00": "#0c0e0f",
@@ -1084,15 +1071,15 @@
 ## COLOR CLASS:
 
 Package contains class `Color` which can be a container for a color scheme
 and has public methods for changing colors according to the HSL color model:
 
 <br/>
 
-![image info](./assets/hsl_example.png)
+![image info](https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/hsl_example.png)
 
 This class is intended to be stored in an attribute `Color.scheme` color scheme in base16 format.\
 And its subsequent use to set the color for various elements.\
 Since there are only 16 colors in base16,
 sometimes this is not enough to place color accents anywhere.\
 Therefore, the class has several methods for adjusting the color.
 > The HSL color model is used here.
@@ -1189,13 +1176,13 @@
             timezone=None,
             update_interval=1.0,
         ),
         #...
     }
   ````
   Result:\
-  ![image info](./assets/qtile_example.png)
+  ![image info](https://raw.githubusercontent.com/MOIS3Y/base16-colorlib/assets/qtile_example.png)
 
 
 # License:
 
-### GPLv3
+GPLv3
```

