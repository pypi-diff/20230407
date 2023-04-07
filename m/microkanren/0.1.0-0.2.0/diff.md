# Comparing `tmp/microkanren-0.1.0.tar.gz` & `tmp/microkanren-0.2.0.tar.gz`

## Comparing `microkanren-0.1.0.tar` & `microkanren-0.2.0.tar`

### file list

```diff
@@ -1,104 +1,127 @@
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 microkanren-0.1.0/.dir-locals.el
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 microkanren-0.1.0/.flake8
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 microkanren-0.1.0/eqstats
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/12d5c5076e7d661a
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/1a3971a8088378fa
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/1db7621172052592
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/219203f970303938
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/243fc0a435fe8f24
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/25656f03f40dcde
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/25a8329fc375eaac
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/28366a523c2300fd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/2ea134d4cabb0ac8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/33b0347acbfe4163
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/374bbc681e8f1ee5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/3b292f2356fbe91c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/3da6c59c12991cbb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/3f4396daed32427
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/3f9291a0c909e64
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/3fc0f873b0fec10f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/46a84ef7a4c12eaa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/47d34b5487e1022f
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/48d7c5a897f27f49
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/49807e9e41e0b2a1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/4ba429114b57df44
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/4dc4c5f638d543a4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/4f110938ecd8bb76
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/502609f0ad43ade4
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/50657b35c5c172b4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/5361b343dc6e7004
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/5605e5849372f227
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/5a75c3340a4cd45e
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/5c1634ffc9b61f89
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/5c3ef838607d0ee6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/5cd7fb71b6f2c48f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/5d7f57c24d828a26
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/6055ed0423c9a8b8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/624bb3c1d125bc54
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/67187c816079efa4
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/67b5173fb3386e82
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/6dd791724c3e1488
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/71543a4e69af6bc4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/748abe5b3f808eae
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/7624bbf3fea25119
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/765d8af091e9b4d8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/7a4a1940926d293f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/7cf868287e752f7d
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/7dfad8bf24d12528
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/854565afaee83f71
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/87e3ca4168ccaadf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/89b01049b2d1276b
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/8a5b4c99aa1ab2d9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/8c43736823982fd7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/8d5565da6200359c
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/9576ec1ba4f157e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/9701ba061431517a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/990796e76d4d0614
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/99790a41b39e7c16
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/9ca2234c1578fc42
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/9e3acf28b1ccb741
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/a156cdb409b56217
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/a1d60687ae98bfdf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/a23d92b739778f3b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/a6f301fad936dd8f
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/a8865d2ebb297bd8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/acb49a39c8a7a7cf
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/ad3088309877b0ca
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/adf8bdbca0957709
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/ae46c6398f715f02
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/b1f7beb124810ce9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/b5bfa3cb56426832
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/b5e3aa96b9c3b299
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/b5f4a66125330968
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/b867605c7e0fa821
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/bc1ae9ffd6f8fe46
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/c11ec8839ed17196
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/c2c13b7ef1746d68
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/cd51bf2f97b44d00
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/d2a2f01d5f84bc18
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/d87db07b1718fea9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/d975526c6a6286f7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/ddc3f3c3e6f84c92
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/e06a399e832adab1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/e2158c003835f1fc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/e8f138dfce2dce04
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/e99b79fb0295b34c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/eae6a6608bcaf8f1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/f44fcef21f89bda
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/f5c966baff1008b8
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 microkanren-0.1.0/.ruff_cache/content/fec3c4b9409ef258
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 microkanren-0.1.0/src/microkanren/__init__.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 microkanren-0.1.0/src/microkanren/cons.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 microkanren-0.1.0/src/microkanren/goals.py
--rw-r--r--   0        0        0    27685 2020-02-02 00:00:00.000000 microkanren-0.1.0/src/microkanren/microkanren.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 microkanren-0.1.0/src/microkanren/utils.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 microkanren-0.1.0/tests/test_ast.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 microkanren-0.1.0/tests/test_core.py
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 microkanren-0.1.0/tests/test_fd.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 microkanren-0.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 microkanren-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microkanren-0.1.0/README.md
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 microkanren-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 microkanren-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 microkanren-0.2.0/.dir-locals.el
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 microkanren-0.2.0/.flake8
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 microkanren-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 microkanren-0.2.0/eqstats
+-rw-r--r--   0        0        0    24114 2020-02-02 00:00:00.000000 microkanren-0.2.0/lambdastats
+-rw-r--r--   0        0        0   108899 2020-02-02 00:00:00.000000 microkanren-0.2.0/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/12b2473498b257a5
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/12d5c5076e7d661a
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/1a3971a8088378fa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/1ba464f4c461a443
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/1db7621172052592
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/219203f970303938
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/2221493465c4b87c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/243fc0a435fe8f24
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/25656f03f40dcde
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/25a8329fc375eaac
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/25ac391031dd7c74
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/28366a523c2300fd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/2ea134d4cabb0ac8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/33b0347acbfe4163
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/374bbc681e8f1ee5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/3b292f2356fbe91c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/3d08eaa4c0663b06
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/3da6c59c12991cbb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/3f4396daed32427
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/3f9291a0c909e64
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/3fc0f873b0fec10f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/46a84ef7a4c12eaa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/47d34b5487e1022f
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/48d7c5a897f27f49
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/49807e9e41e0b2a1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/4ab853408bf4916a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/4ba429114b57df44
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/4dc4c5f638d543a4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/4f110938ecd8bb76
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/502609f0ad43ade4
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/50657b35c5c172b4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/526a985106bd7b39
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/5361b343dc6e7004
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/5605e5849372f227
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/5a75c3340a4cd45e
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/5c1634ffc9b61f89
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/5c3ef838607d0ee6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/5cd7fb71b6f2c48f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/5d7f57c24d828a26
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/5fa638bed8d56fff
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/6055ed0423c9a8b8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/624bb3c1d125bc54
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/67187c816079efa4
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/67b5173fb3386e82
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/6922fb0aa8d4c0c9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/6dd791724c3e1488
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/71543a4e69af6bc4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/748abe5b3f808eae
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/7624bbf3fea25119
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/765d8af091e9b4d8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/7a4a1940926d293f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/7cf868287e752f7d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/7d36ce32b4f6711e
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/7dfad8bf24d12528
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/851365d30f59e319
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/853a33a5ce08b754
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/854565afaee83f71
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/87e3ca4168ccaadf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/89b01049b2d1276b
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/8a5b4c99aa1ab2d9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/8c43736823982fd7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/8d5565da6200359c
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/9576ec1ba4f157e1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/9701ba061431517a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/990796e76d4d0614
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/99790a41b39e7c16
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/9ca2234c1578fc42
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/9e3acf28b1ccb741
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/a156cdb409b56217
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/a1d60687ae98bfdf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/a23d92b739778f3b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/a6f301fad936dd8f
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/a8865d2ebb297bd8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/acb49a39c8a7a7cf
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/ad3088309877b0ca
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/adf8bdbca0957709
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/ae46c6398f715f02
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/b1f7beb124810ce9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/b5bfa3cb56426832
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/b5e3aa96b9c3b299
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/b5f4a66125330968
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/b867605c7e0fa821
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/bc1ae9ffd6f8fe46
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/c11ec8839ed17196
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/c2c13b7ef1746d68
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/c329f98e76946bbc
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/c99eaab4de8198ec
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/cd51bf2f97b44d00
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/d2a2f01d5f84bc18
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/d2b0d38843ee4213
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/d87db07b1718fea9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/d975526c6a6286f7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/da5966ee78c9b514
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/ddc3f3c3e6f84c92
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/de1cd4657a693176
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/df8d6288e2a15497
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/e06a399e832adab1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/e2158c003835f1fc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/e4afce302a4a3f5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/e8f138dfce2dce04
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/e99b79fb0295b34c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/eae6a6608bcaf8f1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/f44fcef21f89bda
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/f5c966baff1008b8
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 microkanren-0.2.0/.ruff_cache/content/fec3c4b9409ef258
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 microkanren-0.2.0/src/microkanren/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 microkanren-0.2.0/src/microkanren/cons.py
+-rw-r--r--   0        0        0    27508 2020-02-02 00:00:00.000000 microkanren-0.2.0/src/microkanren/core.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 microkanren-0.2.0/src/microkanren/goals.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 microkanren-0.2.0/src/microkanren/utils.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 microkanren-0.2.0/tests/test_ast.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 microkanren-0.2.0/tests/test_core.py
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 microkanren-0.2.0/tests/test_fd.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 microkanren-0.2.0/tests/test_lambda.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 microkanren-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 microkanren-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microkanren-0.2.0/README.md
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 microkanren-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 microkanren-0.2.0/PKG-INFO
```

### Comparing `microkanren-0.1.0/.dir-locals.el` & `microkanren-0.2.0/.dir-locals.el`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/eqstats` & `microkanren-0.2.0/eqstats`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/48d7c5a897f27f49` & `microkanren-0.2.0/.ruff_cache/content/48d7c5a897f27f49`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/4dc4c5f638d543a4` & `microkanren-0.2.0/.ruff_cache/content/4dc4c5f638d543a4`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/5605e5849372f227` & `microkanren-0.2.0/.ruff_cache/content/5605e5849372f227`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/5c1634ffc9b61f89` & `microkanren-0.2.0/.ruff_cache/content/5c1634ffc9b61f89`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/67b5173fb3386e82` & `microkanren-0.2.0/.ruff_cache/content/67b5173fb3386e82`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/7dfad8bf24d12528` & `microkanren-0.2.0/.ruff_cache/content/7dfad8bf24d12528`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/854565afaee83f71` & `microkanren-0.2.0/.ruff_cache/content/854565afaee83f71`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/8a5b4c99aa1ab2d9` & `microkanren-0.2.0/.ruff_cache/content/8a5b4c99aa1ab2d9`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/9576ec1ba4f157e1` & `microkanren-0.2.0/.ruff_cache/content/9576ec1ba4f157e1`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/99790a41b39e7c16` & `microkanren-0.2.0/.ruff_cache/content/99790a41b39e7c16`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/a1d60687ae98bfdf` & `microkanren-0.2.0/.ruff_cache/content/a1d60687ae98bfdf`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/a8865d2ebb297bd8` & `microkanren-0.2.0/.ruff_cache/content/a8865d2ebb297bd8`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/ad3088309877b0ca` & `microkanren-0.2.0/.ruff_cache/content/ad3088309877b0ca`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/adf8bdbca0957709` & `microkanren-0.2.0/.ruff_cache/content/adf8bdbca0957709`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/c11ec8839ed17196` & `microkanren-0.2.0/.ruff_cache/content/c11ec8839ed17196`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/d87db07b1718fea9` & `microkanren-0.2.0/.ruff_cache/content/d87db07b1718fea9`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.ruff_cache/content/f5c966baff1008b8` & `microkanren-0.2.0/.ruff_cache/content/f5c966baff1008b8`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/src/microkanren/goals.py` & `microkanren-0.2.0/src/microkanren/goals.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+from fastcons import cons, nil
+
 from microkanren import (
     Goal,
     State,
     Stream,
     Var,
     conj,
     disj,
     eq,
     fail,
     fresh,
     ifte,
     neq,
 )
-from microkanren.cons import Cons, cons, nil
 
 
-def appendo(xs: Cons | Var, ys: Cons | Var, zs: Cons | Var) -> Goal:
+def appendo(xs: cons | Var, ys: cons | Var, zs: cons | Var) -> Goal:
     return disj(
         nullo(xs) & eq(ys, zs),
         fresh(
             lambda a, d, res: conj(
                 conso(a, d, xs),
                 conso(a, res, zs),
                 appendo(d, ys, res),
```

### Comparing `microkanren-0.1.0/src/microkanren/microkanren.py` & `microkanren-0.2.0/src/microkanren/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 """
 
 from collections.abc import Callable, Generator
 from dataclasses import dataclass
 from functools import reduce, update_wrapper, wraps
 from typing import Any, Optional, Protocol, TypeAlias, TypeVar
 
+from fastcons import cons, nil
 from pyrsistent import PClass, field, pmap
 from pyrsistent.typing import PMap
 
-from microkanren.cons import Cons, cons, to_python
 from microkanren.utils import identity, partition
 
 NOT_FOUND = object()
 
 
 @dataclass(slots=True, frozen=True)
 class Var:
@@ -31,15 +31,17 @@
 class ReifiedVar:
     i: int
 
     def __repr__(self):
         return f"_.{self.i}"
 
 
-Value: TypeAlias = Var | int | str | bool | tuple["Value", ...] | list["Value"] | Cons
+Value: TypeAlias = (
+    Var | int | str | bool | tuple["Value", ...] | list["Value"] | cons | nil
+)
 Substitution: TypeAlias = PMap[Var, Value]
 NeqStore: TypeAlias = list[list[tuple[Var, Value]]]
 DomainStore: TypeAlias = PMap[Var, set[int]]
 ConstraintFunction: TypeAlias = Callable[["State"], Optional["State"]]
 ConstraintStore: TypeAlias = list["Constraint"]
 StreamThunk: TypeAlias = Callable[[], "Stream"]
 
@@ -126,17 +128,17 @@
         return conj(self, other)
 
 
 def goal_from_constraint(constraint: ConstraintFunction) -> GoalProto:
     def _goal(state: State) -> StreamThunk:
         match constraint(state):
             case None:
-                return lambda: mzero
+                return mzero
             case _ as next_state:
-                return lambda: unit(next_state)
+                return unit(next_state)
 
     return Goal(_goal)
 
 
 class InvalidStream(Exception):
     pass
 
@@ -159,15 +161,15 @@
         case _:
             raise InvalidStream
 
 
 def bind(stream: Stream, g: GoalProto) -> StreamThunk:
     match stream:
         case ():
-            return lambda: mzero
+            return mzero
         case f if callable(f):
             return lambda: bind(f(), g)
         case (s1, s2):
             return lambda: mplus(g(s1), bind(s2, g))
         case _:
             raise InvalidStream
 
@@ -243,47 +245,47 @@
         return eq(False, True)(state)
 
     return Goal(_fail)
 
 
 def snooze(g: GoalConstructorProto, *args: Value) -> GoalProto:
     def delayed_goal(state) -> StreamThunk:
-        return lambda: g(*args)(state)
+        return g(*args)(state)
 
     return Goal(delayed_goal)
 
 
 def delay(g: GoalProto) -> GoalProto:
-    return Goal(lambda state: lambda: g(state))
+    return Goal(lambda state: g(state))
 
 
 def disj(g: GoalProto, *goals: GoalProto) -> GoalProto:
     if goals == ():
         return delay(g)
     g2, *rest = goals
     return _disj(delay(g), disj(g2, *rest))
 
 
 def _disj(g1: GoalProto, g2: GoalProto) -> GoalProto:
     def __disj(state: State) -> StreamThunk:
-        return lambda: mplus(g1(state), g2(state))
+        return mplus(g1(state), g2(state))
 
     return Goal(__disj)
 
 
 def conj(g: GoalProto, *goals: GoalProto) -> GoalProto:
     if goals == ():
         return delay(g)
     g2, *rest = goals
     return _conj(delay(g), conj(g2, *rest))
 
 
 def _conj(g1: GoalProto, g2: GoalProto) -> GoalProto:
     def __conj(state: State) -> StreamThunk:
-        return lambda: bind(g1(state), g2)
+        return bind(g1(state), g2)
 
     return Goal(__conj)
 
 
 def eq(u: Value, v: Value) -> GoalProto:
     def _eqc(state: State) -> State | None:
         new_sub = unify(u, v, state.sub)
@@ -631,22 +633,19 @@
 ) -> ConstraintFunction:
     prefix_vars = {x for x in prefix.keys() if isinstance(x, Var)}
     prefix_vars.update({x for x in prefix.values() if isinstance(x, Var)})
     return run_constraints(prefix_vars, constraints)
 
 
 def enforce_constraints_neq(_: Var) -> GoalProto:
-    return lambda state: lambda: unit(state)
+    return lambda state: unit(state)
 
 
 def reify_constraints_neq(_: Var, __: Substitution) -> ConstraintFunction:
-    def _reify_constraints_neq(state: State):
-        return state
-
-    return _reify_constraints_neq
+    return identity
 
 
 def process_prefix_fd(
     prefix: Substitution, constraints: ConstraintStore
 ) -> ConstraintFunction:
     if not prefix:
         return identity
@@ -668,15 +667,15 @@
     return _process_prefix_fd
 
 
 def enforce_constraints_fd(x: Var) -> GoalProto:
     def _enforce_constraints(state: State) -> StreamThunk:
         bound_vars = state.domains.keys()
         verify_all_bound(state.constraints, bound_vars)
-        return lambda: onceo(force_answer(bound_vars))(state)
+        return onceo(force_answer(bound_vars))(state)
 
     return conj(force_answer(x), Goal(_enforce_constraints))
 
 
 # TODO
 def reify_constraints_fd(_: Var, __: Substitution) -> ConstraintFunction:
     def _reify_constraints_fd(state: State) -> State | None:
@@ -706,19 +705,19 @@
         verify_all_bound(rest, bound_vars)
 
 
 def force_answer(x: Var | list[Var]) -> GoalProto:
     def _force_answer(state: State) -> StreamThunk:
         match walk(x, state.sub):
             case Var(_) as var if (d := state.get_domain(var)) is not None:
-                return lambda: map_sum(lambda val: eq(x, val), d)(state)
+                return map_sum(lambda val: eq(x, val), d)(state)
             case (first, *rest):
-                return lambda: conj(force_answer(first), force_answer(rest))(state)
+                return conj(force_answer(first), force_answer(rest))(state)
             case _:
-                return lambda: succeed()(state)
+                return succeed()(state)
 
     return _force_answer
 
 
 A = TypeVar("A")
 
 
@@ -754,38 +753,39 @@
             _args = (*args, accum)
         accum = f(*_args)
     return accum
 
 
 def ifte(g1, g2, g3=fail()) -> GoalProto:
     def _ifte(state: State) -> StreamThunk:
+        # TODO: rewrite iteratively
         def ifte_loop(stream: Stream) -> StreamThunk:
             match stream:
                 case ():
-                    return lambda: g3(state)
+                    return g3(state)
                 case (_, _):
-                    return lambda: bind(stream, g2)
+                    return bind(stream, g2)
                 case _:
                     return lambda: ifte_loop(stream())
 
         return ifte_loop(g1(state))
 
     return Goal(_ifte)
 
 
 def onceo(g: GoalProto) -> GoalProto:
     def _onceo(state: State):
         stream = g(state)
         while stream:
             match stream:
                 case (s1, _):
-                    return lambda: unit(s1)
+                    return unit(s1)
                 case _:
                     stream = stream()
-        return lambda: mzero
+        return mzero
 
     return _onceo
 
 
 def fresh(fp: Callable) -> GoalProto:
     n = fp.__code__.co_argcount
 
@@ -852,20 +852,20 @@
         yield from (
             tuple(reify_state(s, var) for var in top_level_vars) for s in states
         )
 
 
 def reify_state(state: State, v: Var) -> Value:
     v = walk_all(v, state.sub)
-    r = reify_sub(v, empty_sub())
-    v = walk_all(v, r)
-    return to_python(v)
-    if len(state.constraints) == 0:
-        return to_python(v)
-    return to_python(reify_constraints(v, r)(state))
+    reified_sub = reify_sub(v, empty_sub())
+    v = walk_all(v, reified_sub)
+    return v
+    # if len(state.constraints) == 0:
+    #     return v
+    # return reify_constraints(v, reified_sub)(state)
 
 
 def walk_all(v: Value, s: Substitution) -> Value:
     v = walk(v, s)
     match v:
         case _ if isinstance(v, Var):
             return v
```

### Comparing `microkanren-0.1.0/tests/test_core.py` & `microkanren-0.2.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/tests/test_fd.py` & `microkanren-0.2.0/tests/test_fd.py`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/.gitignore` & `microkanren-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/LICENSE` & `microkanren-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microkanren-0.1.0/pyproject.toml` & `microkanren-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [project]
 name = "microkanren"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name="Joshua Munn", email="public@elysee-munn.family" },
 ]
-description = "A Python implementation of microKanren extended with constraints"
+description = "A Python implementation of microkanren extended with constraints"
 readme = "README.md"
-requires-python = ">= 3.10"
+requires-python = "==3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
 ]
 dependencies = [
-    "pyrsistent ~= 0.19"
+    "pyrsistent ~= 0.19",
+    "fastcons ~= 0.2.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jams2/microkanren"
 "Bug Tracker" = "https://github.com/jams2/microkanren/issues"
 
 [project.optional-dependencies]
```

### Comparing `microkanren-0.1.0/PKG-INFO` & `microkanren-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: microkanren
-Version: 0.1.0
-Summary: A Python implementation of microKanren extended with constraints
+Version: 0.2.0
+Summary: A Python implementation of microkanren extended with constraints
 Project-URL: Homepage, https://github.com/jams2/microkanren
 Project-URL: Bug Tracker, https://github.com/jams2/microkanren/issues
 Author-email: Joshua Munn <public@elysee-munn.family>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: ==3.11
+Requires-Dist: fastcons~=0.2.0
 Requires-Dist: pyrsistent~=0.19
 Provides-Extra: dev
 Requires-Dist: black~=23.1.0; extra == 'dev'
 Requires-Dist: ruff~=0.0.256; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: pytest-profiling~=1.7.0; extra == 'testing'
 Requires-Dist: pytest~=7.2.2; extra == 'testing'
```

