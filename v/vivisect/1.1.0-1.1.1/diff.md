# Comparing `tmp/vivisect-1.1.0.tar.gz` & `tmp/vivisect-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivisect-1.1.0.tar", last modified: Fri Feb 24 02:24:51 2023, max compression
+gzip compressed data, was "vivisect-1.1.1.tar", last modified: Fri Apr  7 20:03:21 2023, max compression
```

## Comparing `vivisect-1.1.0.tar` & `vivisect-1.1.1.tar`

### file list

```diff
@@ -1,730 +1,730 @@
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.047929 vivisect-1.1.0/
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.007929 vivisect-1.1.0/Elf/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    33903 2023-02-18 04:09:19.000000 vivisect-1.1.0/Elf/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       41 2023-01-13 00:18:01.000000 vivisect-1.1.0/Elf/elf_lookup.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11357 2022-08-31 06:02:46.000000 vivisect-1.1.0/LICENSE.txt
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.007929 vivisect-1.1.0/PE/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    54083 2023-01-13 00:18:01.000000 vivisect-1.1.0/PE/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2611 2023-01-13 00:18:01.000000 vivisect-1.1.0/PE/carve.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6170 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/cofflib.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.007929 vivisect-1.1.0/PE/ordlookup/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      840 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/ordlookup/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3028 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/ordlookup/comctl32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   380351 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/ordlookup/mfc42.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    16265 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/ordlookup/msvbvm60.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10081 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/ordlookup/oleaut32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      647 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/ordlookup/oledlg.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3032 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/ordlookup/ws2_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1362 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/petool.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.007929 vivisect-1.1.0/PE/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      167 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/tests/test_version.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.007929 vivisect-1.1.0/PE/tools/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/tools/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      703 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/tools/printord.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1377 2022-08-31 06:02:46.000000 vivisect-1.1.0/PE/tools/structdump.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2358 2023-02-24 02:24:51.047929 vivisect-1.1.0/PKG-INFO
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1593 2023-01-13 00:18:01.000000 vivisect-1.1.0/README.md
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/cobra/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    37107 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/cobra/auth/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      878 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/auth/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1925 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/auth/shadowfile.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1815 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/cache.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    19277 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/cluster.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3388 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/dcode.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8083 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/devent.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2014 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/dispatcher.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/cobra/hostid/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      341 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/hostid/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1908 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/hostid/darwinhostid.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      278 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/hostid/windowshostid.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    19598 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/http.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2189 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/pool.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2163 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/remoteapp.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/cobra/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      533 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3297 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tests/testbasic.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1048 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tests/testcache.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1195 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tests/testdcode.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      647 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tests/testevents.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      631 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tests/testnewobj.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/cobra/tools/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tools/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2492 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tools/burnapp.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      509 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tools/queend.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      415 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tools/runtests.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      424 2022-08-31 06:02:46.000000 vivisect-1.1.0/cobra/tools/workerd.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/envi/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    51043 2023-02-23 16:57:27.000000 vivisect-1.1.0/envi/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/envi/archs/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      714 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/envi/archs/amd64/
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     5182 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/archs/amd64/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    30851 2023-02-10 15:47:39.000000 vivisect-1.1.0/envi/archs/amd64/disasm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   206683 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/amd64/opcode64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5478 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/amd64/regs.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4731 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/amd64/vmcslookup.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/envi/archs/arm/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4691 2023-02-10 15:47:39.000000 vivisect-1.1.0/envi/archs/arm/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    21305 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/arm/const.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   178363 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/arm/disasm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    74062 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/archs/arm/emu.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7887 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/arm/regs.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/envi/archs/h8/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5519 2023-02-10 15:47:39.000000 vivisect-1.1.0/envi/archs/h8/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      259 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/h8/const.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1859 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/h8/disasm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    36055 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/h8/emu.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    15621 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/h8/operands.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    43111 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/h8/parsers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2955 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/h8/regs.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/envi/archs/i386/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1181 2023-02-10 15:47:39.000000 vivisect-1.1.0/envi/archs/i386/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    42485 2023-02-10 15:47:39.000000 vivisect-1.1.0/envi/archs/i386/disasm.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)    80806 2023-02-10 15:44:31.000000 vivisect-1.1.0/envi/archs/i386/emu.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   187007 2023-01-13 18:44:57.000000 vivisect-1.1.0/envi/archs/i386/opcode86.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11659 2023-01-13 18:44:57.000000 vivisect-1.1.0/envi/archs/i386/opconst.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4447 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/i386/regs.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/envi/archs/msp430/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1150 2023-02-10 15:47:39.000000 vivisect-1.1.0/envi/archs/msp430/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4591 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/msp430/const.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    30649 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/msp430/disasm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    15639 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/msp430/emu.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1313 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/msp430/regs.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.011929 vivisect-1.1.0/envi/archs/thumb16/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      175 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/thumb16/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    91529 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/archs/thumb16/disasm.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.015929 vivisect-1.1.0/envi/archs/z80/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       33 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/z80/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      401 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/z80/const.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2831 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/z80/disasm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      820 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/z80/regs.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    53810 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/archs/z80/z80opcode.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1448 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/bintree.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     9057 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/bits.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5390 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/bytesig.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    29793 2023-01-13 18:44:57.000000 vivisect-1.1.0/envi/cli.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11988 2023-02-10 15:47:39.000000 vivisect-1.1.0/envi/codeflow.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1027 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/common.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8359 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/config.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1032 2023-02-10 15:47:39.000000 vivisect-1.1.0/envi/const.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      608 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/encoding.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6765 2023-02-18 04:09:19.000000 vivisect-1.1.0/envi/exc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4068 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/expression.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2749 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/ieee754.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2453 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/interactive.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.015929 vivisect-1.1.0/envi/memcanvas/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    12090 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/memcanvas/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.015929 vivisect-1.1.0/envi/memcanvas/renderers/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4539 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/memcanvas/renderers/__init__.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)    26522 2023-02-18 04:09:19.000000 vivisect-1.1.0/envi/memory.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2363 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/pagelookup.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      813 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/pyzip.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.015929 vivisect-1.1.0/envi/qt/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       52 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/qt/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2807 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/qt/config.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5201 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/qt/html.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   245078 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/qt/jquery.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10983 2023-02-23 16:57:27.000000 vivisect-1.1.0/envi/qt/memcanvas.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1932 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/qt/memdump.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10569 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/qt/memory.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3954 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/qt/memorymap.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4981 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/qt/memsearch.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8865 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/qt/memwrite.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2027 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/radixtree.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13650 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/registers.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.015929 vivisect-1.1.0/envi/symstore/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      112 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/symstore/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13966 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/symstore/resolver.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3452 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/symstore/symcache.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.015929 vivisect-1.1.0/envi/tests/
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)      426 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10446 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/arm_bit_test_adds.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9971 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/arm_bit_test_cmn.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10223 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/arm_bit_test_cmp.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10656 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/arm_bit_test_subs.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   341046 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/armthumb_tests.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.015929 vivisect-1.1.0/envi/tests/msp430/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3321 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iadc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3063 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iadd.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3722 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iaddc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1434 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iand.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2060 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/ibic.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2118 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/ibis.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1434 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/ibit.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      332 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/ibr.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      386 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/icall.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1236 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iclr.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iclrc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iclrn.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iclrz.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3550 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/icmp.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3027 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/idadc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2732 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/idadd.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2435 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/idec.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3088 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/idecd.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2178 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iinc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3123 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iincd.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1246 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iinv.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5325 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/ijumps.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9646 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/imov.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      302 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/inop.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      698 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/ipop.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      758 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/ipush.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      368 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iret.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2576 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/irla.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3214 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/irlc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1878 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/irra.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1889 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/irrc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3013 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/isbc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/isetc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/isetn.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/isetz.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3410 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/isub.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3422 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/isubc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      341 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/iswpb.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      983 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/isxt.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1278 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/itst.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2145 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/msp430/ixor.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   119817 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_arch_amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      439 2023-02-10 15:44:31.000000 vivisect-1.1.0/envi/tests/test_arch_amd64_emu.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   125660 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/tests/test_arch_arm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18007 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_arch_arm_cmp_flags.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    44966 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_arch_h8.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    32903 2023-01-13 18:44:57.000000 vivisect-1.1.0/envi/tests/test_arch_i386.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10086 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/tests/test_arch_i386_emu.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5915 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_arch_msp430.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1516 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_bits.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      949 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_bytesig.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4708 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/tests/test_cli.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     5065 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_emu_lockstep.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      686 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_envi_config.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      840 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_expression.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1718 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_ieee754.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3368 2023-01-13 00:18:01.000000 vivisect-1.1.0/envi/tests/test_memmap.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     2735 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_memory.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       96 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_radixtree.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1009 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_registers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2603 2022-08-31 06:02:46.000000 vivisect-1.1.0/envi/tests/test_symstore.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5676 2023-01-13 18:44:57.000000 vivisect-1.1.0/envi/threads.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       38 2023-02-24 02:24:51.047929 vivisect-1.1.0/setup.cfg
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1746 2023-02-24 02:07:43.000000 vivisect-1.1.0/setup.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    75087 2023-02-24 02:07:43.000000 vivisect-1.1.0/vdb/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/ext/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/ext/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1119 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/ext/execsc.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/extensions/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2092 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      446 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2153 2023-01-13 00:18:01.000000 vivisect-1.1.0/vdb/extensions/arm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      117 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/darwin.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3669 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/gdbstub.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1799 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/i386.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       36 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/i486.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       36 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/i586.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       36 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/i686.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    36653 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/windows.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    12072 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/extensions/winkern.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/qt/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       65 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/qt/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      924 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/qt/base.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13037 2023-01-13 00:18:01.000000 vivisect-1.1.0/vdb/qt/main.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5442 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/qt/memory.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1299 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/qt/memwrite.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      754 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/qt/registers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      627 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/qt/threads.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/recon/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4371 2023-02-10 15:47:39.000000 vivisect-1.1.0/vdb/recon/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1231 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/recon/dopestack.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2366 2023-02-10 15:47:39.000000 vivisect-1.1.0/vdb/recon/sniper.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      614 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/release.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8426 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/renderers.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/stalker/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6658 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/stalker/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/testmods/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2257 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/testmods/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18341 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/testmods/callingconventions.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7373 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/testmods/hookbptest.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1516 2023-02-10 15:47:39.000000 vivisect-1.1.0/vdb/tests/testrecon.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      557 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/tests/teststalker.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vdb/tools/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/tools/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1084 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/tools/android.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      476 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/tools/androidpy.sh
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2839 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/tools/gendocs.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3639 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/unittest.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     5372 2022-08-31 06:02:46.000000 vivisect-1.1.0/vdb/vdbbin.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/visgraph/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       83 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      769 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/cli.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18970 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/dbcore.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/visgraph/drawing/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       34 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/drawing/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1008 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/drawing/bezier.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      767 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/drawing/catmullrom.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      533 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/exc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    25215 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/graphcore.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/visgraph/layouts/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1509 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/layouts/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    16596 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/layouts/dynadag.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8703 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/layouts/force.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6113 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/pathcore.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/visgraph/renderers/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2108 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/renderers/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5294 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/renderers/gtkrend.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7174 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/renderers/qgraphtree.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2431 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/renderers/qtrend.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2636 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/renderers/svgrend.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/visgraph/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11704 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/tests/test_graphcore.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2480 2022-08-31 06:02:46.000000 vivisect-1.1.0/visgraph/tests/test_layouts.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vivisect/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   113554 2023-02-24 02:07:43.000000 vivisect-1.1.0/vivisect/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vivisect/analysis/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9369 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/analysis/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vivisect/analysis/amd64/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       34 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/amd64/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3858 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/amd64/emulation.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10241 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/amd64/golang.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vivisect/analysis/arm/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/arm/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14887 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/arm/emulation.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      246 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/arm/renaming.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5554 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/arm/thunk_reg.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vivisect/analysis/crypto/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/crypto/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3143 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/crypto/constants.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vivisect/analysis/elf/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1338 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/elf/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    66615 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/analysis/elf/elfplt.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14905 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/analysis/elf/elfplt_late.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3001 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/elf/libc_start_main.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/analysis/generic/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4683 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/codeblocks.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6878 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/analysis/generic/emucode.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      272 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/entrypoints.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1895 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/funcentries.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      805 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/impapi.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2389 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/analysis/generic/linker.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      907 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/mkpointers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1856 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/noret.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3873 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/generic/pointers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1630 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/pointertables.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      543 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/generic/relocations.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1977 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/strconst.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5189 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/generic/switchcase.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    49263 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/generic/symswitchcase.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2618 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/generic/thunks.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/analysis/i386/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      752 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/i386/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5152 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/i386/calling.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6968 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/i386/golang.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      751 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/i386/importcalls.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1686 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/analysis/i386/instrhook.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2241 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/analysis/i386/thunk_reg.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/analysis/ms/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/ms/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      477 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/ms/hotpatch.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1168 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/ms/localhints.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      445 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/ms/msvc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1414 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/ms/msvcfunc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      992 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/ms/vftables.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1306 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/analysis/pe.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    29496 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/base.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    31531 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/cli.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5824 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/codegraph.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1600 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/colormap.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6897 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/const.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3187 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/defconfig.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      666 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/emutils.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2647 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/exc.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/extensions/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1931 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/extensions/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4185 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/extensions/example_gui_extension.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/impapi/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2058 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1673 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/gentool.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/impapi/posix/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/posix/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/posix/amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      298 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/posix/arm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   167388 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/impapi/posix/i386.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/impapi/windows/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/windows/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   110166 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/advapi_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      836 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/advapi_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1851 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      468 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/windows/arm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    78515 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/gdi_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      832 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/gdi_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1840 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/i386.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   128549 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/kernel_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      837 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/kernel_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4612 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr100_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1408 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr100_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4612 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr110_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1408 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr110_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4612 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr120_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1408 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr120_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    83993 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr71_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4626 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr80_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1394 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr80_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4626 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr90_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1394 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcr90_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    80919 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcrt_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1375 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/msvcrt_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   187011 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/ntdll_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1157 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/ntdll_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    46594 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/ole_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      832 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/ole_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    70805 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/rpcrt4_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      836 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/rpcrt4_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1860 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/shell_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      838 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/shell_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    94696 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/user_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      834 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/user_64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    67932 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/ws2plus_32.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      870 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impapi/windows/ws2plus_64.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/impapi/winkern/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/winkern/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      231 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/winkern/amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      229 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/winkern/arm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   213882 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impapi/winkern/i386.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/impemu/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impemu/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    31230 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impemu/emulator.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      977 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impemu/lookup.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7710 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impemu/monitor.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/impemu/platarch/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/impemu/platarch/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2683 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/impemu/platarch/amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14968 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/impemu/platarch/arm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      612 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/impemu/platarch/h8.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2352 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/impemu/platarch/i386.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1013 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/impemu/platarch/linux.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1653 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/impemu/platarch/msp430.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8942 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/impemu/platarch/windows.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/notes/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      605 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/notes/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.023929 vivisect-1.1.0/vivisect/parsers/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2598 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/parsers/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2618 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/parsers/blob.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    41193 2023-02-18 04:09:19.000000 vivisect-1.1.0/vivisect/parsers/elf.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2792 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/parsers/ihex.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6627 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/parsers/macho.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    23790 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/parsers/pe.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2647 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/parsers/srec.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/qt/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/qt/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8512 2023-02-18 04:09:19.000000 vivisect-1.1.0/vivisect/qt/ctxmenu.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    23463 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/qt/default.lyt
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    39588 2023-02-23 16:57:27.000000 vivisect-1.1.0/vivisect/qt/funcgraph.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2617 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/qt/funcviews.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    27701 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/qt/main.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    23578 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/qt/memory.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6559 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/qt/remote.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9515 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/qt/symboliks.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      286 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/qt/tips.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1780 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/qt/ustruct.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11620 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/qt/views.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/remote/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/remote/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      289 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/remote/client.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11384 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/remote/server.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      310 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/remote/share.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/renderers/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8881 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/renderers/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/reports/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      858 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/reports/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      389 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/reports/funccomplexity.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      185 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/reports/locationdist.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      654 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/reports/overlaplocs.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      993 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/reports/undeftargets.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/storage/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      160 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/storage/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1621 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/storage/basicfile.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2140 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/storage/mpfile.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/storage/tools/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/storage/tools/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1283 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/storage/tools/convert.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/symboliks/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    25760 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/symboliks/analysis.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     4932 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/archind.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/symboliks/archs/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/archs/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8245 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/archs/amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    59869 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/archs/i386.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3714 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/callconv.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    30925 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/common.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10340 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/effects.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5174 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/emulator.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5935 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/expression.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1910 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/functions.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11446 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/reducers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4435 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/substitution.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.027929 vivisect-1.1.0/vivisect/symboliks/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6308 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/data_amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1156 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/data_i386.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      245 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/helpers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1088 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_analysis.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5618 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_archind.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1409 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_cache.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1681 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_callingconv.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4682 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_constraints.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    12301 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_effects.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2134 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_emulator.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8435 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_intel.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6012 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_reduce.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1391 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_substitution.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2302 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_translator.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    23017 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/tests/test_walkTree.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2869 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/symboliks/translator.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.031929 vivisect-1.1.0/vivisect/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1992 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/tests/helpers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14035 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/linux_amd64_chown_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   292734 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/linux_amd64_libc_2_27_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)  1848620 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/linux_amd64_libstdc_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14351 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/linux_amd64_ls_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    55128 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/linux_arm_sh_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   291052 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/linux_i386_libc_2_13_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)  2232759 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/linux_i386_libstdc_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      348 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/openbsd_amd64_ls_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    63591 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/qnx_arm_ksh_data.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    55289 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/switchdata.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      253 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/test_helpers.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5564 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/testapihooking.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      660 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testblob.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       91 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testcconvs.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1701 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testcodegraph.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10311 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/testelf.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1378 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testgolang.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      656 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testihex.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      921 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testimpapi.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      790 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/tests/testlinux.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8158 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/testmacho.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2115 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testmalware.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1880 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/tests/testmemory.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    36145 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/testpe.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8900 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/testremote.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2248 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testreports.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      657 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testsrec.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4820 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/teststability.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6185 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/tests/teststorage.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1181 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/teststruct.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7474 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/testswitches.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5803 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/tests/testvampsigs.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5366 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tests/testvivgraph.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    83748 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/tests/testvivisect.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4723 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/tests/testvivisect_multi.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4972 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tests/utils.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.031929 vivisect-1.1.0/vivisect/tools/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tools/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3335 2022-08-31 06:02:46.000000 vivisect-1.1.0/vivisect/tools/fscope.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    30461 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/tools/graphutil.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.031929 vivisect-1.1.0/vivisect/vamp/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2169 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/vamp/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.031929 vivisect-1.1.0/vivisect/vamp/msvc/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8564 2023-02-10 15:47:39.000000 vivisect-1.1.0/vivisect/vamp/msvc/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3005 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/vdbext.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6735 2023-01-13 00:18:01.000000 vivisect-1.1.0/vivisect/vector.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     5968 2023-01-13 18:44:57.000000 vivisect-1.1.0/vivisect/vivbin.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.019929 vivisect-1.1.0/vivisect.egg-info/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2358 2023-02-24 02:24:50.000000 vivisect-1.1.0/vivisect.egg-info/PKG-INFO
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    17747 2023-02-24 02:24:50.000000 vivisect-1.1.0/vivisect.egg-info/SOURCES.txt
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        1 2023-02-24 02:24:50.000000 vivisect-1.1.0/vivisect.egg-info/dependency_links.txt
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       73 2023-02-24 02:24:50.000000 vivisect-1.1.0/vivisect.egg-info/entry_points.txt
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        1 2023-02-24 02:16:52.000000 vivisect-1.1.0/vivisect.egg-info/not-zip-safe
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      213 2023-02-24 02:24:50.000000 vivisect-1.1.0/vivisect.egg-info/requires.txt
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       59 2023-02-24 02:24:50.000000 vivisect-1.1.0/vivisect.egg-info/top_level.txt
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vqt/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7295 2022-09-30 17:04:27.000000 vivisect-1.1.0/vqt/application.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2585 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/basics.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3267 2022-09-30 04:17:35.000000 vivisect-1.1.0/vqt/cli.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3182 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/colors.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10853 2023-01-13 00:18:01.000000 vivisect-1.1.0/vqt/common.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4930 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/hotkeys.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7165 2023-01-13 00:18:01.000000 vivisect-1.1.0/vqt/main.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2649 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/menubuilder.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2541 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/qpython.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      952 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/saveable.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vqt/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      443 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/tests/testmenubuilder.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5518 2022-08-31 06:02:46.000000 vivisect-1.1.0/vqt/tree.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18827 2023-01-13 18:44:57.000000 vivisect-1.1.0/vstruct/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3489 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/bitfield.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7918 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/builder.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/constants/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      930 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/constants/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    46956 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/constants/ntstatus.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5364 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/cparse.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/defs/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      124 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/defs/arm7/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      676 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/arm7/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      647 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/bmp.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/defs/constants/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2023-01-13 00:18:01.000000 vivisect-1.1.0/vstruct/defs/constants/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    27005 2023-02-18 04:09:19.000000 vivisect-1.1.0/vstruct/defs/constants/elf.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18201 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/dns.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    12478 2023-01-13 00:18:01.000000 vivisect-1.1.0/vstruct/defs/elf.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2405 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/gif.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4298 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/ihex.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5135 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/inet.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8130 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/java.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8262 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/kdcom.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/defs/macho/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5292 2023-01-13 18:44:57.000000 vivisect-1.1.0/vstruct/defs/macho/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    17016 2023-01-13 18:44:57.000000 vivisect-1.1.0/vstruct/defs/macho/const.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1314 2023-01-13 00:18:01.000000 vivisect-1.1.0/vstruct/defs/macho/fat.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    25825 2023-01-13 18:44:57.000000 vivisect-1.1.0/vstruct/defs/macho/loader.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4367 2023-01-13 00:18:01.000000 vivisect-1.1.0/vstruct/defs/macho/signing.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      914 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/macho/stabs.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    21050 2023-01-13 18:44:57.000000 vivisect-1.1.0/vstruct/defs/minidump.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    16111 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/pcap.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13821 2023-01-13 00:18:01.000000 vivisect-1.1.0/vstruct/defs/pe.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5628 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/pptp.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13632 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/rar.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4825 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/srec.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    15982 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/swf.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    29393 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/win32.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/defs/windows/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1053 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/defs/windows/win_5_1_i386/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        1 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_5_1_i386/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   114111 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_5_1_i386/ntdll.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   243096 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_5_1_i386/ntoskrnl.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    45928 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_5_1_i386/win32k.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/defs/windows/win_5_2_i386/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_5_2_i386/__init__.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   127514 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_5_2_i386/ntdll.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   255521 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_5_2_i386/ntoskrnl.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)    49833 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_5_2_i386/win32k.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.035929 vivisect-1.1.0/vstruct/defs/windows/win_6_1_amd64/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_amd64/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   184479 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_amd64/ntdll.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   423580 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_amd64/ntoskrnl.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   210698 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_amd64/win32k.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/defs/windows/win_6_1_i386/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_i386/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   174841 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_i386/ntdll.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   397457 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_i386/ntoskrnl.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   192789 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_i386/win32k.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/defs/windows/win_6_1_wow64/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        1 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_wow64/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   171447 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_1_wow64/ntdll.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/defs/windows/win_6_2_amd64/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_amd64/__init__.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   226332 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_amd64/ntdll.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   482447 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_amd64/ntoskrnl.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)       87 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_amd64/win32k.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/defs/windows/win_6_2_i386/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_i386/__init__.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   219099 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_i386/ntdll.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   455279 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_i386/ntoskrnl.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)       86 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_i386/win32k.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/defs/windows/win_6_2_wow64/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_wow64/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   219477 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_2_wow64/ntdll.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/defs/windows/win_6_3_amd64/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_3_amd64/__init__.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   241468 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_3_amd64/ntdll.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   511772 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_3_amd64/ntoskrnl.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/defs/windows/win_6_3_i386/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_3_i386/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   239322 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_3_i386/ntdll.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   482996 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_3_i386/ntoskrnl.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/defs/windows/win_6_3_wow64/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_3_wow64/__init__.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   239285 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/defs/windows/win_6_3_wow64/ntdll.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    24509 2023-01-13 18:44:57.000000 vivisect-1.1.0/vstruct/primitives.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/qt/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5527 2023-01-13 18:44:57.000000 vivisect-1.1.0/vstruct/qt/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1703 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/tests/test_builder.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10604 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/tests/testbasic.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4397 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/tests/tests_vstruct.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vstruct/tools/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/tools/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1663 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/tools/dumpihex.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1392 2022-08-31 06:02:46.000000 vivisect-1.1.0/vstruct/tools/dumpjava.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.039929 vivisect-1.1.0/vtrace/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    51410 2023-01-13 18:44:57.000000 vivisect-1.1.0/vtrace/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.043929 vivisect-1.1.0/vtrace/archs/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      101 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/archs/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1068 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/archs/amd64.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      339 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/archs/arm.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5984 2023-01-13 17:46:49.000000 vivisect-1.1.0/vtrace/archs/i386.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      676 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/archs/ppc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      935 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/audit.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    15294 2023-01-13 18:44:57.000000 vivisect-1.1.0/vtrace/breakpoints.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1525 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/const.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5401 2023-01-13 00:18:01.000000 vivisect-1.1.0/vtrace/envitools.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      235 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/exc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5355 2023-01-13 18:44:57.000000 vivisect-1.1.0/vtrace/notifiers.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.043929 vivisect-1.1.0/vtrace/platforms/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      374 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    31351 2023-01-13 18:44:57.000000 vivisect-1.1.0/vtrace/platforms/base.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.043929 vivisect-1.1.0/vtrace/platforms/darwin/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      355 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/darwin/Makefile
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    36886 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/darwin/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6411 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/darwin/exc.h
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    97707 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/darwin/excServer.c
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    52461 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/darwin/excUser.c
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11216 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/darwin/machhelper.c
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)    43272 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/darwin/machhelper.dylib
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    22968 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/freebsd.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    27978 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/gdbstub.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    33791 2023-01-13 18:44:57.000000 vivisect-1.1.0/vtrace/platforms/linux.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8204 2023-01-13 18:44:57.000000 vivisect-1.1.0/vtrace/platforms/posix.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6681 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/solaris.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4023 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/vmware.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    77712 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/win32.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.043929 vivisect-1.1.0/vtrace/platforms/windll/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/__init__.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.043929 vivisect-1.1.0/vtrace/platforms/windll/amd64/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/amd64/__init__.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)  1532048 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/amd64/dbghelp.dll
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   142992 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/amd64/symsrv.dll
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/amd64/symsrv.yes
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.043929 vivisect-1.1.0/vtrace/platforms/windll/i386/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/i386/__init__.py
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)  1231000 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/i386/dbghelp.dll
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   128152 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/i386/symsrv.dll
--rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/windll/i386/symsrv.yes
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10623 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/platforms/winkern.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    17613 2023-01-13 17:46:49.000000 vivisect-1.1.0/vtrace/qt.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3354 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/rmi.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6454 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/snapshot.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.043929 vivisect-1.1.0/vtrace/tests/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2879 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tests/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      330 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tests/mainwritemem.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      851 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tests/test_expressions.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      817 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tests/test_symcache.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2095 2023-01-13 18:44:57.000000 vivisect-1.1.0/vtrace/tests/testbasic.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      611 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tests/tests_breakpoints.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      392 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tests/tests_envitools.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      825 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tests/testthread.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      712 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tests/testwritemem.py
-drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-02-24 02:24:51.043929 vivisect-1.1.0/vtrace/tools/
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tools/__init__.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2505 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tools/iathook.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1580 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tools/win32alloc.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      797 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tools/win32aslr.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14396 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tools/win32heap.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8575 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/tools/win32stealth.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2696 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/util.py
--rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3019 2022-08-31 06:02:46.000000 vivisect-1.1.0/vtrace/watchpoints.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.658484 vivisect-1.1.1/
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.614484 vivisect-1.1.1/Elf/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    35539 2023-04-03 13:57:39.000000 vivisect-1.1.1/Elf/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       41 2023-03-27 05:03:15.000000 vivisect-1.1.1/Elf/elf_lookup.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11357 2022-08-31 06:02:46.000000 vivisect-1.1.1/LICENSE.txt
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.614484 vivisect-1.1.1/PE/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    54083 2023-03-27 05:02:59.000000 vivisect-1.1.1/PE/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2611 2023-01-13 00:18:01.000000 vivisect-1.1.1/PE/carve.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6170 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/cofflib.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.614484 vivisect-1.1.1/PE/ordlookup/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      840 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/ordlookup/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3028 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/ordlookup/comctl32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   380351 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/ordlookup/mfc42.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    16265 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/ordlookup/msvbvm60.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10081 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/ordlookup/oleaut32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      647 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/ordlookup/oledlg.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3032 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/ordlookup/ws2_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1362 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/petool.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.614484 vivisect-1.1.1/PE/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      167 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/tests/test_version.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.614484 vivisect-1.1.1/PE/tools/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/tools/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      703 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/tools/printord.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1377 2022-08-31 06:02:46.000000 vivisect-1.1.1/PE/tools/structdump.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2358 2023-04-07 20:03:21.658484 vivisect-1.1.1/PKG-INFO
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1593 2023-03-27 05:02:59.000000 vivisect-1.1.1/README.md
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/cobra/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    37095 2023-04-03 13:57:39.000000 vivisect-1.1.1/cobra/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/cobra/auth/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      878 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/auth/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1925 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/auth/shadowfile.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1815 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/cache.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    19217 2023-04-03 13:57:39.000000 vivisect-1.1.1/cobra/cluster.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3388 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/dcode.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8049 2023-04-03 13:57:39.000000 vivisect-1.1.1/cobra/devent.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2014 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/dispatcher.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/cobra/hostid/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      341 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/hostid/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1908 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/hostid/darwinhostid.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      278 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/hostid/windowshostid.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    19575 2023-04-03 13:57:39.000000 vivisect-1.1.1/cobra/http.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2189 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/pool.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2163 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/remoteapp.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/cobra/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      533 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3297 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tests/testbasic.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1048 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tests/testcache.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1195 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tests/testdcode.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      647 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tests/testevents.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      631 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tests/testnewobj.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/cobra/tools/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tools/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2492 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tools/burnapp.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      509 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tools/queend.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      415 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tools/runtests.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      424 2022-08-31 06:02:46.000000 vivisect-1.1.1/cobra/tools/workerd.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/envi/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    49635 2023-04-03 13:57:39.000000 vivisect-1.1.1/envi/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/envi/archs/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      714 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/envi/archs/amd64/
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     5886 2023-04-03 13:57:39.000000 vivisect-1.1.1/envi/archs/amd64/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    30851 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/amd64/disasm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   206683 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/amd64/opcode64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5478 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/amd64/regs.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4731 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/amd64/vmcslookup.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/envi/archs/arm/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4691 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/arm/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    21305 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/arm/const.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   178363 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/arm/disasm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    74062 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/arm/emu.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7887 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/arm/regs.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/envi/archs/h8/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5519 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/h8/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      259 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/h8/const.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1859 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/h8/disasm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    36055 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/h8/emu.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    15621 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/h8/operands.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    43111 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/h8/parsers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2955 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/h8/regs.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.618484 vivisect-1.1.1/envi/archs/i386/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1181 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/i386/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    42485 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/i386/disasm.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)    80324 2023-04-03 13:57:39.000000 vivisect-1.1.1/envi/archs/i386/emu.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   187007 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/i386/opcode86.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11659 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/i386/opconst.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4447 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/i386/regs.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.622484 vivisect-1.1.1/envi/archs/msp430/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1150 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/msp430/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4591 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/msp430/const.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    30649 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/msp430/disasm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    15639 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/msp430/emu.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1313 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/msp430/regs.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.622484 vivisect-1.1.1/envi/archs/thumb16/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      175 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/thumb16/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    91529 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/archs/thumb16/disasm.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.622484 vivisect-1.1.1/envi/archs/z80/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       33 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/z80/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      401 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/z80/const.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2831 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/z80/disasm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      820 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/z80/regs.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    53810 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/archs/z80/z80opcode.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1448 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/bintree.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     9057 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/bits.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5390 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/bytesig.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    29791 2023-04-03 13:57:39.000000 vivisect-1.1.1/envi/cli.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11988 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/codeflow.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1027 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/common.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9385 2023-04-07 04:17:00.000000 vivisect-1.1.1/envi/config.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1032 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/const.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      608 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/encoding.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6765 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/exc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4068 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/expression.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2749 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/ieee754.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2491 2023-04-07 04:17:00.000000 vivisect-1.1.1/envi/interactive.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.622484 vivisect-1.1.1/envi/memcanvas/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    12090 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/memcanvas/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.622484 vivisect-1.1.1/envi/memcanvas/renderers/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4539 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/memcanvas/renderers/__init__.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)    26522 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/memory.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2363 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/pagelookup.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      813 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/pyzip.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.622484 vivisect-1.1.1/envi/qt/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       52 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/qt/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2807 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/qt/config.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5201 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/qt/html.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   245078 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/qt/jquery.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10983 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/qt/memcanvas.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1932 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/qt/memdump.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10569 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/qt/memory.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3954 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/qt/memorymap.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4981 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/qt/memsearch.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8865 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/qt/memwrite.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2027 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/radixtree.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13650 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/registers.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.622484 vivisect-1.1.1/envi/symstore/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      112 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/symstore/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13966 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/symstore/resolver.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3452 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/symstore/symcache.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.622484 vivisect-1.1.1/envi/tests/
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)      426 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10446 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/arm_bit_test_adds.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9971 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/arm_bit_test_cmn.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10223 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/arm_bit_test_cmp.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10656 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/arm_bit_test_subs.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   341046 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/armthumb_tests.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/envi/tests/msp430/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3321 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iadc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3063 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iadd.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3722 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iaddc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1434 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iand.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2060 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/ibic.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2118 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/ibis.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1434 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/ibit.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      332 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/ibr.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      386 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/icall.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1236 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iclr.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iclrc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iclrn.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iclrz.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3550 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/icmp.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3027 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/idadc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2732 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/idadd.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2435 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/idec.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3088 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/idecd.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2178 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iinc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3123 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iincd.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1246 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iinv.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5325 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/ijumps.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9646 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/imov.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      302 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/inop.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      698 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/ipop.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      758 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/ipush.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      368 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iret.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2576 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/irla.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3214 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/irlc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1878 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/irra.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1889 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/irrc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3013 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/isbc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/isetc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/isetn.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/isetz.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3410 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/isub.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3422 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/isubc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      341 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/iswpb.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      983 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/isxt.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1278 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/itst.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2145 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/msp430/ixor.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   119817 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_arch_amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      745 2023-04-03 13:57:39.000000 vivisect-1.1.1/envi/tests/test_arch_amd64_emu.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   125660 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/tests/test_arch_arm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18007 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_arch_arm_cmp_flags.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    44966 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_arch_h8.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    32903 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/tests/test_arch_i386.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10217 2023-04-03 13:57:39.000000 vivisect-1.1.1/envi/tests/test_arch_i386_emu.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5915 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_arch_msp430.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1516 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_bits.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      949 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_bytesig.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4708 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/tests/test_cli.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     5065 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_emu_lockstep.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1271 2023-04-07 04:17:00.000000 vivisect-1.1.1/envi/tests/test_envi_config.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      840 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_expression.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1718 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_ieee754.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3368 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/tests/test_memmap.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     2735 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_memory.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       96 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_radixtree.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1009 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_registers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2603 2022-08-31 06:02:46.000000 vivisect-1.1.1/envi/tests/test_symstore.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5676 2023-03-27 05:02:59.000000 vivisect-1.1.1/envi/threads.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       38 2023-04-07 20:03:21.658484 vivisect-1.1.1/setup.cfg
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1746 2023-04-07 20:03:05.000000 vivisect-1.1.1/setup.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    75521 2023-04-07 20:03:05.000000 vivisect-1.1.1/vdb/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/ext/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/ext/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1119 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/ext/execsc.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/extensions/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2092 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      446 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2153 2023-03-27 05:02:59.000000 vivisect-1.1.1/vdb/extensions/arm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      117 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/darwin.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3669 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/gdbstub.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1799 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/i386.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       36 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/i486.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       36 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/i586.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       36 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/i686.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    36653 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/windows.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    12072 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/extensions/winkern.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/qt/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       65 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/qt/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      924 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/qt/base.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13037 2023-03-27 05:02:59.000000 vivisect-1.1.1/vdb/qt/main.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5442 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/qt/memory.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1299 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/qt/memwrite.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      754 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/qt/registers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      627 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/qt/threads.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/recon/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4371 2023-03-27 05:02:59.000000 vivisect-1.1.1/vdb/recon/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1231 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/recon/dopestack.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2366 2023-03-27 05:02:59.000000 vivisect-1.1.1/vdb/recon/sniper.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      614 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/release.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8426 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/renderers.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/stalker/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6658 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/stalker/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/testmods/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2257 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/testmods/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18341 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/testmods/callingconventions.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7373 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/testmods/hookbptest.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1516 2023-03-27 05:02:59.000000 vivisect-1.1.1/vdb/tests/testrecon.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      557 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/tests/teststalker.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/vdb/tools/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/tools/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1084 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/tools/android.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      476 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/tools/androidpy.sh
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2839 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/tools/gendocs.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3639 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/unittest.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     5372 2022-08-31 06:02:46.000000 vivisect-1.1.1/vdb/vdbbin.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/visgraph/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       83 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      769 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/cli.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18970 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/dbcore.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/visgraph/drawing/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       34 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/drawing/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1008 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/drawing/bezier.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      767 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/drawing/catmullrom.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      533 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/exc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    25215 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/graphcore.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/visgraph/layouts/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1509 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/layouts/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    16596 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/layouts/dynadag.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8703 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/layouts/force.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6113 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/pathcore.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.626484 vivisect-1.1.1/visgraph/renderers/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2108 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/renderers/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5294 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/renderers/gtkrend.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7174 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/renderers/qgraphtree.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2431 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/renderers/qtrend.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2636 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/renderers/svgrend.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/visgraph/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11704 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/tests/test_graphcore.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2480 2022-08-31 06:02:46.000000 vivisect-1.1.1/visgraph/tests/test_layouts.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   113662 2023-04-07 20:03:05.000000 vivisect-1.1.1/vivisect/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/analysis/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9369 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/analysis/amd64/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       34 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/amd64/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3858 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/amd64/emulation.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10241 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/amd64/golang.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/analysis/arm/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/arm/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14887 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/arm/emulation.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      246 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/arm/renaming.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5554 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/arm/thunk_reg.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/analysis/crypto/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/crypto/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3143 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/crypto/constants.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/analysis/elf/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1338 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/elf/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    66615 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/elf/elfplt.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14905 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/elf/elfplt_late.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3001 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/elf/libc_start_main.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/analysis/generic/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4683 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/codeblocks.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6878 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/generic/emucode.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      272 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/entrypoints.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1895 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/funcentries.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      805 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/impapi.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2389 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/generic/linker.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      907 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/mkpointers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1856 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/noret.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3873 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/generic/pointers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1630 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/pointertables.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      543 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/generic/relocations.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1977 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/strconst.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5189 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/generic/switchcase.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    49263 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/generic/symswitchcase.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2618 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/generic/thunks.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/analysis/i386/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      752 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/i386/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5152 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/i386/calling.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6968 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/i386/golang.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      751 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/i386/importcalls.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1686 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/i386/instrhook.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2241 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/analysis/i386/thunk_reg.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/analysis/ms/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/ms/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      477 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/ms/hotpatch.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1168 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/ms/localhints.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      445 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/ms/msvc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1414 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/ms/msvcfunc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      992 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/ms/vftables.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1306 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/analysis/pe.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    29496 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/base.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    31531 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/cli.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5824 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/codegraph.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1600 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/colormap.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6897 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/const.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3187 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/defconfig.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      666 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/emutils.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2647 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/exc.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/extensions/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1931 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/extensions/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4185 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/extensions/example_gui_extension.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/impapi/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2058 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1673 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/gentool.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect/impapi/posix/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/posix/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      304 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/posix/amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      298 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/posix/arm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   167388 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/posix/i386.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.634484 vivisect-1.1.1/vivisect/impapi/windows/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/windows/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   110166 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/advapi_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      836 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/advapi_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1851 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      468 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/windows/arm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    78515 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/gdi_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      832 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/gdi_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1840 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/i386.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   128549 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/kernel_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      837 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/kernel_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4612 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr100_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1408 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr100_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4612 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr110_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1408 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr110_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4612 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr120_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1408 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr120_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    83993 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr71_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4626 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr80_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1394 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr80_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4626 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr90_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1394 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcr90_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    80919 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcrt_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1375 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/msvcrt_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   187011 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/ntdll_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1157 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/ntdll_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    46594 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/ole_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      832 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/ole_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    70805 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/rpcrt4_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      836 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/rpcrt4_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1860 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/shell_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      838 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/shell_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    94696 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/user_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      834 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/user_64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    67932 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/ws2plus_32.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      870 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impapi/windows/ws2plus_64.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.634484 vivisect-1.1.1/vivisect/impapi/winkern/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/winkern/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      231 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/winkern/amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      229 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/winkern/arm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   213882 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impapi/winkern/i386.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.634484 vivisect-1.1.1/vivisect/impemu/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impemu/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    31230 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/emulator.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      977 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/lookup.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7710 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impemu/monitor.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.634484 vivisect-1.1.1/vivisect/impemu/platarch/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/impemu/platarch/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2683 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/platarch/amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14968 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/platarch/arm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      612 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/platarch/h8.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2352 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/platarch/i386.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1013 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/platarch/linux.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1653 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/platarch/msp430.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8942 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/impemu/platarch/windows.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.634484 vivisect-1.1.1/vivisect/notes/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      605 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/notes/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.634484 vivisect-1.1.1/vivisect/parsers/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2598 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/parsers/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2618 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/parsers/blob.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    41193 2023-03-29 03:35:23.000000 vivisect-1.1.1/vivisect/parsers/elf.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2792 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/parsers/ihex.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6627 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/parsers/macho.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    23788 2023-04-07 04:17:00.000000 vivisect-1.1.1/vivisect/parsers/pe.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2647 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/parsers/srec.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/qt/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/qt/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8512 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/qt/ctxmenu.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    23463 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/qt/default.lyt
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    39592 2023-04-03 13:57:39.000000 vivisect-1.1.1/vivisect/qt/funcgraph.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2617 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/qt/funcviews.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    27701 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/qt/main.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    24102 2023-04-03 13:57:39.000000 vivisect-1.1.1/vivisect/qt/memory.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6559 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/qt/remote.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9515 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/qt/symboliks.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      286 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/qt/tips.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1780 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/qt/ustruct.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11620 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/qt/views.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/remote/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/remote/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      289 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/remote/client.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11384 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/remote/server.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      310 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/remote/share.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/renderers/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8881 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/renderers/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/reports/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      858 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/reports/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      389 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/reports/funccomplexity.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      185 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/reports/locationdist.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      654 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/reports/overlaplocs.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      993 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/reports/undeftargets.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/storage/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      160 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/storage/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1621 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/storage/basicfile.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2140 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/storage/mpfile.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/storage/tools/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/storage/tools/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1283 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/storage/tools/convert.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/symboliks/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    25760 2023-04-07 04:16:58.000000 vivisect-1.1.1/vivisect/symboliks/analysis.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     4932 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/archind.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/symboliks/archs/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/archs/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8245 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/archs/amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    59869 2023-04-07 04:16:58.000000 vivisect-1.1.1/vivisect/symboliks/archs/i386.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3714 2023-04-07 04:16:58.000000 vivisect-1.1.1/vivisect/symboliks/callconv.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    30925 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/common.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10340 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/effects.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5174 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/emulator.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5935 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/expression.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1910 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/functions.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11446 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/reducers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4435 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/substitution.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.638484 vivisect-1.1.1/vivisect/symboliks/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6308 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/data_amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1156 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/data_i386.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      245 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/helpers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1088 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_analysis.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5618 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_archind.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1409 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_cache.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1681 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_callingconv.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4682 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_constraints.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    12301 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_effects.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2134 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_emulator.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8435 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_intel.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6012 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_reduce.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1391 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_substitution.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2302 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_translator.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    23017 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/tests/test_walkTree.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2869 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/symboliks/translator.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.642484 vivisect-1.1.1/vivisect/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1992 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/helpers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14035 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/linux_amd64_chown_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   292734 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/linux_amd64_libc_2_27_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)  1848620 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/linux_amd64_libstdc_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14351 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/linux_amd64_ls_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    55128 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/linux_arm_sh_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   291052 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/linux_i386_libc_2_13_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)  2232759 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/linux_i386_libstdc_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      348 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/openbsd_amd64_ls_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    63591 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/qnx_arm_ksh_data.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    55289 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/switchdata.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      253 2023-03-29 03:35:23.000000 vivisect-1.1.1/vivisect/tests/test_helpers.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5564 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testapihooking.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      660 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testblob.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       91 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testcconvs.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1701 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testcodegraph.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10311 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testelf.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1378 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testgolang.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      656 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testihex.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      921 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testimpapi.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      790 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testlinux.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8158 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testmacho.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2115 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testmalware.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1880 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testmemory.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    36145 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testpe.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     9010 2023-04-03 13:57:39.000000 vivisect-1.1.1/vivisect/tests/testremote.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2248 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testreports.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      657 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testsrec.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4820 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/teststability.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6185 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/teststorage.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1181 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/teststruct.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7474 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testswitches.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5803 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testvampsigs.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5366 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tests/testvivgraph.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    83748 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testvivisect.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4723 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/testvivisect_multi.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4972 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tests/utils.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.642484 vivisect-1.1.1/vivisect/tools/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tools/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3335 2022-08-31 06:02:46.000000 vivisect-1.1.1/vivisect/tools/fscope.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    30461 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/tools/graphutil.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.642484 vivisect-1.1.1/vivisect/vamp/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2169 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/vamp/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.642484 vivisect-1.1.1/vivisect/vamp/msvc/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8564 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/vamp/msvc/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3005 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/vdbext.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6735 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/vector.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)     5968 2023-03-27 05:02:59.000000 vivisect-1.1.1/vivisect/vivbin.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.630484 vivisect-1.1.1/vivisect.egg-info/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2358 2023-04-07 20:03:21.000000 vivisect-1.1.1/vivisect.egg-info/PKG-INFO
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    17747 2023-04-07 20:03:21.000000 vivisect-1.1.1/vivisect.egg-info/SOURCES.txt
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        1 2023-04-07 20:03:21.000000 vivisect-1.1.1/vivisect.egg-info/dependency_links.txt
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       73 2023-04-07 20:03:21.000000 vivisect-1.1.1/vivisect.egg-info/entry_points.txt
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        1 2023-04-07 20:03:21.000000 vivisect-1.1.1/vivisect.egg-info/not-zip-safe
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      213 2023-04-07 20:03:21.000000 vivisect-1.1.1/vivisect.egg-info/requires.txt
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)       59 2023-04-07 20:03:21.000000 vivisect-1.1.1/vivisect.egg-info/top_level.txt
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vqt/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vqt/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7295 2022-09-30 17:04:27.000000 vivisect-1.1.1/vqt/application.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2585 2022-08-31 06:02:46.000000 vivisect-1.1.1/vqt/basics.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3267 2022-09-30 04:17:35.000000 vivisect-1.1.1/vqt/cli.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3182 2022-08-31 06:02:46.000000 vivisect-1.1.1/vqt/colors.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10853 2023-03-27 05:02:59.000000 vivisect-1.1.1/vqt/common.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5131 2023-04-03 13:57:39.000000 vivisect-1.1.1/vqt/hotkeys.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7171 2023-04-03 13:57:39.000000 vivisect-1.1.1/vqt/main.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2649 2022-08-31 06:02:46.000000 vivisect-1.1.1/vqt/menubuilder.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2524 2023-04-03 13:57:39.000000 vivisect-1.1.1/vqt/qpython.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      952 2022-08-31 06:02:46.000000 vivisect-1.1.1/vqt/saveable.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vqt/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vqt/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      443 2022-08-31 06:02:46.000000 vivisect-1.1.1/vqt/tests/testmenubuilder.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5518 2022-08-31 06:02:46.000000 vivisect-1.1.1/vqt/tree.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18827 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3489 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/bitfield.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     7918 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/builder.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/constants/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      930 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/constants/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    46956 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/constants/ntstatus.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5364 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/cparse.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/defs/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      124 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/defs/arm7/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      676 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/arm7/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      647 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/bmp.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/defs/constants/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/constants/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    27005 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/constants/elf.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    18201 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/dns.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    12478 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/elf.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2405 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/gif.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4298 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/ihex.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5135 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/inet.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8130 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/java.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8262 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/kdcom.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/defs/macho/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5292 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/macho/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    17016 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/macho/const.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1314 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/macho/fat.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    25825 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/macho/loader.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4367 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/macho/signing.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      914 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/macho/stabs.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    21050 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/minidump.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    16111 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/pcap.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13821 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/defs/pe.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5628 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/pptp.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    13632 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/rar.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4825 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/srec.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    15982 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/swf.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    29393 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/win32.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/defs/windows/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1053 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/defs/windows/win_5_1_i386/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        1 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_5_1_i386/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   114111 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_5_1_i386/ntdll.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   243096 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_5_1_i386/ntoskrnl.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    45928 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_5_1_i386/win32k.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/defs/windows/win_5_2_i386/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_5_2_i386/__init__.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   127514 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_5_2_i386/ntdll.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   255521 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_5_2_i386/ntoskrnl.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)    49833 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_5_2_i386/win32k.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.646484 vivisect-1.1.1/vstruct/defs/windows/win_6_1_amd64/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_amd64/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   184479 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_amd64/ntdll.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   423580 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_amd64/ntoskrnl.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   210698 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_amd64/win32k.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.650484 vivisect-1.1.1/vstruct/defs/windows/win_6_1_i386/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_i386/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   174841 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_i386/ntdll.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   397457 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_i386/ntoskrnl.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   192789 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_i386/win32k.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.650484 vivisect-1.1.1/vstruct/defs/windows/win_6_1_wow64/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        1 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_wow64/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   171447 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_1_wow64/ntdll.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.650484 vivisect-1.1.1/vstruct/defs/windows/win_6_2_amd64/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_amd64/__init__.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   226332 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_amd64/ntdll.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   482447 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_amd64/ntoskrnl.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)       87 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_amd64/win32k.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.650484 vivisect-1.1.1/vstruct/defs/windows/win_6_2_i386/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_i386/__init__.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   219099 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_i386/ntdll.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   455279 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_i386/ntoskrnl.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)       86 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_i386/win32k.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.650484 vivisect-1.1.1/vstruct/defs/windows/win_6_2_wow64/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_wow64/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   219477 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_2_wow64/ntdll.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.650484 vivisect-1.1.1/vstruct/defs/windows/win_6_3_amd64/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_3_amd64/__init__.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   241468 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_3_amd64/ntdll.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   511772 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_3_amd64/ntoskrnl.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vstruct/defs/windows/win_6_3_i386/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_3_i386/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)   239322 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_3_i386/ntdll.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   482996 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_3_i386/ntoskrnl.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vstruct/defs/windows/win_6_3_wow64/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_3_wow64/__init__.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   239285 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/defs/windows/win_6_3_wow64/ntdll.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    24509 2023-03-29 03:35:23.000000 vivisect-1.1.1/vstruct/primitives.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vstruct/qt/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5527 2023-03-27 05:02:59.000000 vivisect-1.1.1/vstruct/qt/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vstruct/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1703 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/tests/test_builder.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10604 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/tests/testbasic.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4395 2023-04-03 13:57:39.000000 vivisect-1.1.1/vstruct/tests/tests_vstruct.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vstruct/tools/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/tools/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1663 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/tools/dumpihex.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1392 2022-08-31 06:02:46.000000 vivisect-1.1.1/vstruct/tools/dumpjava.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vtrace/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    51410 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vtrace/archs/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      101 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/archs/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1068 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/archs/amd64.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      339 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/archs/arm.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5984 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/archs/i386.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      676 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/archs/ppc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      935 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/audit.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    15294 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/breakpoints.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1525 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/const.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5401 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/envitools.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      235 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/exc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     5355 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/notifiers.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vtrace/platforms/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      374 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    31351 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/platforms/base.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vtrace/platforms/darwin/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      355 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/darwin/Makefile
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    36886 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/darwin/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6411 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/darwin/exc.h
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    97707 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/darwin/excServer.c
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    52461 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/darwin/excUser.c
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    11216 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/darwin/machhelper.c
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)    43272 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/darwin/machhelper.dylib
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    22968 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/freebsd.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    27978 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/gdbstub.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    33791 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/platforms/linux.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8204 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/platforms/posix.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6681 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/solaris.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     4023 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/vmware.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    77712 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/win32.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.654484 vivisect-1.1.1/vtrace/platforms/windll/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/__init__.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.658484 vivisect-1.1.1/vtrace/platforms/windll/amd64/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/amd64/__init__.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)  1532048 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/amd64/dbghelp.dll
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   142992 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/amd64/symsrv.dll
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/amd64/symsrv.yes
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.658484 vivisect-1.1.1/vtrace/platforms/windll/i386/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/i386/__init__.py
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)  1231000 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/i386/dbghelp.dll
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)   128152 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/i386/symsrv.dll
+-rwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/windll/i386/symsrv.yes
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    10623 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/platforms/winkern.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    17613 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/qt.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3354 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/rmi.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     6454 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/snapshot.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.658484 vivisect-1.1.1/vtrace/tests/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2879 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tests/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      330 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tests/mainwritemem.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      851 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tests/test_expressions.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      817 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tests/test_symcache.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2095 2023-03-27 05:02:59.000000 vivisect-1.1.1/vtrace/tests/testbasic.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      611 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tests/tests_breakpoints.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      392 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tests/tests_envitools.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      825 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tests/testthread.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      712 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tests/testwritemem.py
+drwxrwxr-x   0 rakuyo    (1000) rakuyo    (1000)        0 2023-04-07 20:03:21.658484 vivisect-1.1.1/vtrace/tools/
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)        0 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tools/__init__.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2505 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tools/iathook.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     1580 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tools/win32alloc.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)      797 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tools/win32aslr.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)    14396 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tools/win32heap.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     8575 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/tools/win32stealth.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     2696 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/util.py
+-rw-rw-r--   0 rakuyo    (1000) rakuyo    (1000)     3019 2022-08-31 06:02:46.000000 vivisect-1.1.1/vtrace/watchpoints.py
```

### Comparing `vivisect-1.1.0/Elf/__init__.py` & `vivisect-1.1.1/Elf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,39 +97,80 @@
         self.symbols_by_name = {}
         self.symbols_by_addr = {}
         self.dynamics = []      # deprecated - 2019-10-21
         self.dynamic_symbols = []
         self.dynstrtabmeta = (None, None)
         self.dynstrtab = []
         self.dynsymtabct = None     # populated by _parseDynStrs()
-        logger.info('self._parsePheaders')
-        self._parsePheaders()
-        logger.info('self._parseDynLinkInfo')
-        self._parseDynLinkInfo()
-
-        logger.info('self._parseSections')
-        self._parseSections()
-        logger.info('self._parseDynamicsFromSections')
-        self._parseDynamicsFromSections()
+
+        try:
+            logger.info('self._parsePheaders')
+            self._parsePheaders()
+        except Exception as e:
+            logger.warning("Exception parsing Program Headers: %r" % e, exc_info=1)
+
+        try:
+            logger.info('self._parseDynLinkInfo')
+            self._parseDynLinkInfo()
+        except Exception as e:
+            logger.warning("Exception parsing Program Headers: %r" % e, exc_info=1)
+
+
+        try:
+            logger.info('self._parseSections')
+            self._parseSections()
+        except Exception as e:
+            logger.warning("Exception parsing Sections: %r" % e, exc_info=1)
+
+        try:
+            logger.info('self._parseDynamicsFromSections')
+            self._parseDynamicsFromSections()
+        except Exception as e:
+            logger.warning("Exception parsing Dynamics from Sections: %r" % e, exc_info=1)
+
 
         # load symbols and relocs from DYNAMICS
-        logger.info('self._parseDynStrs')
-        self._parseDynStrs()
-        logger.info('self._parseDynSyms')
-        self._parseDynSyms()
-        logger.info('self._parseDynRelocs')
-        self._parseDynRelocs()
+        try:
+            logger.info('self._parseDynStrs')
+            self._parseDynStrs()
+        except Exception as e:
+            logger.warning("Exception parsing String Table (via dynamics): %r" % e, exc_info=1)
+
+        try:
+            logger.info('self._parseDynSyms')
+            self._parseDynSyms()
+        except Exception as e:
+            logger.warning("Exception parsing Symbols (via dynamics): %r" % e, exc_info=1)
+
+        try:
+            logger.info('self._parseDynRelocs')
+            self._parseDynRelocs()
+        except Exception as e:
+            logger.warning("Exception parsing Relocations (via dynamics): %r" % e, exc_info=1)
+
 
         # load symbols and relocs from SECTIONS
-        logger.info('self._parseDynSymsFromSections')
-        self._parseDynSymsFromSections()
-        logger.info('self._parseSectionSymbols')
-        self._parseSectionSymbols()
-        logger.info('self._parseSectionRelocs')
-        self._parseSectionRelocs()
+        try:
+            logger.info('self._parseDynSymsFromSections')
+            self._parseDynSymsFromSections()
+        except Exception as e:
+            logger.warning("Exception parsing Dynamic Symbols (via Sections): %r" % e, exc_info=1)
+
+        try:
+            logger.info('self._parseSectionSymbols')
+            self._parseSectionSymbols()
+        except Exception as e:
+            logger.warning("Exception parsing Symbols (via Sections): %r" % e, exc_info=1)
+
+        try:
+            logger.info('self._parseSectionRelocs')
+            self._parseSectionRelocs()
+        except Exception as e:
+            logger.warning("Exception parsing Relocations (via Sections): %r" % e, exc_info=1)
+
         logger.info('done parsing ELF')
 
     def __del__(self):
         try:
             self.fd.close()
         except:
             pass  # whatever. we're tearing down anyway
@@ -182,14 +223,18 @@
             slen = self.e_shentsize
             if len(sec) != slen:
                 raise Exception('Invalid Section Header Size: %d' % slen)
 
             secbytes = self.readAtOffset(sbase, self.e_shnum * slen)
 
             secs = sec * self.e_shnum
+            secslen = slen * self.e_shnum
+            if secslen != len(secbytes):
+                logger.warning('Invalid Section-Headers Size: should be: %d   retrieved: %d', secslen, len(secbytes))
+
             vstruct.VArray(elems=secs).vsParse(secbytes, fast=True)
 
             self.sections.extend(secs)
 
             # Populate the section names
             strsec = self.sections[self.e_shstrndx]
             names = self.readAtOffset(strsec.sh_offset, strsec.sh_size)
```

### Comparing `vivisect-1.1.0/LICENSE.txt` & `vivisect-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/__init__.py` & `vivisect-1.1.1/PE/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/carve.py` & `vivisect-1.1.1/PE/carve.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/cofflib.py` & `vivisect-1.1.1/PE/cofflib.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/ordlookup/__init__.py` & `vivisect-1.1.1/PE/ordlookup/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/ordlookup/comctl32.py` & `vivisect-1.1.1/PE/ordlookup/comctl32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/ordlookup/mfc42.py` & `vivisect-1.1.1/PE/ordlookup/mfc42.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/ordlookup/msvbvm60.py` & `vivisect-1.1.1/PE/ordlookup/msvbvm60.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/ordlookup/oleaut32.py` & `vivisect-1.1.1/PE/ordlookup/oleaut32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/ordlookup/oledlg.py` & `vivisect-1.1.1/PE/ordlookup/oledlg.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/ordlookup/ws2_32.py` & `vivisect-1.1.1/PE/ordlookup/ws2_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/petool.py` & `vivisect-1.1.1/PE/petool.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/tools/printord.py` & `vivisect-1.1.1/PE/tools/printord.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PE/tools/structdump.py` & `vivisect-1.1.1/PE/tools/structdump.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/PKG-INFO` & `vivisect-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivisect
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pure python disassembler, debugger, emulator, and static analysis framework
 Home-page: https://github.com/vivisect/vivisect
 Author: The Vivisect Peeps
 Author-email: 
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Disassemblers
 Classifier: Topic :: Software Development :: Debuggers
```

### Comparing `vivisect-1.1.0/README.md` & `vivisect-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/__init__.py` & `vivisect-1.1.1/cobra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pickle
 import socket
 import struct
 import logging
 import traceback
 import urllib.parse
 
-from threading import currentThread, Thread, RLock, Timer, Lock
+from threading import current_thread, Thread, RLock, Timer, Lock
 from socketserver import ThreadingTCPServer, BaseRequestHandler
 try:
     import msgpack
     dumpargs = {}
     loadargs = {'use_list': 0}
     if msgpack.version >= (0, 4, 1):
         dumpargs['use_bin_type'] = 1
@@ -102,42 +102,42 @@
 
 def getCallerInfo():
     """
     This function may be used from *inside* a method being called
     by a remote caller.  It will return a tuple of host,port for the
     other side of the connection... use wisely ;)
     """
-    return getattr(currentThread(), "_cobra_caller_info", None)
+    return getattr(current_thread(), "_cobra_caller_info", None)
 
 def getLocalInfo():
     """
     This function returns the local host,port combination being
     used in the socket servicing the current request
     """
-    return getattr(currentThread(), "_cobra_local_info", None)
+    return getattr(current_thread(), "_cobra_local_info", None)
 
 def getUserInfo():
     '''
     Get the cobra authenticated username of the current user
     ( or None if no user was authenticated )
     '''
-    return getattr(currentThread(), "_cobra_authuser", None)
+    return getattr(current_thread(), "_cobra_authuser", None)
 
 def setCallerInfo(callerinfo):
     """
     This is necessary because of crazy python method call
     name munging for thread attributes ;)
     """
-    currentThread()._cobra_caller_info = callerinfo
+    current_thread()._cobra_caller_info = callerinfo
 
 def setUserInfo(authuser):
-    currentThread()._cobra_authuser = authuser
+    current_thread()._cobra_authuser = authuser
 
 def setLocalInfo(localinfo):
-    currentThread()._cobra_local_info = localinfo
+    current_thread()._cobra_local_info = localinfo
 
 def nocobra(f):
     f.__no_cobra__ = True
     return f
 
 def newobj(f):
     f._cobra_newobj = True
@@ -537,16 +537,15 @@
         '''
         Set the cert/key used by this server to negotiate SSL.
         '''
         self.sslcrt = crtfile
         self.sslkey = keyfile
 
     def fireThread(self):
-        self.thr = Thread(target=self.serve_forever)
-        self.thr.setDaemon(True)
+        self.thr = Thread(target=self.serve_forever, daemon=True)
         self.thr.start()
 
     def stopServer(self):
         self.run = False
         self.shutdown()
         self.server_close()
         self.thr.join()
@@ -1011,15 +1010,15 @@
         return False
 
     def _cobra_getsock(self, thr=None):
         if self._cobra_spoolcnt:
             sock = self._cobra_sockpool.get()
         else:
             if not thr: # if thread isn't specified, use the current thread
-                thr = currentThread()
+                thr = current_thread()
 
             tsocks = getattr(thr, 'cobrasocks', None)
             if tsocks is None:
                 tsocks = {}
                 thr.cobrasocks = tsocks
             sock = tsocks.get(self._cobra_slookup)
```

### Comparing `vivisect-1.1.0/cobra/auth/__init__.py` & `vivisect-1.1.1/cobra/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/auth/shadowfile.py` & `vivisect-1.1.1/cobra/auth/shadowfile.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/cache.py` & `vivisect-1.1.1/cobra/cache.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/cluster.py` & `vivisect-1.1.1/cobra/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,15 @@
         # you want notifications.
         self.callback = None
 
         if docode:
             dcode.enableDcodeServer(daemon=self.cobrad)
 
         # Fire the timeout monitor thread...
-        thr = threading.Thread(target=self.timerThread)
-        thr.setDaemon(True)
+        thr = threading.Thread(target=self.timerThread, daemon=True)
         thr.start()
 
     def addClusterQueen(self, queenhost):
         '''
         Inform the ClusterServer about the presence of a ClusterQueen instance
         on the given host.  When the ClusterServer begins to announce work,
         he will do so in "infrastructure mode" and ask any set queens for help.
@@ -317,16 +316,15 @@
         else:
             buf = "cobra:%s:%s:%d" % (self.name, self.cobraname, self.cobrad.port)
             self.sendsock.sendto(buf.encode('utf-8'), (cluster_ip, cluster_port))
 
     def runServer(self, firethread=False):
 
         if firethread:
-            thr = threading.Thread(target=self.runServer)
-            thr.setDaemon(True)
+            thr = threading.Thread(target=self.runServer, daemon=True)
             thr.start()
 
         else:
             self.cobrad.fireThread()
             while self.go:
 
                 if len(self.queue):
@@ -539,16 +537,15 @@
 
             port = int(portstr)
 
             uri = "%s://%s:%d/%s" % (cc,server,port,cobject)
             self.fireRunner(uri)
 
     def fireRunner(self, uri):
-        thr = threading.Thread(target=self.threadForker, args=(uri,))
-        thr.setDaemon(True)
+        thr = threading.Thread(target=self.threadForker, args=(uri,), daemon=True)
         thr.start()
 
     def threadForker(self, uri):
         self.width += 1
         cmd = sub_cmd % (uri, self.docode)
         try:
             sub = subprocess.Popen([sys.executable, '-c', cmd], stdin=subprocess.PIPE)
@@ -610,16 +607,15 @@
         work.excinfo = formatted
         logger.error(formatted)
         server.failWork(work)
 
 def runAndWaitWork(server, work):
 
     work.touch()
-    thr = threading.Thread(target=workThread, args=(server, work))
-    thr.setDaemon(True)
+    thr = threading.Thread(target=workThread, args=(server, work), daemon=True)
     thr.start()
 
     # Wait around for done or timeout
     while True:
         if work.isTimedOut():
             break
```

### Comparing `vivisect-1.1.0/cobra/dcode.py` & `vivisect-1.1.1/cobra/dcode.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/devent.py` & `vivisect-1.1.1/cobra/devent.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,15 @@
 
         evt = CobraEventCore()
         evt.addEventCallback( mycallback )
 
         NOTE: This API is *not* cobra proxy call safe.
         '''
         if firethread:
-            thr = threading.Thread(target=self.addEventCallback, args=(callback, qmax, False))
-            thr.setDaemon(True)
+            thr = threading.Thread(target=self.addEventCallback, args=(callback, qmax, False), daemon=True)
             thr.start()
             return
 
         chanid = self.initEventChannel(qmax=qmax)
         q = self._ce_chanlookup.get(chanid)
         while True:
 
@@ -222,16 +221,15 @@
         self._ce_ecastsock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._ce_ecastsock.bind((bind, port))
 
         # Join the multicast IP
         mreq = struct.pack("4sL", socket.inet_aton(mcast), socket.INADDR_ANY)
         self._ce_ecastsock.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
 
-        thr = threading.Thread(target=self._runSocketListener)
-        thr.setDaemon(True)
+        thr = threading.Thread(target=self._runSocketListener, daemon=True)
         thr.start()
 
     def _runSocketListener(self):
         sock = self._ce_ecastsock
         while True:
             sockdata, sockaddr = sock.recvfrom(4096)
             etup = json.loads(sockdata)
```

### Comparing `vivisect-1.1.0/cobra/dispatcher.py` & `vivisect-1.1.1/cobra/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/hostid/darwinhostid.py` & `vivisect-1.1.1/cobra/hostid/darwinhostid.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/http.py` & `vivisect-1.1.1/cobra/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import logging
 import urlparse
 import traceback
 import BaseHTTPServer
 
 import cobra as c_cobra
 
-from threading import currentThread,Thread,RLock
+from threading import current_thread,Thread,RLock
 from SocketServer import ThreadingTCPServer
 
 logger = logging.getLogger(__name__)
 daemon = None
 version = "Cobra2"
 COBRA_PORT = 80
 COBRASSL_PORT = 443
@@ -292,16 +292,15 @@
         if sslca and not os.path.isfile(sslca):
             raise Exception('CobraDaemon: sslca param must be a file!')
 
 
         #ThreadingTCPServer.__init__(self, (host, port), CobraHttpConnectionHandler)
         ThreadingTCPServer.__init__(self, (host, port), CobraHttpRequestHandler)
 
-        t = Thread(target=self._timeoutSessions)
-        t.setDaemon(1)
+        t = Thread(target=self._timeoutSessions, daemon=True)
         t.start()
 
         if port == 0:
             self.port = self.socket.getsockname()[1]
 
         self.daemon_threads = True
         self.recvtimeout = None
@@ -310,16 +309,15 @@
         while True:
             time.sleep( self.sess_timeout  )
             for key, (authinfo, tstamp) in self.sessions.items():
                 if time.time()-tstamp > self.sess_timeout:
                     self.sessions.pop(key)
 
     def fireThread(self):
-        thr = Thread(target=self.serve_forever)
-        thr.setDaemon(True)
+        thr = Thread(target=self.serve_forever, daemon=True)
         thr.start()
 
     def setAuthModule(self, authmod):
         '''
         Enable an authentication module for this server
         ( all connections *must* be authenticated through the authmod )
 
@@ -405,15 +403,15 @@
 
         data = CobraHttpMethod(self, '__cobra_hello')()
 
         self._cobra_gothello = True
         self._cobra_methods = data
 
     def _cobra_http_getsock(self):
-        thr = currentThread()
+        thr = current_thread()
         tsocks = getattr(thr, 'cobrahttpsocks', None)
         if tsocks is None:
             tsocks = {}
             thr.cobrahttpsocks = tsocks
 
         sock = tsocks.get(self._cobra_slookup)
         if not sock or sock.trashed:
```

### Comparing `vivisect-1.1.0/cobra/pool.py` & `vivisect-1.1.1/cobra/pool.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/remoteapp.py` & `vivisect-1.1.1/cobra/remoteapp.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/tests/__init__.py` & `vivisect-1.1.1/cobra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/tests/testbasic.py` & `vivisect-1.1.1/cobra/tests/testbasic.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/tests/testcache.py` & `vivisect-1.1.1/cobra/tests/testcache.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/tests/testdcode.py` & `vivisect-1.1.1/cobra/tests/testdcode.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/tests/testevents.py` & `vivisect-1.1.1/cobra/tests/testevents.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/tests/testnewobj.py` & `vivisect-1.1.1/cobra/tests/testnewobj.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/cobra/tools/burnapp.py` & `vivisect-1.1.1/cobra/tools/burnapp.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/__init__.py` & `vivisect-1.1.1/envi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import os
 import sys
 import copy
 import types
 import struct
 import logging
 import platform
+import importlib
 import contextlib
-import importlib.util as imputil
 
 from envi.exc import *
 
 logger = logging.getLogger(__name__)
 
 # TODO: move into const.py
 # Parsed Opcode Formats
@@ -654,14 +654,18 @@
         return remote_branches
 
     def getBranches(self, emu=None):
         """
         Return a list of tuples.  Each tuple contains the target VA of the
         branch, and a possible set of flags showing what type of branch it is.
 
+        Without an emulator, dynamic branches may not be resolvable, and will
+        return a VA of None.  This is intended, and used by codeflow analysis
+        to mark dynamic branches for later analysis (eg. Switchcase analysis).
+
         See the BR_FOO types for all the supported envi branch flags....
         Example: for bva,bflags in op.getBranches():
         """
         return ()
 
     def genRefOpers(self, emu=None):
         '''
@@ -1509,79 +1513,29 @@
         raise ArchNotImplemented(name, "Architecture not defined")
 
     if arch_defs.get(archnum).get('disabled'):
         raise ArchNotImplemented(name, "Architecture Disabled")
 
     # retrieve path and class info.  envi/archs/<archname>/__init__.py with amodname()
     modpathtup = arch_defs[archnum]['modpath']
+    impname = ".".join(modpathtup)
     amodname = arch_defs[archnum].get('clsname')
 
     # load the module (given the path and module name)
     try:
-        module = loadModuleFromPathTup(rname, modpathtup)
-
-    except ModuleLoadFailure as e:
-        raise ArchNotImplemented(e.component, e.message)
+        module = importlib.import_module(impname)
+    except ImportError as e:
+        raise ArchNotImplemented(impname, e.message)
 
     # instantiate the ArchitectureModule
     cls = getattr(module, amodname)
     archmod = cls()
     
     return archmod
 
-def loadModuleFromPathTup(modname, modpathtup):
-    '''
-    Load a Python module given a module path tuple
-
-    Searches through the PYTHONPATH for a matching module
-    '''
-    modpath = os.path.join(*modpathtup)
-    for pathbase in sys.path:
-        tmppath = os.path.join(pathbase, modpath)
-        if os.path.exists(tmppath):
-            modpath = tmppath
-            break
-    
-    return loadModuleFromAbsolutePath(modname, modpath)
-
-def loadModuleFromAbsolutePathTup(modname, modpathtup):
-    '''
-    Load a Python module given an absolute module path tuple
-    '''
-    modpath = os.sep + os.path.join(*modpathtup)
-    return loadModuleFromAbsolutePath(modname, modpath)
-
-def loadModuleFromAbsolutePath(modname, modpath):
-    '''
-    Load a Python module given an absolute module path string
-    '''
-    # if we hand in the path to the directory, load the __init__.py
-    if os.path.isdir(modpath):
-        modpath = os.path.join(modpath, '__init__.py')
-
-    if not os.path.exists(modpath):
-        raise ModuleLoadFailure(modname, "Path does not exist: %r" % modpath)
-
-    # get the module spec
-    spec = imputil.spec_from_file_location(modname, modpath)
-    if not spec:
-        raise ModuleLoadFailure(modname, "Failed to load module")
-
-    # create an unintialized module from the spec
-    module = imputil.module_from_spec(spec)
-    if not module:
-        raise ModuleLoadFailure(modname, "Failed to create uninitialized module from the spec")
-
-    # insert the module into sys.modules:
-    sys.modules[modname] = module
-
-    # initialize the module (actually "importing" it)
-    spec.loader.exec_module(module)
-
-    return module
 
 def getArchModules(default=ARCH_DEFAULT):
     '''
     Retrieve a default array of arch modules ( where index 0 is
     also the "named" or "default" arch module.
     '''
     archs = []
```

### Comparing `vivisect-1.1.0/envi/archs/__init__.py` & `vivisect-1.1.1/envi/archs/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/amd64/__init__.py` & `vivisect-1.1.1/envi/archs/amd64/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,36 @@
 
     def i_pextrd_q(self, op):
         if op.prefixes & PREFIX_REX_W:
             self.i_pextrb(op, width=8)
         else:
             self.i_pextrb(op, width=4)
 
+    def i_div(self, op):
+        tsize = op.opers[0].tsize
+        if tsize == 8:
+            val = self.getOperValue(op, 0)
+            if val == 0:
+                raise e_exc.DivideByZero(self)
+
+            rax = self.getRegister(REG_RAX)
+            rdx = self.getRegister(REG_RDX)
+            tot = (rdx << 64) + rax
+            quot = int(tot // val)
+            rem = tot % val
+
+            if tot > (2**128)-1:
+                mesg = '0x%.8x: division exception on %s' % (op.va, str(op))
+                raise e_exc.DivideError(self, msg=mesg)
+
+            self.setRegister(REG_RAX, quot)
+            self.setRegister(REG_RDX, rem)
+        else:
+            e_i386.IntelEmulator.i_div(self, op)
+
     def i_idiv(self, op):
         tsize = op.opers[0].tsize
         if tsize == 8:
             val = self.twoRegCompound(REG_RDX, REG_RAX, 8)
             val = e_bits.signed(val, 16)
             d = self.getOperValue(op, 0)
             d = e_bits.signed(d, 8)
```

### Comparing `vivisect-1.1.0/envi/archs/amd64/disasm.py` & `vivisect-1.1.1/envi/archs/amd64/disasm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/amd64/opcode64.py` & `vivisect-1.1.1/envi/archs/amd64/opcode64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/amd64/regs.py` & `vivisect-1.1.1/envi/archs/amd64/regs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/amd64/vmcslookup.py` & `vivisect-1.1.1/envi/archs/amd64/vmcslookup.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/arm/__init__.py` & `vivisect-1.1.1/envi/archs/arm/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/arm/const.py` & `vivisect-1.1.1/envi/archs/arm/const.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/arm/disasm.py` & `vivisect-1.1.1/envi/archs/arm/disasm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/arm/emu.py` & `vivisect-1.1.1/envi/archs/arm/emu.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/arm/regs.py` & `vivisect-1.1.1/envi/archs/arm/regs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/h8/__init__.py` & `vivisect-1.1.1/envi/archs/h8/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/h8/disasm.py` & `vivisect-1.1.1/envi/archs/h8/disasm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/h8/emu.py` & `vivisect-1.1.1/envi/archs/h8/emu.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/h8/operands.py` & `vivisect-1.1.1/envi/archs/h8/operands.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/h8/parsers.py` & `vivisect-1.1.1/envi/archs/h8/parsers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/h8/regs.py` & `vivisect-1.1.1/envi/archs/h8/regs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/i386/__init__.py` & `vivisect-1.1.1/envi/archs/i386/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/i386/disasm.py` & `vivisect-1.1.1/envi/archs/i386/disasm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/i386/emu.py` & `vivisect-1.1.1/envi/archs/i386/emu.py`

 * *Files 1% similar despite different names*

```diff
@@ -952,28 +952,14 @@
 
             #if quot > 0xffffffff:
                 #"FIXME: division exception"
 
             self.setRegister(REG_EAX, quot)
             self.setRegister(REG_EDX, rem)
 
-        elif dsize == 8:
-            rax = self.getRegisterByName("rax")
-            rdx = self.getRegisterByName("rdx")
-            tot = (rdx << 64) + rax
-            quot = int(tot / val)
-            rem = tot % val
-
-            if tot > (2**64)-1:
-                mesg = '0x%.8x: division exception on %s' % (op.va, str(op))
-                raise e_exc.DivideError(self, msg=mesg)
-
-            self.setRegisterByName("rax", quot)
-            self.setRegisterByName("rdx", rem)
-
         else:
             raise e_exc.UnsupportedInstruction(self, op)
 
     def i_enter(self, op):
         locsize = self.getOperValue(op, 0)
         depth = self.getOperValue(op, 1)
         if depth != 0:
```

### Comparing `vivisect-1.1.0/envi/archs/i386/opcode86.py` & `vivisect-1.1.1/envi/archs/i386/opcode86.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/i386/opconst.py` & `vivisect-1.1.1/envi/archs/i386/opconst.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/i386/regs.py` & `vivisect-1.1.1/envi/archs/i386/regs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/msp430/__init__.py` & `vivisect-1.1.1/envi/archs/msp430/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/msp430/const.py` & `vivisect-1.1.1/envi/archs/msp430/const.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/msp430/disasm.py` & `vivisect-1.1.1/envi/archs/msp430/disasm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/msp430/emu.py` & `vivisect-1.1.1/envi/archs/msp430/emu.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/msp430/regs.py` & `vivisect-1.1.1/envi/archs/msp430/regs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/thumb16/disasm.py` & `vivisect-1.1.1/envi/archs/thumb16/disasm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/z80/disasm.py` & `vivisect-1.1.1/envi/archs/z80/disasm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/z80/regs.py` & `vivisect-1.1.1/envi/archs/z80/regs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/archs/z80/z80opcode.py` & `vivisect-1.1.1/envi/archs/z80/z80opcode.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/bintree.py` & `vivisect-1.1.1/envi/bintree.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/bits.py` & `vivisect-1.1.1/envi/bits.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/bytesig.py` & `vivisect-1.1.1/envi/bytesig.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/cli.py` & `vivisect-1.1.1/envi/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from getopt import getopt
 
 
 logger = logging.getLogger(__name__)
 
 def splitargs(cmdline):
     cmdline = cmdline.replace('\\\\"', '"').replace('\\"', '')
-    patt = re.compile('\".+?\"|\S+')
+    patt = re.compile(r'".+?"|\S+')
     for item in cmdline.split('\n'):
         return [s.strip('"') for s in patt.findall(item)]
 
 def formatargs(args):
     ret = []
     subcmds = [args[i:i+5] for i in range(0, len(args), 5)]
     for cmdnames in subcmds:
@@ -394,15 +394,15 @@
             optname = subnames[-1]
             optval = cfg.get(optname)
             if optval is None:
                 self.vprint('No Such Config Option: %s' % optname)
                 return
 
             if len(parts) == 2:
-                # the config entry already has a value, let's use it to decide 
+                # the config entry already has a value, let's use it to decide
                 # whether to convert it to an int or leave it as a str.
                 if type(cfg[optname]) == int:
                     newval = int(parts[1], 0)
                 else:
                     newval = parts[1]
 
                 if (not isinstance(newval, str)) or not isinstance(optval, str):
```

### Comparing `vivisect-1.1.0/envi/codeflow.py` & `vivisect-1.1.1/envi/codeflow.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/common.py` & `vivisect-1.1.1/envi/common.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/config.py` & `vivisect-1.1.1/envi/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,14 +69,44 @@
         Example:
             doc = config.getOptionDoc('woot')
             if doc is not None:
                 print('woot: %s' % doc)
         '''
         return self.cfgdocs.get(optname)
 
+    def getOptionByString(self, pathstring):
+        '''
+        Retrieve config options as a single dot-separated string.
+
+        This is a convenience function for reading config options dynamically from a single
+        string, which has benefits over config-object manipulation for alternative UIs or 
+        plugins.
+
+        Example:
+            opt = config.getOptionByString('foo.bar.baz.info')
+
+            where:
+                info is a data option in side of baz
+                baz is a subconfig of bar
+                bar is a subconfig of foo
+                foo is a top level subconfig
+        '''
+        optparts = pathstring.split('.')
+        config = self
+        for opart in optparts[:-1]:
+            config = config.getSubConfig(opart, add=False)
+            if config is None:
+                raise e_exc.ConfigInvalidName(pathstring)
+
+        optname = optparts[-1]
+        if optname not in config.cfginfo:
+            raise e_exc.ConfigInvalidOption(optname)
+
+        return config[optname]
+
     def getConfigPaths(self):
         '''
         Return a list of tuples including: (type, valid path strings, existing value)
 
         'type' can be CONFIG_PATH or CONFIG_ENTRY to indicate whether the tuple
         represents a subconfig or an actual key/value pair
         '''
```

### Comparing `vivisect-1.1.0/envi/const.py` & `vivisect-1.1.1/envi/const.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/encoding.py` & `vivisect-1.1.1/envi/encoding.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/exc.py` & `vivisect-1.1.1/envi/exc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/expression.py` & `vivisect-1.1.1/envi/expression.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/ieee754.py` & `vivisect-1.1.1/envi/ieee754.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/interactive.py` & `vivisect-1.1.1/envi/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,18 @@
                     ipsh = TerminalInteractiveShell()
                     ipsh.user_global_ns.update(gbls)
                     ipsh.user_global_ns.update(lcls)
                     ipsh.autocall = 2       # don't require parenthesis around *everything*.  be smart!
                     shelltype = STYPE_IPYTHON
 
                 except ImportError as e:
+                    import code
                     print(e)
                     shell = code.InteractiveConsole(gbls)
-                    shelltype = STYPE_IPYTHON
+                    shelltype = STYPE_CODE_INTERACT
 
     if shelltype == STYPE_IPYTHON_NEW:
         globals().update(gbls)
         locals().update(lcls)
         embed()
 
     elif shelltype == STYPE_IPYTHON:
```

### Comparing `vivisect-1.1.0/envi/memcanvas/__init__.py` & `vivisect-1.1.1/envi/memcanvas/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/memcanvas/renderers/__init__.py` & `vivisect-1.1.1/envi/memcanvas/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/memory.py` & `vivisect-1.1.1/envi/memory.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/pagelookup.py` & `vivisect-1.1.1/envi/pagelookup.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/pyzip.py` & `vivisect-1.1.1/envi/pyzip.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/config.py` & `vivisect-1.1.1/envi/qt/config.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/html.py` & `vivisect-1.1.1/envi/qt/html.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/jquery.py` & `vivisect-1.1.1/envi/qt/jquery.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/memcanvas.py` & `vivisect-1.1.1/envi/qt/memcanvas.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/memdump.py` & `vivisect-1.1.1/envi/qt/memdump.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/memory.py` & `vivisect-1.1.1/envi/qt/memory.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/memorymap.py` & `vivisect-1.1.1/envi/qt/memorymap.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/memsearch.py` & `vivisect-1.1.1/envi/qt/memsearch.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/qt/memwrite.py` & `vivisect-1.1.1/envi/qt/memwrite.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/radixtree.py` & `vivisect-1.1.1/envi/radixtree.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/registers.py` & `vivisect-1.1.1/envi/registers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/symstore/resolver.py` & `vivisect-1.1.1/envi/symstore/resolver.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/symstore/symcache.py` & `vivisect-1.1.1/envi/symstore/symcache.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/arm_bit_test_adds.py` & `vivisect-1.1.1/envi/tests/arm_bit_test_adds.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/arm_bit_test_cmn.py` & `vivisect-1.1.1/envi/tests/arm_bit_test_cmn.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/arm_bit_test_cmp.py` & `vivisect-1.1.1/envi/tests/arm_bit_test_cmp.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/arm_bit_test_subs.py` & `vivisect-1.1.1/envi/tests/arm_bit_test_subs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/armthumb_tests.py` & `vivisect-1.1.1/envi/tests/armthumb_tests.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/iadc.py` & `vivisect-1.1.1/envi/tests/msp430/iadc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/iadd.py` & `vivisect-1.1.1/envi/tests/msp430/iadd.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/iaddc.py` & `vivisect-1.1.1/envi/tests/msp430/iaddc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/iand.py` & `vivisect-1.1.1/envi/tests/msp430/iand.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/ibic.py` & `vivisect-1.1.1/envi/tests/msp430/ibic.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/ibis.py` & `vivisect-1.1.1/envi/tests/msp430/ibis.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/ibit.py` & `vivisect-1.1.1/envi/tests/msp430/ibit.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/iclr.py` & `vivisect-1.1.1/envi/tests/msp430/iclr.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/icmp.py` & `vivisect-1.1.1/envi/tests/msp430/icmp.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/idadc.py` & `vivisect-1.1.1/envi/tests/msp430/idadc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/idadd.py` & `vivisect-1.1.1/envi/tests/msp430/idadd.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/idec.py` & `vivisect-1.1.1/envi/tests/msp430/idec.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/idecd.py` & `vivisect-1.1.1/envi/tests/msp430/idecd.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/iinc.py` & `vivisect-1.1.1/envi/tests/msp430/iinc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/iincd.py` & `vivisect-1.1.1/envi/tests/msp430/iincd.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/iinv.py` & `vivisect-1.1.1/envi/tests/msp430/iinv.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/ijumps.py` & `vivisect-1.1.1/envi/tests/msp430/ijumps.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/imov.py` & `vivisect-1.1.1/envi/tests/msp430/imov.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/ipop.py` & `vivisect-1.1.1/envi/tests/msp430/ipop.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/ipush.py` & `vivisect-1.1.1/envi/tests/msp430/ipush.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/irla.py` & `vivisect-1.1.1/envi/tests/msp430/irla.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/irlc.py` & `vivisect-1.1.1/envi/tests/msp430/irlc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/irra.py` & `vivisect-1.1.1/envi/tests/msp430/irra.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/irrc.py` & `vivisect-1.1.1/envi/tests/msp430/irrc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/isbc.py` & `vivisect-1.1.1/envi/tests/msp430/isbc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/isub.py` & `vivisect-1.1.1/envi/tests/msp430/isub.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/isubc.py` & `vivisect-1.1.1/envi/tests/msp430/isubc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/isxt.py` & `vivisect-1.1.1/envi/tests/msp430/isxt.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/itst.py` & `vivisect-1.1.1/envi/tests/msp430/itst.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/msp430/ixor.py` & `vivisect-1.1.1/envi/tests/msp430/ixor.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_arch_amd64.py` & `vivisect-1.1.1/envi/tests/test_arch_amd64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_arch_arm.py` & `vivisect-1.1.1/envi/tests/test_arch_arm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_arch_arm_cmp_flags.py` & `vivisect-1.1.1/envi/tests/test_arch_arm_cmp_flags.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_arch_h8.py` & `vivisect-1.1.1/envi/tests/test_arch_h8.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_arch_i386.py` & `vivisect-1.1.1/envi/tests/test_arch_i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_arch_i386_emu.py` & `vivisect-1.1.1/envi/tests/test_arch_i386_emu.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,18 @@
     {'bytes': 'f7e2',
      'setup': ({'eax': 0x47b3, 'edx': 0x898937}, {}),
      'tests': ({'eax': 0x85393275, 'edx': 0x26}, {})},
     # div ax
     {'bytes': '66f7f0',
      'setup': ({'eax': 48, 'edx': 1}, {}),
      'tests': ({'eax': 1366, 'edx': 16}, {})},
+    # div eax
+    {'bytes': 'f7f0',
+     'setup': ({'eax': 48, 'edx': 1}, {}),
+     'tests': ({'eax': 89478486, 'edx': 16}, {})},
     # idiv edi
     {'bytes': 'f7ff',
      'setup': ({'eax': 0xffffffe2, 'edx': 0xffffffff}, {}),
      'tests': ({'eax': 0, 'edx': 0xffffffe2}, {})},
     # rol eax, 4
     {'bytes': 'c1c004',
      'setup': ({'eax': 5}, {}),
@@ -249,8 +253,8 @@
 
         emu32.setRegisterByName('eax', 0)
         emu32.setRegisterByName('ecx', -1)
         emu32.setRegisterByName('edi', 0x4000000d)
         emu32.executeOpcode(op_zscasb)
         self.assertEqual(emu32.getRegisterByName('ecx'), 0xffffffff - min(TEST_REPMAX, len("\x00\x00\x00f")))
 
-        emu32.setEmuOpt("i386:repmax", orig_repmax)
+        emu32.setEmuOpt("i386:repmax", orig_repmax)
```

### Comparing `vivisect-1.1.0/envi/tests/test_arch_msp430.py` & `vivisect-1.1.1/envi/tests/test_arch_msp430.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_bits.py` & `vivisect-1.1.1/envi/tests/test_bits.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_bytesig.py` & `vivisect-1.1.1/envi/tests/test_bytesig.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_cli.py` & `vivisect-1.1.1/envi/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_emu_lockstep.py` & `vivisect-1.1.1/envi/tests/test_emu_lockstep.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_envi_config.py` & `vivisect-1.1.1/envi/tests/test_envi_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,7 +17,24 @@
 
         self.assertEqual(cfg.woot, 10)
         self.assertEqual(cfg.foosub.bar, 'qwer')
         self.assertEqual(cfg.foosub.baz[0], 'one')
         self.assertEqual(cfg.biz, '0x41414141')
         for idx, item in enumerate(cfg.foosub.baz):
             self.assertEqual(defaults['foosub']['baz'][idx], item)
+
+    def test_config_by_string(self):
+        defaults = {
+            'woot': 10,
+            'biz': '0x41414141',
+            'foosub': {
+                'bar': 'qwer',
+                'baz': ('one', 'two', 'three'),
+            }
+        }
+        cfg = e_config.EnviConfig(defaults=defaults)
+
+        self.assertEqual(cfg.getOptionByString('woot'), 0xa)
+        self.assertEqual(cfg.getOptionByString('biz'), '0x41414141')
+        self.assertEqual(cfg.getOptionByString('foosub.bar'), 'qwer')
+        self.assertEqual(cfg.getOptionByString('foosub.baz'), ('one', 'two', 'three'))
+
```

### Comparing `vivisect-1.1.0/envi/tests/test_expression.py` & `vivisect-1.1.1/envi/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_ieee754.py` & `vivisect-1.1.1/envi/tests/test_ieee754.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_memmap.py` & `vivisect-1.1.1/envi/tests/test_memmap.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_memory.py` & `vivisect-1.1.1/envi/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_registers.py` & `vivisect-1.1.1/envi/tests/test_registers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/tests/test_symstore.py` & `vivisect-1.1.1/envi/tests/test_symstore.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/envi/threads.py` & `vivisect-1.1.1/envi/threads.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/setup.py` & `vivisect-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 from os import path
 
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 
 dirn = path.abspath(path.dirname(__file__))
 with open(path.join(dirn, 'README.md'), 'r') as fd:
     desc = fd.read()
 
 setup(
     name='vivisect',
```

### Comparing `vivisect-1.1.0/vdb/__init__.py` & `vivisect-1.1.1/vdb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,15 @@
 
     def __setitem__(self, key, item):
         UserDict.__setitem__(self, key, item)
         UserDict.__setitem__(self, item, key)
 
 class ScriptThread(threading.Thread):
     def __init__(self, cobj, locals):
-        threading.Thread.__init__(self)
-        self.setDaemon(True)
+        super.__init__(self, daemon=True)
         self.cobj = cobj
         self.locals = locals
 
     def run(self):
         try:
             exec(self.cobj, self.locals)
         except Exception as e:
@@ -1031,29 +1030,31 @@
         -A <addr>  - Step to <addr>
         -B         - Step past the next branch instruction
         -C <count> - Step <count> instructions
         -R         - Step to return from this function
         -V         - Show operand values during single step (verbose!)
         -U         - Remainder of args is "step until" expression (stop on True)
         -Q         - Do not output to canvas
+        -O         - Step Over calls (ie. stay in this function)
         """
         t = self.trace
         argv = e_cli.splitargs(line)
         try:
-            opts,args = getopt(argv, "A:BC:RVUQ")
+            opts,args = getopt(argv, "A:BC:RVUOQ")
         except Exception as e:
             return self.do_help("stepi")
 
         until = None
         count = None
         taddr = None
         toret = False
         tobrn = False
         showop = False
         quiet = False
+        stepover = False
 
         for opt, optarg in opts:
 
             if opt == '-A':
                 taddr = t.parseExpression(optarg)
 
             elif opt == '-B':
@@ -1070,14 +1071,17 @@
 
             elif opt == '-U':
                 until = ' '.join(args)
 
             elif opt == '-Q':
                 quiet = True
 
+            elif opt == '-O':
+                stepover = True
+
         if ( count is None 
              and taddr is None
              and until is None
              and toret == False 
              and tobrn == False):
             count = 1
 
@@ -1118,26 +1122,32 @@
                                 self.canvas.addText('0x%.8x ' % val)
                             except Exception as e:
                                 self.canvas.addText(str(e))
 
                     if not quiet:
                         self.canvas.addText('\n')
 
-                    if op.iflags & envi.IF_CALL:
+                    if op.iflags & envi.IF_CALL and not stepover:
                         depth += 1
 
                     elif op.iflags & envi.IF_RET:
                         depth -= 1
                 except Exception as e:
                     print("[E@0x%x] %r" % (pc, e))
 
 
-                tid = t.getCurrentThread()
+                # execute the instruction
+                if op.iflags & envi.IF_CALL and stepover:
+                    bp = vtrace.breakpoints.OneTimeBreak(op.va + op.size)
+                    self.trace.addBreakpoint(bp)
+                    self.trace.run()
 
-                t.stepi()
+                else:
+                    tid = t.getCurrentThread()
+                    t.stepi()
 
                 if until and t.parseExpression(until):
                     break
 
                 # If we get an event from a different thread, get out!
                 if t.getCurrentThread() != tid:
                     break
@@ -2351,10 +2361,10 @@
         if not text:
             return libnames
         return [ i for i in libnames if i.startswith( text ) ]
 
 ##############################################################################
 # The following are touched during the release process by bump2version.
 # You should have no reason to modify these yourself
-version = (1, 1, 0)
+version = (1, 1, 1)
 verstring = '.'.join([str(x) for x in version])
 commit = ''
```

### Comparing `vivisect-1.1.0/vdb/ext/execsc.py` & `vivisect-1.1.1/vdb/ext/execsc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/extensions/__init__.py` & `vivisect-1.1.1/vdb/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/extensions/arm.py` & `vivisect-1.1.1/vdb/extensions/arm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/extensions/gdbstub.py` & `vivisect-1.1.1/vdb/extensions/gdbstub.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/extensions/i386.py` & `vivisect-1.1.1/vdb/extensions/i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/extensions/windows.py` & `vivisect-1.1.1/vdb/extensions/windows.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/extensions/winkern.py` & `vivisect-1.1.1/vdb/extensions/winkern.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/qt/base.py` & `vivisect-1.1.1/vdb/qt/base.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/qt/main.py` & `vivisect-1.1.1/vdb/qt/main.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/qt/memory.py` & `vivisect-1.1.1/vdb/qt/memory.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/qt/memwrite.py` & `vivisect-1.1.1/vdb/qt/memwrite.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/qt/registers.py` & `vivisect-1.1.1/vdb/qt/registers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/qt/threads.py` & `vivisect-1.1.1/vdb/qt/threads.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/recon/__init__.py` & `vivisect-1.1.1/vdb/recon/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/recon/dopestack.py` & `vivisect-1.1.1/vdb/recon/dopestack.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/recon/sniper.py` & `vivisect-1.1.1/vdb/recon/sniper.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/release.py` & `vivisect-1.1.1/vdb/release.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/renderers.py` & `vivisect-1.1.1/vdb/renderers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/stalker/__init__.py` & `vivisect-1.1.1/vdb/stalker/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/testmods/__init__.py` & `vivisect-1.1.1/vdb/testmods/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/testmods/callingconventions.py` & `vivisect-1.1.1/vdb/testmods/callingconventions.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/testmods/hookbptest.py` & `vivisect-1.1.1/vdb/testmods/hookbptest.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/tests/testrecon.py` & `vivisect-1.1.1/vdb/tests/testrecon.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/tests/teststalker.py` & `vivisect-1.1.1/vdb/tests/teststalker.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/tools/android.py` & `vivisect-1.1.1/vdb/tools/android.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/tools/gendocs.py` & `vivisect-1.1.1/vdb/tools/gendocs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/unittest.py` & `vivisect-1.1.1/vdb/unittest.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vdb/vdbbin.py` & `vivisect-1.1.1/vdb/vdbbin.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/cli.py` & `vivisect-1.1.1/visgraph/cli.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/dbcore.py` & `vivisect-1.1.1/visgraph/dbcore.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/drawing/bezier.py` & `vivisect-1.1.1/visgraph/drawing/bezier.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/drawing/catmullrom.py` & `vivisect-1.1.1/visgraph/drawing/catmullrom.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/exc.py` & `vivisect-1.1.1/visgraph/exc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/graphcore.py` & `vivisect-1.1.1/visgraph/graphcore.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/layouts/__init__.py` & `vivisect-1.1.1/visgraph/layouts/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/layouts/dynadag.py` & `vivisect-1.1.1/visgraph/layouts/dynadag.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/layouts/force.py` & `vivisect-1.1.1/visgraph/layouts/force.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/pathcore.py` & `vivisect-1.1.1/visgraph/pathcore.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/renderers/__init__.py` & `vivisect-1.1.1/visgraph/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/renderers/gtkrend.py` & `vivisect-1.1.1/visgraph/renderers/gtkrend.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/renderers/qgraphtree.py` & `vivisect-1.1.1/visgraph/renderers/qgraphtree.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/renderers/qtrend.py` & `vivisect-1.1.1/visgraph/renderers/qtrend.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/renderers/svgrend.py` & `vivisect-1.1.1/visgraph/renderers/svgrend.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/tests/test_graphcore.py` & `vivisect-1.1.1/visgraph/tests/test_graphcore.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/visgraph/tests/test_layouts.py` & `vivisect-1.1.1/visgraph/tests/test_layouts.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/__init__.py` & `vivisect-1.1.1/vivisect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,16 +640,15 @@
         self.leaders.update(self.server.getLeaderSessions())
         self.leaderloc.update(self.server.getLeaderLocations())
 
         wsevents = self.server.exportWorkspace()
         self.importWorkspace(wsevents)
         self.server.vprint('%s connection complete!' % uname)
 
-        thr = threading.Thread(target=self._clientThread)
-        thr.setDaemon(True)
+        thr = threading.Thread(target=self._clientThread, daemon=True)
         thr.start()
 
         timeout = self.config.viv.remote.wait_for_plat_arch
         self._load_event.wait(timeout=timeout)
         self._snapInAnalysisModules()
 
     def _clientThread(self):
@@ -1854,14 +1853,17 @@
         return [ xtup for xtup in xrefs if xtup[XR_RTYPE] == rtype ]
 
     def addMemoryMap(self, va, perms, fname, bytes, align=None):
         """
         Add a memory map to the workspace.  This is the *only* way to
         get memory backings into the workspace.
         """
+        # handle nasty special case of an empty map with an alignment
+        if not len(bytes):
+            bytes = b'\0'
         self._fireEvent(VWE_ADDMMAP, (va, perms, fname, bytes, align))
 
         # since we don't return anything from _fireEvent(), pull the new info:
         mva, msz, mperm, mbytes = self.getMemoryMap(va)
         return msz
 
     def delMemoryMap(self, mapva):
@@ -3278,10 +3280,10 @@
     dname = os.path.abspath(dname)
     return os.path.join(dname, *pathents)
 
 
 ##############################################################################
 # The following are touched during the release process by bump2version.
 # You should have no reason to modify these directly
-version = (1, 1, 0)
+version = (1, 1, 1)
 verstring = '.'.join([str(x) for x in version])
 commit = ''
```

### Comparing `vivisect-1.1.0/vivisect/analysis/__init__.py` & `vivisect-1.1.1/vivisect/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/amd64/emulation.py` & `vivisect-1.1.1/vivisect/analysis/amd64/emulation.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/amd64/golang.py` & `vivisect-1.1.1/vivisect/analysis/amd64/golang.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/arm/emulation.py` & `vivisect-1.1.1/vivisect/analysis/arm/emulation.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/arm/thunk_reg.py` & `vivisect-1.1.1/vivisect/analysis/arm/thunk_reg.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/crypto/constants.py` & `vivisect-1.1.1/vivisect/analysis/crypto/constants.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/elf/__init__.py` & `vivisect-1.1.1/vivisect/analysis/elf/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/elf/elfplt.py` & `vivisect-1.1.1/vivisect/analysis/elf/elfplt.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/elf/elfplt_late.py` & `vivisect-1.1.1/vivisect/analysis/elf/elfplt_late.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/elf/libc_start_main.py` & `vivisect-1.1.1/vivisect/analysis/elf/libc_start_main.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/codeblocks.py` & `vivisect-1.1.1/vivisect/analysis/generic/codeblocks.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/emucode.py` & `vivisect-1.1.1/vivisect/analysis/generic/emucode.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/funcentries.py` & `vivisect-1.1.1/vivisect/analysis/generic/funcentries.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/impapi.py` & `vivisect-1.1.1/vivisect/analysis/generic/impapi.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/linker.py` & `vivisect-1.1.1/vivisect/analysis/generic/linker.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/mkpointers.py` & `vivisect-1.1.1/vivisect/analysis/generic/mkpointers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/noret.py` & `vivisect-1.1.1/vivisect/analysis/generic/noret.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/pointers.py` & `vivisect-1.1.1/vivisect/analysis/generic/pointers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/pointertables.py` & `vivisect-1.1.1/vivisect/analysis/generic/pointertables.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/relocations.py` & `vivisect-1.1.1/vivisect/analysis/generic/relocations.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/strconst.py` & `vivisect-1.1.1/vivisect/analysis/generic/strconst.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/switchcase.py` & `vivisect-1.1.1/vivisect/analysis/generic/switchcase.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/symswitchcase.py` & `vivisect-1.1.1/vivisect/analysis/generic/symswitchcase.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/generic/thunks.py` & `vivisect-1.1.1/vivisect/analysis/generic/thunks.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/i386/__init__.py` & `vivisect-1.1.1/vivisect/analysis/i386/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/i386/calling.py` & `vivisect-1.1.1/vivisect/analysis/i386/calling.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/i386/golang.py` & `vivisect-1.1.1/vivisect/analysis/i386/golang.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/i386/importcalls.py` & `vivisect-1.1.1/vivisect/analysis/i386/importcalls.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/i386/instrhook.py` & `vivisect-1.1.1/vivisect/analysis/i386/instrhook.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/i386/thunk_reg.py` & `vivisect-1.1.1/vivisect/analysis/i386/thunk_reg.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/ms/localhints.py` & `vivisect-1.1.1/vivisect/analysis/ms/localhints.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/ms/msvcfunc.py` & `vivisect-1.1.1/vivisect/analysis/ms/msvcfunc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/ms/vftables.py` & `vivisect-1.1.1/vivisect/analysis/ms/vftables.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/analysis/pe.py` & `vivisect-1.1.1/vivisect/analysis/pe.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/base.py` & `vivisect-1.1.1/vivisect/base.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/cli.py` & `vivisect-1.1.1/vivisect/cli.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/codegraph.py` & `vivisect-1.1.1/vivisect/codegraph.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/colormap.py` & `vivisect-1.1.1/vivisect/colormap.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/const.py` & `vivisect-1.1.1/vivisect/const.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/defconfig.py` & `vivisect-1.1.1/vivisect/defconfig.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/emutils.py` & `vivisect-1.1.1/vivisect/emutils.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/exc.py` & `vivisect-1.1.1/vivisect/exc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/extensions/__init__.py` & `vivisect-1.1.1/vivisect/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/extensions/example_gui_extension.py` & `vivisect-1.1.1/vivisect/extensions/example_gui_extension.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/__init__.py` & `vivisect-1.1.1/vivisect/impapi/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/gentool.py` & `vivisect-1.1.1/vivisect/impapi/gentool.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/posix/i386.py` & `vivisect-1.1.1/vivisect/impapi/posix/i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/advapi_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/advapi_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/advapi_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/advapi_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/amd64.py` & `vivisect-1.1.1/vivisect/impapi/windows/amd64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/gdi_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/gdi_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/gdi_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/gdi_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/i386.py` & `vivisect-1.1.1/vivisect/impapi/windows/i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/kernel_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/kernel_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/kernel_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/kernel_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr100_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr100_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr100_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr100_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr110_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr110_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr110_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr110_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr120_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr120_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr120_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr120_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr71_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr71_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr80_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr80_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr80_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr80_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr90_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr90_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcr90_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcr90_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcrt_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcrt_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/msvcrt_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/msvcrt_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/ntdll_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/ntdll_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/ntdll_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/ntdll_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/ole_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/ole_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/ole_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/ole_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/rpcrt4_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/rpcrt4_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/rpcrt4_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/rpcrt4_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/shell_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/shell_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/shell_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/shell_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/user_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/user_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/user_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/user_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/ws2plus_32.py` & `vivisect-1.1.1/vivisect/impapi/windows/ws2plus_32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/windows/ws2plus_64.py` & `vivisect-1.1.1/vivisect/impapi/windows/ws2plus_64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impapi/winkern/i386.py` & `vivisect-1.1.1/vivisect/impapi/winkern/i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/emulator.py` & `vivisect-1.1.1/vivisect/impemu/emulator.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/lookup.py` & `vivisect-1.1.1/vivisect/impemu/lookup.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/monitor.py` & `vivisect-1.1.1/vivisect/impemu/monitor.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/platarch/amd64.py` & `vivisect-1.1.1/vivisect/impemu/platarch/amd64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/platarch/arm.py` & `vivisect-1.1.1/vivisect/impemu/platarch/arm.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/platarch/h8.py` & `vivisect-1.1.1/vivisect/impemu/platarch/h8.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/platarch/i386.py` & `vivisect-1.1.1/vivisect/impemu/platarch/i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/platarch/linux.py` & `vivisect-1.1.1/vivisect/impemu/platarch/linux.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/platarch/msp430.py` & `vivisect-1.1.1/vivisect/impemu/platarch/msp430.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/impemu/platarch/windows.py` & `vivisect-1.1.1/vivisect/impemu/platarch/windows.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/notes/__init__.py` & `vivisect-1.1.1/vivisect/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/parsers/__init__.py` & `vivisect-1.1.1/vivisect/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/parsers/blob.py` & `vivisect-1.1.1/vivisect/parsers/blob.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/parsers/elf.py` & `vivisect-1.1.1/vivisect/parsers/elf.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/parsers/ihex.py` & `vivisect-1.1.1/vivisect/parsers/ihex.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/parsers/macho.py` & `vivisect-1.1.1/vivisect/parsers/macho.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/parsers/pe.py` & `vivisect-1.1.1/vivisect/parsers/pe.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,15 @@
         endva = mapva + lenbytes
         if endva > topmem:
             topmem = endva
 
     size = topmem - baseaddr
 
     if baseaddr == 0:
-        baseaddr = vw.config.viv.parsers.pe.baseoffset
+        baseaddr = vw.config.viv.parsers.pe.baseaddr
 
     if savebase:
         # if we provided a baseaddr, override what the file wants
         baseaddr = savebase
         
     return baseaddr, size
```

### Comparing `vivisect-1.1.0/vivisect/parsers/srec.py` & `vivisect-1.1.1/vivisect/parsers/srec.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/qt/ctxmenu.py` & `vivisect-1.1.1/vivisect/qt/ctxmenu.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/qt/default.lyt` & `vivisect-1.1.1/vivisect/qt/default.lyt`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/qt/funcgraph.py` & `vivisect-1.1.1/vivisect/qt/funcgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,26 +462,26 @@
         immediately display.  Perhaps someday this will update only the blocks
         that have changed since last update, and be fast, so we can update
         after every change.
         '''
         # debounce logic
         if self._renderWaiting:
             # if we are already rendering... and another thing is waiting
-            #logger.debug('(%r) someone is already waiting... returning', threading.currentThread())
+            #logger.debug('(%r) someone is already waiting... returning', threading.current_thread())
             return
 
         while self._rendering:
-            #logger.debug('(%r) waiting for render to complete...', threading.currentThread())
+            #logger.debug('(%r) waiting for render to complete...', threading.current_thread())
             self._renderWaiting = True
             time.sleep(.1)
 
         self._renderWaiting = False
 
         with self._renderlock:
-            #logger.debug('(%r) render beginning...', threading.currentThread())
+            #logger.debug('(%r) render beginning...', threading.current_thread())
             self._rendering = True
 
         # actually do the refresh
         self._last_viewpt = self.mem_canvas.page().scrollPosition()
         # TODO: history should track this as well and return to the same place
         self.clearText()
         self.fva = None
@@ -497,15 +497,15 @@
             return
 
         self.mem_canvas.setScrollPosition(self._last_viewpt.x(), self._last_viewpt.y())
         self._last_viewpt = None
 
         with self._renderlock:
             self._rendering = False
-        #logger.debug('(%r) render finished!', threading.currentThread())
+        #logger.debug('(%r) render finished!', threading.current_thread())
 
         # update the "real" _xref_cache from the one we just built
         with self._xref_cache_lock:
             self._xref_cache = self._xref_cache_bg.copy()
 
     def _histSetupMenu(self):
         self.histmenu.clear()
```

### Comparing `vivisect-1.1.0/vivisect/qt/funcviews.py` & `vivisect-1.1.1/vivisect/qt/funcviews.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/qt/main.py` & `vivisect-1.1.1/vivisect/qt/main.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/qt/memory.py` & `vivisect-1.1.1/vivisect/qt/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         self.addHotKey('ctrl+2', 'viv:make:number:two')
         self.addHotKey('ctrl+4', 'viv:make:number:four')
         self.addHotKey('ctrl+6', 'viv:make:number:sixteen')
         self.addHotKey('ctrl+8', 'viv:make:number:eight')
 
         self.addHotKey('down', 'viv:nav:nextva')
         self.addHotKey('up', 'viv:nav:prevva')
+        self.addHotKey('pgdown', 'viv:nav:nextpage')
+        self.addHotKey('pgup', 'viv:nav:prevpage')
         self.addHotKey('ctrl+down', 'viv:nav:nextundef')
         self.addHotKey('ctrl+up', 'viv:nav:prevundef')
 
         self.loadHotKeys(self.vw._viv_gui._vq_settings)
 
         # All extenders must implement vivColorMap
         vqtconnect(self.vivColorMap, 'viv:colormap')
@@ -110,14 +112,30 @@
 
         loc = self.vw.getPrevLocation(self._canv_curva)
         if loc is None:
             loc = (self._canv_curva - 1, 1, None, None)
 
         self._selectVa(loc[0])
 
+    @vq_hotkey.hotkey('viv:nav:nextpage')
+    def _hotkey_nav_nextva(self):
+        if self._canv_curva is None:
+            return
+
+        self.scrollEvent()
+        return False
+
+    @vq_hotkey.hotkey('viv:nav:prevpage')
+    def _hotkey_nav_prevva(self):
+        if self._canv_curva is None:
+            return
+
+        self.scrollEvent()
+        return False
+
     @vq_hotkey.hotkey('viv:nav:nextundef')
     def _hotkey_nav_nextundef(self):
         if self._canv_curva is None:
             return
 
         vw = self.vw
         va = self._canv_curva
@@ -324,15 +342,15 @@
         if loc is not None:
             va = loc[L_VA]
         return e_mem_canvas.VQMemoryCanvas.getVaTag(self, va)
 
 
 class VQVivMemoryCanvas(VivCanvasBase):
 
-    def _wheelEventCallback(self, data):
+    def _scrollEventCallback(self, data):
         '''
         Ugh. Yes. I know this sucks.
         But we have to do this because QtWebEngine does't natively let you get the max scroll size.
         You *have* to go through javascript to get those elements, and the only way to be sure of
         the function finishing (and being able to get a value outta js) is via this callback
         mechanism they set up.
         '''
@@ -354,26 +372,28 @@
         elif spos == smin:
             firstva, firstsize = self._canv_rendvas[0]
             mapva, mapsize, mperm, mfname = self.vw.getMemoryMap(firstva)
             sizeremain = firstva - mapva
             if sizeremain:
                 self.renderMemoryPrepend(min(sizeremain, 128))
 
-    def wheelEvent(self, event):
+    def scrollEvent(self):
         page = self.page()
         page.runJavaScript('''
         var pcur = window.innerHeight + window.pageYOffset
         var scrollMaxY = Math.max(
             document.body.scrollHeight, document.documentElement.scrollHeight,
             document.body.offsetHeight, document.documentElement.offsetHeight,
             document.body.clientHeight, document.documentElement.clientHeight,
         );
         [window.innerHeight, pcur, scrollMaxY];
-        ''', self._wheelEventCallback)
+        ''', self._scrollEventCallback)
 
+    def wheelEvent(self, event):
+        self.scrollEvent()
         return e_mem_canvas.VQMemoryCanvas.wheelEvent(self, event)
 
     def _clearColorMap(self):
         page = self.page()
         page.runJavaScript('var node = document.querySelector("#cmapstyle"); node.innerHTML = "";')
 
     def _navExpression(self, expr):
```

### Comparing `vivisect-1.1.0/vivisect/qt/remote.py` & `vivisect-1.1.1/vivisect/qt/remote.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/qt/symboliks.py` & `vivisect-1.1.1/vivisect/qt/symboliks.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/qt/ustruct.py` & `vivisect-1.1.1/vivisect/qt/ustruct.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/qt/views.py` & `vivisect-1.1.1/vivisect/qt/views.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/remote/server.py` & `vivisect-1.1.1/vivisect/remote/server.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/renderers/__init__.py` & `vivisect-1.1.1/vivisect/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/reports/__init__.py` & `vivisect-1.1.1/vivisect/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/reports/overlaplocs.py` & `vivisect-1.1.1/vivisect/reports/overlaplocs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/reports/undeftargets.py` & `vivisect-1.1.1/vivisect/reports/undeftargets.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/storage/basicfile.py` & `vivisect-1.1.1/vivisect/storage/basicfile.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/storage/mpfile.py` & `vivisect-1.1.1/vivisect/storage/mpfile.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/storage/tools/convert.py` & `vivisect-1.1.1/vivisect/storage/tools/convert.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/analysis.py` & `vivisect-1.1.1/vivisect/symboliks/analysis.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/archind.py` & `vivisect-1.1.1/vivisect/symboliks/archind.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/archs/amd64.py` & `vivisect-1.1.1/vivisect/symboliks/archs/amd64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/archs/i386.py` & `vivisect-1.1.1/vivisect/symboliks/archs/i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/callconv.py` & `vivisect-1.1.1/vivisect/symboliks/callconv.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/common.py` & `vivisect-1.1.1/vivisect/symboliks/common.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/effects.py` & `vivisect-1.1.1/vivisect/symboliks/effects.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/emulator.py` & `vivisect-1.1.1/vivisect/symboliks/emulator.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/expression.py` & `vivisect-1.1.1/vivisect/symboliks/expression.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/functions.py` & `vivisect-1.1.1/vivisect/symboliks/functions.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/reducers.py` & `vivisect-1.1.1/vivisect/symboliks/reducers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/substitution.py` & `vivisect-1.1.1/vivisect/symboliks/substitution.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/data_amd64.py` & `vivisect-1.1.1/vivisect/symboliks/tests/data_amd64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/data_i386.py` & `vivisect-1.1.1/vivisect/symboliks/tests/data_i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_analysis.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_archind.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_archind.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_cache.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_callingconv.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_callingconv.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_constraints.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_effects.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_effects.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_emulator.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_emulator.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_intel.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_intel.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_reduce.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_reduce.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_substitution.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_substitution.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_translator.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/tests/test_walkTree.py` & `vivisect-1.1.1/vivisect/symboliks/tests/test_walkTree.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/symboliks/translator.py` & `vivisect-1.1.1/vivisect/symboliks/translator.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/helpers.py` & `vivisect-1.1.1/vivisect/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/linux_amd64_chown_data.py` & `vivisect-1.1.1/vivisect/tests/linux_amd64_chown_data.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/linux_amd64_libc_2_27_data.py` & `vivisect-1.1.1/vivisect/tests/linux_amd64_libc_2_27_data.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/linux_amd64_libstdc_data.py` & `vivisect-1.1.1/vivisect/tests/linux_amd64_libstdc_data.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/linux_amd64_ls_data.py` & `vivisect-1.1.1/vivisect/tests/linux_amd64_ls_data.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/linux_arm_sh_data.py` & `vivisect-1.1.1/vivisect/tests/linux_arm_sh_data.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/linux_i386_libc_2_13_data.py` & `vivisect-1.1.1/vivisect/tests/linux_i386_libc_2_13_data.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/linux_i386_libstdc_data.py` & `vivisect-1.1.1/vivisect/tests/linux_i386_libstdc_data.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/qnx_arm_ksh_data.py` & `vivisect-1.1.1/vivisect/tests/qnx_arm_ksh_data.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/switchdata.py` & `vivisect-1.1.1/vivisect/tests/switchdata.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testapihooking.py` & `vivisect-1.1.1/vivisect/tests/testapihooking.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testblob.py` & `vivisect-1.1.1/vivisect/tests/testblob.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testcodegraph.py` & `vivisect-1.1.1/vivisect/tests/testcodegraph.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testelf.py` & `vivisect-1.1.1/vivisect/tests/testelf.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testgolang.py` & `vivisect-1.1.1/vivisect/tests/testgolang.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testihex.py` & `vivisect-1.1.1/vivisect/tests/testihex.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testimpapi.py` & `vivisect-1.1.1/vivisect/tests/testimpapi.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testlinux.py` & `vivisect-1.1.1/vivisect/tests/testlinux.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testmacho.py` & `vivisect-1.1.1/vivisect/tests/testmacho.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testmalware.py` & `vivisect-1.1.1/vivisect/tests/testmalware.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testmemory.py` & `vivisect-1.1.1/vivisect/tests/testmemory.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testpe.py` & `vivisect-1.1.1/vivisect/tests/testpe.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testremote.py` & `vivisect-1.1.1/vivisect/tests/testremote.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,26 @@
     vw.loadFromFile(testfile)
     vw.setMeta('StorageName', name)
     vw.saveWorkspace()
 
     v_r_server.runMainServer(dirn, port)
 
 
+def getOutput(strcanv, timeout=10):
+    '''
+    Watches a StringCanvas for data up to a given timeout
+    '''
+    starttime = time.time()
+    output = strcanv.strval
+    while not output and (time.time() - starttime) < timeout:
+        time.sleep(.1)
+
+    strcanv.strval = ''
+    return output
+
 class VivisectRemoteTests(unittest.TestCase):
     '''
     So...what would be fun is basically a chain of remote workspaces all tied in interesting
     configurations.
     '''
     def test_basic(self):
         testfile = helpers.getTestPath('windows', 'amd64', 'firefox.exe')
@@ -144,23 +156,21 @@
 
 
                 # test the CLI:
                 rmtvw.canvas = e_mcanvas.StringMemoryCanvas(rmtvw)
 
                 # empty leaders
                 rmtvw.do_leaders('')
-                output = rmtvw.canvas.strval
+                output = getOutput(rmtvw.canvas)
                 self.assertIn('Manage Leader Sessions.', output)
-                rmtvw.canvas.strval = ''
 
                 # list leaders
                 rmtvw.do_leaders('list')
-                output = rmtvw.canvas.strval
+                output = getOutput(rmtvw.canvas)
                 self.assertIn("rakuy0's moving castle", output)
-                rmtvw.canvas.strval = ''
 
                 # modify a leader session
                 rmtvw.do_leaders('mod %s foo foo bar baz' % testuuid)
                 retry = 0
                 while retry < 5:
                     ldrsess = rmtvw2.getLeaderSessions().get(testuuid)
                     if ldrsess:
@@ -168,33 +178,31 @@
                         if user == 'foo':
                             break
 
                     retry += 1
                     time.sleep(.1)
                     sys.stderr.write('%d' % retry)
 
-                output = rmtvw.canvas.strval
+                output = getOutput(rmtvw.canvas)
                 self.assertIn("foo bar baz", output)
-                rmtvw.canvas.strval = ''
 
                 # kill leader session
                 rmtvw.do_leaders('kill %s' % testuuid)
                 retry = 0
                 while retry < 5:
                     ldrsess = rmtvw2.getLeaderSessions().get(testuuid)
                     if not ldrsess:
                         break
 
                     retry += 1
                     time.sleep(.1)
                     sys.stderr.write('%d' % retry)
 
-                output = rmtvw.canvas.strval
+                output = getOutput(rmtvw.canvas)
                 self.assertIn("*Ended: foo's session 'foo bar baz'", output)
-                rmtvw.canvas.strval = ''
 
 
                 # kill all (which means we need to add a few)
                 #   repopulate
                 rmtvw.iAmLeader(testuuid+'1', "castle 1")
                 rmtvw.iAmLeader(testuuid+'2', "castle 2")
                 rmtvw.iAmLeader(testuuid+'3', "castle 3")
@@ -218,18 +226,17 @@
                     if not len(ldrsessions):
                         break
 
                     retry += 1
                     time.sleep(.1)
                     sys.stderr.write('%d' % retry)
 
-                output = rmtvw.canvas.strval
+                output = getOutput(rmtvw.canvas)
                 self.assertIn("castle 3", output)
                 self.assertEqual(len(rmtvw2.getLeaderSessions()), 0)
-                rmtvw.canvas.strval = ''
 
 
                 # close down tests
                 try:
                     rmtvw.server = None
                     rmtvw2.server = None
```

### Comparing `vivisect-1.1.0/vivisect/tests/testreports.py` & `vivisect-1.1.1/vivisect/tests/testreports.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testsrec.py` & `vivisect-1.1.1/vivisect/tests/testsrec.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/teststability.py` & `vivisect-1.1.1/vivisect/tests/teststability.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/teststorage.py` & `vivisect-1.1.1/vivisect/tests/teststorage.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/teststruct.py` & `vivisect-1.1.1/vivisect/tests/teststruct.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testswitches.py` & `vivisect-1.1.1/vivisect/tests/testswitches.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testvampsigs.py` & `vivisect-1.1.1/vivisect/tests/testvampsigs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testvivgraph.py` & `vivisect-1.1.1/vivisect/tests/testvivgraph.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testvivisect.py` & `vivisect-1.1.1/vivisect/tests/testvivisect.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/testvivisect_multi.py` & `vivisect-1.1.1/vivisect/tests/testvivisect_multi.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tests/utils.py` & `vivisect-1.1.1/vivisect/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tools/fscope.py` & `vivisect-1.1.1/vivisect/tools/fscope.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/tools/graphutil.py` & `vivisect-1.1.1/vivisect/tools/graphutil.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/vamp/__init__.py` & `vivisect-1.1.1/vivisect/vamp/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/vamp/msvc/__init__.py` & `vivisect-1.1.1/vivisect/vamp/msvc/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/vdbext.py` & `vivisect-1.1.1/vivisect/vdbext.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/vector.py` & `vivisect-1.1.1/vivisect/vector.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect/vivbin.py` & `vivisect-1.1.1/vivisect/vivbin.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vivisect.egg-info/PKG-INFO` & `vivisect-1.1.1/vivisect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivisect
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pure python disassembler, debugger, emulator, and static analysis framework
 Home-page: https://github.com/vivisect/vivisect
 Author: The Vivisect Peeps
 Author-email: 
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Disassemblers
 Classifier: Topic :: Software Development :: Debuggers
```

### Comparing `vivisect-1.1.0/vivisect.egg-info/SOURCES.txt` & `vivisect-1.1.1/vivisect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vqt/application.py` & `vivisect-1.1.1/vqt/application.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vqt/basics.py` & `vivisect-1.1.1/vqt/basics.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vqt/cli.py` & `vivisect-1.1.1/vqt/cli.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vqt/colors.py` & `vivisect-1.1.1/vqt/colors.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vqt/common.py` & `vivisect-1.1.1/vqt/common.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vqt/hotkeys.py` & `vivisect-1.1.1/vqt/hotkeys.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     0x1000000: 'esc',
     0x1000003: 'bs',
     0x1000004: 'enter',
     0x1000012: 'left',
     0x1000013: 'up',
     0x1000014: 'right',
     0x1000015: 'down',
+    0x1000016: 'pgup',
+    0x1000017: 'pgdown',
 }
 
 fkey_base = 0x100002f
 for i in range(1,12):
     special_keys[ fkey_base + i ] = 'f%d' % i
 
 def hotkey(targname):
@@ -142,15 +144,18 @@
     def eatKeyPressEvent(self, event):
         hotkey = self.getHotKeyFromEvent(event)
 
         target = self._vq_hotkeys.get(hotkey)
         if target is not None:
             callback, args, kwargs = self._vq_hotkey_targets.get(target)
             try:
-                callback(*args, **kwargs)
+                cbret = callback(*args, **kwargs)
+                # if callback returns False, let the default behavior happen
+                if cbret == False:
+                    return False
             except:
                 logger.warning("error in eatKeyPressEvent(%r, %r, %r)", event, args, kwargs)
                 logger.debug(''.join(traceback.format_exception(*sys.exc_info())))
 
             event.accept()
             return True
```

### Comparing `vivisect-1.1.0/vqt/main.py` & `vivisect-1.1.1/vqt/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import logging
 import functools
 
 from queue import Queue
-from threading import currentThread
+from threading import current_thread
 
 from PyQt5 import QtCore
 from PyQt5.QtWidgets import *
 
 import envi.threads as e_threads
 
 logger = logging.getLogger(__name__)
@@ -33,30 +33,30 @@
 def workthread(func):
     '''
     Proxy a call through the single vqt.main worker thread
     (who exists to keep the GUI from blocking on stuff... )
     '''
     # If we're already the work thread, just do it.
     def workadd(*args, **kwargs):
-        if getattr(currentThread(),'VQtWorkerThread',False):
+        if getattr(current_thread(),'VQtWorkerThread',False):
             return func(*args, **kwargs)
 
         workerq.append( (func,args,kwargs) )
 
     functools.update_wrapper(workadd,func)
     return workadd
 
 def boredthread(func):
     '''
     The same as "workthread" above, but drop the request on the
     floor if the worker thread already has better things to do...
     '''
     # If we're already the work thread, just do it.
     def workadd(*args, **kwargs):
-        if getattr(currentThread(),'VQtWorkerThread',False):
+        if getattr(current_thread(),'VQtWorkerThread',False):
             return func(*args, **kwargs)
 
         if not len(workerq):
             workerq.append( (func,args,kwargs) )
 
     functools.update_wrapper(workadd,func)
     return workadd
@@ -100,15 +100,15 @@
         func._qt_thread.start()
         return func._qt_thread
 
     functools.update_wrapper(doqtthread,func)
     return doqtthread
 
 def iAmQtSafeThread():
-    return getattr(currentThread(),'QtSafeThread',False)
+    return getattr(current_thread(),'QtSafeThread',False)
 
 class QEventThread(QtCore.QThread):
     '''
     A thread who exists to consume callback requests from the
     given workq and fire them into Qt *safely*.
     '''
     idleadd = QtCore.pyqtSignal(object, object, object)
@@ -149,15 +149,15 @@
 class QEventChannel(QtCore.QObject):
     guievents = QtCore.pyqtSignal(str,object)
 
 
 @e_threads.firethread
 def workerThread():
     # We are *not* allowed to make Qt API calls
-    currentThread().VQtWorkerThread = True
+    current_thread().VQtWorkerThread = True
     while True:
         try:
             todo = workerq.get()
             if todo is not None:
                 func, args, kwargs = todo
 
                 if func is None:
@@ -185,15 +185,15 @@
     if isGuiStarted():
         print("Returning from startup... already QApplication running")
         return
 
     guiq = e_threads.EnviQueue()
     workerq = e_threads.EnviQueue()
 
-    currentThread().QtSafeThread = True
+    current_thread().QtSafeThread = True
     qapp = VQApplication(sys.argv)
     if css:
         qapp.setStyleSheet( css )
 
     ethread = QEventThread(guiq)
     ethread.idleadd.connect( qapp.callFromQtLoop )
     ethread.start()
```

### Comparing `vivisect-1.1.0/vqt/menubuilder.py` & `vivisect-1.1.1/vqt/menubuilder.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vqt/qpython.py` & `vivisect-1.1.1/vqt/qpython.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 from vqt.basics import *
 from vqt.common import scripterr
 
 
 class ScriptThread(Thread):
 
     def __init__(self, cobj, locals):
-        Thread.__init__(self)
-        self.setDaemon(True)
+        super.__init__(self, daemon=True)
         self.cobj = cobj
         self.locals = locals
 
     def run(self):
         try:
             exec(self.cobj, self.locals)
         except Exception as e:
```

### Comparing `vivisect-1.1.0/vqt/saveable.py` & `vivisect-1.1.1/vqt/saveable.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vqt/tree.py` & `vivisect-1.1.1/vqt/tree.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/__init__.py` & `vivisect-1.1.1/vstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/bitfield.py` & `vivisect-1.1.1/vstruct/bitfield.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/builder.py` & `vivisect-1.1.1/vstruct/builder.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/constants/__init__.py` & `vivisect-1.1.1/vstruct/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/constants/ntstatus.py` & `vivisect-1.1.1/vstruct/constants/ntstatus.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/cparse.py` & `vivisect-1.1.1/vstruct/cparse.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/arm7/__init__.py` & `vivisect-1.1.1/vstruct/defs/arm7/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/bmp.py` & `vivisect-1.1.1/vstruct/defs/bmp.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/constants/elf.py` & `vivisect-1.1.1/vstruct/defs/constants/elf.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/dns.py` & `vivisect-1.1.1/vstruct/defs/dns.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/elf.py` & `vivisect-1.1.1/vstruct/defs/elf.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/gif.py` & `vivisect-1.1.1/vstruct/defs/gif.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/ihex.py` & `vivisect-1.1.1/vstruct/defs/ihex.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/inet.py` & `vivisect-1.1.1/vstruct/defs/inet.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/java.py` & `vivisect-1.1.1/vstruct/defs/java.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/kdcom.py` & `vivisect-1.1.1/vstruct/defs/kdcom.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/macho/__init__.py` & `vivisect-1.1.1/vstruct/defs/macho/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/macho/const.py` & `vivisect-1.1.1/vstruct/defs/macho/const.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/macho/fat.py` & `vivisect-1.1.1/vstruct/defs/macho/fat.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/macho/loader.py` & `vivisect-1.1.1/vstruct/defs/macho/loader.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/macho/signing.py` & `vivisect-1.1.1/vstruct/defs/macho/signing.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/macho/stabs.py` & `vivisect-1.1.1/vstruct/defs/macho/stabs.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/minidump.py` & `vivisect-1.1.1/vstruct/defs/minidump.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/pcap.py` & `vivisect-1.1.1/vstruct/defs/pcap.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/pe.py` & `vivisect-1.1.1/vstruct/defs/pe.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/pptp.py` & `vivisect-1.1.1/vstruct/defs/pptp.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/rar.py` & `vivisect-1.1.1/vstruct/defs/rar.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/srec.py` & `vivisect-1.1.1/vstruct/defs/srec.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/swf.py` & `vivisect-1.1.1/vstruct/defs/swf.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/win32.py` & `vivisect-1.1.1/vstruct/defs/win32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/__init__.py` & `vivisect-1.1.1/vstruct/defs/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_5_1_i386/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_5_1_i386/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_5_1_i386/ntoskrnl.py` & `vivisect-1.1.1/vstruct/defs/windows/win_5_1_i386/ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_5_1_i386/win32k.py` & `vivisect-1.1.1/vstruct/defs/windows/win_5_1_i386/win32k.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_5_2_i386/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_5_2_i386/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_5_2_i386/ntoskrnl.py` & `vivisect-1.1.1/vstruct/defs/windows/win_5_2_i386/ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_5_2_i386/win32k.py` & `vivisect-1.1.1/vstruct/defs/windows/win_5_2_i386/win32k.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_1_amd64/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_1_amd64/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_1_amd64/ntoskrnl.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_1_amd64/ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_1_amd64/win32k.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_1_amd64/win32k.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_1_i386/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_1_i386/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_1_i386/ntoskrnl.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_1_i386/ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_1_i386/win32k.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_1_i386/win32k.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_1_wow64/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_1_wow64/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_2_amd64/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_2_amd64/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_2_amd64/ntoskrnl.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_2_amd64/ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_2_i386/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_2_i386/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_2_i386/ntoskrnl.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_2_i386/ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_2_wow64/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_2_wow64/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_3_amd64/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_3_amd64/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_3_amd64/ntoskrnl.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_3_amd64/ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_3_i386/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_3_i386/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_3_i386/ntoskrnl.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_3_i386/ntoskrnl.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/defs/windows/win_6_3_wow64/ntdll.py` & `vivisect-1.1.1/vstruct/defs/windows/win_6_3_wow64/ntdll.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/primitives.py` & `vivisect-1.1.1/vstruct/primitives.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/qt/__init__.py` & `vivisect-1.1.1/vstruct/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/tests/test_builder.py` & `vivisect-1.1.1/vstruct/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/tests/testbasic.py` & `vivisect-1.1.1/vstruct/tests/testbasic.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/tests/tests_vstruct.py` & `vivisect-1.1.1/vstruct/tests/tests_vstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,19 +43,19 @@
         self.assertIs(fobj, self.s.vsGetField('four'))
 
     def test_vsGetFieldByOffset_maxval_neg(self):
         with self.assertRaisesRegex(Exception, 'Invalid Offset Specified'):
             tup = self.s.vsGetFieldByOffset(-1)
 
     def test_vsGetFieldByOffset_maxval_pos(self):
-        with self.assertRaisesRegexp(Exception, 'Invalid Offset Specified'):
+        with self.assertRaisesRegex(Exception, 'Invalid Offset Specified'):
             tup = self.s.vsGetFieldByOffset(0xffffffff)
 
     def test_vsGetFieldByOffset_maxval_plus1_pos(self):
-        with self.assertRaisesRegexp(Exception, 'Invalid Offset Specified'):
+        with self.assertRaisesRegex(Exception, 'Invalid Offset Specified'):
             tup = self.s.vsGetFieldByOffset(len(self.s))
 
     def test_vsGetFieldByOffset_nested1(self):
         fname, fobj = self.s.vsGetFieldByOffset(5)
         self.assertEqual(fname, 'two.foo')
         self.assertIs(fobj, self.s.two.vsGetField('foo'))
```

### Comparing `vivisect-1.1.0/vstruct/tools/dumpihex.py` & `vivisect-1.1.1/vstruct/tools/dumpihex.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vstruct/tools/dumpjava.py` & `vivisect-1.1.1/vstruct/tools/dumpjava.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/__init__.py` & `vivisect-1.1.1/vtrace/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/archs/amd64.py` & `vivisect-1.1.1/vtrace/archs/amd64.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/archs/i386.py` & `vivisect-1.1.1/vtrace/archs/i386.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/archs/ppc.py` & `vivisect-1.1.1/vtrace/archs/ppc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/audit.py` & `vivisect-1.1.1/vtrace/audit.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/breakpoints.py` & `vivisect-1.1.1/vtrace/breakpoints.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/const.py` & `vivisect-1.1.1/vtrace/const.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/envitools.py` & `vivisect-1.1.1/vtrace/envitools.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/notifiers.py` & `vivisect-1.1.1/vtrace/notifiers.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/base.py` & `vivisect-1.1.1/vtrace/platforms/base.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/darwin/__init__.py` & `vivisect-1.1.1/vtrace/platforms/darwin/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/darwin/exc.h` & `vivisect-1.1.1/vtrace/platforms/darwin/exc.h`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/darwin/excServer.c` & `vivisect-1.1.1/vtrace/platforms/darwin/excServer.c`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/darwin/excUser.c` & `vivisect-1.1.1/vtrace/platforms/darwin/excUser.c`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/darwin/machhelper.c` & `vivisect-1.1.1/vtrace/platforms/darwin/machhelper.c`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/darwin/machhelper.dylib` & `vivisect-1.1.1/vtrace/platforms/darwin/machhelper.dylib`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/freebsd.py` & `vivisect-1.1.1/vtrace/platforms/freebsd.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/gdbstub.py` & `vivisect-1.1.1/vtrace/platforms/gdbstub.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/linux.py` & `vivisect-1.1.1/vtrace/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/posix.py` & `vivisect-1.1.1/vtrace/platforms/posix.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/solaris.py` & `vivisect-1.1.1/vtrace/platforms/solaris.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/vmware.py` & `vivisect-1.1.1/vtrace/platforms/vmware.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/win32.py` & `vivisect-1.1.1/vtrace/platforms/win32.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/windll/amd64/dbghelp.dll` & `vivisect-1.1.1/vtrace/platforms/windll/amd64/dbghelp.dll`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/windll/amd64/symsrv.dll` & `vivisect-1.1.1/vtrace/platforms/windll/amd64/symsrv.dll`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/windll/i386/dbghelp.dll` & `vivisect-1.1.1/vtrace/platforms/windll/i386/dbghelp.dll`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/windll/i386/symsrv.dll` & `vivisect-1.1.1/vtrace/platforms/windll/i386/symsrv.dll`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/platforms/winkern.py` & `vivisect-1.1.1/vtrace/platforms/winkern.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/qt.py` & `vivisect-1.1.1/vtrace/qt.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/rmi.py` & `vivisect-1.1.1/vtrace/rmi.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/snapshot.py` & `vivisect-1.1.1/vtrace/snapshot.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tests/__init__.py` & `vivisect-1.1.1/vtrace/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tests/test_expressions.py` & `vivisect-1.1.1/vtrace/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tests/test_symcache.py` & `vivisect-1.1.1/vtrace/tests/test_symcache.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tests/testbasic.py` & `vivisect-1.1.1/vtrace/tests/testbasic.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tests/tests_breakpoints.py` & `vivisect-1.1.1/vtrace/tests/tests_breakpoints.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tests/testthread.py` & `vivisect-1.1.1/vtrace/tests/testthread.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tests/testwritemem.py` & `vivisect-1.1.1/vtrace/tests/testwritemem.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tools/iathook.py` & `vivisect-1.1.1/vtrace/tools/iathook.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tools/win32alloc.py` & `vivisect-1.1.1/vtrace/tools/win32alloc.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tools/win32aslr.py` & `vivisect-1.1.1/vtrace/tools/win32aslr.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tools/win32heap.py` & `vivisect-1.1.1/vtrace/tools/win32heap.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/tools/win32stealth.py` & `vivisect-1.1.1/vtrace/tools/win32stealth.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/util.py` & `vivisect-1.1.1/vtrace/util.py`

 * *Files identical despite different names*

### Comparing `vivisect-1.1.0/vtrace/watchpoints.py` & `vivisect-1.1.1/vtrace/watchpoints.py`

 * *Files identical despite different names*

