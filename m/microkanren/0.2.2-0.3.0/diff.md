# Comparing `tmp/microkanren-0.2.2.tar.gz` & `tmp/microkanren-0.3.0.tar.gz`

## Comparing `microkanren-0.2.2.tar` & `microkanren-0.3.0.tar`

### file list

```diff
@@ -1,127 +1,132 @@
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 microkanren-0.2.2/.dir-locals.el
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 microkanren-0.2.2/.flake8
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 microkanren-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 microkanren-0.2.2/eqstats
--rw-r--r--   0        0        0    24114 2020-02-02 00:00:00.000000 microkanren-0.2.2/lambdastats
--rw-r--r--   0        0        0   108899 2020-02-02 00:00:00.000000 microkanren-0.2.2/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/12b2473498b257a5
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/12d5c5076e7d661a
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/1a3971a8088378fa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/1ba464f4c461a443
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/1db7621172052592
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/219203f970303938
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/2221493465c4b87c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/243fc0a435fe8f24
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/25656f03f40dcde
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/25a8329fc375eaac
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/25ac391031dd7c74
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/28366a523c2300fd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/2ea134d4cabb0ac8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/33b0347acbfe4163
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/374bbc681e8f1ee5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/3b292f2356fbe91c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/3d08eaa4c0663b06
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/3da6c59c12991cbb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/3f4396daed32427
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/3f9291a0c909e64
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/3fc0f873b0fec10f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/46a84ef7a4c12eaa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/47d34b5487e1022f
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/48d7c5a897f27f49
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/49807e9e41e0b2a1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/4ab853408bf4916a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/4ba429114b57df44
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/4dc4c5f638d543a4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/4f110938ecd8bb76
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/502609f0ad43ade4
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/50657b35c5c172b4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/526a985106bd7b39
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/5361b343dc6e7004
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/5605e5849372f227
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/5a75c3340a4cd45e
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/5c1634ffc9b61f89
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/5c3ef838607d0ee6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/5cd7fb71b6f2c48f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/5d7f57c24d828a26
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/5fa638bed8d56fff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/6055ed0423c9a8b8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/624bb3c1d125bc54
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/67187c816079efa4
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/67b5173fb3386e82
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/6922fb0aa8d4c0c9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/6dd791724c3e1488
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/71543a4e69af6bc4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/748abe5b3f808eae
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/7624bbf3fea25119
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/765d8af091e9b4d8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/7a4a1940926d293f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/7cf868287e752f7d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/7d36ce32b4f6711e
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/7dfad8bf24d12528
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/851365d30f59e319
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/853a33a5ce08b754
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/854565afaee83f71
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/87e3ca4168ccaadf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/89b01049b2d1276b
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/8a5b4c99aa1ab2d9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/8c43736823982fd7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/8d5565da6200359c
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/9576ec1ba4f157e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/9701ba061431517a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/990796e76d4d0614
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/99790a41b39e7c16
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/9ca2234c1578fc42
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/9e3acf28b1ccb741
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/a156cdb409b56217
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/a1d60687ae98bfdf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/a23d92b739778f3b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/a6f301fad936dd8f
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/a8865d2ebb297bd8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/acb49a39c8a7a7cf
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/ad3088309877b0ca
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/adf8bdbca0957709
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/ae46c6398f715f02
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/b1f7beb124810ce9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/b5bfa3cb56426832
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/b5e3aa96b9c3b299
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/b5f4a66125330968
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/b867605c7e0fa821
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/bc1ae9ffd6f8fe46
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/c11ec8839ed17196
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/c2c13b7ef1746d68
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/c329f98e76946bbc
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/c99eaab4de8198ec
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/cd51bf2f97b44d00
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/d2a2f01d5f84bc18
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/d2b0d38843ee4213
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/d87db07b1718fea9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/d975526c6a6286f7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/da5966ee78c9b514
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/ddc3f3c3e6f84c92
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/de1cd4657a693176
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/df8d6288e2a15497
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/e06a399e832adab1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/e2158c003835f1fc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/e4afce302a4a3f5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/e8f138dfce2dce04
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/e99b79fb0295b34c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/eae6a6608bcaf8f1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/f44fcef21f89bda
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/f5c966baff1008b8
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 microkanren-0.2.2/.ruff_cache/content/fec3c4b9409ef258
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 microkanren-0.2.2/src/microkanren/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 microkanren-0.2.2/src/microkanren/cons.py
--rw-r--r--   0        0        0    27531 2020-02-02 00:00:00.000000 microkanren-0.2.2/src/microkanren/core.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 microkanren-0.2.2/src/microkanren/goals.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 microkanren-0.2.2/src/microkanren/utils.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 microkanren-0.2.2/tests/test_ast.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 microkanren-0.2.2/tests/test_core.py
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 microkanren-0.2.2/tests/test_fd.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 microkanren-0.2.2/tests/test_lambda.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 microkanren-0.2.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 microkanren-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microkanren-0.2.2/README.md
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 microkanren-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 microkanren-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 microkanren-0.3.0/.dir-locals.el
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 microkanren-0.3.0/.flake8
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 microkanren-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 microkanren-0.3.0/eqstats
+-rw-r--r--   0        0        0    24114 2020-02-02 00:00:00.000000 microkanren-0.3.0/lambdastats
+-rw-r--r--   0        0        0   108899 2020-02-02 00:00:00.000000 microkanren-0.3.0/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/12b2473498b257a5
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/12d5c5076e7d661a
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/1a3971a8088378fa
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/1ac35766268534af
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/1ba464f4c461a443
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/1db7621172052592
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/219203f970303938
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/2221493465c4b87c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/243fc0a435fe8f24
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/25656f03f40dcde
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/25a8329fc375eaac
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/25ac391031dd7c74
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/28366a523c2300fd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/2ea134d4cabb0ac8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/33b0347acbfe4163
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/366e123530c9524
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/373241c8743e947e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/374bbc681e8f1ee5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3b292f2356fbe91c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3d08eaa4c0663b06
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3da6c59c12991cbb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3f4396daed32427
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3f9291a0c909e64
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3fc0f873b0fec10f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/46a84ef7a4c12eaa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/47d34b5487e1022f
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/48d7c5a897f27f49
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/49807e9e41e0b2a1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/4ab853408bf4916a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/4ba429114b57df44
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/4dc4c5f638d543a4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/4f110938ecd8bb76
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/502609f0ad43ade4
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/50657b35c5c172b4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/526a985106bd7b39
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5361b343dc6e7004
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5605e5849372f227
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5a75c3340a4cd45e
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5c1634ffc9b61f89
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5c3ef838607d0ee6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5cd7fb71b6f2c48f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5d7f57c24d828a26
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5fa638bed8d56fff
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/6055ed0423c9a8b8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/624bb3c1d125bc54
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/67187c816079efa4
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/67b5173fb3386e82
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/6922fb0aa8d4c0c9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/6dd791724c3e1488
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/71543a4e69af6bc4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/748abe5b3f808eae
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7624bbf3fea25119
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/765d8af091e9b4d8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7a4a1940926d293f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7cf868287e752f7d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7d36ce32b4f6711e
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7dfad8bf24d12528
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/851365d30f59e319
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/853a33a5ce08b754
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/854565afaee83f71
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/87e3ca4168ccaadf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/89b01049b2d1276b
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/89b43b5f4dedf5b3
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/8a5b4c99aa1ab2d9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/8c43736823982fd7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/8d5565da6200359c
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9576ec1ba4f157e1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9701ba061431517a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/990796e76d4d0614
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/99790a41b39e7c16
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9ca2234c1578fc42
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9e3acf28b1ccb741
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9f438292f325350a
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a156cdb409b56217
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a1d60687ae98bfdf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a23d92b739778f3b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a6f301fad936dd8f
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a8865d2ebb297bd8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/acb49a39c8a7a7cf
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/ad3088309877b0ca
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/adf8bdbca0957709
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/ae46c6398f715f02
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b1f7beb124810ce9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b5bfa3cb56426832
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b5e3aa96b9c3b299
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b5f4a66125330968
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b867605c7e0fa821
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/bc1ae9ffd6f8fe46
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/c11ec8839ed17196
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/c2c13b7ef1746d68
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/c329f98e76946bbc
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/c99eaab4de8198ec
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/cd51bf2f97b44d00
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/d2a2f01d5f84bc18
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/d2b0d38843ee4213
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/d87db07b1718fea9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/d975526c6a6286f7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/da5966ee78c9b514
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/ddc3f3c3e6f84c92
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/de1cd4657a693176
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/df8d6288e2a15497
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e06a399e832adab1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e2158c003835f1fc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e4afce302a4a3f5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e8f138dfce2dce04
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e99b79fb0295b34c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/eae6a6608bcaf8f1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/f44fcef21f89bda
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/f5c966baff1008b8
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/fec3c4b9409ef258
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/cons.py
+-rw-r--r--   0        0        0    27492 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/core.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/goals.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/utils.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 microkanren-0.3.0/tests/test_ast.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 microkanren-0.3.0/tests/test_core.py
+-rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 microkanren-0.3.0/tests/test_fd.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 microkanren-0.3.0/tests/test_lambda.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 microkanren-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 microkanren-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 microkanren-0.3.0/README.md
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 microkanren-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 microkanren-0.3.0/PKG-INFO
```

### Comparing `microkanren-0.2.2/.dir-locals.el` & `microkanren-0.3.0/.dir-locals.el`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/eqstats` & `microkanren-0.3.0/eqstats`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/lambdastats` & `microkanren-0.3.0/lambdastats`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl` & `microkanren-0.3.0/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/48d7c5a897f27f49` & `microkanren-0.3.0/.ruff_cache/content/48d7c5a897f27f49`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/4dc4c5f638d543a4` & `microkanren-0.3.0/.ruff_cache/content/4dc4c5f638d543a4`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/5605e5849372f227` & `microkanren-0.3.0/.ruff_cache/content/5605e5849372f227`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/5c1634ffc9b61f89` & `microkanren-0.3.0/.ruff_cache/content/5c1634ffc9b61f89`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/67b5173fb3386e82` & `microkanren-0.3.0/.ruff_cache/content/67b5173fb3386e82`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/7dfad8bf24d12528` & `microkanren-0.3.0/.ruff_cache/content/7dfad8bf24d12528`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/854565afaee83f71` & `microkanren-0.3.0/.ruff_cache/content/854565afaee83f71`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/8a5b4c99aa1ab2d9` & `microkanren-0.3.0/.ruff_cache/content/8a5b4c99aa1ab2d9`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/9576ec1ba4f157e1` & `microkanren-0.3.0/.ruff_cache/content/9576ec1ba4f157e1`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/99790a41b39e7c16` & `microkanren-0.3.0/.ruff_cache/content/99790a41b39e7c16`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/a1d60687ae98bfdf` & `microkanren-0.3.0/.ruff_cache/content/a1d60687ae98bfdf`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/a8865d2ebb297bd8` & `microkanren-0.3.0/.ruff_cache/content/a8865d2ebb297bd8`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/ad3088309877b0ca` & `microkanren-0.3.0/.ruff_cache/content/ad3088309877b0ca`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/adf8bdbca0957709` & `microkanren-0.3.0/.ruff_cache/content/adf8bdbca0957709`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/c11ec8839ed17196` & `microkanren-0.3.0/.ruff_cache/content/c11ec8839ed17196`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/d87db07b1718fea9` & `microkanren-0.3.0/.ruff_cache/content/d87db07b1718fea9`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/df8d6288e2a15497` & `microkanren-0.3.0/.ruff_cache/content/df8d6288e2a15497`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/.ruff_cache/content/f5c966baff1008b8` & `microkanren-0.3.0/.ruff_cache/content/f5c966baff1008b8`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/src/microkanren/core.py` & `microkanren-0.3.0/src/microkanren/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     Var | int | str | bool | tuple["Value", ...] | list["Value"] | cons | nil
 )
 Substitution: TypeAlias = PMap[Var, Value]
 NeqStore: TypeAlias = list[list[tuple[Var, Value]]]
 DomainStore: TypeAlias = PMap[Var, set[int]]
 ConstraintFunction: TypeAlias = Callable[["State"], Optional["State"]]
 ConstraintStore: TypeAlias = list["Constraint"]
-StreamThunk: TypeAlias = Callable[[], "Stream"]
 
 
 def empty_sub() -> Substitution:
     return pmap()
 
 
 def empty_domain_store() -> DomainStore:
@@ -99,41 +98,41 @@
     return make_domain(*range(start, end + 1))
 
 
 Stream: TypeAlias = tuple[()] | Callable[[], "Stream"] | tuple[State, "Stream"]
 
 
 class GoalProto(Protocol):
-    def __call__(self, state: State) -> StreamThunk:
+    def __call__(self, state: State) -> Stream:
         ...
 
 
 class GoalConstructorProto(Protocol):
     def __call__(self, *args: Value) -> GoalProto:
         ...
 
 
 class Goal:
     def __init__(self, goal: GoalProto):
         update_wrapper(self, goal)
         self.goal = goal
 
-    def __call__(self, state: State) -> StreamThunk:
+    def __call__(self, state: State) -> Stream:
         return lambda: self.goal(state)
 
     def __or__(self, other):
         # Use disj and conj instead of _disj and _conj, as the former delay their goals
         return disj(self, other)
 
     def __and__(self, other):
         return conj(self, other)
 
 
 def goal_from_constraint(constraint: ConstraintFunction) -> GoalProto:
-    def _goal(state: State) -> StreamThunk:
+    def _goal(state: State) -> Stream:
         match constraint(state):
             case None:
                 return mzero
             case _ as next_state:
                 return unit(next_state)
 
     return Goal(_goal)
@@ -146,27 +145,27 @@
 mzero = ()
 
 
 def unit(state: State) -> Stream:
     return (state, mzero)
 
 
-def mplus(s1: Stream, s2: Stream) -> StreamThunk:
+def mplus(s1: Stream, s2: Stream) -> Stream:
     match s1:
         case ():
             return lambda: s2
         case f if callable(f):
             return lambda: mplus(s2, f())
         case (head, tail):
             return lambda: (head, mplus(s2, tail))
         case _:
             raise InvalidStream
 
 
-def bind(stream: Stream, g: GoalProto) -> StreamThunk:
+def bind(stream: Stream, g: GoalProto) -> Stream:
     match stream:
         case ():
             return mzero
         case f if callable(f):
             return lambda: bind(f(), g)
         case (s1, s2):
             return lambda: mplus(g(s1), bind(s2, g))
@@ -244,47 +243,45 @@
     def _fail(state):
         return eq(False, True)(state)
 
     return Goal(_fail)
 
 
 def snooze(g: GoalConstructorProto, *args: Value) -> GoalProto:
-    def delayed_goal(state) -> StreamThunk:
+    def delayed_goal(state) -> Stream:
         return g(*args)(state)
 
     return Goal(delayed_goal)
 
 
 def delay(g: GoalProto) -> GoalProto:
     return Goal(lambda state: g(state))
 
 
 def disj(g: GoalProto, *goals: GoalProto) -> GoalProto:
     if goals == ():
         return delay(g)
-    g2, *rest = goals
-    return _disj(delay(g), disj(g2, *rest))
+    return reduce(_disj, (delay(goal) for goal in goals), delay(g))
 
 
 def _disj(g1: GoalProto, g2: GoalProto) -> GoalProto:
-    def __disj(state: State) -> StreamThunk:
+    def __disj(state: State) -> Stream:
         return mplus(g1(state), g2(state))
 
     return Goal(__disj)
 
 
 def conj(g: GoalProto, *goals: GoalProto) -> GoalProto:
     if goals == ():
         return delay(g)
-    g2, *rest = goals
-    return _conj(delay(g), conj(g2, *rest))
+    return reduce(_conj, (delay(goal) for goal in goals), delay(g))
 
 
 def _conj(g1: GoalProto, g2: GoalProto) -> GoalProto:
-    def __conj(state: State) -> StreamThunk:
+    def __conj(state: State) -> Stream:
         return bind(g1(state), g2)
 
     return Goal(__conj)
 
 
 def eq(u: Value, v: Value) -> GoalProto:
     def _eqc(state: State) -> State | None:
@@ -293,15 +290,17 @@
             # Unification failed
             return None
         elif new_sub == state.sub:
             # Unification succeeded without new associations
             return state
         else:
             prefix = get_sub_prefix(new_sub, state.sub)
-            return process_prefix(prefix, state.constraints)(state.set(sub=new_sub))
+            return Hooks.process_prefix(prefix, state.constraints)(
+                state.set(sub=new_sub)
+            )
 
     return goal_from_constraint(_eqc)
 
 
 def unify_all(
     constraint: list[tuple[Var, Value]], sub: Substitution
 ) -> Substitution | None:
@@ -664,15 +663,15 @@
             return compose_constraints(process_domain(v, domain_x), t)(state)
         return t(state)
 
     return _process_prefix_fd
 
 
 def enforce_constraints_fd(x: Var) -> GoalProto:
-    def _enforce_constraints(state: State) -> StreamThunk:
+    def _enforce_constraints(state: State) -> Stream:
         bound_vars = state.domains.keys()
         verify_all_bound(state.constraints, bound_vars)
         return onceo(force_answer(bound_vars))(state)
 
     return conj(force_answer(x), Goal(_enforce_constraints))
 
 
@@ -702,15 +701,15 @@
                 raise UnboundConstrainedVariable(
                     f"Constrained variable {var} has no domain"
                 )
         verify_all_bound(rest, bound_vars)
 
 
 def force_answer(x: Var | list[Var]) -> GoalProto:
-    def _force_answer(state: State) -> StreamThunk:
+    def _force_answer(state: State) -> Stream:
         match walk(x, state.sub):
             case Var(_) as var if (d := state.get_domain(var)) is not None:
                 return map_sum(lambda val: eq(x, val), d)(state)
             case (first, *rest) | cons(first, rest):
                 return conj(force_answer(first), force_answer(rest))(state)
             case _:
                 return succeed()(state)
@@ -752,17 +751,17 @@
         else:
             _args = (*args, accum)
         accum = f(*_args)
     return accum
 
 
 def ifte(g1, g2, g3=fail()) -> GoalProto:
-    def _ifte(state: State) -> StreamThunk:
+    def _ifte(state: State) -> Stream:
         # TODO: rewrite iteratively
-        def ifte_loop(stream: Stream) -> StreamThunk:
+        def ifte_loop(stream: Stream) -> Stream:
             match stream:
                 case ():
                     return g3(state)
                 case (_, _):
                     return bind(stream, g2)
                 case _:
                     return lambda: ifte_loop(stream())
@@ -854,18 +853,15 @@
         )
 
 
 def reify_state(state: State, v: Var) -> Value:
     v = walk_all(v, state.sub)
     reified_sub = reify_sub(v, empty_sub())
     v = walk_all(v, reified_sub)
-    return v
-    # if len(state.constraints) == 0:
-    #     return v
-    # return reify_constraints(v, reified_sub)(state)
+    return Hooks.reify_value(Hooks.reify_constraints(v, reified_sub, state))
 
 
 def walk_all(v: Value, s: Substitution) -> Value:
     v = walk(v, s)
     match v:
         case _ if isinstance(v, Var):
             return v
@@ -880,15 +876,15 @@
 
 
 def reify_sub(v: Value, s: Substitution) -> Substitution:
     # Allows us to control how fresh Vars are reified
     v = walk(v, s)
     match v:
         case _ if isinstance(v, Var):
-            return extend_substitution(v, ReifiedVar(len(s)), s)
+            return extend_substitution(v, Hooks.reify_var(v, s), s)
         case (a, *d) | cons(a, d):
             return reify_sub(d, reify_sub(a, s))
         case _:
             return s
 
 
 def call_with_empty_state(g: GoalProto) -> Stream:
@@ -897,87 +893,81 @@
 
 def run(n: int, f_fresh_vars: Callable[..., GoalProto]):
     n_vars = f_fresh_vars.__code__.co_argcount
     fresh_vars = tuple(Var(i) for i in range(n_vars))
     state = State.empty().set(var_count=n_vars)
     goal = conj(
         f_fresh_vars(*fresh_vars),
-        *map(enforce_constraints, fresh_vars),
+        *map(Hooks.enforce_constraints, fresh_vars),
     )
     return reify(take(n, goal(state)), *fresh_vars)
 
 
 def run_all(f_fresh_vars: Callable[..., GoalProto]):
     n_vars = f_fresh_vars.__code__.co_argcount
     fresh_vars = tuple(Var(i) for i in range(n_vars))
     state = State.empty().set(var_count=n_vars)
     goal = conj(
         f_fresh_vars(*fresh_vars),
-        *map(enforce_constraints, fresh_vars),
+        *map(Hooks.enforce_constraints, fresh_vars),
     )
     return reify(take_all(goal(state)), *fresh_vars)
 
 
 def irun(f_fresh_vars: Callable[..., GoalProto]):
     n_vars = f_fresh_vars.__code__.co_argcount
     fresh_vars = tuple(Var(i) for i in range(n_vars))
     state = State.empty().set(var_count=n_vars)
     goal = conj(
         f_fresh_vars(*fresh_vars),
-        *map(enforce_constraints, fresh_vars),
+        *map(Hooks.enforce_constraints, fresh_vars),
     )
     return ireify(itake(goal(state)), *fresh_vars)
 
 
 def default_process_prefix(*_):
     return identity
 
 
 def default_enforce_constraints(*_):
     return succeed()
 
 
-def default_reify_constraints(*_):
-    return succeed()
-
-
-__PROCESS_PREFIX__: Callable[
-    [Substitution, ConstraintStore],
-    ConstraintFunction,
-] = default_process_prefix
-__ENFORCE_CONSTRAINTS__: Callable[[Var], GoalProto] = default_enforce_constraints
-__REIFY_CONSTRAINTS__: Callable[
-    [Var, Substitution],
-    GoalProto,
-] = default_reify_constraints
-
-
-def set_process_prefix(constraint_function):
-    global __PROCESS_PREFIX__
-    __PROCESS_PREFIX__ = constraint_function
+def default_reify_constraints(value, *_):
+    return value
 
 
-def set_enforce_constraints(goal):
-    global __ENFORCE_CONSTRAINTS__
-    __ENFORCE_CONSTRAINTS__ = goal
+def default_reify_var(_, substitution):
+    return ReifiedVar(len(substitution))
 
 
-def set_reify_constraints(goal):
-    global __REIFY_CONSTRAINTS__
-    __REIFY_CONSTRAINTS__ = goal
+def default_reify_value(value):
+    return value
 
 
-def process_prefix(
-    prefix: Substitution, constraints: ConstraintStore
-) -> ConstraintFunction:
-    global __PROCESS_PREFIX__
-    return __PROCESS_PREFIX__(prefix, constraints)
-
-
-def enforce_constraints(x: Var) -> GoalProto:
-    global __ENFORCE_CONSTRAINTS__
-    return __ENFORCE_CONSTRAINTS__(x)
+class HooksMeta(type):
+    def _set_hook(cls, name):
+        def update_hooks(hook_function):
+            if not hasattr(cls, name):
+                raise AttributeError(
+                    f"Cannot set unknown hook '{name}' on registry '{cls.__name__}'"
+                )
+            setattr(cls, name, hook_function)
 
+        return update_hooks
 
-def reify_constraints(x: Var, s: Substitution) -> GoalProto:
-    global __REIFY_CONSTRAINTS__
-    return __REIFY_CONSTRAINTS__(x, s)
+    def __getattribute__(cls, attr):
+        if attr.startswith("set_"):
+            return cls._set_hook(attr[4:])
+        return super().__getattribute__(attr)
+
+
+class Hooks(metaclass=HooksMeta):
+    process_prefix: Callable[
+        [Substitution, ConstraintStore], ConstraintFunction
+    ] = default_process_prefix
+    enforce_constraints: Callable[[Var], GoalProto] = default_enforce_constraints
+    reify_constraints: Callable[
+        [Value, Substitution, State], Any
+    ] = default_reify_constraints
+    reify_var: Callable[[Var, Substitution], Any] = default_reify_var
+    reify_value: Callable[[Any], Any] = default_reify_value
```

### Comparing `microkanren-0.2.2/src/microkanren/goals.py` & `microkanren-0.3.0/src/microkanren/goals.py`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/tests/test_core.py` & `microkanren-0.3.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/tests/test_fd.py` & `microkanren-0.3.0/tests/test_fd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from itertools import permutations
 from math import sqrt
 
 import pytest
 
 from microkanren import (
+    Hooks,
     alldifffd,
     compose_constraints,
     conj,
     default_enforce_constraints,
     default_process_prefix,
     domfd,
     enforce_constraints_fd,
@@ -21,41 +22,39 @@
     neq,
     neqfd,
     plusfd,
     process_prefix_fd,
     process_prefix_neq,
     run,
     run_all,
-    set_enforce_constraints,
-    set_process_prefix,
 )
 
 
 @pytest.fixture(autouse=True, scope="module")
 def setup_process_prefix():
     def process_prefix(prefix, constraints):
         return compose_constraints(
             process_prefix_neq(prefix, constraints),
             process_prefix_fd(prefix, constraints),
         )
 
-    yield set_process_prefix(process_prefix)
-    set_process_prefix(default_process_prefix)
+    yield Hooks.set_process_prefix(process_prefix)
+    Hooks.set_process_prefix(default_process_prefix)
 
 
 @pytest.fixture(autouse=True, scope="module")
 def setup_enforce_constraints():
     def enforce_constraints(var):
         return conj(
             enforce_constraints_neq(var),
             enforce_constraints_fd(var),
         )
 
-    yield set_enforce_constraints(enforce_constraints)
-    set_enforce_constraints(default_enforce_constraints)
+    yield Hooks.set_enforce_constraints(enforce_constraints)
+    Hooks.set_enforce_constraints(default_enforce_constraints)
 
 
 class TestFdConstraints:
     @pytest.mark.parametrize("domain", [make_domain(1, 2, 3), make_domain(5, 7, 9)])
     def test_domfd(self, domain):
         result = run_all(lambda x: domfd(x, domain))
         assert set(result) == set(domain)
```

### Comparing `microkanren-0.2.2/tests/test_lambda.py` & `microkanren-0.3.0/tests/test_lambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from microkanren import (
     Constraint,
+    Hooks,
     Var,
     conj,
     disj,
     eq,
     extend_constraint_store,
     fresh,
     goal_from_constraint,
     run_constraints,
-    set_process_prefix,
     walk,
 )
 from microkanren.cons import cons
 
 
 def vcons(*args):
     return cons.from_xs(args)
@@ -61,15 +61,15 @@
     return _typeoc
 
 
 def process_prefix_typeo(prefix, constraints):
     return run_constraints(prefix.keys(), constraints)
 
 
-set_process_prefix(process_prefix_typeo)
+Hooks.set_process_prefix(process_prefix_typeo)
 
 
 def lambda_term(term):
     return disj(
         variable(term),
         fresh(
             lambda arg, body: conj(
```

### Comparing `microkanren-0.2.2/.gitignore` & `microkanren-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/LICENSE` & `microkanren-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microkanren-0.2.2/pyproject.toml` & `microkanren-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [project]
 name = "microkanren"
-version = "0.2.2"
+version = "0.3.0"
 authors = [
     { name="Joshua Munn", email="public@elysee-munn.family" },
 ]
 description = "A Python implementation of microkanren extended with constraints"
 readme = "README.md"
 requires-python = "~=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
 ]
 dependencies = [
     "pyrsistent ~= 0.19",
     "fastcons ~= 0.2.0",
 ]
+license = {file = "LICENSE"}
 
 [project.urls]
 "Homepage" = "https://github.com/jams2/microkanren"
 "Bug Tracker" = "https://github.com/jams2/microkanren/issues"
 
 [project.optional-dependencies]
 dev = [
@@ -36,21 +38,25 @@
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 minversion = 7.0
 
 [tool.ruff]
 line-length = 88
 src = ["src", "tests"]
+target-version = "py311"
 select = [
   "E",   # pycodestyle
   "F",   # pyflakes
   "UP",  # pyupgrade
   "I",   # isort
   "ARG", # unused arguments
   "PT",  # pytest style
   "T10", # flake8-debugger
   "C4",  # flake8-comprehensions
 ]
+unfixable = [
+  "ARG", # unused arguments
+]
 
 [tool.pyright]
-pythonVersion = "3.10"
+pythonVersion = "3.11"
 stubPath = ""
```

