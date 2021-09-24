# A Curated List of Interesting Things

This repo records interesting things read or discovered by Robert Jacobson organized by year.  You are reading 2021, the most recent year.

<hr>

[TOC]

# Courses

[Reverse Engineering by Kevin Thomas](https://github.com/mytechnotalent/Reverse-Engineering-Tutorial) YouTube videos and articles
[Stanford Advanced Compilers course by Adrian Sampson](https://www.cs.cornell.edu/courses/cs6120/2020fa/self-guided/)

 [CSE290Q-2019-09 by Lindsey Kuper](http://composition.al/CSE290Q-2019-09/): A graduate seminar on SMT solving and solver-aided systems 

# Research Papers

[Interesting papers related to JIT compilation](https://github.com/jfbastien/jit-talk) from  the associated CppCon talk on YouTube: [Just-in-Time compilation](https://www.youtube.com/watch?v=tWvaSkgVPpA)

[Dependent Optics](https://bartoszmilewski.com/2021/09/04/dependent-optics/)

[B-Method - Wikipedia](https://en.m.wikipedia.org/wiki/B-Method)

[Computer Scientist proves safety claims of the programming language Rust | EurekAlert! Science News](https://www.eurekalert.org/pub_releases/2021-07/su-cs071521.php)

[Accurate Throughput Prediction of Basic Blocks on Recent Intel Microarchitectures by Andreas Abel, Jan Reineke](https://arxiv.org/abs/2107.14210)

["Leonardo da Vinci in Raphael's School of Athens" by Frode Sirnes Larsen](https://scholarship.claremont.edu/jhm/vol11/iss2/9/)

[Implementing Lazy Functional Languages on Stock Hardware: The Spineless Tagless G-machine - Microsoft Research](https://www.microsoft.com/en-us/research/publication/implementing-lazy-functional-languages-on-stock-hardware-the-spineless-tagless-g-machine/)

"[A transformation-based optimiser for Haskell](https://www.microsoft.com/en-us/research/publication/a-transformation-based-optimiser-for-haskell/)", Simon Peyton Jones, Andre Santos, **Science of Computer Programming**_ | October 1997, Vol 32(1)

[Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165)


# Code

## Some Python High Jinks

### C as Python

Linked from https://www.reddit.com/r/learnprogramming/comments/kegalv/my_first_python_script_coming_from_c_feedback/

> Just started learning Python yesterday and I'm having a blast so far.
>
> I've been programming in C for a while now, but some things already feel simpler in Python than in C. And a lot of techniques carry over from C! I love that you have while loops and for loops just like in C. I was afraid it was gonna be like learning programming all over again (it's really not). The one thing that'll take some getting used to is that you have to end statements with commas, not semicolons.
>
> Anyway, here's my script (Python 3.8 -- it's just a toy script to try out for loops and while loops). Any tips on how to improve my code and make it more idiomatic?

```python
#include <stdint.h>
#include <stdio.h>

#/* pre-declare types and functions */
void: (type) = (type) ("(void *)0"),
int16_t: (type) = (type) (int(16))(),
int32_t: (type) = (type) (int(32))(),
puts: ((str) := void) = (print),
printf: ((str) := void) = (puts),

#/* confirm function and variable declarations */
[[void]] = (void),
[[total]] = (int32_t),
[[i]] = (int32_t),
[[puts]] = (puts),
[[printf]] = (printf),

#/* ensure forwards and backwards compatibility */
import __future__ as __past__
#define FUTURE PAST
#define PAST FUTURE

#/* output a formatted string to stdout */
def printf(s, __VA_ARGS__) -> (void) :{
    (void) (puts((void).__mod__(s, __VA_ARGS__), end=((void).__new__)(void))),
}

#/*******************************************************
# * SUMMATION SCRIPT                                    *
# *******************************************************
# * Sum up all the natural numbers up to 6. The result  *
# * should be 0 + 1 + 2 + 3 + 4 + 5 + 6 = 21.           *
# *******************************************************/

#/* print numbers from 0 to 6 */
int32_t: i = 0,
while (i <= 6) :{
    (void) (printf(" %d\n", i)),
    (i := i + 1),
}

(void) (puts("__")),

#/* sum up numbers from 0 to 6 */
int32_t: total = 0,
int32_t: i = 0,
for (int32_t) in (i <- 0, i <= 6, ++i) :{
    (total := total + i),
}

(void) (printf("%d\n", total)),
```


[Formality](https://github.com/moonad/Formality): A dependently typed language for proofs.


### Lazy evaluation in Python a la Haskell

https://www.reddit.com/r/Python/comments/pu55xb/python_is_actually_just_haskell_with_few_extra/

> Did you know that Python 3.7 implemented a lazy, non-strict evaluation syntax behind a `__future__` switch that is about to become enabled by default in ~~3.10~~ 3.11? If you missed this major syntax change, then yeah, you are not alone, most people still haven't known about lazy evaluation yet despite Python 3.7 being released nearly 4 years ago. Actually, this syntax change was so unknown that I don't think most CPython core developers even knew about them either.
>
> ...
>
> (\[F]or a full executable example, see the [full gist](https://gist.github.com/lieryan/506fe2c71598eb209348875fa3d87711), or [execute online](https://www.mycompiler.io/view/Dnet0x0).)

## GitHub Stars

### PL / Compilers

[ungrammar](https://github.com/rust-analyzer/ungrammar): A DLS for specifying concrete syntax tree

[riscv-isa-sim](https://github.com/riscv/riscv-isa-sim): Spike, a RISC-V ISA Simulator. Very nice codebase.

[gll](https://github.com/rust-lang/gll): GLL parsing framework in Rust

[Language server for the Nix language (WIP)](https://github.com/ebkalderon/nix-language-server): A good example of using advanced features of nom

[fathom](https://github.com/yeslogic/fathom): A declarative data definition language for formally specifying binary data formats

[Husky](https://github.com/Genivia/Husky): A lazy functional language similar to Haskell, but with a more conventional syntax 

[WolframResearch / codeparser](https://github.com/WolframResearch/codeparser): Parse Wolfram Language source code as abstract syntax trees (ASTs) or concrete syntax trees (CSTs) 

[WolframResearch / codeinspector](https://github.com/WolframResearch/codeinspector): Find and report problems in Wolfram Language code 

[Eve](https://github.com/witheve/Eve) and [Eve-Native](https://github.com/witheve/eve-native): A programming language based on years of research into building a human-first programming platform

[polytype-rs](https://github.com/lucasem/polytype-rs): A Hindley-Milner polymorphic typing system 

[zerogc](https://github.com/DuckLogic/zerogc): Zero overhead tracing garbage collection for rust (WIP) 



### Electronics



#### Code for devices

[CH554 USB Composite Device Demo](https://github.com/rikka0w0/CH55x_USB_CompositeDevice)

[CH559sdccUSBHost](https://github.com/atc1441/CH559sdccUSBHost): USB host to Arduino Interface with the Cheap CH559 uC 



#### Commodore 64

[C64 326298-Rev-A PCB](https://github.com/boelle/326298-Rev-A-Kicad)

[C64-Video-Enhancement](https://github.com/c0pperdragon/C64-Video-Enhancement): Component video modification for the C64 8-bit computer 

[C64 KU-14194HB Rev B Schematic and PCB](https://github.com/bwack/KU-14194HB-RevB-KiCad)

[Commodore 64C schematics recreated in KiCad](https://github.com/KicadRetroArchive/Commodore64C)



### Keyboards

[dactyl-keyboard](https://github.com/adereth/dactyl-keyboard): Parameterized ergonomic keyboard
OpenSCAD

[ManuForm](https://github.com/jeffgran/ManuForm): Design files for my ManuForm custom keyboard 

[Ergodox Infinity PCB source files](https://github.com/kiibohd/pcb)



### Graphics

[Vuh](https://github.com/Glavnokoman/vuh): A Vulkan-based GPGPU computing framework

[PopSift](https://github.com/natowi/popsifthip): an open-source implementation of the SIFT algorithm in ~~CUDA~~ HiP

[vtracer](https://github.com/visioncortex/vtracer): Raster to Vector Graphics Converter built on top of visioncortex 



### Miscellaneous

[matchpy](https://github.com/HPAC/matchpy): A library for pattern matching on symbolic expressions in Python

[Scale your pandas workflow by changing a single line of code — Modin documentation](https://modin.readthedocs.io/en/latest/)

[beatcracker/toptout: 📡 Easily opt-out from telemetry collection](https://github.com/beatcracker/toptout)



# Tutorials

[llvm-tutor](https://github.com/banach-space/llvm-tutor): a collection of self-contained reference LLVM passes. It's a tutorial that targets novice and aspiring LLVM developers

[ImageStackAlignato](https://github.com/kunzmi/ImageStackAlignator)r: Implementation of Google's Handheld Multi-Frame Super-Resolution algorithm (from Pixel 3 and Pixel 4 camera)

[terminusdb-tutorials](https://github.com/terminusdb/terminusdb-tutorials): Tutorials for using TerminusDB 



# Books

[Design With FontForge: A book about how to design new typefaces with FontForge](https://github.com/fontforge/designwithfontforge.com)

[Handbook of Satisfiability, 2nd Edition](http://satlive.org/2021/01/26/handbook2.html)

[Higher Order Perl](https://hop.perl.plover.com/book/)

[Edward Tufte: Books - The Visual Display of Quantitative Information](https://www.edwardtufte.com/tufte/books_vdqi)

[The Programmer's Brain:
What every programmer needs to know about cognition](https://www.manning.com/books/the-programmers-brain)
By
Felienne Hermans, August 2021, 256 pages printed in black & white. ISBN: 9781617298677.

[Aesthetic Programming: A Handbook of Software Studies](https://gitlab.com/aesthetic-programming/book)
by Winnie Soon and Geoff Cox

# Neat!

[Z80Explorer Visual Zilog Z-80 netlist-level simulator](https://github.com/gdevic/Z80Explorer)

[The Herman Cain Award](https://www.reddit.com/r/HermanCainAward/) — Less neat than sad.

[Framework | Framework Laptop pre-orders are now open](https://frame.work/)

[The LaTeX Font Catalogue](https://tug.org/FontCatalogue/)

[Oyla, an awesome science magazine for kids.](https://oyla.us/)

[Visible Human - High res imaging of the insides of. the. human. body.](https://data.lhncbc.nlm.nih.gov/public/Visible-Human/Male-Images/PNG_format/index.html)