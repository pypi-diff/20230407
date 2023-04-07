# Comparing `tmp/waterline-0.1.4-py3-none-any.whl.zip` & `tmp/waterline-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,68 @@
-Zip file size: 7595 bytes, number of entries: 11
--rw-rw-r--  2.0 unx      106 b- defN 23-Apr-05 02:12 waterline/__init__.py
--rw-rw-r--  2.0 unx      729 b- defN 23-Apr-05 20:12 waterline/pipeline.py
--rw-rw-r--  2.0 unx     2708 b- defN 23-Apr-05 20:28 waterline/suite.py
--rw-rw-r--  2.0 unx     6610 b- defN 23-Apr-05 20:29 waterline/suites.py
--rw-rw-r--  2.0 unx      494 b- defN 23-Apr-05 20:28 waterline/utils.py
--rw-rw-r--  2.0 unx     4168 b- defN 23-Apr-05 20:28 waterline/workspace.py
--rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-05 20:30 waterline-0.1.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx      256 b- defN 23-Apr-05 20:30 waterline-0.1.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-05 20:30 waterline-0.1.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Apr-05 20:30 waterline-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      853 b- defN 23-Apr-05 20:30 waterline-0.1.4.dist-info/RECORD
-11 files, 17083 bytes uncompressed, 6161 bytes compressed:  63.9%
+Zip file size: 6215066 bytes, number of entries: 66
+-rw-rw-r--  2.0 unx      205 b- defN 23-Apr-07 20:48 waterline/__init__.py
+-rw-rw-r--  2.0 unx     1805 b- defN 23-Apr-07 00:51 waterline/jobs.py
+-rw-rw-r--  2.0 unx      792 b- defN 23-Apr-06 16:35 waterline/pipeline.py
+-rw-rw-r--  2.0 unx      290 b- defN 23-Apr-07 20:58 waterline/run.py
+-rw-rw-r--  2.0 unx     3382 b- defN 23-Apr-07 20:58 waterline/suite.py
+-rw-rw-r--  2.0 unx     7123 b- defN 23-Apr-06 17:01 waterline/suites.py
+-rw-rw-r--  2.0 unx      486 b- defN 23-Apr-06 14:11 waterline/utils.py
+-rw-rw-r--  2.0 unx     4958 b- defN 23-Apr-07 20:56 waterline/workspace.py
+-rw-rw-r--  2.0 unx      135 b- defN 23-Apr-07 15:59 waterline/suites/__init__.py
+-rw-rw-r--  2.0 unx     1484 b- defN 23-Apr-06 21:03 waterline/suites/gap.py
+-rw-rw-r--  2.0 unx     8637 b- defN 23-Apr-06 21:01 waterline/suites/mibench.py
+-rw-rw-r--  2.0 unx     2528 b- defN 23-Apr-06 21:02 waterline/suites/nas.py
+-rw-rw-r--  2.0 unx     3478 b- defN 23-Apr-07 18:33 waterline/suites/polybench.py
+-rw-rw-r--  2.0 unx     2079 b- defN 23-Apr-07 20:36 waterline/suites/spec2017.py
+-rw-rw-r--  2.0 unx     1297 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/Makefile
+-rw-rw-r--  2.0 unx     2959 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/README
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-07 16:10 waterline/suites/SPEC2017/test.txt
+-rwxrwxr-x  2.0 unx  4511744 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/benchmarks/omnetpp_s/omnetpp_s
+-rw-rw-r--  2.0 unx  5067012 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/benchmarks/omnetpp_s/omnetpp_s.bc
+-rwxrwxr-x  2.0 unx 12596976 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/benchmarks/xalancbmk_s/xalancbmk_s
+-rw-rw-r--  2.0 unx      446 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/Makefile
+-rwxrwxr-x  2.0 unx      296 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/bin/run.sh
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/doc/README
+-rw-rw-r--  2.0 unx       17 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/log/README
+-rw-rw-r--  2.0 unx      854 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/binary.con
+-rwxrwxr-x  2.0 unx      365 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/binary.sh
+-rwxrwxr-x  2.0 unx     1141 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/clean.sh
+-rwxrwxr-x  2.0 unx     1713 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/compareTimes.sh
+-rw-rw-r--  2.0 unx     1435 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/generateCondorScript.py
+-rwxrwxr-x  2.0 unx      890 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/generateCondorScript.sh
+-rw-rw-r--  2.0 unx      813 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/optimize.con
+-rwxrwxr-x  2.0 unx      474 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/optimize.sh
+-rw-rw-r--  2.0 unx      889 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/run.con
+-rwxrwxr-x  2.0 unx      753 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/run.sh
+-rw-rw-r--  2.0 unx      864 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/speedup.con
+-rwxrwxr-x  2.0 unx     2483 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/speedup.sh
+-rwxrwxr-x  2.0 unx       82 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/condor/scripts/submit.sh
+-rw-rw-r--  2.0 unx     2129 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/makefiles/Makefile
+-rwxrwxr-x  2.0 unx      433 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/makefiles/download.sh
+-rwxrwxr-x  2.0 unx      342 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/makefiles/fetchRuntime.sh
+-rwxrwxr-x  2.0 unx      236 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/makefiles/run.sh
+-rw-rw-r--  2.0 unx    17132 b- defN 23-Apr-07 18:26 waterline/suites/SPEC2017/patches/gclang.cfg
+-rw-rw-r--  2.0 unx    10360 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/patches/parest_r_patch.tar.xz
+-rw-rw-r--  2.0 unx      475 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/patches/pure_c_cpp_rate.bset
+-rw-rw-r--  2.0 unx      466 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/patches/pure_c_cpp_speed.bset
+-rw-rw-r--  2.0 unx       79 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/patches/SPEC2017/README
+-rw-rw-r--  2.0 unx       55 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/plot/Makefile
+-rw-rw-r--  2.0 unx     2201 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/plot/barplot.py
+-rwxrwxr-x  2.0 unx       71 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/plot/barplot.sh
+-rw-rw-r--  2.0 unx       21 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/plot/barplot.txt
+-rwxrwxr-x  2.0 unx      393 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/plot/virtualEnv.sh
+-rwxrwxr-x  2.0 unx     1516 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/scripts/binary.sh
+-rwxrwxr-x  2.0 unx     2323 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/scripts/bitcode.sh
+-rwxrwxr-x  2.0 unx      650 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/scripts/bitcode_copy.sh
+-rwxrwxr-x  2.0 unx     2024 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/scripts/collect_output.sh
+-rwxrwxr-x  2.0 unx      423 b- defN 23-Apr-07 16:50 waterline/suites/SPEC2017/scripts/compile.sh
+-rwxrwxr-x  2.0 unx      586 b- defN 23-Apr-07 16:24 waterline/suites/SPEC2017/scripts/install.sh
+-rwxrwxr-x  2.0 unx     1410 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/scripts/optimization.sh
+-rwxrwxr-x  2.0 unx     2626 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/scripts/run.sh
+-rwxrwxr-x  2.0 unx     2757 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/scripts/setup.sh
+-rwxrwxr-x  2.0 unx      267 b- defN 23-Apr-07 16:15 waterline/suites/SPEC2017/scripts/uninstall.sh
+-rw-rw-r--  2.0 unx     1057 b- defN 23-Apr-07 21:22 waterline-0.1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      246 b- defN 23-Apr-07 21:22 waterline-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-07 21:22 waterline-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-07 21:22 waterline-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6386 b- defN 23-Apr-07 21:22 waterline-0.1.5.dist-info/RECORD
+66 files, 22289108 bytes uncompressed, 6204606 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,34 +1,199 @@
 Filename: waterline/__init__.py
 Comment: 
 
+Filename: waterline/jobs.py
+Comment: 
+
 Filename: waterline/pipeline.py
 Comment: 
 
+Filename: waterline/run.py
+Comment: 
+
 Filename: waterline/suite.py
 Comment: 
 
 Filename: waterline/suites.py
 Comment: 
 
 Filename: waterline/utils.py
 Comment: 
 
 Filename: waterline/workspace.py
 Comment: 
 
-Filename: waterline-0.1.4.dist-info/LICENSE
+Filename: waterline/suites/__init__.py
+Comment: 
+
+Filename: waterline/suites/gap.py
+Comment: 
+
+Filename: waterline/suites/mibench.py
+Comment: 
+
+Filename: waterline/suites/nas.py
+Comment: 
+
+Filename: waterline/suites/polybench.py
+Comment: 
+
+Filename: waterline/suites/spec2017.py
+Comment: 
+
+Filename: waterline/suites/SPEC2017/Makefile
+Comment: 
+
+Filename: waterline/suites/SPEC2017/README
+Comment: 
+
+Filename: waterline/suites/SPEC2017/test.txt
+Comment: 
+
+Filename: waterline/suites/SPEC2017/benchmarks/omnetpp_s/omnetpp_s
+Comment: 
+
+Filename: waterline/suites/SPEC2017/benchmarks/omnetpp_s/omnetpp_s.bc
+Comment: 
+
+Filename: waterline/suites/SPEC2017/benchmarks/xalancbmk_s/xalancbmk_s
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/Makefile
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/bin/run.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/doc/README
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/log/README
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/binary.con
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/binary.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/clean.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/compareTimes.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/generateCondorScript.py
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/generateCondorScript.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/optimize.con
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/optimize.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/run.con
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/run.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/speedup.con
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/speedup.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/condor/scripts/submit.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/makefiles/Makefile
+Comment: 
+
+Filename: waterline/suites/SPEC2017/makefiles/download.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/makefiles/fetchRuntime.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/makefiles/run.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/patches/gclang.cfg
+Comment: 
+
+Filename: waterline/suites/SPEC2017/patches/parest_r_patch.tar.xz
+Comment: 
+
+Filename: waterline/suites/SPEC2017/patches/pure_c_cpp_rate.bset
+Comment: 
+
+Filename: waterline/suites/SPEC2017/patches/pure_c_cpp_speed.bset
+Comment: 
+
+Filename: waterline/suites/SPEC2017/patches/SPEC2017/README
+Comment: 
+
+Filename: waterline/suites/SPEC2017/plot/Makefile
+Comment: 
+
+Filename: waterline/suites/SPEC2017/plot/barplot.py
+Comment: 
+
+Filename: waterline/suites/SPEC2017/plot/barplot.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/plot/barplot.txt
+Comment: 
+
+Filename: waterline/suites/SPEC2017/plot/virtualEnv.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/binary.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/bitcode.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/bitcode_copy.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/collect_output.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/compile.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/install.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/optimization.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/run.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/setup.sh
+Comment: 
+
+Filename: waterline/suites/SPEC2017/scripts/uninstall.sh
+Comment: 
+
+Filename: waterline-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: waterline-0.1.4.dist-info/METADATA
+Filename: waterline-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: waterline-0.1.4.dist-info/WHEEL
+Filename: waterline-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: waterline-0.1.4.dist-info/top_level.txt
+Filename: waterline-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: waterline-0.1.4.dist-info/RECORD
+Filename: waterline-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## waterline/__init__.py

```diff
@@ -1,5 +1,6 @@
 from __future__ import annotations
-
-
 from .workspace import Workspace
 from .suite import Suite, Benchmark
+from .run import RunConfiguration
+
+__all__ = ["Workspace", "Suite", "Benchmark", "RunConfiguration"]
```

## waterline/pipeline.py

```diff
@@ -1,26 +1,27 @@
 from pathlib import Path
 import shutil
 from .suite import Benchmark
+from . import jobs
 
 
 class Pipeline:
     def __init__(self, name: str):
         self.name = name
         self.stages = []
 
-    def add_stage(self, stage):
-        self.stages.append(stage)
+    def add_stage(self, stage, name=None):
+        self.stages.append((stage, name))
 
     def run(self, input_bc: Path, output_bc: Path, bench: Benchmark):
-      shutil.copy(input_bc, output_bc)
-      dir = output_bc.parent
-      for i, stage in enumerate(self.stages):
-          stage(output_bc)
+        shutil.copy(input_bc, output_bc)
+        dir = output_bc.parent
+        for i, stage in enumerate(self.stages):
+            stage(output_bc)
 
     def create_jobs(self, input_bc: Path, output_bc: Path, bench: Benchmark):
         shutil.copy(input_bc, output_bc)
 
-        jobs = []
-        for i, stage in enumerate(self.stages):
-            jobs.append((f'{self.name} stage {i+1}', stage, output_bc))
-        return jobs
+        out = []
+        for i, (stage, name) in enumerate(self.stages):
+            out.append(jobs.FunctionJob(f"stage {i+1}: {name}", stage, output_bc))
+        return out
```

## waterline/suite.py

```diff
@@ -1,94 +1,116 @@
-
 from pathlib import Path
 from typing import List
+from .run import RunConfiguration
+from . import jobs
+
 
-class Runner:
+class JobRunner:
     pass
 
 
-class ShellRunner(Runner):
+class ShellRunner(JobRunner):
     pass
 
 
-class TimeRunner(Runner):
+class TimeRunner(JobRunner):
     pass
 
 
-class CondorRunner(Runner):
+class CondorRunner(JobRunner):
     pass
 
 
 class Suite:
     """
     A suite is a standard benchmark suite, which contains multiple Benchmark instances.
     The main functionality of a Suite is to fetch the contents of a benchmark, initialize
     the benchmark with patches or configuration, and to expose each benchmark as a
     `waterline.Benchmark` that can be put through the benchmarking pipeline defined by the
     user. A suite also defines how a benchmark is converted from bitcode to an executable.
     """
 
-    name = 'unknown'
+    name = "unknown"
 
     def __init__(self, workspace):
         """
         Initialize the benchmark suite with a context and a name
         """
         self.workspace = workspace
         self.benchmarks: List[Benchmark] = []
 
         self.src = self.workspace.src_dir / self.name
         self.bin = self.workspace.bin_dir / self.name
         self.ir = self.workspace.ir_dir / self.name
 
     def configure(self, *args, **kwargs):
         """
-        Called by the Workspace to initialize this benchmark suite with 
+        Called by the Workspace to initialize this benchmark suite with
         """
         pass
 
     def acquire(self):
         """
         Download, clone, or otherwise acquire the benchmark suite into a certain path.
-        This function also emits 
+        This function also emits
         """
-        print(f'acquire suite {self.name} to {self.src}')
+        print(f"acquire suite {self.name} to {self.src}")
 
-    def add_benchmark(self, benchmark, name: str, *args):
-        self.benchmarks.append(benchmark(self, name, *args))
+    def add_benchmark(self, benchmark, name: str, *args, **kwargs):
+        self.benchmarks.append(benchmark(self, name, *args, **kwargs))
 
-    def get_compile_jobs(self):
+    def compile_jobs(self):
         """
-        Compile each of the benchmarks in the suite. By default this 
+        Compile each of the benchmarks in the suite. By default this
         simply defers to each benchmark, but it could do it some other
         way if the suite has a goofy build system.
         """
 
-        jobs = []
         for benchmark in self.benchmarks:
             bench_bin_dir = self.bin / benchmark.name
             bench_bin_dir.mkdir(exist_ok=True)
 
-            bin_file = bench_bin_dir / 'a.out'
+            bin_file = bench_bin_dir / "a.out"
             if not bin_file.exists():
-                jobs.append((f'compile {self.name}/{benchmark.name}', benchmark.compile, bin_file))
-        return jobs
+                yield jobs.FunctionJob(
+                    f"compile {self.name}/{benchmark.name}",
+                    benchmark.compile,
+                    bin_file,
+                )
+
 
 class Benchmark:
     def __init__(self, suite: Suite, name: str):
         self.suite = suite
         self.name = name
 
+    def __repr__(self):
+        return f"Benchmark({self.suite.name},{self.name})"
+
+    def run_configs(self):
+        yield RunConfiguration(self.name)
+
     def compile(self, output: Path):
         """
         Compile this benchmark to a certain output file
         """
         pass
 
-    def link(self, bitcode: Path, destination: Path):
+    def link(self, object: Path, destination: Path):
         """
-        Link a bitcode file of this benchmark into a complete executable.
+        Link an object file of this benchmark into a complete executable.
         """
-        print(f'link {bitcode} to {destination} not implemented')
+        print(f"link {object} to {destination} not implemented")
+
+    def link_bitcode(self, bitcode: Path, destination: Path):
+        """
+        Compile a bitcode file to an object file, then link the object file to the destination
+        using `self.link()`
+        """
+        object = bitcode.parent / (bitcode.stem + ".o")
+        self.shell("llc", "-O3", bitcode, "--filetype=obj", "-o", object)
+
+        self.link(object, destination)
+        pass
 
     def shell(self, *args):
         self.suite.workspace.shell(*args)
```

## waterline/suites.py

```diff
@@ -1,159 +1,204 @@
 from waterline import Suite, Benchmark, Workspace
 from waterline.utils import run_command
 from pathlib import Path
 import waterline.utils
 import shutil
 from typing import Tuple
 
+
 class NASBenchmark(Benchmark):
     def compile(self, output: Path):
         """
         Compile this benchmark to a certain output directory
         """
-        self.shell('make', '-C', self.suite.src, self.name,
-                   f'CLASS={self.suite.suite_class}')
+        self.shell(
+            "make", "-C", self.suite.src, self.name, f"CLASS={self.suite.suite_class}"
+        )
         # if that compiled, copy the binary to the right location
-        compiled = self.suite.src / 'bin' / \
-            (self.name + '.' + self.suite.suite_class)
+        compiled = self.suite.src / "bin" / (self.name + "." + self.suite.suite_class)
         shutil.copy(compiled, output)
 
     def link(self, bitcode: Path, dest: Path):
-        self.shell('clang', '-lomp', bitcode, '-o', dest, '-lm', '-fopenmp')
+        self.shell("clang", "-lomp", bitcode, "-o", dest, "-lm", "-fopenmp")
 
 
 class NAS(Suite):
-    name = 'NAS'
+    name = "NAS"
 
-    def configure(self, enable_openmp: bool = True, suite_class: str = 'B'):
+    def configure(self, enable_openmp: bool = True, suite_class: str = "B"):
         self.enable_openmp = enable_openmp
         self.suite_class = suite_class
 
         # this is also hacky
-        self.add_benchmark(NASBenchmark, 'bt')
-        self.add_benchmark(NASBenchmark, 'sp')
-        self.add_benchmark(NASBenchmark, 'lu')
-        self.add_benchmark(NASBenchmark, 'mg')
-        self.add_benchmark(NASBenchmark, 'ft')
-        self.add_benchmark(NASBenchmark, 'is')
-        self.add_benchmark(NASBenchmark, 'cg')
-        self.add_benchmark(NASBenchmark, 'ep')
+        self.add_benchmark(NASBenchmark, "bt")
+        self.add_benchmark(NASBenchmark, "sp")
+        self.add_benchmark(NASBenchmark, "lu")
+        self.add_benchmark(NASBenchmark, "mg")
+        self.add_benchmark(NASBenchmark, "ft")
+        self.add_benchmark(NASBenchmark, "is")
+        self.add_benchmark(NASBenchmark, "cg")
+        self.add_benchmark(NASBenchmark, "ep")
 
     def acquire(self):
         self.workspace.shell(
-            'git', 'clone', 'https://github.com/nickwanninger/NPB3.0-omp-C.git', self.src, '--depth', '1')
+            "git",
+            "clone",
+            "https://github.com/nickwanninger/NPB3.0-omp-C.git",
+            self.src,
+            "--depth",
+            "1",
+        )
         # This is really gross. TODO: refactor this!
-        (self.src / 'bin').mkdir(exist_ok=True)
-        make_def_path = self.src / 'config' / 'make.def'
-        with make_def_path.open('w') as cfg:
-            cfg.write(f'CC    = gclang\n')
-            cfg.write(f'CLINK = gclang\n')
-            cfg.write(f'C_LIB = -lm\n')
-            cfg.write(f'C_INC = -I../common\n')
+        (self.src / "bin").mkdir(exist_ok=True)
+        make_def_path = self.src / "config" / "make.def"
+        with make_def_path.open("w") as cfg:
+            cfg.write(f"CC    = gclang\n")
+            cfg.write(f"CLINK = gclang\n")
+            cfg.write(f"C_LIB = -lm\n")
+            cfg.write(f"C_INC = -I../common\n")
             if self.enable_openmp:
-                cfg.write(f'CFLAGS = -O3 -fPIC -fopenmp\n')
+                cfg.write(f"CFLAGS = -O3 -fPIC -fopenmp\n")
             else:
-                cfg.write(f'CFLAGS = -O3 -fPIC\n')
-            cfg.write('CLINKFLAGS = -fPIC -lm -fopenmp\n')
-            cfg.write('UCC = cc -O\n')
-            cfg.write('BINDIR	= ../bin\n')
-            cfg.write('RAND	= randdp\n')
-            cfg.write('WTIME	= wtime.c\n')
+                cfg.write(f"CFLAGS = -O3 -fPIC\n")
+            cfg.write("CLINKFLAGS = -fPIC -lm -fopenmp\n")
+            cfg.write("UCC = cc -O\n")
+            cfg.write("BINDIR	= ../bin\n")
+            cfg.write("RAND	= randdp\n")
+            cfg.write("WTIME	= wtime.c\n")
 
 
 class GAPBenchmark(Benchmark):
     def compile(self, suite_path: Path, output: Path):
 
-        source_file = suite_path / 'src' / (self.name + '.cc')
+        source_file = suite_path / "src" / (self.name + ".cc")
         print(source_file)
-        run_command(['gclang++', source_file, '-fopenmp', '-std=c++11',
-                    '-O3', '-Wall', '-o', output])
+        run_command(
+            [
+                "gclang++",
+                source_file,
+                "-fopenmp",
+                "-std=c++11",
+                "-O3",
+                "-Wall",
+                "-o",
+                output,
+            ]
+        )
 
     def link(self, bitcode: Path, output: Path):
-        run_command(['gclang++', bitcode, '-fopenmp', '-std=c++11',
-                    '-O3', '-Wall', '-o', output])
+        run_command(
+            [
+                "gclang++",
+                bitcode,
+                "-fopenmp",
+                "-std=c++11",
+                "-O3",
+                "-Wall",
+                "-o",
+                output,
+            ]
+        )
 
 
 class GAP(Suite):
     def __init__(self, enable_openmp: bool = True):
-        super().__init__('GAP')
+        super().__init__("GAP")
         self.enable_openmp = enable_openmp
 
-        self.add_benchmark(GAPBenchmark, 'bc')
-        self.add_benchmark(GAPBenchmark, 'bfs')
-        self.add_benchmark(GAPBenchmark, 'cc')
-        self.add_benchmark(GAPBenchmark, 'cc_sv')
-        self.add_benchmark(GAPBenchmark, 'converter')
-        self.add_benchmark(GAPBenchmark, 'pr')
-        self.add_benchmark(GAPBenchmark, 'pr_spmv')
-        self.add_benchmark(GAPBenchmark, 'sssp')
-        self.add_benchmark(GAPBenchmark, 'tc')
+        self.add_benchmark(GAPBenchmark, "bc")
+        self.add_benchmark(GAPBenchmark, "bfs")
+        self.add_benchmark(GAPBenchmark, "cc")
+        self.add_benchmark(GAPBenchmark, "cc_sv")
+        self.add_benchmark(GAPBenchmark, "converter")
+        self.add_benchmark(GAPBenchmark, "pr")
+        self.add_benchmark(GAPBenchmark, "pr_spmv")
+        self.add_benchmark(GAPBenchmark, "sssp")
+        self.add_benchmark(GAPBenchmark, "tc")
 
     def acquire(self, path: Path):
-        waterline.utils.git_clone('https://github.com/sbeamer/gapbs.git', path)
+        waterline.utils.git_clone("https://github.com/sbeamer/gapbs.git", path)
 
 
 polybench_benchmarks: Tuple[str, str] = [
-    ('datamining/correlation/correlation.c', 'correlation'),
-    ('datamining/covariance/covariance.c', 'covariance'),
-    ('linear-algebra/kernels/2mm/2mm.c', '2mm'),
-    ('linear-algebra/kernels/3mm/3mm.c', '3mm'),
-    ('linear-algebra/kernels/atax/atax.c', 'atax'),
-    ('linear-algebra/kernels/bicg/bicg.c', 'bicg'),
-    ('linear-algebra/kernels/cholesky/cholesky.c', 'cholesky'),
-    ('linear-algebra/kernels/doitgen/doitgen.c', 'doitgen'),
-    ('linear-algebra/kernels/gemm/gemm.c', 'gemm'),
-    ('linear-algebra/kernels/gemver/gemver.c', 'gemver'),
-    ('linear-algebra/kernels/gesummv/gesummv.c', 'gesummv'),
-    ('linear-algebra/kernels/mvt/mvt.c', 'mvt'),
-    ('linear-algebra/kernels/symm/symm.c', 'symm'),
-    ('linear-algebra/kernels/syr2k/syr2k.c', 'syr2k'),
-    ('linear-algebra/kernels/syrk/syrk.c', 'syrk'),
-    ('linear-algebra/kernels/trisolv/trisolv.c', 'trisolv'),
-    ('linear-algebra/kernels/trmm/trmm.c', 'trmm'),
-    ('linear-algebra/solvers/durbin/durbin.c', 'durbin'),
-    ('linear-algebra/solvers/dynprog/dynprog.c', 'dynprog'),
-    ('linear-algebra/solvers/gramschmidt/gramschmidt.c', 'gramschmidt'),
-    ('linear-algebra/solvers/lu/lu.c', 'lu'),
-    ('linear-algebra/solvers/ludcmp/ludcmp.c', 'ludcmp'),
-    ('medley/floyd-warshall/floyd-warshall.c', 'floyd-warshall'),
-    ('medley/reg_detect/reg_detect.c', 'reg_detect'),
-    ('stencils/adi/adi.c', 'adi'),
-    ('stencils/fdtd-2d/fdtd-2d.c', 'fdtd-2d'),
-    ('stencils/fdtd-apml/fdtd-apml.c', 'fdtd-apml'),
-    ('stencils/jacobi-1d-imper/jacobi-1d-imper.c', 'jacobi-1d-imper'),
-    ('stencils/jacobi-2d-imper/jacobi-2d-imper.c', 'jacobi-2d-imper'),
-    ('stencils/seidel-2d/seidel-2d.c', 'seidel-2d')
+    ("datamining/correlation/correlation.c", "correlation"),
+    ("datamining/covariance/covariance.c", "covariance"),
+    ("linear-algebra/kernels/2mm/2mm.c", "2mm"),
+    ("linear-algebra/kernels/3mm/3mm.c", "3mm"),
+    ("linear-algebra/kernels/atax/atax.c", "atax"),
+    ("linear-algebra/kernels/bicg/bicg.c", "bicg"),
+    ("linear-algebra/kernels/cholesky/cholesky.c", "cholesky"),
+    ("linear-algebra/kernels/doitgen/doitgen.c", "doitgen"),
+    ("linear-algebra/kernels/gemm/gemm.c", "gemm"),
+    ("linear-algebra/kernels/gemver/gemver.c", "gemver"),
+    ("linear-algebra/kernels/gesummv/gesummv.c", "gesummv"),
+    ("linear-algebra/kernels/mvt/mvt.c", "mvt"),
+    ("linear-algebra/kernels/symm/symm.c", "symm"),
+    ("linear-algebra/kernels/syr2k/syr2k.c", "syr2k"),
+    ("linear-algebra/kernels/syrk/syrk.c", "syrk"),
+    ("linear-algebra/kernels/trisolv/trisolv.c", "trisolv"),
+    ("linear-algebra/kernels/trmm/trmm.c", "trmm"),
+    ("linear-algebra/solvers/durbin/durbin.c", "durbin"),
+    ("linear-algebra/solvers/dynprog/dynprog.c", "dynprog"),
+    ("linear-algebra/solvers/gramschmidt/gramschmidt.c", "gramschmidt"),
+    ("linear-algebra/solvers/lu/lu.c", "lu"),
+    ("linear-algebra/solvers/ludcmp/ludcmp.c", "ludcmp"),
+    ("medley/floyd-warshall/floyd-warshall.c", "floyd-warshall"),
+    ("medley/reg_detect/reg_detect.c", "reg_detect"),
+    ("stencils/adi/adi.c", "adi"),
+    ("stencils/fdtd-2d/fdtd-2d.c", "fdtd-2d"),
+    ("stencils/fdtd-apml/fdtd-apml.c", "fdtd-apml"),
+    ("stencils/jacobi-1d-imper/jacobi-1d-imper.c", "jacobi-1d-imper"),
+    ("stencils/jacobi-2d-imper/jacobi-2d-imper.c", "jacobi-2d-imper"),
+    ("stencils/seidel-2d/seidel-2d.c", "seidel-2d"),
 ]
 
 
 class PolyBenchBenchmark(Benchmark):
     def __init__(self, suite, name, source):
         super().__init__(suite, name)
         self.source = source
 
     def compile(self, output: Path):
         source_file = self.suite.src / self.source
-        self.shell('gclang', '-DLARGE_DATASET', '-DPOLYBENCH_TIME', '-O1', '-Xclang', '-disable-llvm-passes', '-Xclang', '-disable-O0-optnone', f'-I{self.suite.src}/utilities', f'-I{source_file.parent}',
-                    self.suite.src / 'utilities' / 'polybench.c', source_file, '-lm', '-Wno-implicit-function-declaration',  '-o', output)
+        self.shell(
+            "gclang",
+            "-DLARGE_DATASET",
+            "-DPOLYBENCH_TIME",
+            "-O1",
+            "-Xclang",
+            "-disable-llvm-passes",
+            "-Xclang",
+            "-disable-O0-optnone",
+            f"-I{self.suite.src}/utilities",
+            f"-I{source_file.parent}",
+            self.suite.src / "utilities" / "polybench.c",
+            source_file,
+            "-lm",
+            "-Wno-implicit-function-declaration",
+            "-o",
+            output,
+        )
 
     def link(self, bitcode: Path, output: Path):
-        self.shell('gclang', bitcode, '-lm', '-o', output)
+        self.shell("gclang", bitcode, "-lm", "-o", output)
 
 
 class PolyBench(Suite):
-    name = 'PolyBench'
+    name = "PolyBench"
+
     def configure(self):
         for source, name in polybench_benchmarks:
             self.add_benchmark(PolyBenchBenchmark, name, source)
 
     def acquire(self):
-        tarball = self.src.parent / 'polybench-3.1.tar.gz'
-        print('get poybench to', self.src)
+        tarball = self.src.parent / "polybench-3.1.tar.gz"
         waterline.utils.download(
-            'http://web.cse.ohio-state.edu/~pouchet.2/software/polybench/download/polybench-3.1.tar.gz', tarball)
+            "http://web.cse.ohio-state.edu/~pouchet.2/software/polybench/download/polybench-3.1.tar.gz",
+            tarball,
+        )
 
-        shutil.unpack_archive(tarball, self.src.parent, 'gztar')
-        shutil.move(self.src.parent / 'polybench-3.1', self.src)
+        shutil.unpack_archive(tarball, self.src.parent, "gztar")
+        shutil.move(self.src.parent / "polybench-3.1", self.src)
         # waterline.utils.shell(f'tar xf {out} -C {path.parent}')
 
         # shutil.(out / 'polybench-3.1', path)
```

## waterline/utils.py

```diff
@@ -1,23 +1,22 @@
 from pathlib import Path
 import subprocess
 import requests
-from typing import List
 
 
-def run_command(args: List[str]):
-  print('running command', ' '.join(map(str, args)))
-  output = subprocess.check_output(args)
+def run_command(args: list[str]):
+    print("running command", " ".join(map(str, args)))
+    output = subprocess.check_output(args)
 
 
 def shell(commnad: str):
-  run_command(['sh', '-c', commnad])
+    run_command(["sh", "-c", commnad])
 
 
 def git_clone(url: str, destination: Path):
-  shell(f'git clone {url} {destination} --depth 1')
+    shell(f"git clone {url} {destination} --depth 1")
 
 
 def download(url: str, output: Path):
-  r = requests.get(url)
-  with open(output, 'wb') as f:
-    f.write(r.content)
+    r = requests.get(url)
+    with open(output, "wb") as f:
+        f.write(r.content)
```

## waterline/workspace.py

```diff
@@ -1,111 +1,136 @@
 from pathlib import Path
 from .suite import Suite
 from .utils import *
 from .pipeline import *
-from typing import Tuple
-from alive_progress import alive_bar
+from typing import Tuple, List
+from . import jobs
 
 
 class Workspace:
+    suites: List[Suite] = []
+
     def __init__(self, dir: str):
         self.dir = Path(dir).absolute()
         # make sure the workspace directory exists.
         self.dir.mkdir(exist_ok=True)
 
-        self.src_dir = self.dir / 'src'
+        self.src_dir = self.dir / "src"
         self.src_dir.mkdir(exist_ok=True)
 
-        self.bin_dir = self.dir / 'bin'
+        self.bin_dir = self.dir / "bin"
         self.bin_dir.mkdir(exist_ok=True)
 
-        self.ir_dir = self.dir / 'ir'
+        self.ir_dir = self.dir / "ir"
         self.ir_dir.mkdir(exist_ok=True)
 
-        self.suites = []
-
     def add_suite(self, suite, *args, **kwargs):
         s = suite(self)
         s.configure(*args, **kwargs)
         self.suites.append(s)
 
     def dump_benchmarks(self):
         for suite in self.suites:
-            print(f'suite {suite.name}')
+            print(f"suite {suite.name}")
             for benchmark in suite.benchmarks:
-                print(f'  {benchmark.name}')
+                print(f"  {benchmark.name}")
 
     def extract_bitcode(self, input, output):
-        self.shell('get-bc', '-o', output, input)
-        self.shell('llvm-dis', input)
-
-    def run_jobs(self, jobs):
-        if len(jobs) > 0:
-            with alive_bar(len(jobs)) as bar:  # declare your expected total
-                for jobname, op, *args in jobs:
-                    bar.text(jobname)
-                    op(*args)
-                    bar()
+        self.shell("get-bc", "-o", output, input)
+        self.shell("llvm-dis", output)
 
     def prepare(self):
+        """Prepare this workspace to have bitcode pipeline applied."""
         # a list of jobs to work on. This will be appended to and
         # worked through before a pipeline can run.
-        jobs: Tuple[str, function] = []
+        runner = jobs.JobRunner()
 
         # first, make sure all the benchmarks are acquired. We just do this by
         # checking if the directory of the suite exists.
         for suite in self.suites:
             if not suite.src.exists():
-                jobs.append((f'acquire {suite.name}', suite.acquire))
+                runner.add(jobs.FunctionJob(f"acquire {suite.name}", suite.acquire))
+        runner.title = "acquire suites"
+        runner.run(parallel=True)
 
         # second, compile the a.out files for each benchmark suite. If the a.out
         # file doesn't exist, add it to the job list.
         for suite in self.suites:
             suite_bin = self.bin_dir / suite.name
             suite_bin.mkdir(exist_ok=True)
-            jobs += suite.get_compile_jobs()
+            for job in suite.compile_jobs():
+                runner.add(job)
+        runner.title = "compile baseline"
+        runner.run(parallel=True)
 
         # Third, make sure input.bc exists in each ir/<suite>/<benchmark>/ folder
         for suite in self.suites:
             suite_ir = self.ir_dir / suite.name
             suite_ir.mkdir(exist_ok=True)
             suite_bin = self.bin_dir / suite.name
             suite_bin.mkdir(exist_ok=True)
             for benchmark in suite.benchmarks:
                 benchmark_ir_dir = suite_ir / benchmark.name
                 benchmark_ir_dir.mkdir(exist_ok=True)
 
-                input = suite_bin / benchmark.name / 'a.out'
-                output = benchmark_ir_dir / 'input.bc'
+                input = suite_bin / benchmark.name / "a.out"
+                output = benchmark_ir_dir / "input.bc"
                 if not output.exists():
-                    jobs.append(
-                        (f'extract {suite.name}/{benchmark.name}', self.extract_bitcode, input, output))
-
-        # Execute those jobs we just made.
-        self.run_jobs(jobs)
+                    runner.add(
+                        jobs.FunctionJob(
+                            f"extract {suite.name}/{benchmark.name}",
+                            self.extract_bitcode,
+                            input,
+                            output,
+                        )
+                    )
+        runner.title = "extract bitcode"
+        runner.run()
 
     def run_pipeline(self, pipeline: Pipeline):
+        """Run a pipeline over the bitcodes of each benchmark in this workspace"""
         # Make sure everything is setup!
         self.prepare()
         # Now run the pipeline on every benchmark's IR
-        jobs = []
+        runner = jobs.JobRunner(f"pipeline: {pipeline.name}")
+
         for suite in self.suites:
             suite_ir = self.ir_dir / suite.name
             for benchmark in suite.benchmarks:
                 benchmark_ir_dir = suite_ir / benchmark.name
-                benchmark_ir_input = benchmark_ir_dir / 'input.bc'
+                benchmark_ir_input = benchmark_ir_dir / "input.bc"
 
-                output = benchmark_ir_dir / f'{pipeline.name}.bc'
-                jobs += pipeline.create_jobs(benchmark_ir_input,
-                                             output, benchmark)
-                benchmark_link_dest = self.bin_dir / suite.name / benchmark.name / pipeline.name
-                jobs.append((f'link {suite.name}/{benchmark.name} for pipeline {pipeline.name}',
-                            benchmark.link, output, benchmark_link_dest))
+                output = benchmark_ir_dir / f"{pipeline.name}.bc"
+                runner.add(*pipeline.create_jobs(benchmark_ir_input, output, benchmark))
+                benchmark_link_dest = (
+                    self.bin_dir / suite.name / benchmark.name / pipeline.name
+                )
+
+                runner.add(
+                    jobs.FunctionJob(
+                        f"link {suite.name}/{benchmark.name}",
+                        benchmark.link_bitcode,
+                        output,
+                        benchmark_link_dest,
+                    )
+                )
+
+        runner.run(parallel=False)
+
+    def run(self):
+        configs = []
+        for suite in self.suites:
+            for benchmark in suite.benchmarks:
+                for config in benchmark.run_configs():
+                    configs.append((benchmark, config))
 
-        self.run_jobs(jobs)
+        print(configs)
 
     def shell(self, *args):
         # print('running: ', *args)
-        with open(self.dir / 'output.txt', 'a+') as out:
-            out.write(f'XXXXXX RUNNING COMMAND {args}\n')
+        with open(self.dir / "output.txt", "a+") as out:
+            out.write("\n\n")
+            out.write("$ " + " ".join(map(str, args)) + "\n")
+            out.flush()
             proc = subprocess.Popen(args, stdout=out, stderr=out)
-            proc.wait()
+            if not proc.wait() == 0:
+                raise RuntimeError("failed to run", *args)
```

## Comparing `waterline-0.1.4.dist-info/LICENSE` & `waterline-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

