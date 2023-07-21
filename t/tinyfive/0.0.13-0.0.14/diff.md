# Comparing `tmp/tinyfive-0.0.13.tar.gz` & `tmp/tinyfive-0.0.14.tar.gz`

## Comparing `tinyfive-0.0.13.tar` & `tinyfive-0.0.14.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfive-0.0.13/tinyfive/__init__.py
--rw-r--r--   0        0        0    31932 2020-02-02 00:00:00.000000 tinyfive-0.0.13/tinyfive/machine.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinyfive-0.0.13/LICENSE
--rw-r--r--   0        0        0    27141 2020-02-02 00:00:00.000000 tinyfive-0.0.13/README.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 tinyfive-0.0.13/pyproject.toml
--rw-r--r--   0        0        0    27741 2020-02-02 00:00:00.000000 tinyfive-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfive-0.0.14/tinyfive/__init__.py
+-rw-r--r--   0        0        0    32325 2020-02-02 00:00:00.000000 tinyfive-0.0.14/tinyfive/machine.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinyfive-0.0.14/LICENSE
+-rw-r--r--   0        0        0    27375 2020-02-02 00:00:00.000000 tinyfive-0.0.14/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 tinyfive-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0    27975 2020-02-02 00:00:00.000000 tinyfive-0.0.14/PKG-INFO
```

### Comparing `tinyfive-0.0.13/tinyfive/machine.py` & `tinyfive-0.0.14/tinyfive/machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,16 +70,16 @@
   def BNE (s,rs1,rs2,imm): s.pc += imm if s.x[rs1]      != s.x[rs2]      else 4
   def BLT (s,rs1,rs2,imm): s.pc += imm if s.x[rs1]      <  s.x[rs2]      else 4
   def BGE (s,rs1,rs2,imm): s.pc += imm if s.x[rs1]      >= s.x[rs2]      else 4
   def BLTU(s,rs1,rs2,imm): s.pc += imm if s.u(s.x[rs1]) <  s.u(s.x[rs2]) else 4
   def BGEU(s,rs1,rs2,imm): s.pc += imm if s.u(s.x[rs1]) >= s.u(s.x[rs2]) else 4
 
   # jump
-  def JAL (s,rd,imm): s.x[rd] = s.pc + 4; s.pc += imm
-  def JALR(s,rd,rs1,imm): t = s.pc + 4; s.pc = (s.x[rs1] + imm) & ~1; s.x[rd] = t
+  def JAL (s,rd,imm): s.x[rd] = s.pc + 4; s.pc += imm; s.x[0] = 0
+  def JALR(s,rd,rs1,imm): t = s.pc + 4; s.pc = (s.x[rs1] + imm) & ~1; s.x[rd] = t; s.x[0] = 0
 
   # load immediate
   def LUI  (s,rd,imm): s.x[rd] = imm << 12;          s.ipc()
   def AUIPC(s,rd,imm): s.x[rd] = s.pc + (imm << 12); s.ipc()
 
   # load, note the different argument order, example: 'lb rd, offset(rs1)'
   def LB (s,rd,imm,rs1): s.x[rd] =  s.i8(s.mem[s.x[rs1] + imm]);  s.ipc()
@@ -100,14 +100,19 @@
   def SW(s,rs2,imm,rs1): s.mem[s.x[rs1] + imm]   =  s.x[rs2] & 0xff; s.ipc(); \
                          s.mem[s.x[rs1] + imm+1] = (s.x[rs2] >> 8)  & 0xff; \
                          s.mem[s.x[rs1] + imm+2] = (s.x[rs2] >> 16) & 0xff; \
                          s.mem[s.x[rs1] + imm+3] = (s.x[rs2] >> 24) & 0xff
 
   # the 3 missing instructions FENCE, ECALL, EBREAK are not needed here
 
+  # TODO: when using the above uppercase instructions, then there is no check if
+  # an immediate exceeds the 12-bit limit. Therefore, consider replacing 'imm'
+  # by 'ci(imm)', where ci() is a def that raises an error flag if the immediate
+  # exceeds the 12-bit limit.
+
   #-------------------------------------------------------------------------------
   # M-extension (RV32M)
   def muls(s,a,b): return np.multiply(    a,      b,  dtype=np.int64)
   def mulu(s,a,b): return np.multiply(s.u(a), s.u(b), dtype=np.uint64)
   def MUL   (s,rd,rs1,rs2): s.x[rd] = s.muls(s.x[rs1],    s.x[rs2]);        s.ipc()
   def MULH  (s,rd,rs1,rs2): s.x[rd] = s.muls(s.x[rs1],    s.x[rs2])  >> 32; s.ipc()
   def MULHSU(s,rd,rs1,rs2): s.x[rd] = s.muls(s.x[rs1],s.u(s.x[rs2])) >> 32; s.ipc()
@@ -424,25 +429,27 @@
         inst = s.read_i32(s.pc)  # fetch instruction from memory
         s.dec(np.binary_repr(s.u(inst), 32))
 
   #-------------------------------------------------------------------------------
   # pseudoinstructions
 
   def hi20(s, val): return (val + 0x800) >> 12  # higher 20 bits (+1 if val[11]==1)
-  def lo12(s, val): return val & 0xfff          # lower 12 bits
-  # above functions are copied from LLVM
+  def lo12(s, val):
+    return (val & 0x7ff) - (val & 0x800) # lower 12 bits and convert to signed int12
+  # above functions are similar to LLVM
   # https://github.com/llvm/llvm-project/blob/main/lld/ELF/Arch/RISCV.cpp
   # note that ADDI interprets the immediate as a 12-bit signed. So if bit[11] is
   # set (i.e. value -2048 = -0x800), then we have to add +1 to the upper 20 bits
   # (i.e. +0x1000) so that (hi20 >> 12) + lo12 is the same as 'val'. The term
   # '(val + 0x800) >> 12' in hi20 def will only add +1 if bit val[11] is set.
+  # Example: 0xdeadbeef -> hi20 = 0xdeadc; lo12 = -273
 
   def LI(s, rd, imm):
-    LUI (s, rd,     hi20(imm))
-    ADDI(s, rd, rd, lo12(imm))
+    s.LUI (rd,     s.hi20(imm))
+    s.ADDI(rd, rd, s.lo12(imm))
   # TODO: add a corresponding lower-case instruction
 
   # TODO: add more pseudoinstructions
 
   #-------------------------------------------------------------------------------
   # useful functions for accessing state and memory
```

### Comparing `tinyfive-0.0.13/LICENSE` & `tinyfive-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyfive-0.0.13/README.md` & `tinyfive-0.0.14/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ## Contents
 - [Installation](#installation)
 - [Usage](#usage)
   - [Example 1: Multiply two numbers](#example-1-multiply-two-numbers)
   - [Example 2: Add two vectors](#example-2-add-two-vectors)
   - [Example 3: Multiply two matrices](#example-3-multiply-two-matrices)
+  - [Example 4: Neural network layers](#example-4-neural-network-layers)
 - [Running in colab](#running-in-colab)
 - [Running without package](#running-without-package)
 - [Speed](#speed)
 - [Latest status](#latest-status)
 - [Comparison](#comparison)
 - [References](#references)
 - [Tiny Tech promise](#tiny-tech-promise)
@@ -379,14 +380,17 @@
 - For 16x16 or larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/discovering-novel-algorithms-with-alphatensor) can reduce the total number of multiplications and additions if they are applied recursively.
 
 |             | Image | Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup |
 |:-----------:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:-------:|
 | Example 3.3 | 92B   | 9         | 80   | 16    | 64  | 89  | 20     | 269       | 1       |
 | Example 3.4 | 640B  | 22        | 32   | 16    | 64  | 48  | 0      | 160       | 1.7     |
 
+### Example 4: Neural network layers
+Coming soon, see [file layer_examples.py](layer_examples.py)
+
 ## Running in colab
 <a href="https://colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/colab.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Colab" height="20">
 </a>  This is the quickest way to get started and should work on any machine.
 
 If you have a free Google Drive account, you can make a copy of this colab via the menu `File` -> `Save a copy in Drive`. Now you can edit the code.
 
@@ -426,15 +430,15 @@
 
 # run test suite
 !python3 tests.py
 ```
 
 ## Speed
 - TinyFive is not optimized for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/Source_lines_of_code)).
-- You could use PyPy to speed it up (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
+- You might be able to use [Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
 - If you only use the upper-case instructions such as `ADD()`, then TinyFive is very fast because there is no instruction decoding. And you should be able to accelerate it on a GPU or TPU.
 - If you use the lower-case instructions with `asm()` and `exe()`, then execution of these functions is slow as they involve look-up and string matching with O(n) complexity where "n" is the total number of instructions. The current implementations of `asm()` and `dec()` are optimized for ease-of-use and readability. A faster implementation would collapse multiple look-ups into one look-up, optimize the pattern-matching for the instruction decoding (bits -> instruction), and change the order of the instructions so that more frequently used instructions are at the top of the list. [Here is an older version](https://github.com/OpenMachine-ai/tinyfive/blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster `dec()` function that collapses two look-ups (`bits -> instruction` and `instruction -> uppeer-case instruction`) and doesn't use `fnmatch`.
 
 ## Latest status
 - TinyFive is still under construction, many things haven't been implemented and tested yet.
 - 37 of the 40 base instructions (RV32I), all instructions of the M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode are already implemented, and many of them are tested.  (The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not applicable here.)
 - Remaining work: improve testing, add perhaps more extensions. See TODOs in the code for more details.
```

#### html2text {}

```diff
@@ -12,15 +12,16 @@
 learn how RISC-V works, TinyFive lets you play with instructions and assembly
 code. - Can be very fast if you only use the upper-case instructions defined in
 the [first ~200 lines of machine.py](machine.py#L1-L200). - [Fewer than 1000
 lines](machine.py) of code (w/o tests and examples) - Uses NumPy for math ##
 Contents - [Installation](#installation) - [Usage](#usage) - [Example 1:
 Multiply two numbers](#example-1-multiply-two-numbers) - [Example 2: Add two
 vectors](#example-2-add-two-vectors) - [Example 3: Multiply two matrices]
-(#example-3-multiply-two-matrices) - [Running in colab](#running-in-colab) -
+(#example-3-multiply-two-matrices) - [Example 4: Neural network layers]
+(#example-4-neural-network-layers) - [Running in colab](#running-in-colab) -
 [Running without package](#running-without-package) - [Speed](#speed) - [Latest
 status](#latest-status) - [Comparison](#comparison) - [References](#references)
 - [Tiny Tech promise](#tiny-tech-promise) ## Installation ``` pip install
 tinyfive ``` ## Usage TinyFive can be used in the following three ways: -
 **Option A:** Use upper-case instructions such as `ADD()` and `MUL()`, see
 examples 1.1, 1.2, 2.1, and 3.1 below. - **Option B:** Use `asm()` and `exe()`
 functions without branch instructions, see examples 1.3 and 2.2 below. -
@@ -238,92 +239,95 @@
 larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/
 Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/
 discovering-novel-algorithms-with-alphatensor) can reduce the total number of
 multiplications and additions if they are applied recursively. | | Image |
 Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup | |:-------
 ----:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:----
 ---:| | Example 3.3 | 92B | 9 | 80 | 16 | 64 | 89 | 20 | 269 | 1 | | Example
-3.4 | 640B | 22 | 32 | 16 | 64 | 48 | 0 | 160 | 1.7 | ## Running in colab
-[Colab] This is the quickest way to get started and should work on any machine.
-If you have a free Google Drive account, you can make a copy of this colab via
-the menu `File` -> `Save a copy in Drive`. Now you can edit the code.
-Alternatively, start a new colab in your Google Drive as follows: [Go here]
-(https://drive.google.com/drive/my-drive) and click on `New` -> `More` -
-> `Google Colaboratory`. Then copy below lines into your colab: ```python !pip
-install tinyfive from tinyfive.machine import machine import numpy as np m =
-machine(mem_size=4000) # instantiate RISC-V machine with 4KB of memory ``` ##
-Running without package If you don't want to use the TinyFive python package,
-then you can clone the latest repo and install numpy as follows: ```bash git
-clone https://github.com/OpenMachine-ai/tinyfive.git cd tinyfive pip install
-numpy ``` To run the examples, type: ```bash python3 examples.py ``` To run the
-test suite, type: ```bash python3 tests.py ``` If you don't want to run above
-steps on your local machine, you can run it in a colab as follows: Start a new
-colab in your Google Drive by [going here](https://drive.google.com/drive/my-
-drive) and clicking on `New` -> `More` -> `Google Colaboratory`. Then copy
-below lines into your colab: ```python !git clone https://github.com/
-OpenMachine-ai/tinyfive.git %cd tinyfive # run examples !python3 examples.py #
-run test suite !python3 tests.py ``` ## Speed - TinyFive is not optimized for
-speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/
-Source_lines_of_code)). - You could use PyPy to speed it up (see e.g. the
-[Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf)
-for details). - If you only use the upper-case instructions such as `ADD()`,
-then TinyFive is very fast because there is no instruction decoding. And you
-should be able to accelerate it on a GPU or TPU. - If you use the lower-case
-instructions with `asm()` and `exe()`, then execution of these functions is
-slow as they involve look-up and string matching with O(n) complexity where "n"
-is the total number of instructions. The current implementations of `asm()` and
-`dec()` are optimized for ease-of-use and readability. A faster implementation
-would collapse multiple look-ups into one look-up, optimize the pattern-
-matching for the instruction decoding (bits -> instruction), and change the
-order of the instructions so that more frequently used instructions are at the
-top of the list. [Here is an older version](https://github.com/OpenMachine-ai/
-tinyfive/blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive
-with a faster `dec()` function that collapses two look-ups (`bits -
-> instruction` and `instruction -> uppeer-case instruction`) and doesn't use
-`fnmatch`. ## Latest status - TinyFive is still under construction, many things
-haven't been implemented and tested yet. - 37 of the 40 base instructions
-(RV32I), all instructions of the M-extension (RV32M) and the F-extension
-(RV32F) with the default rounding mode are already implemented, and many of
-them are tested. (The three missing RV32I instructions `fence`, `ebreak`, and
-`ecall` are not applicable here.) - Remaining work: improve testing, add
-perhaps more extensions. See TODOs in the code for more details. ## Comparison
-The table below compares TinyFive with other [ISS](https://en.wikipedia.org/
-wiki/Instruction_set_simulator) and emulator projects. | ISS | Author |
-Language | Mature? | Extensions | LOC | | --- | ------ | -------- | ------- | -
---------- | --- | | [TinyFive](https://github.com/OpenMachine-ai/tinyfive) |
-OpenMachine | Python | No | I, M, some F | < 1k | | [Pydgin](https://
-github.com/cornell-brg/pydgin) | Cornell University | Python, C | Last update
-2016 | A, D, F, I, M | | | [Spike](https://github.com/riscv-software-src/riscv-
-isa-sim) | UC Berkeley | C, C++ | Yes | All | | | [QEMU](https://www.qemu.org/
-) | [Fabrice Bellard](https://en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes
-| All | | | [TinyEMU](https://bellard.org/tinyemu/) | [Fabrice Bellard](https:/
-/en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim]
-(https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All
-| | | [Whisper](https://github.com/chipsalliance/SweRV-ISS) | Western Digital |
-C, C++ | Yes | Almost all | | | [Sail Model](https://github.com/riscv/sail-
-riscv) | Cambridge, Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https:/
-/github.com/PiMaker/rvc) | PiMaker | C | | | | | [mini-rv32ima](https://
-github.com/cnlohr/mini-rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr
-| < 1k | ## References - Official [RISC-V spec](https://github.com/riscv/riscv-
-isa-manual/releases/download/Ratified-IMAFDQC/riscv-spec-20191213.pdf) - See
-[this RISC-V card](https://inst.eecs.berkeley.edu/~cs61c/fa18/img/
-riscvcard.pdf) for a brief description of most instructions. See also the
-[RISC-V reference card](http://riscvbook.com/greencard-20181213.pdf). - Book
-"The RISC-V Reader: An Open Architecture Atlas" by David Patterson and Andrew
-Waterman. Appendix A of this book defines all instructions. The Spanish version
-of this book is [available for free](http://riscvbook.com/spanish/guia-
-practica-de-risc-v-1.0.5.pdf), other free versions are [available here](http://
-riscvbook.com). - Pydgin [paper](https://www.csl.cornell.edu/~berkin/ilbeyi-
-pydgin-riscv2016.pdf) and [video](https://youtu.be/-p_AGki7Vsk) - [Online
-simulator](https://ascslab.org/research/briscv/simulator/simulator.html) for
-debug ## Tiny Tech promise Similar to [tinygrad](https://github.com/geohot/
-tinygrad), [micrograd](https://github.com/karpathy/micrograd), and other
-âtiny techâ projects, we believe that core technology should be simple and
-small (in terms of LOC). Therefore, we will make sure that the core of TinyFive
-(without tests and examples) will always be below 1000 lines. Simplicity and
-size (in terms of number of instructions) is a key feature of [RISC](https://
-en.wikipedia.org/wiki/Reduced_instruction_set_computer): the "R" in RISC stands
-for "reduced" (as opposed to complex CISC). Specifically, the ISA manual of
-RISC-V has only ~200 pages while the ARM-32 manual is over 2000 pages long
-according to Fig. 1.6 of the [RISC-V Reader](http://riscvbook.com/spanish/guia-
-practica-de-risc-v-1.0.5.pdf).
+3.4 | 640B | 22 | 32 | 16 | 64 | 48 | 0 | 160 | 1.7 | ### Example 4: Neural
+network layers Coming soon, see [file layer_examples.py](layer_examples.py) ##
+Running in colab [Colab] This is the quickest way to get started and should
+work on any machine. If you have a free Google Drive account, you can make a
+copy of this colab via the menu `File` -> `Save a copy in Drive`. Now you can
+edit the code. Alternatively, start a new colab in your Google Drive as
+follows: [Go here](https://drive.google.com/drive/my-drive) and click on `New`
+-> `More` -> `Google Colaboratory`. Then copy below lines into your colab:
+```python !pip install tinyfive from tinyfive.machine import machine import
+numpy as np m = machine(mem_size=4000) # instantiate RISC-V machine with 4KB of
+memory ``` ## Running without package If you don't want to use the TinyFive
+python package, then you can clone the latest repo and install numpy as
+follows: ```bash git clone https://github.com/OpenMachine-ai/tinyfive.git cd
+tinyfive pip install numpy ``` To run the examples, type: ```bash python3
+examples.py ``` To run the test suite, type: ```bash python3 tests.py ``` If
+you don't want to run above steps on your local machine, you can run it in a
+colab as follows: Start a new colab in your Google Drive by [going here](https:
+//drive.google.com/drive/my-drive) and clicking on `New` -> `More` -> `Google
+Colaboratory`. Then copy below lines into your colab: ```python !git clone
+https://github.com/OpenMachine-ai/tinyfive.git %cd tinyfive # run examples
+!python3 examples.py # run test suite !python3 tests.py ``` ## Speed - TinyFive
+is not optimized for speed (but for ease-of-use and [LOC](https://
+en.wikipedia.org/wiki/Source_lines_of_code)). - You might be able to use
+[Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see
+e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-
+riscv2016.pdf) for details). - If you only use the upper-case instructions such
+as `ADD()`, then TinyFive is very fast because there is no instruction
+decoding. And you should be able to accelerate it on a GPU or TPU. - If you use
+the lower-case instructions with `asm()` and `exe()`, then execution of these
+functions is slow as they involve look-up and string matching with O(n)
+complexity where "n" is the total number of instructions. The current
+implementations of `asm()` and `dec()` are optimized for ease-of-use and
+readability. A faster implementation would collapse multiple look-ups into one
+look-up, optimize the pattern-matching for the instruction decoding (bits -
+> instruction), and change the order of the instructions so that more
+frequently used instructions are at the top of the list. [Here is an older
+version](https://github.com/OpenMachine-ai/tinyfive/blob/
+2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster
+`dec()` function that collapses two look-ups (`bits -> instruction` and
+`instruction -> uppeer-case instruction`) and doesn't use `fnmatch`. ## Latest
+status - TinyFive is still under construction, many things haven't been
+implemented and tested yet. - 37 of the 40 base instructions (RV32I), all
+instructions of the M-extension (RV32M) and the F-extension (RV32F) with the
+default rounding mode are already implemented, and many of them are tested.
+(The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not
+applicable here.) - Remaining work: improve testing, add perhaps more
+extensions. See TODOs in the code for more details. ## Comparison The table
+below compares TinyFive with other [ISS](https://en.wikipedia.org/wiki/
+Instruction_set_simulator) and emulator projects. | ISS | Author | Language |
+Mature? | Extensions | LOC | | --- | ------ | -------- | ------- | ---------- |
+--- | | [TinyFive](https://github.com/OpenMachine-ai/tinyfive) | OpenMachine |
+Python | No | I, M, some F | < 1k | | [Pydgin](https://github.com/cornell-brg/
+pydgin) | Cornell University | Python, C | Last update 2016 | A, D, F, I, M | |
+| [Spike](https://github.com/riscv-software-src/riscv-isa-sim) | UC Berkeley |
+C, C++ | Yes | All | | | [QEMU](https://www.qemu.org/) | [Fabrice Bellard]
+(https://en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [TinyEMU]
+(https://bellard.org/tinyemu/) | [Fabrice Bellard](https://en.wikipedia.org/
+wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim](https://github.com/
+riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All | | | [Whisper]
+(https://github.com/chipsalliance/SweRV-ISS) | Western Digital | C, C++ | Yes |
+Almost all | | | [Sail Model](https://github.com/riscv/sail-riscv) | Cambridge,
+Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https://github.com/PiMaker/
+rvc) | PiMaker | C | | | | | [mini-rv32ima](https://github.com/cnlohr/mini-
+rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr | < 1k | ## References
+- Official [RISC-V spec](https://github.com/riscv/riscv-isa-manual/releases/
+download/Ratified-IMAFDQC/riscv-spec-20191213.pdf) - See [this RISC-V card]
+(https://inst.eecs.berkeley.edu/~cs61c/fa18/img/riscvcard.pdf) for a brief
+description of most instructions. See also the [RISC-V reference card](http://
+riscvbook.com/greencard-20181213.pdf). - Book "The RISC-V Reader: An Open
+Architecture Atlas" by David Patterson and Andrew Waterman. Appendix A of this
+book defines all instructions. The Spanish version of this book is [available
+for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
+other free versions are [available here](http://riscvbook.com). - Pydgin
+[paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and
+[video](https://youtu.be/-p_AGki7Vsk) - [Online simulator](https://ascslab.org/
+research/briscv/simulator/simulator.html) for debug ## Tiny Tech promise
+Similar to [tinygrad](https://github.com/geohot/tinygrad), [micrograd](https://
+github.com/karpathy/micrograd), and other âtiny techâ projects, we believe
+that core technology should be simple and small (in terms of LOC). Therefore,
+we will make sure that the core of TinyFive (without tests and examples) will
+always be below 1000 lines. Simplicity and size (in terms of number of
+instructions) is a key feature of [RISC](https://en.wikipedia.org/wiki/
+Reduced_instruction_set_computer): the "R" in RISC stands for "reduced" (as
+opposed to complex CISC). Specifically, the ISA manual of RISC-V has only ~200
+pages while the ARM-32 manual is over 2000 pages long according to Fig. 1.6 of
+the [RISC-V Reader](http://riscvbook.com/spanish/guia-practica-de-risc-v-
+1.0.5.pdf).
      [https://github.com/OpenMachine-ai/tinyfive/blob/main/misc/logo.jpg]
```

### Comparing `tinyfive-0.0.13/pyproject.toml` & `tinyfive-0.0.14/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyfive"
-version = "0.0.13"
+version = "0.0.14"
 authors = [
   { name="Open Machine", email="tinyfive@openmachine.ai" },
 ]
 description = "TinyFive is a lightweight RISC-V emulator and assembler written entirely in Python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tinyfive-0.0.13/PKG-INFO` & `tinyfive-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyfive
-Version: 0.0.13
+Version: 0.0.14
 Summary: TinyFive is a lightweight RISC-V emulator and assembler written entirely in Python
 Project-URL: Homepage, https://github.com/OpenMachine-ai/tinyfive
 Project-URL: Bug Tracker, https://github.com/OpenMachine-ai/tinyfive/issues
 Author-email: Open Machine <tinyfive@openmachine.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,14 +29,15 @@
 
 ## Contents
 - [Installation](#installation)
 - [Usage](#usage)
   - [Example 1: Multiply two numbers](#example-1-multiply-two-numbers)
   - [Example 2: Add two vectors](#example-2-add-two-vectors)
   - [Example 3: Multiply two matrices](#example-3-multiply-two-matrices)
+  - [Example 4: Neural network layers](#example-4-neural-network-layers)
 - [Running in colab](#running-in-colab)
 - [Running without package](#running-without-package)
 - [Speed](#speed)
 - [Latest status](#latest-status)
 - [Comparison](#comparison)
 - [References](#references)
 - [Tiny Tech promise](#tiny-tech-promise)
@@ -394,14 +395,17 @@
 - For 16x16 or larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/discovering-novel-algorithms-with-alphatensor) can reduce the total number of multiplications and additions if they are applied recursively.
 
 |             | Image | Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup |
 |:-----------:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:-------:|
 | Example 3.3 | 92B   | 9         | 80   | 16    | 64  | 89  | 20     | 269       | 1       |
 | Example 3.4 | 640B  | 22        | 32   | 16    | 64  | 48  | 0      | 160       | 1.7     |
 
+### Example 4: Neural network layers
+Coming soon, see [file layer_examples.py](layer_examples.py)
+
 ## Running in colab
 <a href="https://colab.research.google.com/github/OpenMachine-ai/tinyfive/blob/main/misc/colab.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Colab" height="20">
 </a>  This is the quickest way to get started and should work on any machine.
 
 If you have a free Google Drive account, you can make a copy of this colab via the menu `File` -> `Save a copy in Drive`. Now you can edit the code.
 
@@ -441,15 +445,15 @@
 
 # run test suite
 !python3 tests.py
 ```
 
 ## Speed
 - TinyFive is not optimized for speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/Source_lines_of_code)).
-- You could use PyPy to speed it up (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
+- You might be able to use [Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) for details).
 - If you only use the upper-case instructions such as `ADD()`, then TinyFive is very fast because there is no instruction decoding. And you should be able to accelerate it on a GPU or TPU.
 - If you use the lower-case instructions with `asm()` and `exe()`, then execution of these functions is slow as they involve look-up and string matching with O(n) complexity where "n" is the total number of instructions. The current implementations of `asm()` and `dec()` are optimized for ease-of-use and readability. A faster implementation would collapse multiple look-ups into one look-up, optimize the pattern-matching for the instruction decoding (bits -> instruction), and change the order of the instructions so that more frequently used instructions are at the top of the list. [Here is an older version](https://github.com/OpenMachine-ai/tinyfive/blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster `dec()` function that collapses two look-ups (`bits -> instruction` and `instruction -> uppeer-case instruction`) and doesn't use `fnmatch`.
 
 ## Latest status
 - TinyFive is still under construction, many things haven't been implemented and tested yet.
 - 37 of the 40 base instructions (RV32I), all instructions of the M-extension (RV32M) and the F-extension (RV32F) with the default rounding mode are already implemented, and many of them are tested.  (The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not applicable here.)
 - Remaining work: improve testing, add perhaps more extensions. See TODOs in the code for more details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyfive Version: 0.0.13 Summary: TinyFive is a
+Metadata-Version: 2.1 Name: tinyfive Version: 0.0.14 Summary: TinyFive is a
 lightweight RISC-V emulator and assembler written entirely in Python Project-
 URL: Homepage, https://github.com/OpenMachine-ai/tinyfive Project-URL: Bug
 Tracker, https://github.com/OpenMachine-ai/tinyfive/issues Author-email: Open
 Machine
 openmachine.ai> License-File: LICENSE Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist:
@@ -21,15 +21,16 @@
 learn how RISC-V works, TinyFive lets you play with instructions and assembly
 code. - Can be very fast if you only use the upper-case instructions defined in
 the [first ~200 lines of machine.py](machine.py#L1-L200). - [Fewer than 1000
 lines](machine.py) of code (w/o tests and examples) - Uses NumPy for math ##
 Contents - [Installation](#installation) - [Usage](#usage) - [Example 1:
 Multiply two numbers](#example-1-multiply-two-numbers) - [Example 2: Add two
 vectors](#example-2-add-two-vectors) - [Example 3: Multiply two matrices]
-(#example-3-multiply-two-matrices) - [Running in colab](#running-in-colab) -
+(#example-3-multiply-two-matrices) - [Example 4: Neural network layers]
+(#example-4-neural-network-layers) - [Running in colab](#running-in-colab) -
 [Running without package](#running-without-package) - [Speed](#speed) - [Latest
 status](#latest-status) - [Comparison](#comparison) - [References](#references)
 - [Tiny Tech promise](#tiny-tech-promise) ## Installation ``` pip install
 tinyfive ``` ## Usage TinyFive can be used in the following three ways: -
 **Option A:** Use upper-case instructions such as `ADD()` and `MUL()`, see
 examples 1.1, 1.2, 2.1, and 3.1 below. - **Option B:** Use `asm()` and `exe()`
 functions without branch instructions, see examples 1.3 and 2.2 below. -
@@ -247,92 +248,95 @@
 larger matrices, [Strassen's algorithm](https://en.wikipedia.org/wiki/
 Strassen_algorithm) and [DeepMind's AlphaTensor](https://www.deepmind.com/blog/
 discovering-novel-algorithms-with-alphatensor) can reduce the total number of
 multiplications and additions if they are applied recursively. | | Image |
 Registers | Load | Store | Mul | Add | Branch | Total ops | Speedup | |:-------
 ----:|:-----:|:---------:|:----:|:-----:|:---:|:---:|:------:|:---------:|:----
 ---:| | Example 3.3 | 92B | 9 | 80 | 16 | 64 | 89 | 20 | 269 | 1 | | Example
-3.4 | 640B | 22 | 32 | 16 | 64 | 48 | 0 | 160 | 1.7 | ## Running in colab
-[Colab] This is the quickest way to get started and should work on any machine.
-If you have a free Google Drive account, you can make a copy of this colab via
-the menu `File` -> `Save a copy in Drive`. Now you can edit the code.
-Alternatively, start a new colab in your Google Drive as follows: [Go here]
-(https://drive.google.com/drive/my-drive) and click on `New` -> `More` -
-> `Google Colaboratory`. Then copy below lines into your colab: ```python !pip
-install tinyfive from tinyfive.machine import machine import numpy as np m =
-machine(mem_size=4000) # instantiate RISC-V machine with 4KB of memory ``` ##
-Running without package If you don't want to use the TinyFive python package,
-then you can clone the latest repo and install numpy as follows: ```bash git
-clone https://github.com/OpenMachine-ai/tinyfive.git cd tinyfive pip install
-numpy ``` To run the examples, type: ```bash python3 examples.py ``` To run the
-test suite, type: ```bash python3 tests.py ``` If you don't want to run above
-steps on your local machine, you can run it in a colab as follows: Start a new
-colab in your Google Drive by [going here](https://drive.google.com/drive/my-
-drive) and clicking on `New` -> `More` -> `Google Colaboratory`. Then copy
-below lines into your colab: ```python !git clone https://github.com/
-OpenMachine-ai/tinyfive.git %cd tinyfive # run examples !python3 examples.py #
-run test suite !python3 tests.py ``` ## Speed - TinyFive is not optimized for
-speed (but for ease-of-use and [LOC](https://en.wikipedia.org/wiki/
-Source_lines_of_code)). - You could use PyPy to speed it up (see e.g. the
-[Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf)
-for details). - If you only use the upper-case instructions such as `ADD()`,
-then TinyFive is very fast because there is no instruction decoding. And you
-should be able to accelerate it on a GPU or TPU. - If you use the lower-case
-instructions with `asm()` and `exe()`, then execution of these functions is
-slow as they involve look-up and string matching with O(n) complexity where "n"
-is the total number of instructions. The current implementations of `asm()` and
-`dec()` are optimized for ease-of-use and readability. A faster implementation
-would collapse multiple look-ups into one look-up, optimize the pattern-
-matching for the instruction decoding (bits -> instruction), and change the
-order of the instructions so that more frequently used instructions are at the
-top of the list. [Here is an older version](https://github.com/OpenMachine-ai/
-tinyfive/blob/2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive
-with a faster `dec()` function that collapses two look-ups (`bits -
-> instruction` and `instruction -> uppeer-case instruction`) and doesn't use
-`fnmatch`. ## Latest status - TinyFive is still under construction, many things
-haven't been implemented and tested yet. - 37 of the 40 base instructions
-(RV32I), all instructions of the M-extension (RV32M) and the F-extension
-(RV32F) with the default rounding mode are already implemented, and many of
-them are tested. (The three missing RV32I instructions `fence`, `ebreak`, and
-`ecall` are not applicable here.) - Remaining work: improve testing, add
-perhaps more extensions. See TODOs in the code for more details. ## Comparison
-The table below compares TinyFive with other [ISS](https://en.wikipedia.org/
-wiki/Instruction_set_simulator) and emulator projects. | ISS | Author |
-Language | Mature? | Extensions | LOC | | --- | ------ | -------- | ------- | -
---------- | --- | | [TinyFive](https://github.com/OpenMachine-ai/tinyfive) |
-OpenMachine | Python | No | I, M, some F | < 1k | | [Pydgin](https://
-github.com/cornell-brg/pydgin) | Cornell University | Python, C | Last update
-2016 | A, D, F, I, M | | | [Spike](https://github.com/riscv-software-src/riscv-
-isa-sim) | UC Berkeley | C, C++ | Yes | All | | | [QEMU](https://www.qemu.org/
-) | [Fabrice Bellard](https://en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes
-| All | | | [TinyEMU](https://bellard.org/tinyemu/) | [Fabrice Bellard](https:/
-/en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim]
-(https://github.com/riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All
-| | | [Whisper](https://github.com/chipsalliance/SweRV-ISS) | Western Digital |
-C, C++ | Yes | Almost all | | | [Sail Model](https://github.com/riscv/sail-
-riscv) | Cambridge, Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https:/
-/github.com/PiMaker/rvc) | PiMaker | C | | | | | [mini-rv32ima](https://
-github.com/cnlohr/mini-rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr
-| < 1k | ## References - Official [RISC-V spec](https://github.com/riscv/riscv-
-isa-manual/releases/download/Ratified-IMAFDQC/riscv-spec-20191213.pdf) - See
-[this RISC-V card](https://inst.eecs.berkeley.edu/~cs61c/fa18/img/
-riscvcard.pdf) for a brief description of most instructions. See also the
-[RISC-V reference card](http://riscvbook.com/greencard-20181213.pdf). - Book
-"The RISC-V Reader: An Open Architecture Atlas" by David Patterson and Andrew
-Waterman. Appendix A of this book defines all instructions. The Spanish version
-of this book is [available for free](http://riscvbook.com/spanish/guia-
-practica-de-risc-v-1.0.5.pdf), other free versions are [available here](http://
-riscvbook.com). - Pydgin [paper](https://www.csl.cornell.edu/~berkin/ilbeyi-
-pydgin-riscv2016.pdf) and [video](https://youtu.be/-p_AGki7Vsk) - [Online
-simulator](https://ascslab.org/research/briscv/simulator/simulator.html) for
-debug ## Tiny Tech promise Similar to [tinygrad](https://github.com/geohot/
-tinygrad), [micrograd](https://github.com/karpathy/micrograd), and other
-âtiny techâ projects, we believe that core technology should be simple and
-small (in terms of LOC). Therefore, we will make sure that the core of TinyFive
-(without tests and examples) will always be below 1000 lines. Simplicity and
-size (in terms of number of instructions) is a key feature of [RISC](https://
-en.wikipedia.org/wiki/Reduced_instruction_set_computer): the "R" in RISC stands
-for "reduced" (as opposed to complex CISC). Specifically, the ISA manual of
-RISC-V has only ~200 pages while the ARM-32 manual is over 2000 pages long
-according to Fig. 1.6 of the [RISC-V Reader](http://riscvbook.com/spanish/guia-
-practica-de-risc-v-1.0.5.pdf).
+3.4 | 640B | 22 | 32 | 16 | 64 | 48 | 0 | 160 | 1.7 | ### Example 4: Neural
+network layers Coming soon, see [file layer_examples.py](layer_examples.py) ##
+Running in colab [Colab] This is the quickest way to get started and should
+work on any machine. If you have a free Google Drive account, you can make a
+copy of this colab via the menu `File` -> `Save a copy in Drive`. Now you can
+edit the code. Alternatively, start a new colab in your Google Drive as
+follows: [Go here](https://drive.google.com/drive/my-drive) and click on `New`
+-> `More` -> `Google Colaboratory`. Then copy below lines into your colab:
+```python !pip install tinyfive from tinyfive.machine import machine import
+numpy as np m = machine(mem_size=4000) # instantiate RISC-V machine with 4KB of
+memory ``` ## Running without package If you don't want to use the TinyFive
+python package, then you can clone the latest repo and install numpy as
+follows: ```bash git clone https://github.com/OpenMachine-ai/tinyfive.git cd
+tinyfive pip install numpy ``` To run the examples, type: ```bash python3
+examples.py ``` To run the test suite, type: ```bash python3 tests.py ``` If
+you don't want to run above steps on your local machine, you can run it in a
+colab as follows: Start a new colab in your Google Drive by [going here](https:
+//drive.google.com/drive/my-drive) and clicking on `New` -> `More` -> `Google
+Colaboratory`. Then copy below lines into your colab: ```python !git clone
+https://github.com/OpenMachine-ai/tinyfive.git %cd tinyfive # run examples
+!python3 examples.py # run test suite !python3 tests.py ``` ## Speed - TinyFive
+is not optimized for speed (but for ease-of-use and [LOC](https://
+en.wikipedia.org/wiki/Source_lines_of_code)). - You might be able to use
+[Codon](https://github.com/exaloop/codon) or PyPy to speed up TinyFive (see
+e.g. the [Pydgin paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-
+riscv2016.pdf) for details). - If you only use the upper-case instructions such
+as `ADD()`, then TinyFive is very fast because there is no instruction
+decoding. And you should be able to accelerate it on a GPU or TPU. - If you use
+the lower-case instructions with `asm()` and `exe()`, then execution of these
+functions is slow as they involve look-up and string matching with O(n)
+complexity where "n" is the total number of instructions. The current
+implementations of `asm()` and `dec()` are optimized for ease-of-use and
+readability. A faster implementation would collapse multiple look-ups into one
+look-up, optimize the pattern-matching for the instruction decoding (bits -
+> instruction), and change the order of the instructions so that more
+frequently used instructions are at the top of the list. [Here is an older
+version](https://github.com/OpenMachine-ai/tinyfive/blob/
+2aa4987391561c9c6692602ed3fccdeaee333e0b/tinyfive.py) of TinyFive with a faster
+`dec()` function that collapses two look-ups (`bits -> instruction` and
+`instruction -> uppeer-case instruction`) and doesn't use `fnmatch`. ## Latest
+status - TinyFive is still under construction, many things haven't been
+implemented and tested yet. - 37 of the 40 base instructions (RV32I), all
+instructions of the M-extension (RV32M) and the F-extension (RV32F) with the
+default rounding mode are already implemented, and many of them are tested.
+(The three missing RV32I instructions `fence`, `ebreak`, and `ecall` are not
+applicable here.) - Remaining work: improve testing, add perhaps more
+extensions. See TODOs in the code for more details. ## Comparison The table
+below compares TinyFive with other [ISS](https://en.wikipedia.org/wiki/
+Instruction_set_simulator) and emulator projects. | ISS | Author | Language |
+Mature? | Extensions | LOC | | --- | ------ | -------- | ------- | ---------- |
+--- | | [TinyFive](https://github.com/OpenMachine-ai/tinyfive) | OpenMachine |
+Python | No | I, M, some F | < 1k | | [Pydgin](https://github.com/cornell-brg/
+pydgin) | Cornell University | Python, C | Last update 2016 | A, D, F, I, M | |
+| [Spike](https://github.com/riscv-software-src/riscv-isa-sim) | UC Berkeley |
+C, C++ | Yes | All | | | [QEMU](https://www.qemu.org/) | [Fabrice Bellard]
+(https://en.wikipedia.org/wiki/Fabrice_Bellard) | C | Yes | All | | | [TinyEMU]
+(https://bellard.org/tinyemu/) | [Fabrice Bellard](https://en.wikipedia.org/
+wiki/Fabrice_Bellard) | C | Yes | All | | | [riscvOVPsim](https://github.com/
+riscv-ovpsim/imperas-riscv-tests) | Imperas | C | Yes | All | | | [Whisper]
+(https://github.com/chipsalliance/SweRV-ISS) | Western Digital | C, C++ | Yes |
+Almost all | | | [Sail Model](https://github.com/riscv/sail-riscv) | Cambridge,
+Edinburgh | Sail, C | Yes | All | | | [PiMaker/rvc](https://github.com/PiMaker/
+rvc) | PiMaker | C | | | | | [mini-rv32ima](https://github.com/cnlohr/mini-
+rv32ima) | Charles Lohr | C | | A, I, M, Zifencei, Zicsr | < 1k | ## References
+- Official [RISC-V spec](https://github.com/riscv/riscv-isa-manual/releases/
+download/Ratified-IMAFDQC/riscv-spec-20191213.pdf) - See [this RISC-V card]
+(https://inst.eecs.berkeley.edu/~cs61c/fa18/img/riscvcard.pdf) for a brief
+description of most instructions. See also the [RISC-V reference card](http://
+riscvbook.com/greencard-20181213.pdf). - Book "The RISC-V Reader: An Open
+Architecture Atlas" by David Patterson and Andrew Waterman. Appendix A of this
+book defines all instructions. The Spanish version of this book is [available
+for free](http://riscvbook.com/spanish/guia-practica-de-risc-v-1.0.5.pdf),
+other free versions are [available here](http://riscvbook.com). - Pydgin
+[paper](https://www.csl.cornell.edu/~berkin/ilbeyi-pydgin-riscv2016.pdf) and
+[video](https://youtu.be/-p_AGki7Vsk) - [Online simulator](https://ascslab.org/
+research/briscv/simulator/simulator.html) for debug ## Tiny Tech promise
+Similar to [tinygrad](https://github.com/geohot/tinygrad), [micrograd](https://
+github.com/karpathy/micrograd), and other âtiny techâ projects, we believe
+that core technology should be simple and small (in terms of LOC). Therefore,
+we will make sure that the core of TinyFive (without tests and examples) will
+always be below 1000 lines. Simplicity and size (in terms of number of
+instructions) is a key feature of [RISC](https://en.wikipedia.org/wiki/
+Reduced_instruction_set_computer): the "R" in RISC stands for "reduced" (as
+opposed to complex CISC). Specifically, the ISA manual of RISC-V has only ~200
+pages while the ARM-32 manual is over 2000 pages long according to Fig. 1.6 of
+the [RISC-V Reader](http://riscvbook.com/spanish/guia-practica-de-risc-v-
+1.0.5.pdf).
      [https://github.com/OpenMachine-ai/tinyfive/blob/main/misc/logo.jpg]
```

