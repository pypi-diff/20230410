# Comparing `tmp/spacer_tutorial-0.0.2.tar.gz` & `tmp/spacer_tutorial-0.0.3.tar.gz`

## Comparing `spacer_tutorial-0.0.2.tar` & `spacer_tutorial-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0   190977 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/Dagstuhl2019.ipynb
--rw-r--r--   0        0        0   138361 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/ECE750T29_Fall2019.ipynb
--rw-r--r--   0        0        0   168100 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/FSU_2023.ipynb
--rw-r--r--   0        0        0    98022 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/Synasc2019.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/requirements.txt
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/token-test.ag
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/__init__.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/bakery.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/cfa.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/chc.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/dcfa.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/fml.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/proof.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/solve.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/ts.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/src/spacer_tutorial/vcgen.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/LICENSE
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/.z3-trace
+-rw-r--r--   0        0        0   190977 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/Dagstuhl2019.ipynb
+-rw-r--r--   0        0        0   138361 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/ECE750T29_Fall2019.ipynb
+-rw-r--r--   0        0        0   186200 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/FSU_2023.ipynb
+-rw-r--r--   0        0        0    98022 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/Synasc2019.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/token-test.ag
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/__init__.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/bakery.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/cfa.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/chc.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/dcfa.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/fml.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/proof.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/solve.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/ts.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/vcgen.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/src/spacer_tutorial/xnet.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/LICENSE
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 spacer_tutorial-0.0.3/PKG-INFO
```

### Comparing `spacer_tutorial-0.0.2/Dagstuhl2019.ipynb` & `spacer_tutorial-0.0.3/Dagstuhl2019.ipynb`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/ECE750T29_Fall2019.ipynb` & `spacer_tutorial-0.0.3/ECE750T29_Fall2019.ipynb`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/FSU_2023.ipynb` & `spacer_tutorial-0.0.3/FSU_2023.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9943436013674197%*

 * *Differences: {"'cells'": "{1: {'execution_count': 10}, 2: {'execution_count': 11}, 4: {'execution_count': 12}, "*

 * *            "5: {'execution_count': 13}, 6: {'execution_count': 14, 'outputs': {0: "*

 * *            "{'execution_count': 14}}}, 10: {'source': ['## Analyzing XNET with Interpolants\\n', "*

 * *            "'\\n', 'An interesting question for the above network is how it behaves for given "*

 * *            'restrictions on input and/or output. We can answer this question using '*

 * *            "interpolants!']}, 11: {'executi […]*

```diff
@@ -8,15 +8,15 @@
                 "# Spacer on Jupyter\n",
                 "\n",
                 "This is an interactive document. You can follow along on the cloud, change, play, go deeper into the code.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 10,
             "metadata": {
                 "trusted": true
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -41,15 +41,15 @@
                 "# install spacer_tutorial if needed\n",
                 "if importlib.util.find_spec('spacer_tutorial') is None:\n",
                 "    !{sys.executable} -m pip install spacer-tutorial"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 11,
             "metadata": {
                 "code_folding": [
                     3,
                     16,
                     22,
                     31
                 ],
@@ -90,15 +90,15 @@
                 "  2. $\\forall b, c \\cdot Itp(c) \\wedge B(b, c) \\implies False$\n",
                 " \n",
                 "where uninterpreted constants $c$ are shared between $A$ and $B$, and uninterpreted constants $a$ and $b$ are  local to $A$ and $B$, respectively."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 12,
             "metadata": {
                 "trusted": true
             },
             "outputs": [],
             "source": [
                 "# Binary Craig Interpolation by reduction to CHC\n",
                 "def interpolate(A, B, verbosity=0):\n",
@@ -117,41 +117,41 @@
                 "    if res == z3.sat:\n",
                 "        return answer.eval(Itp(shared))\n",
                 "    return None "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 13,
             "metadata": {
                 "trusted": true
             },
             "outputs": [],
             "source": [
                 "a, b, x, y, z = z3.Ints('a b x y z')\n",
                 "itp = interpolate(z3.And(a < x, x < b), b < a)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 14,
             "metadata": {
                 "trusted": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "&not;(b + -1&middot;a &le; 1)"
                         ],
                         "text/plain": [
                             "&not;(b + -1&middot;a &le; 1)"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "itp"
             ]
@@ -172,100 +172,336 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Analyzing Neural Networks with Interpolation"
+                "# Analyzing Neural Networks with Interpolation\n",
+                "Contributed by Nham Le\n",
+                "\n",
+                "## XNET: approximating analog XOR function using Neural net\n",
+                "### Why XOR?\n",
+                "Before ChatGPT, Stable Diffusion, and AlphaGo, approximating XOR function was the holy grail of Machine Learning. In their book [Perceptron][1], the famous pioneers in AI Marvin Minsky and Seymour Papert claimed that the simple XOR cannot be resolved by two-layer of feedforward neural networks. This \"drove research away from neural networks in the 1970s, and contributed to the so-called AI winter\".\n",
+                "\n",
+                "[1]: https://en.wikipedia.org/wiki/Perceptrons_(book)\n",
+                "\n",
+                "Of course, nowaday this is considered a toy problem. If you are curious, what makes the whole thing possible was the introduction of non-linear activation functions, such as ReLU.\n",
+                "\n",
+                "#### XOR function: \n",
+                "```\n",
+                "XOR(True, True) = XOR(False, False) = False \n",
+                "XOR(True, False) = XOR(False, True) = True\n",
+                "```\n",
+                "#### Analog XOR function that is approximated by XNET:\n",
+                "A real-valued input signal $x$ is considered True if $0.7\\leq x \\leq 1$, and False if $0\\leq x \\leq 0.3$.\n",
+                "```\n",
+                "AXOR(True, True) = AXOR(False, False) = 0 \n",
+                "AXOR(True, False) = AXOR(False, True) = 1\n",
+                "```\n",
+                "\n",
+                "### XNET\n",
+                "XNET is a two-layer feed forward neural network that approximates the Analog XOR function. The network takes in 2 inputs: $x_0$ and $x_1$, and produces two outputs: $y_0$ and  $y_1$. We say that $\\mathit{XNET}(x_0, x_1) = 0$ if $y_0>y_1$, and $XNET(x_0, x_1) = 1$ if $y_0<y_1$\n",
+                "\n",
+                "Here is a learned version of XNET"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 15,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "image/svg+xml": [
+                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
+                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
+                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
+                            "<!-- Generated by graphviz version 7.1.0 (20230121.1956)\n",
+                            " -->\n",
+                            "<!-- Title: G Pages: 1 -->\n",
+                            "<svg width=\"245pt\" height=\"305pt\"\n",
+                            " viewBox=\"0.00 0.00 244.83 305.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
+                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 301)\">\n",
+                            "<title>G</title>\n",
+                            "<polygon fill=\"white\" stroke=\"none\" points=\"-4,4 -4,-301 240.83,-301 240.83,4 -4,4\"/>\n",
+                            "<!-- x0 -->\n",
+                            "<g id=\"node1\" class=\"node\">\n",
+                            "<title>x0</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"41.83\" cy=\"-279\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"41.83\" y=\"-275.3\" font-family=\"Times,serif\" font-size=\"14.00\">x0</text>\n",
+                            "</g>\n",
+                            "<!-- v0 -->\n",
+                            "<g id=\"node2\" class=\"node\">\n",
+                            "<title>v0</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"34.83\" cy=\"-192\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"34.83\" y=\"-188.3\" font-family=\"Times,serif\" font-size=\"14.00\">v0</text>\n",
+                            "</g>\n",
+                            "<!-- x0&#45;&gt;v0 -->\n",
+                            "<g id=\"edge1\" class=\"edge\">\n",
+                            "<title>x0&#45;&gt;v0</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M22.15,-266.17C14.29,-260.29 6.1,-252.41 1.83,-243 -2.75,-232.91 2.19,-222.57 9.52,-213.92\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"11.82,-216.58 16.33,-206.99 6.82,-211.67 11.82,-216.58\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"10.83\" y=\"-231.8\" font-family=\"Times,serif\" font-size=\"14.00\">0.1</text>\n",
+                            "</g>\n",
+                            "<!-- v1 -->\n",
+                            "<g id=\"node3\" class=\"node\">\n",
+                            "<title>v1</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"120.83\" cy=\"-192\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"120.83\" y=\"-188.3\" font-family=\"Times,serif\" font-size=\"14.00\">v1</text>\n",
+                            "</g>\n",
+                            "<!-- x0&#45;&gt;v1 -->\n",
+                            "<g id=\"edge2\" class=\"edge\">\n",
+                            "<title>x0&#45;&gt;v1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M37.85,-260.9C36.43,-250.55 36.5,-237.56 42.83,-228 48.11,-220.02 67.86,-211.2 86.17,-204.41\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"87.27,-207.73 95.52,-201.07 84.93,-201.13 87.27,-207.73\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"53.83\" y=\"-231.8\" font-family=\"Times,serif\" font-size=\"14.00\">&#45;4.3</text>\n",
+                            "</g>\n",
+                            "<!-- v2 -->\n",
+                            "<g id=\"node4\" class=\"node\">\n",
+                            "<title>v2</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"202.83\" cy=\"-192\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"202.83\" y=\"-188.3\" font-family=\"Times,serif\" font-size=\"14.00\">v2</text>\n",
+                            "</g>\n",
+                            "<!-- x0&#45;&gt;v2 -->\n",
+                            "<g id=\"edge3\" class=\"edge\">\n",
+                            "<title>x0&#45;&gt;v2</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M63.86,-268C77.47,-261.49 95.09,-252.48 109.83,-243 118.87,-237.18 119.68,-233.67 128.83,-228 141.66,-220.04 156.59,-212.66 169.66,-206.75\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"170.99,-209.99 178.73,-202.76 168.17,-203.58 170.99,-209.99\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"137.83\" y=\"-231.8\" font-family=\"Times,serif\" font-size=\"14.00\">4.2</text>\n",
+                            "</g>\n",
+                            "<!-- v3 -->\n",
+                            "<g id=\"node6\" class=\"node\">\n",
+                            "<title>v3</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"34.83\" cy=\"-105\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"34.83\" y=\"-101.3\" font-family=\"Times,serif\" font-size=\"14.00\">v3</text>\n",
+                            "</g>\n",
+                            "<!-- v0&#45;&gt;v3 -->\n",
+                            "<g id=\"edge7\" class=\"edge\">\n",
+                            "<title>v0&#45;&gt;v3</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M34.83,-173.8C34.83,-162.58 34.83,-147.67 34.83,-134.69\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"38.33,-134.98 34.83,-124.98 31.33,-134.98 38.33,-134.98\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"51.83\" y=\"-144.8\" font-family=\"Times,serif\" font-size=\"14.00\">ReLU</text>\n",
+                            "</g>\n",
+                            "<!-- v4 -->\n",
+                            "<g id=\"node7\" class=\"node\">\n",
+                            "<title>v4</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"120.83\" cy=\"-105\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"120.83\" y=\"-101.3\" font-family=\"Times,serif\" font-size=\"14.00\">v4</text>\n",
+                            "</g>\n",
+                            "<!-- v1&#45;&gt;v4 -->\n",
+                            "<g id=\"edge8\" class=\"edge\">\n",
+                            "<title>v1&#45;&gt;v4</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M120.83,-173.8C120.83,-162.58 120.83,-147.67 120.83,-134.69\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"124.33,-134.98 120.83,-124.98 117.33,-134.98 124.33,-134.98\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"137.83\" y=\"-144.8\" font-family=\"Times,serif\" font-size=\"14.00\">ReLU</text>\n",
+                            "</g>\n",
+                            "<!-- v5 -->\n",
+                            "<g id=\"node8\" class=\"node\">\n",
+                            "<title>v5</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"202.83\" cy=\"-105\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"202.83\" y=\"-101.3\" font-family=\"Times,serif\" font-size=\"14.00\">v5</text>\n",
+                            "</g>\n",
+                            "<!-- v2&#45;&gt;v5 -->\n",
+                            "<g id=\"edge9\" class=\"edge\">\n",
+                            "<title>v2&#45;&gt;v5</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M202.83,-173.8C202.83,-162.58 202.83,-147.67 202.83,-134.69\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"206.33,-134.98 202.83,-124.98 199.33,-134.98 206.33,-134.98\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"219.83\" y=\"-144.8\" font-family=\"Times,serif\" font-size=\"14.00\">ReLU</text>\n",
+                            "</g>\n",
+                            "<!-- x1 -->\n",
+                            "<g id=\"node5\" class=\"node\">\n",
+                            "<title>x1</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"172.83\" cy=\"-279\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"172.83\" y=\"-275.3\" font-family=\"Times,serif\" font-size=\"14.00\">x1</text>\n",
+                            "</g>\n",
+                            "<!-- x1&#45;&gt;v0 -->\n",
+                            "<g id=\"edge4\" class=\"edge\">\n",
+                            "<title>x1&#45;&gt;v0</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M148.6,-270.67C130.93,-264.72 106.86,-255.29 87.83,-243 76.27,-235.54 64.97,-225.4 55.8,-216.2\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"58.52,-213.98 49.07,-209.21 53.48,-218.84 58.52,-213.98\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"98.83\" y=\"-231.8\" font-family=\"Times,serif\" font-size=\"14.00\">&#45;0.6</text>\n",
+                            "</g>\n",
+                            "<!-- x1&#45;&gt;v1 -->\n",
+                            "<g id=\"edge5\" class=\"edge\">\n",
+                            "<title>x1&#45;&gt;v1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M166.85,-261.17C162.96,-251.17 157.39,-238.44 150.83,-228 148.28,-223.96 145.3,-219.9 142.22,-216.06\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"145.12,-214.08 135.98,-208.72 139.79,-218.61 145.12,-214.08\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"166.83\" y=\"-231.8\" font-family=\"Times,serif\" font-size=\"14.00\">4.4</text>\n",
+                            "</g>\n",
+                            "<!-- x1&#45;&gt;v2 -->\n",
+                            "<g id=\"edge6\" class=\"edge\">\n",
+                            "<title>x1&#45;&gt;v2</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M182.7,-262.07C185.98,-256.24 189.41,-249.48 191.83,-243 194.4,-236.09 196.47,-228.4 198.08,-221.17\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"201.48,-221.98 200.01,-211.49 194.62,-220.61 201.48,-221.98\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"206.83\" y=\"-231.8\" font-family=\"Times,serif\" font-size=\"14.00\">&#45;4.2</text>\n",
+                            "</g>\n",
+                            "<!-- y0 -->\n",
+                            "<g id=\"node9\" class=\"node\">\n",
+                            "<title>y0</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"56.83\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"56.83\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">y0</text>\n",
+                            "</g>\n",
+                            "<!-- v3&#45;&gt;y0 -->\n",
+                            "<g id=\"edge10\" class=\"edge\">\n",
+                            "<title>v3&#45;&gt;y0</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M22.98,-88.43C16.89,-78.43 11.72,-65.26 16.83,-54 19.49,-48.12 23.69,-42.84 28.39,-38.27\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"30.63,-40.95 35.99,-31.81 26.11,-35.61 30.63,-40.95\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"25.83\" y=\"-57.8\" font-family=\"Times,serif\" font-size=\"14.00\">0.4</text>\n",
+                            "</g>\n",
+                            "<!-- y1 -->\n",
+                            "<g id=\"node10\" class=\"node\">\n",
+                            "<title>y1</title>\n",
+                            "<ellipse fill=\"none\" stroke=\"black\" cx=\"146.83\" cy=\"-18\" rx=\"27\" ry=\"18\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"146.83\" y=\"-14.3\" font-family=\"Times,serif\" font-size=\"14.00\">y1</text>\n",
+                            "</g>\n",
+                            "<!-- v3&#45;&gt;y1 -->\n",
+                            "<g id=\"edge11\" class=\"edge\">\n",
+                            "<title>v3&#45;&gt;y1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M51.84,-91.09C70.09,-77.24 99.32,-55.05 120.54,-38.95\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"122.6,-41.78 128.45,-32.95 118.37,-36.2 122.6,-41.78\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"107.83\" y=\"-57.8\" font-family=\"Times,serif\" font-size=\"14.00\">&#45;0.4</text>\n",
+                            "</g>\n",
+                            "<!-- v4&#45;&gt;y0 -->\n",
+                            "<g id=\"edge12\" class=\"edge\">\n",
+                            "<title>v4&#45;&gt;y0</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M96.16,-97.04C82.33,-91.74 66.21,-82.94 57.83,-69 53.95,-62.56 52.58,-54.75 52.47,-47.24\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"55.95,-47.62 53.05,-37.43 48.96,-47.2 55.95,-47.62\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"68.83\" y=\"-57.8\" font-family=\"Times,serif\" font-size=\"14.00\">&#45;4.9</text>\n",
+                            "</g>\n",
+                            "<!-- v4&#45;&gt;y1 -->\n",
+                            "<g id=\"edge13\" class=\"edge\">\n",
+                            "<title>v4&#45;&gt;y1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M125.96,-87.21C129.46,-75.76 134.19,-60.32 138.25,-47.02\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"141.59,-48.08 141.17,-37.5 134.9,-46.04 141.59,-48.08\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"143.83\" y=\"-57.8\" font-family=\"Times,serif\" font-size=\"14.00\">3.9</text>\n",
+                            "</g>\n",
+                            "<!-- v5&#45;&gt;y0 -->\n",
+                            "<g id=\"edge14\" class=\"edge\">\n",
+                            "<title>v5&#45;&gt;y0</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M191.91,-88.56C183.44,-77.58 170.82,-63.21 156.83,-54 151.11,-50.24 118.27,-39.03 91.76,-30.3\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"92.92,-27 82.33,-27.21 90.74,-33.65 92.92,-27\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"182.83\" y=\"-57.8\" font-family=\"Times,serif\" font-size=\"14.00\">3.9</text>\n",
+                            "</g>\n",
+                            "<!-- v5&#45;&gt;y1 -->\n",
+                            "<g id=\"edge15\" class=\"edge\">\n",
+                            "<title>v5&#45;&gt;y1</title>\n",
+                            "<path fill=\"none\" stroke=\"black\" d=\"M208.76,-87.19C211.31,-76.95 212.55,-63.97 206.83,-54 201.12,-44.07 191.39,-36.68 181.4,-31.33\"/>\n",
+                            "<polygon fill=\"black\" stroke=\"black\" points=\"182.97,-28.2 172.43,-27.11 179.98,-34.53 182.97,-28.2\"/>\n",
+                            "<text text-anchor=\"middle\" x=\"218.83\" y=\"-57.8\" font-family=\"Times,serif\" font-size=\"14.00\">4.6</text>\n",
+                            "</g>\n",
+                            "</g>\n",
+                            "</svg>\n"
+                        ],
+                        "text/plain": [
+                            "<graphviz.sources.Source at 0x10d5bffa0>"
+                        ]
+                    },
+                    "execution_count": 15,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "xnet_graph()"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Analyzing XNET with Interpolants\n",
+                "\n",
+                "An interesting question for the above network is how it behaves for given restrictions on input and/or output. We can answer this question using interpolants!"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def mkReLU(n):\n",
+                "    \"\"\"Create ReLU constraint using ITE logical construct\"\"\"\n",
                 "    return z3.If(n > 0, n, 0)\n",
                 "\n",
                 "# inputs\n",
                 "x0, x1 = z3.Reals(\"x0 x1\")\n",
                 "# outputs\n",
                 "y0, y1 = z3.Reals(\"y0 y1\")\n",
                 "# hidden \n",
                 "v0, v1, v2, v3, v4, v5 = z3.Reals('v0 v1 v2 v3 v4 v5')\n",
                 "\n",
                 "init = z3.And(0<x0, x0<0.3, \n",
                 "              0<x1, x1<0.3)\n",
-                "layer1 = z3.And(v0 ==  0.1*x0 - 0.6*x1,\n",
-                "                v1 == -4.3*x0 + 4.4*x1,\n",
-                "                v2 ==  4.2*x0-  4.2*x1) \n",
+                "layer1 = z3.And(v0 ==  0.1*x0 -  0.6*x1,\n",
+                "                v1 == -4.3*x0 +  4.4*x1,\n",
+                "                v2 ==  4.2*x0 -  4.2*x1) \n",
                 "relu_layer = z3.And(v3 == mkReLU(v0), \n",
                 "                    v4 == mkReLU(v1), \n",
                 "                    v5 == mkReLU(v2)) \n",
                 "layer2 = z3.And(y0 ==  0.4*v3 - 4.9*v4 + 3.9*v5 + 6.7,\n",
                 "                y1 == -0.4*v3 + 3.9*v4 + 4.6*v5 - 7.4)\n",
                 "network = z3.And(layer1, relu_layer, layer2)\n",
                 "A = z3.And(init, network)\n",
                 "# claim that in the given init region, the output is always y0 >= y1\n",
                 "B = z3.Not(y0 >= y1)\n",
                 "itp = interpolate(A, B)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "&not;(25/968&middot;y0 + -25/968&middot;y1 &le; 621/9680)"
+                            "&not;(25/946&middot;y1 + -25/946&middot;y0 &ge; -621/9460)"
                         ],
                         "text/plain": [
-                            "&not;(25/968&middot;y0 + -25/968&middot;y1 &le; 621/9680)"
+                            "&not;(25/946&middot;y1 + -25/946&middot;y0 &ge; -621/9460)"
                         ]
                     },
-                    "execution_count": 26,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "itp"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "First of all, note that there is an interpolant. This means, that our property is correct. In the given input region, $y0 \\geq y1$. The interpolant tells us a little more about the output"
+                "First of all, note that there is an interpolant. This means, that our property is correct. In the given input region, $x_0,x_1 \\in (0.0,0.3)$, the output satsifies $y_0 \\geq y_1$. The interpolant tells us a little more about the output. Simplifying, we get:\n",
+                "  * $\\frac{2}{2}$\n",
+                "\n",
+                "It is also possible to interpolate `init` to see what are the restrictions needed on the input to maintain the property."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "&not;(43/44&middot;x0 + -1&middot;x1 &le; -3/10) &and;\n",
-                            "&not;(x0 &le; 0) &and;\n",
-                            "&not;(143/123&middot;x0 + -1&middot;x1 &ge; 143/410)"
+                            "&not;(x1 + -143/123&middot;x0 &le; -143/410) &and; &not;(x1 + -43/44&middot;x0 &ge; 3/10)"
                         ],
                         "text/plain": [
-                            "&not;(43/44&middot;x0 + -1&middot;x1 &le; -3/10) &and;\n",
-                            "&not;(x0 &le; 0) &and;\n",
-                            "&not;(143/123&middot;x0 + -1&middot;x1 &ge; 143/410)"
+                            "&not;(x1 + -143/123&middot;x0 &le; -143/410) &and; &not;(x1 + -43/44&middot;x0 &ge; 3/10)"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "A = init\n",
                 "# claim that in the given init region, the output is always y0 >= y1\n",
@@ -275,15 +511,48 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The above shows that instead  we can also use interpolant to find a larger input region for which the property still holds"
+                "The above interpolant shows that the property is true in almost all of the input region. This is easiest to see by graphing the interpolant in 2D, as shown below:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 19,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "\n",
+                            "        <iframe\n",
+                            "            width=\"720\"\n",
+                            "            height=\"480\"\n",
+                            "            src=\"https://www.geogebra.org/classic/qhtrrkrp\"\n",
+                            "            frameborder=\"0\"\n",
+                            "            allowfullscreen\n",
+                            "            \n",
+                            "        ></iframe>\n",
+                            "        "
+                        ],
+                        "text/plain": [
+                            "<IPython.lib.display.IFrame at 0x10d338820>"
+                        ]
+                    },
+                    "execution_count": 19,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from IPython.display import IFrame\n",
+                "IFrame(\"https://www.geogebra.org/classic/qhtrrkrp\",720,480)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Principle of Induction\n",
@@ -3996,14 +4265,47 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Conclusion\n",
                 "\n",
                 "This is the end of the interactive portion of the tutorial"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "\n",
+                            "        <iframe\n",
+                            "            width=\"720\"\n",
+                            "            height=\"480\"\n",
+                            "            src=\"https://www.geogebra.org/classic/qhtrrkrp\"\n",
+                            "            frameborder=\"0\"\n",
+                            "            allowfullscreen\n",
+                            "            \n",
+                            "        ></iframe>\n",
+                            "        "
+                        ],
+                        "text/plain": [
+                            "<IPython.lib.display.IFrame at 0x10d5bf730>"
+                        ]
+                    },
+                    "execution_count": 9,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "from IPython.display import IFrame\n",
+                "IFrame(\"https://www.geogebra.org/classic/qhtrrkrp\",720,480)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "venv",
             "language": "python",
             "name": "python3"
```

### Comparing `spacer_tutorial-0.0.2/Synasc2019.ipynb` & `spacer_tutorial-0.0.3/Synasc2019.ipynb`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/bakery.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/bakery.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/cfa.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/cfa.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/chc.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/chc.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/dcfa.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/dcfa.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/fml.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/fml.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/proof.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/proof.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/solve.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/solve.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/ts.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/ts.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/src/spacer_tutorial/vcgen.py` & `spacer_tutorial-0.0.3/src/spacer_tutorial/vcgen.py`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/LICENSE` & `spacer_tutorial-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacer_tutorial-0.0.2/pyproject.toml` & `spacer_tutorial-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spacer_tutorial"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Arie Gurfinkel", email="arie.gurfinkel@uwaterloo.ca" },
 ]
 description = "Transition systems and other support for Spacer Jupyter Tutorial"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `spacer_tutorial-0.0.2/PKG-INFO` & `spacer_tutorial-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacer_tutorial
-Version: 0.0.2
+Version: 0.0.3
 Summary: Transition systems and other support for Spacer Jupyter Tutorial
 Project-URL: Homepage, https://github.com/agurfinkel/spacer-on-jupyter
 Project-URL: Bug Tracker, https://github.com/agurfinkel/spacer-on-jupyter/issues
 Author-email: Arie Gurfinkel <arie.gurfinkel@uwaterloo.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

