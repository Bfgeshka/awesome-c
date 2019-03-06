# Awesome C #

A curated list of C good stuff.

**An important note:** first and foremost linked resources are for C, therefore
C++ is an afterthought.

**Note:** there are several awesome-c lists already, but they are having
somewhat different sets of libraries in them. This list tries to incorporate
them all, and many more other resources. Consider it my personal cheat sheet and
index for easier search instead of github stars. Also, original list categories
are a mess.

Incorporated lists:

* https://github.com/aleksandar-todorovic/awesome-c (rare updates, too vague and
  sometimes mismatched categories, not very wide selection of content)
* https://github.com/kozross/awesome-c (updated regularly, but has even less
  content than one above)
* https://github.com/uhub/awesome-c (regular updated, much more content, but
  much more of it doesn't even belong to C list. Also, no structure at all)

--------------------------------------------------------------------------------

## Index ##

* [Meta](#meta)
	* [Standarts](#standarts)
	* [Tooling](#tooling)
		* [Build Systems](#build-systems)
		* [Compilers](#compilers)
		* [Debugging and Analysis](#debugging-and-analysis)
		* [Documentation Generation](#documentation-generation)
		* [Editors](#editors)
		* [Microsoft Windows Environment](#microsoft-windows-environment)
		* [Profiling](#profiling)
		* [Text Editor Extensions](#text-editor-extensions)
		* [Utilities](#utilities)
	* [Reading material](#reading-material)
		* [Books](#books)
			* [Reference Books](#reference-books)
			* [Beginner Books](#beginner-books)
			* [Intermediate Books](#intermediate-books)
			* [Advanced Books](#advanced-books)
		* [Articles and Other Resources](#articles-and-other-resources)
			* [Reference](#reference)
			* [Benchmarks](#benchmarks)
			* [Beginner Level](#beginner-level)
			* [Intermediate Level](#intermediate-level)
			* [Advanced Level](#advanced-level)
		* [Code Examples](#code-examples)
		* [Courses](#courses)

--------------------------------------------------------------------------------

* [AI](#ai)
* [Algoritm Implementations](#algoritm-implementations)
* [Argument Parsing](#argument-parsing)
* [Calculations](#calculations)
* [Compression](#compression)
* [Concurrency and Parallelism](#concurrency-and-parallelism)
* [Crypto](#crypto)
* [Databases](#databases)
* [Data Structures](#data-structures)
* [Events](#events)
* [FFI](#ffi)
* [Flow Control and Language Extension](#flow-control-and-language-extension)
* [Game Development](#game-development)
* [Graphics](#graphics)
* [GUI](#gui)
* [Hardware Oriented](#hardware-oriented)
* [Hashing](#hashing)
* [Image Processing and Computer Vision](#image-processing-and-computer-vision)
* [Integrated Debugging](#integrated-debugging)
* [Lexing and Parsing](#lexing-and-parsing)
* [Memory Management](#memory-management)
* [Multimedia](#multimedia)
* [Multiple Purpose Libraries](#multiple-purpose-libraries)
* [Networking](#networking)
	* [DNS](#dns)
	* [HTTP](#http)
	* [Mail](#mail)
	* [Messaging](#messaging)
	* [Other Networking](#other-networking)
	* [Websockets](#websockets)
* [OS Specifics](#os-specifics)
* [Procedural Generation](#procedural-generation)
* [Regex](#regex)
* [Serialization](#serialization)
* [Source Code Collections](#source-code-collections)
* [Standard Libraries](#standart-libraries)
* [String Manipulation](#string-manipulation)
* [Structured File Processing](#structured-file-processing)
	* [Binaries](#binaries)
	* [CSV](#csv)
	* [JSON](#json)
	* [INI](#ini)
	* [Other Filetypes](#other-filetypes)
	* [XML](#xml)
	* [YAML](#yaml)
* [Testing](#testing)
* [TUI](#tui)
* [Web Frameworks](#web-frameworks)
* [Web Service APIs](#web-service-apis)

--------------------------------------------------------------------------------

* [Uncategorized](#uncategorized)
* [Unsorted](#unsorted)

--------------------------------------------------------------------------------

## Meta ##
### Standarts ###
* [Draft C89 standard][1-1]
* [Draft C99 standard][1-2]
* [Draft C11 standard][1-3]
* [Draft C18 standard][1-4]

[1-1]: https://port70.net/~nsz/c/c89/c89-draft.html
[1-2]: https://port70.net/~nsz/c/c99/n1256.html
[1-3]: https://port70.net/~nsz/c/c11/n1570.html
[1-4]: https://web.archive.org/web/20181230041359if_/http://www.open-std.org/jtc1/sc22/wg14/www/abq/c17_updated_proposed_fdis.pdf

### Tooling ###
#### Build Systems ####
* [aimake][2-1] - Build tool designed to avoid complex configurations. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Autoconf][2-2] - Extensible package of M4 macros that produce shell scripts
  to automatically configure software source code packages. Part of the
  Autotools. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Automake][2-3] - Tool for automatically generating `Makefile.in` files
  compliant with the GNU Coding Standards. Requires the use of Autoconf. Part of
  the Autotools. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Bazel][2-4] - Build system for various operating systems and targets. [``Apache-2.0``][Apache-2.0]
* [Buck][2-5] - Build system created and used by Facebook. [``Apache-2.0``][Apache-2.0]
* [CMake][2-6] - Cross-platform family of tools designed to build, package and
  test software. Written in C++11. [``BSD-3-Clause``][BSD-3-Clause]
* [GNU Make][2-7] - Tool which controls the generation of executables and other
  non-source files of a program. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GMSL][2-8] - GNU Make Standard Library; a collection of additional
  functionality for GNU Make. [``BSD-3-Clause``][BSD-3-Clause]
* [Jam][2-9] - Build system, designed to be easier than make. Understands C
  build rules implicitly. [``Jam License``][2-10]
* [Libtool][2-11] - Generic library support script. Part of the Autotools. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Meson][2-12] - Build system based on Ninja and Python. [``Apache-2.0``][Apache-2.0]
* [Ninja][2-13] - Small, simple build system with a focus on speed. [``Apache-2.0``][Apache-2.0]
* [Premake][2-14] - Generates project files for Visual Studio, Xcode and GNU
  Make. Targets suppport can be extended via modules. [``BSD-3-Clause``][BSD-3-Clause]
* [Qbs][2-15] - Modern build tool for software projects. [``LGPL-3.0-only``][LGPL-3.0-only]
* [qmake][2-16] - Build system included with the Qt Framework. [`GNU GPL3 with Qt Exception`][2-17]
* [SCons][2-18] - Software construction tool based on Python. [``MIT``][MIT]
* [xmake][2-19] - Cross-platform build utility based on Lua. [``Apache-2.0``][Apache-2.0]
* [zproject][2-20] - Project generator and build system support tool for ZeroMQ
  project. [``MPL-2.0``][MPL-2.0]
* [tup](http://gittup.org/tup/index.html) - Very fast, file-based, cross-platform build system. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)

[2-1]: http://nethack4.org/projects/aimake/
[2-2]: https://www.gnu.org/software/autoconf/autoconf.html
[2-3]: https://www.gnu.org/software/automake/automake.html
[2-4]: https://bazel.build/
[2-5]: https://buckbuild.com/
[2-6]: https://cmake.org/
[2-7]: https://www.gnu.org/software/make/
[2-8]: https://gmsl.sourceforge.net/
[2-9]: https://www.perforce.com/documentation/jam-documentation
[2-10]: https://en.wikipedia.org/wiki/Perforce_Jam#License
[2-11]: https://www.gnu.org/software/libtool/
[2-12]: http://mesonbuild.com/
[2-13]: https://github.com/ninja-build/ninja
[2-14]: https://github.com/premake/premake-core
[2-15]: http://doc.qt.io/qbs/
[2-16]: https://doc.qt.io/qt-5/qmake-manual.html
[2-17]: https://github.com/qt/qtbase/blob/5.11/LICENSE.GPL3-EXCEPT
[2-18]: https://www.scons.org/
[2-19]: https://xmake.io/
[2-20]: https://github.com/zeromq/zproject

#### Compilers ####
* [Clang][3-2] - Compiler for LLVM. Supports C11. [``NCSA``][NCSA]
* [CompCert][3-5] - Fully-verified C compiler. Supports almost all of C89. [`GPL2.1-or-later`][GPL-2.0-or-later]
* [GCC][3-1] a C compiler as part of its compiler set. Supports C11. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Intel SPMD][3-7] - Compiler for a variant of the C language, for single
  program, multiple data programming. [``Various licenses``][3-8]
* [PCC][3-3] - Venerable compiler. Supports C99. [``Various licenses``][3-4]
* [TCC][3-6] - Tiny C Compiler; a small, fast C compiler. Supports C99 (except
  complex types). [``LGPL2.1``][LGPL-2.1-only]
* [rui314/8cc](https://github.com/rui314/8cc) - A Small C Compiler
* [LuaDist/tcc](https://github.com/LuaDist/tcc) - Small but fast C compiler.  Supports ANSI C, most of the new ISO C99 standard, and many GNUC extensions, including inline assembly.

[3-1]: https://gcc.gnu.org/
[3-2]: https://clang.llvm.org/
[3-3]: http://pcc.ludd.ltu.se/
[3-4]: http://pcc.ludd.ltu.se/licenses/
[3-5]: http://compcert.inria.fr/
[3-6]: https://bellard.org/tcc/
[3-7]: http://ispc.github.io/
[3-8]: https://github.com/ispc/ispc/blob/master/LICENSE.txt

#### Debugging and Analysis ####
* [address-sanitizer][4-3] - Fast memory error detector. [``Apache-2.0``][Apache-2.0]
* [C-Reduce][4-1] - Tool that takes a large C file with a property of interest
  and automatically produces a much smaller C file that has the same property.
  Intended to help create minimal bug-demonstrating cases in complex code. [``BSD-3-Clause``][BSD-3-Clause]
* [CBMC][4-2] - C Bounded Model Checker; a tool for verification of array
  bounds, pointer safety and user-specified assertions. [``BSD-4-Clause``][BSD-4-Clause]
* [ClangCheck][4-4] - Static analysis tool, designed to work with Clang. [``NCSA``][NCSA]
* [Cppcheck][4-5] - Static analysis tool. Despite the name, works well with C. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GNU cflow][4-6] - Analyzes a collection of source files and prints a graph
  charting control flow in the program. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GNU Complexity][4-7] - Tool for measuring the complexity of source code. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [CScout][4-8] - Source code analyzer and refactoring browser for C programs. [``GPL-3.0-only``][GPL-3.0-only]
* [GNU DDD][4-9] - Graphical front-end for a range of command-line debuggers. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GDB][4-10] - GNU Project debugger. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [lldb][4-11] - LLVM debugger. [``NCSA``][NCSA]
* [rr][4-12] - Debugger that records non-deterministic executions to allow for
  deterministic debugging. [``BSD-2-Clause``][BSD-2-Clause]
* [Valgrind][4-13] - Range of dynamic analysis tools, including a leak checker. [``GPL-2.0-only``][GPL-2.0-only]
* [SVF-tools/SVF](https://github.com/SVF-tools/SVF) - Pointer Analysis and Program Dependence Analysis for C and C++ Programs

[4-1]: https://embed.cs.utah.edu/creduce/
[4-2]: https://www.cprover.org/cbmc/
[4-3]: https://github.com/google/sanitizers
[4-4]: https://clang.llvm.org/docs/ClangCheck.html
[4-5]: http://cppcheck.sourceforge.net/
[4-6]: http://www.gnu.org/software/cflow/
[4-7]: https://www.gnu.org/software/complexity/
[4-8]: https://www.spinellis.gr/cscout/
[4-9]: https://www.gnu.org/software/ddd/ddd.html
[4-10]: https://www.gnu.org/software/gdb/
[4-11]: https://lldb.llvm.org/
[4-12]: https://rr-project.org/
[4-13]: http://www.valgrind.org/

#### Documentation Generation ####
* [Cxref][5-1] - Generates documentation in either LaTeX, HTML, RTF or SGML. [``GPL-2.0-only``][GPL-2.0-only]
* [DocOnce][5-2] - Modestly tagged markup language that can be used to generate
  a range of formats. [``BSD-3-Clause``][BSD-3-Clause]
* [Doxygen][5-3] - De-facto standard tool for generating documentation from
  annotated sources. Can generate a large range of formats. [``GPL-2.0-only``][GPL-2.0-only]
* [GTK-Doc][5-4] - Tool for generating C documentation from annotated sources.
  Has support for the Autotools. Various licenses.

[5-1]: http://www.gedanken.org.uk/software/cxref/
[5-2]: https://hplgit.github.io/doconce/doc/web/index.html
[5-3]: http://www.doxygen.nl/
[5-4]: https://www.gtk.org/gtk-doc/

#### Editors ####
* [Anjuta DevStudio][6-1] - GNOME IDE. [``GPL-2.0-only``][GPL-2.0-only]
* [Atom][6-3] - Hackable text editor for the 21st century. [``MIT``][MIT]
* [Code::Blocks][6-2] - Extendable, configurable IDE supporting C. [``GPL-3.0-only``][GPL-3.0-only]
* [CodeLite][6-4] - Cross-platform IDE. [``GPL-2.0-only``][GPL-2.0-only]
* [Eclipse][6-6] - IDE written in Java. [``EPL``][6-7]
* [Geany][6-5] - Small and fast IDE. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [KDevelop][6-8] - KDE IDE. [``GPL-2.0-only``][GPL-2.0-only]
* [Qt Creator][6-9] - Cross-platform IDE written with C++ and Qt, part of the
  Qt SDK. Supports Clang Code Model. [``GNU GPL3 with Qt exception``][6-10]
* [Visual Studio Code][6-11] - Code editing, redefined. Visual Studio Code. [``MIT``][MIT]

[6-1]: http://anjuta.org/
[6-2]: http://www.codeblocks.org/
[6-3]: https://atom.io/
[6-4]: https://codelite.org/
[6-5]: https://www.geany.org/
[6-6]: http://www.eclipse.org/ide/
[6-7]: https://directory.fsf.org/wiki/License:EPL-1.0
[6-8]: https://www.kdevelop.org/
[6-9]: https://www.qt.io/qt-features-libraries-apis-tools-and-ide/#ide
[6-10]: https://github.com/qt-creator/qt-creator/blob/master/LICENSE.GPL3-EXCEPT
[6-11]: https://github.com/Microsoft/vscode

#### Microsoft Windows Environment ####
* [Cygwin][7-1] - Designed to emulate a POSIX-compatible environment extensively
  under Windows. [Various licenses, all open source][7-2].
* [MinGW-w64][7-3] - Minimalist environment for C development on Windows with
  64 bit support. [Various licenses, all open source][7-4].
* [MSYS2][7-5] - Minimal SYStem 2; aims to provide support for a POSIX
  environment on Windows, with a package manager based on Arch Linux's
  pacman. Packages have individual licenses, otherwise, as MinGW and Cygwin.
* [reactos/reactos](https://github.com/reactos/reactos) - A free Windows-compatible Operating System

[7-1]: https://cygwin.com/
[7-2]: https://cygwin.com/licensing.html
[7-3]: http://mingw-w64.yaxm.org/doku.php/start
[7-4]: http://mingw.org/license
[7-5]: http://msys2.github.io/

#### Profiling ####
* [gperftools][8-1] - Collection of utilities for measuring and improving
  performance. [``BSD-3-Clause``][BSD-3-Clause]
* [gprof][8-2] - Performance analysis tool. Part of GNU binutils. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [OProfile][8-3] - Statistical profiler for Linux. Can profile any code
  (including the kernel!) with low overhead and without recompilation. [``GPL-2.0-only``][GPL-2.0-only]
* [perf][8-4] - Linux kernel-based profiler with a lot of functionality. [``GPL-2.0-only``][GPL-2.0-only]

[8-1]: https://github.com/gperftools/gperftools
[8-2]: https://www.gnu.org/software/binutils/
[8-3]: http://oprofile.sourceforge.net/news/
[8-4]: https://perf.wiki.kernel.org/index.php/Main_Page

#### Text Editor Extensions ####
* [CCompletion][9-1] - Notepad++ autocompletion plugin. Works with all
  identifiers recognized by Ctags. This is a download link. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [CEDET][9-2] - Collection of Emacs Development Environment Tools; designed to
  provide IDE-like features to Emacs. Built-in. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Flycheck][9-3] - Modern syntax checking for Emacs. For C, it can use either
  GCC or Clang as a back-end. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [linter-clang][9-4] - Lint C code in Atom, using Clang. [``MIT``][MIT]
* [linter-gcc][9-5] - Lint C code in Atom, using GCC. [``MIT``][MIT]
* [Neomake][9-6] - Async :make and linting framework for Neovim/Vim. [``MIT``][MIT]
* [Syntastic][9-7] - Syntax checking and linting for Vim. [``WTFPL``][WTFPL]
* [YASnippet][9-8] - Emacs code template system, with C templates for common
  snippets. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [YouCompleteMe][9-9] - Code completion engine for Vim. [``GPL-3.0-only``][GPL-3.0-only]

[9-1]: http://freeweb.siol.net/rmihor/NppCCompletionPlugin.zip
[9-2]: http://cedet.sourceforge.net/
[9-3]: https://github.com/flycheck/flycheck
[9-4]: https://github.com/AtomLinter/linter-clang
[9-5]: https://github.com/hebaishi/linter-gcc
[9-6]: https://github.com/neomake/neomake
[9-7]: https://github.com/vim-syntastic/syntastic
[9-8]: http://joaotavora.github.io/yasnippet/
[9-9]: http://valloric.github.io/YouCompleteMe/

#### Utilities ####
* [Artistic Style][10-4] - Fast and small automatic source code formatter that
  supports C. [``LGPL-3.0-only``][LGPL-3.0-only]
* [biicode][10-5] - Dependency manager. [``MIT``][MIT]
* [c][10-6] - Compile and execute C "scripts" in one go on the command line. Also
  has shebang support. [``MIT``][MIT]
* [c99sh][10-7] - Run C files using hash-bang. [``BSD-2-Clause``][BSD-2-Clause]
* [ccache][10-1] - Compiler cache designed to speed up recompilation. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [cdecl][10-8] - Online service to translate C declarations into English and
  vice versa. Public domain.
* [cinclude2dot][10-9] - Graphs include dependencies in a project using Graphviz. [GPL-1.0-or-later][335] or [``GPL-2.0-or-later``][GPL-2.0-or-later] or [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [distcc][10-2] - Program that allows builds to be distributed among several
  machines. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [Firm][10-3] - Library that provides a graph-based intermediate representation,
  optimizations and assembly code generation suitable for use in compilers.
  Comes with an example C front-end under the same license. [``LGPL-2.1-only``][LGPL-2.1-only]
* [GNU Global][10-10] - Source code tagging tool. [``GPL-3.0-only``][GPL-3.0-only]
* [GPP][10-11] - General-purpose preprocessor. More versatile than the C
  preprocessor, but more flexible than m4. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [Highlight][10-12] - Converts source code to formatted text with highlighting. [``GPL-3.0-only``][GPL-3.0-only]
* [include-what-you-use][10-13] - Helps find unecessary inclusions and make
  suggestions for fixing them. Based on LLVM/Clang (and only works with it). [``NCSA``][NCSA]
* [indent][10-14] - Formats C source code automatically to make it easier to
  read. Also converts from one style of source to another. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [SMACK][10-15] - Modular software verification toolchain and a self-contained
  software verifier. Currently only works with programs compiled using Clang. [``MIT``][MIT]
* [unifdef][10-16] - Removes #ifdef and #if directives with their delimited text
  without touching any other part of the file. [``BSD-3-Clause``][BSD-3-Clause] or [``BSD-2-Clause``][BSD-2-Clause]
* [mcpp](http://mcpp.sourceforge.net/) - Portable C preprocessor. [`2-clause BSD`](https://opensource.org/licenses/BSD-2-Clause)
* [Capstone](https://github.com/aquynh/capstone) - Dissasembly/disassembler framework. [`BSD 3-clause`](https://github.com/aquynh/capstone/blob/master/LICENSE.TXT)

[10-1]: https://ccache.samba.org/
[10-2]: https://github.com/distcc/distcc
[10-3]: https://pp.ipd.kit.edu/firm/
[10-4]: http://astyle.sourceforge.net/
[10-5]: https://biicode.github.io/biicode/
[10-6]: https://github.com/ryanmjacobs/c
[10-7]: https://github.com/RhysU/c99sh
[10-8]: https://cdecl.org/
[10-9]: https://www.flourish.org/cinclude2dot/
[10-10]: https://www.gnu.org/software/global/
[10-11]: https://logological.org/gpp
[10-12]: http://www.andre-simon.de/doku/highlight/en/highlight.php
[10-13]: https://github.com/include-what-you-use/include-what-you-use
[10-14]: https://www.gnu.org/software/indent/
[10-15]: https://github.com/smackers/smack
[10-16]: http://dotat.at/prog/unifdef/

### Reading Material ###
#### Books ####
##### Reference Books #####
* [C in a Nushell 2E][11-1] - Concise reference book for C11.
* [C Pocket Reference][11-2] - Concise reference book for C99.
* [C: A Reference Manual 5E][11-3] - Full reference book for C99.
* [SEI CERT C Coding Standard][11-4] - Coding  recommendations from CERT.
* [The C Programming Language 2E][11-5] - Original book on C, by its creators.

[11-1]: http://shop.oreilly.com/product/0636920033844.do
[11-2]: http://shop.oreilly.com/product/9780596004361.do
[11-3]: http://careferencemanual.com/
[11-4]: https://wiki.sei.cmu.edu/confluence/display/c/SEI+CERT+C+Coding+Standard
[11-5]: https://en.wikipedia.org/wiki/The_C_Programming_Language

##### Beginner Books #####
* [C Primer Plus 6E][12-1] - Complete tutorial on programming in C11.
* [C Programming: A Modern Approach][12-2] - Book to learn the basics of C.
* [Head First C][12-3] - 'Head-first' style book for learning C.
* [The GNU C Programming Tutorial][12-4] - Beware, GNU C is not standart C.

[12-1]: https://www.pearson.com/us/higher-education/program/Prata-C-Primer-Plus-6th-Edition/PGM4399.html
[12-2]: http://knking.com/books/c2/index.html
[12-3]: http://shop.oreilly.com/product/0636920015482.do
[12-4]: http://www.crasseux.com/books/ctut.pdf

##### Intermediate Books #####
* [21st Century C][13-1] - Programming book on C that touches tooling subject.
* [Understanding and Using C Pointers][13-2] - In-depth book on pointers in C.

[13-1]: http://shop.oreilly.com/product/0636920033677.do
[13-2]: http://shop.oreilly.com/product/0636920028000.do

##### Advanced Books #####
* [Expert C Programming: Deep C Secrets][14-1] - Interesting, in-depth and
  entertaining look at the innards of C.
* [C Programming Wikibook][14-2] - Actually touches topics for all levels.

[14-1]: https://dl.acm.org/citation.cfm?id=179241
[14-2]: https://en.wikibooks.org/wiki/C_Programming

#### Articles and Other Resources ####
##### Reference #####
* [C FAQ - comp.lang.c Frequently Asked Questions](http://c-faq.com/)

##### Benchmarks #####
* [Benchmarks of the Lockless Memory Allocator][451]
* [Comparison of C/POSIX standard library implementations for Linux][453]
* [Finding the best 64-bit simulation PRNG][454]

##### Beginner Level #####
* [A tutorial on pointers][455]
* [A tutorial on portable Makefiles][456]
* [Building C Projects][457]
* [Introduction to \`fun' C][459]
* [Learning C with GDB][460]
* [POSIX Threads Programming tutorial][462]
* [Templating in C][464]
* [Tutorial on pointers](http://home.netcom.com/~tjensen/ptr/pointers.htm)
* [Building C Projects](http://nethack4.org/blog/building-c.html)
* [C Programming Wikibook](https://en.wikibooks.org/wiki/C_Programming)
* [Introduction to 'fun' C](https://gist.github.com/eatonphil/21b3d6569f24ad164365)
* [Learning C with GDB](https://www.recurse.com/blog/5-learning-c-with-gdb)
* [POSIX Threads Programming tutorial](https://computing.llnl.gov/tutorials/pthreads/) (a little dated, but most of it is still valid and useful)
* [The GNU C Programming Tutorial](http://www.crasseux.com/books/ctut.pdf) (online PDF)
* [Templating in C](http://blog.pkh.me/p/20-templating-in-c.html)
* [Akagi201/learning-cmake](https://github.com/Akagi201/learning-cmake) - learning cmake

##### Intermediate Level #####
* [memcpy vs memmove][461]
* [8 gdb tricks you should know][465]
* [10 C99 tricks][466]
* [A comprehensive MPI tutorial resource][467]
* [Diving into concurrency: trying out mutexes and atomics][468]
* [Generic C reference counting][469]
* [How to write portable C without complicating your build][470]
* [Introduction to OpenMP][471] (video)
* [OpenMP tutorial][472]
* [MPI tutorial][473]
* [Scalable C - Writing Large-Scale Distributed C][474]
* [Some unknown features or tricks in C language][475]
* [What every C programmer should know about undefined behaviour][476]
* [8 gdb tricks you should know](https://blogs.oracle.com/linux/8-gdb-tricks-you-should-know-v2)
* [10 C99 tricks](https://blog.noctua-software.com/c-tricks.html)
* [Diving into concurrency: trying out mutexes and atomics](https://jvns.ca/blog/2014/12/14/fun-with-threads/)
* [Introduction to OpenMP](https://www.youtube.com/playlist?list=PLLX-Q6B8xqZ8n8bwjGdzBJ25X2utwnoEG) (video)
* [OpenMP tutorial](https://computing.llnl.gov/tutorials/openMP/) (for the OpenMP3 standard)
* [memcpy vs memmove](https://web.archive.org/web/20170620131430/https://www.tedunangst.com/flak/post/memcpy-vs-memmove)
* [MPI tutorial](https://computing.llnl.gov/tutorials/mpi/)
* [Some unknown features or tricks in C language](https://proprogramming.org/some-unknown-features-or-tricks-in-c-language/)
* [The lost art of C structure packing](http://www.catb.org/esr/structure-packing/)
* [What a C programmer should know about memory](http://marek.vavrusa.com/memory/)
* [What every C programmer should know about undefined behaviour](http://blog.llvm.org/2011/05/what-every-c-programmer-should-know.html)

##### Advanced Level #####
* [Advanced metaprogramming in C][477]
* [A quick tutorial on implementing and debugging malloc, free, calloc, and realloc][478]
* [Bit twiddling hacks][479]
* [Implementing smart pointers for the C programming language][480]
* [Inline functions in C][481]
* [Metaprogramming custom control structures in C][482]
* [Some dark corners of C][483]
* [Writing efficient C and C code optimization][484]
* [Advanced metaprogramming in C](http://250bpm.com/blog:56)
* [Quick tutorial on implementing and debugging malloc, free, calloc, and realloc](http://danluu.com/malloc-tutorial/)
* [Bit twiddling hacks](https://graphics.stanford.edu/~seander/bithacks.html)
* [I do not know C](https://kukuruku.co/post/i-do-not-know-c/)
* [Implementing smart pointers for the C programming language](https://snai.pe/c/c-smart-pointers/)
* [Inline functions in C](http://www.greenend.org.uk/rjk/tech/inline.html)
* [Metaprogramming custom control structures in C](https://www.chiark.greenend.org.uk/~sgtatham/mp/)
* [Some dark corners of C](https://docs.google.com/presentation/d/1h49gY3TSiayLMXYmRMaAEMl05FaJ-Z6jDOWOz3EsqqQ/edit?pli=1#slide=id.gaf50702c_0153)
* [Writing efficient C and C code optimization](https://www.codeproject.com/articles/6154/writing-efficient-c-and-c-code-optimization)
* [What every programmer should know about memory](https://www.akkadia.org/drepper/cpumemory.pdf)

#### Code Examples ####
* [0intro/plan9](https://github.com/0intro/plan9) - Plan 9 from Bell Labs
* [CTurt/Cinoop](https://github.com/CTurt/Cinoop) - Multiplatform Game Boy emulator
* [ChibiOS/ChibiOS](https://github.com/ChibiOS/ChibiOS) - Read only mirror of SVN ChibiOS repository. Official forum http://forum.chibios.org  Bugtracker http://sourceforge.net/projects/chibios
* [EtchedPixels/FUZIX](https://github.com/EtchedPixels/FUZIX) - FuzixOS: Because Small Is Beautiful
* [Fedjmike/mini-c](https://github.com/Fedjmike/mini-c) - Dr Strangehack, or: how to write a self-hosting C compiler in 10 hours
* [FreddieV4/DailyProgrammerChallenges](https://github.com/FreddieV4/DailyProgrammerChallenges) - External Repo of Challenges from r/dailyprogrammer
* [Harvey-OS/harvey](https://github.com/Harvey-OS/harvey) - A distributed operating system
* [HarveyHunt/howm](https://github.com/HarveyHunt/howm) - A lightweight, X11 tiling window manager that behaves like vim
* [HuoLanguage/huo](https://github.com/HuoLanguage/huo) - interpreted language written in C
* [LIJI32/SameBoy](https://github.com/LIJI32/SameBoy) - Game Boy and Game Boy Color emulator written in C
* [LemonBoy/bar](https://github.com/LemonBoy/bar) - A featherweight, lemon-scented, bar based on xcb
* [MagerValp/AsmHeap](https://github.com/MagerValp/AsmHeap) - Heap data structure in 6502 assembler
* [MinhasKamal/CreepyCodeCollection](https://github.com/MinhasKamal/CreepyCodeCollection) - A Nonsense Collection of Disgusting Codes (quine-polyglot-code-golf-obfuscated-signature-creepy-codes-mandelbrot-esoteric-language-esoteric-programming-strange-golfing-spooky-weird)
* [MoarVM/MoarVM](https://github.com/MoarVM/MoarVM) - A VM with adaptive optimization and JIT compilation, built for Rakudo Perl 6
* [RIOT-OS/RIOT](https://github.com/RIOT-OS/RIOT) - RIOT -  The friendly OS for IoT
* [SilverRainZ/OS67](https://github.com/SilverRainZ/OS67) - An unix-like toy kernel.

#### Courses ####
* [AC-2015-Sem2/DSA-lab](https://github.com/AC-2015-Sem2/DSA-lab) - Data Structures and Algorithms lab repository
* [CoreData/cs50](https://github.com/CoreData/cs50) - CS50 Rep
* [McNopper/OpenGL](https://github.com/McNopper/OpenGL) - OpenGL 3 and 4 with GLSL
* [OpenGLInsights/OpenGLInsightsCode](https://github.com/OpenGLInsights/OpenGLInsightsCode) - Source code for OpenGL Insights
* [RPISEC/MBE](https://github.com/RPISEC/MBE) - Course materials for Modern Binary Exploitation by RPISEC

--------------------------------------------------------------------------------

## AI ##
Neural nets, machine learning, and other similar things.
* [Cranium][6] - Portable, header-only ANN library in C99. [``MIT``][MIT]
* [FANN][7] - Fast Artifical Neural Network library; an implementation of neural
  networks. [``GPL-2.0-only``][GPL-2.0-only]
* [Genann][8] - Simple ANN in C89, without additional dependencies. [``Zlib``][Zlib]
* [KANN][9] - Two-file ANN library. [``MIT``][MIT]
* [LibDEEP][10] - Deep learning library. [``BSD-3-Clause``][BSD-3-Clause]
* [Darknet](https://pjreddie.com/darknet/) - Open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.
* [100/Cranium](https://github.com/100/Cranium) - 🤖   A portable, header-only, artificial neural network library written in C99
* [2hanson/DecisionTree](https://github.com/2hanson/DecisionTree) - Decision Tree
* [Blei-Lab/lda-c](https://github.com/Blei-Lab/lda-c) - This is a C implementation of variational EM for latent Dirichlet allocation (LDA), a topic model for text or other discrete data.
* [GHamrouni/Recommender](https://github.com/GHamrouni/Recommender) - A C library for product recommendations/suggestions using collaborative filtering (CF)
* [H2CO3/libsprec](https://github.com/H2CO3/libsprec) - C library for speech recognition using the Google Speech API
* [HIPS/Probabilistic-Backpropagation](https://github.com/HIPS/Probabilistic-Backpropagation) - Implementation in C and Theano of the method Probabilistic Backpropagation for scalable Bayesian inference in deep neural networks.
* [JulienPalard/Mine](https://github.com/JulienPalard/Mine) - Little data miner

## Algoritm Implementations ##
* [sort][434] - Collection of sorting routines, which type-specialize at
  compile-time with a user-defined type. [``MIT``][MIT]
* [dlx][418] - Implementation of [Knuth's Algorithm X][419], with example
  solvers. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [BigZaphod/AStar](https://github.com/BigZaphod/AStar) - C Implementation of the A* Pathfinding Algorithm
* [uastar][195] - Minimal A\* implementation. [``ZLib``][Zlib]
* [BlackLight/fkmeans](https://github.com/BlackLight/fkmeans) - A tiny library in C for managing kmeans clusterization algorithm over arbitrary data sets, both by manually specifying the number k of clusters and computing it automatically using Schwarz criterion
* [CVLearner/Mixture-of-Gaussians](https://github.com/CVLearner/Mixture-of-Gaussians) - Fit a Gaussian mixture model given a set of data
* [Cyan4973/FiniteStateEntropy](https://github.com/Cyan4973/FiniteStateEntropy) - New generation entropy codecs : Finite State Entropy and Huff0
* [IAIK/CJAG](https://github.com/IAIK/CJAG) - CJAG is an open-source implementation of our cache-based jamming agreement.
* [Kevincav/Radix-Sort](https://github.com/Kevincav/Radix-Sort) - Radix Sort with different data types.
* [Soryusan/Ranking_Algorithm](https://github.com/Soryusan/Ranking_Algorithm) - Ranking algorithm data collector/cruncher

## Argument Parsing ##
* [parg][410] - A single-file reimplementation of ``getopt`` with better
  defaults. [``CC0-1.0``][CC0-1.0]
* [argparse][411] - Command-line argument parsing library, inspired by Python's
  argparse module. [``MIT``][MIT]
* [docopt.c][412] - Implementation of a command-line option parser. [``MIT``][MIT]
* [PaulStoffregen/teensy_loader_cli](https://github.com/PaulStoffregen/teensy_loader_cli) - Command line Teensy Loader

## Calculations ##
* [apophenia][250] - Library for statistical and scientific computing. [``GPL-2.0-only``][GPL-2.0-only]
* [Arb][251] - Library for arbitrary-precision interval arithmetic. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [ATLAS][252] - Automatically Tuned Linear Algebra Software. [``BSD-3-Clause``][BSD-3-Clause]
* [clBLAS][253] - BLAS functions written in OpenCL. [``Apache-2.0``][Apache-2.0]
* [cmathl][254] - Math library with a great variety of mathematical functions
  with CMake build support. Seeks to be close to C89/C90 compliant for
  portability. [``MIT``][MIT]
* [Cuba][255] - Library for multidimensional numerical integration. [``LGPL-3.0-only``][LGPL-3.0-only]
* [fft-c][256] - A high-performance Fourier Transform from netlib's fftpack;
  wrapped in a user-friendly format [``MIT``][ MIT]
* [FFTW][257] - The Fastest Fourier Transform in the West; a highly optimized
  fast Fourier transform routine. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [FLINT][258] - Fast Library for Number Theory; a library supporting arithmetic
  with numbers, polynomials, power series and matrices, among others. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [GLPK][259] - GNU Linear Programming Kit; a package designed for solving
  large-scale linear programming, mixed integer programming and other related
  problems. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GMP][260] - GNU Multple Precision Arithmetic Library; a library for
  arbitrary-precision arithmetic. [``GPL-2.0-only``][GPL-2.0-only] or [``LGPL-3.0-only``][LGPL-3.0-only]
* [GNU MPC][261] - Library for complex number arithmetic. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [GNU MPFR][262] - Library for arbitrary-precision floating-point arithmetic. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [GNU MPRIA][263] - Portable mathematics library for multi-precision rational
  interval arithmetic. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GSL][264] - The GNU Scientific Library; a sophisticated numerical library. [``GPL-3.0-only``][GPL-3.0-only].
* [KISS FFT][265] - Simple fast Fourier transform library. [``BSD-3-Clause``][BSD-3-Clause]
* [LAPACKE][266] - Interface to [LAPACK][134]. [``BSD-3-Clause``][BSD-3-Clause]
* [LibTomMath][267] - Portable, number-theoretic, multiple-precision integer
  library. Supports algebra, digit manipulation, modular reductions, and various
  number-theoretic routines. Public domain.
* [LibTomPoly][268] - Polynomial-related maths library. Public domain.
* [PARI/GP][269] - Computer algebra system for number theory; includes a
  compiler to C. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [PETSc][270] - Suite of data structures and routines for scalable parallel
  solution of scientific applications modelled by partial differential
  equations. [``BSD-2-Clause``][BSD-2-Clause]
* [SCS][271] - Splitting Conic Solver; a numerical optimization package for
  solving large-scale convex cone problems. [``MIT``][MIT]
* [SLEPc][272] - Library for the solution of large, sparse eigenvalue
  problems on parallel computers. [``LGPL-3.0-only``][LGPL-3.0-only]
* [TomsFastMath][273] - Set of optimized maths operations (in assembly),
  suitable for cryptographic use. Public domain.
* [Yeppp!][274] - Fast, SIMD-optimized mathematical library. [``BSD-3-Clause``][BSD-3-Clause]
* [tinyexpr][379] - Tiny recursive-descent parser, compiler and evaluation
  engine for simple mathematical expressions. [``BSD-3-Clause``][BSD-3-Clause]
* [apophenia](http://apophenia.info/) - Library for statistical and scientific computing. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [ATLAS](http://math-atlas.sourceforge.net/) - Automatically Tuned Linear Algebra Software. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [BLAS](http://www.netlib.org/blas/) - Basic Linear Algebra Subprograms; a set of routines that provide vector and matrix operations. [`BLAS license`](http://www.netlib.org/blas/#_licensing)
* [CDFLIB](https://people.sc.fsu.edu/~jburkardt/c_src/cdflib/cdflib.html) - Library with routines to evaluate cumulative density functions fo a variety of standard probability distributions.  Also can compute one parameter of the CDF given the others.  (No license given)
* [cmathl](https://scientificc.github.io/cmathl/) - Pure-C Math library with a great variety of mathematical functions and CMake build support. Seeks to be close to C89/C90 compliant for portability. [`MIT`](https://github.com/ScientificC/cmathl/blob/master/LICENSE)
* [Cuba](http://www.feynarts.de/cuba/) - Library for multidimensional numerical integration. [`GNU LGPLv3`](http://www.gnu.org/licenses/lgpl.html)
* [FFTW](http://www.fftw.org/) - The Fastest Fourier Transform in the West; a highly-optimized fast Fourier transform routine. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [FLINT](http://flintlib.org/) - Fast Library for Number Theory; a library supporting arithmetic with numbers, polynomials, power series and matrices, among others. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [GLPK](https://www.gnu.org/software/glpk/) - GNU Linear Programming Kit; a package designed for solving large-scale linear programming, mixed integer programming and other related problems. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [GMP](https://gmplib.org/) - GNU Multple Precision Arithmetic Library; a library for arbitrary-precision arithmetic. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html) and [`GNU LGPLv3`](http://www.gnu.org/licenses/lgpl.html)
* [GNU MPC](http://www.multiprecision.org/mpc/) - Library for complex number arithmetic. [`GNU LGPL3 or later`](http://www.gnu.org/licenses/lgpl.html)
* [GNU MPFR](https://www.mpfr.org/index.html) - Library for arbitrary-precision floating-point arithmetic. [`GNU LGPL3 or later`](http://www.gnu.org/licenses/lgpl.html) or [`GNU LGPL2.1 or later (until version 2.4.x)`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [GNU MPRIA](https://www.gnu.org/software/mpria/) - Portable mathematics library for multi-precision rational interval arithmetic. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [GSL](http://www.gnu.org/software/gsl/) - The GNU Scientific Library; a sophisticated numerical library. [`GNU GPL3`](http://www.gnu.org/licenses/gpl.html)
* [igraph](https://igraph.org/) - Library for creating and manipulating large graphs. [`GNU GPL2`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [KISS FFT](https://sourceforge.net/projects/kissfft/) - Very simple fast Fourier transform library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [LAPACKE](http://www.netlib.org/lapack/lapacke.html) - C interface to [LAPACK](http://www.netlib.org/lapack/). [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [PARI/GP](http://pari.math.u-bordeaux.fr/) - Computer algebra system for number theory; includes a compiler to C. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [PETSc](https://www.mcs.anl.gov/petsc/) - Suite of data structures and routines for scalable parallel solution of scientific applications modelled by partial differential equations. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [PROB](https://people.sc.fsu.edu/~jburkardt/c_src/prob/prob.html) - Library that handles various discrete and continuous probability density functions.  [`GNU LGPL3`](https://people.sc.fsu.edu/~jburkardt/txt/gnu_lgpl.txt)
* [Yeppp!](https://bitbucket.org/MDukhan/yeppp) - Very fast, SIMD-optimized mathematical library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [gjrand](https://sourceforge.net/projects/gjrand/) - Library of random-number generation routines. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html) or [`GNU GPLv3`](http://www.gnu.org/licenses/gpl.html)
* [FFTW/fftw3](https://github.com/FFTW/fftw3) - This is the official repository for the FFTW Fourier transform library, version 3.x
* [HdrHistogram/HdrHistogram_c](https://github.com/HdrHistogram/HdrHistogram_c) - C port of the HdrHistogram
* [JuliaMath/openlibm](https://github.com/JuliaMath/openlibm) - High quality system independent, portable, open source libm implementation
* [KhronosGroup/OpenCL-Headers](https://github.com/KhronosGroup/OpenCL-Headers) - Khronos OpenCL-Headers
* [Lichtso/CCWT](https://github.com/Lichtso/CCWT) - Complex Continuous Wavelet Transformation
* [NCrashed/bzip2](https://github.com/NCrashed/bzip2) - Bindings for bzip2 library, a freely available, patent free, high-quality data compressor.
* [PetteriAimonen/libfixmatrix](https://github.com/PetteriAimonen/libfixmatrix) - C library for fixed point matrix, quaternion and vector calculations

## Compression ##
* [blosc][25] - Fast, multi-threaded, meta-compressor library. Various licenses,
  all open source.
* [Brotli][26] - General-purpose lossless compression algorithm library. Has
  speeds comparable to DEFLATE, but much higher compression ratios. [``MIT``][MIT].
* [clzip][27] - C [lzip][28] implementation. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [CRoaring][29] - C implementation of [Roaring bitmaps][30]. [``Apache-2.0``][Apache-2.0]
* [FiniteStateEntropy][31] - Two efficient compression codecs optimized for
  modern CPUs. [``BSD-2-Clause``][BSD-2-Clause]
* [DENSITY][32] - Fast compression library. [``BSD-3-Clause``][BSD-3-Clause]
* [heatshrink][33] - Data compression/decompression library for embedded and
  real-time systems. [``ISC``][ISC]
* [fast\_zlib][34] - Improved zlib, which runs 2 to 10 times faster. [``BSD-3-Clause``][BSD-3-Clause]
* [huffandpuff][35] - Minimal Huffman encoder and decoder. Public domain.
* [libbzip2][36] - Patent-free, high-quality data compression library. [``BSD-4-Clause``][BSD-4-Clause]
* [Lizard][37] - Formerly LZ5. Achieves compression ratios comparable with zip
  and zlib at decompression speeds of 1000MB/s and faster. [``BSD-2-Clause``][BSD-2-Clause]
* [lz4][38] - Fast compression algorithm. [``BSD-2-Clause``][BSD-2-Clause]
* [lzo][39] - Fast data compression library. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [pixz][40] - Parallel, indexed xz compressor. [``BSD-2-Clause``][BSD-2-Clause]
* [shoco][41] - Compressor for small text strings. [``MIT``][MIT]
* [SIMDComp][42] - Simple library for compressing lists of integers using
  binary packing. Makes use of SIMD instructions on x86. [``BSD-3-Clause``][BSD-3-Clause]
* [smaz][43] - Efficient string compression library. [``BSD-3-Clause``][BSD-3-Clause]
* [squash][44] - Compression abstraction library, complete with some utilities. [``MIT``][MIT]
* [TurboPFor][45] - Fast integer compression. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [TurboRLE][46] - Efficient run-length encoding. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [zip][47] - Small zip archive processing library. [``Unlicense``][Unlicense]
* [Zlib][48] - Popular compression library. [``BSD-3-Clause``][BSD-3-Clause]
* [libarchive][49] - libarchive is a portable, efficient C library that can read
  and write streaming archives in a variety of formats. [``BSD-3-Clause``][BSD-3-Clause]
* [zlib-ng][50] - Zlib replacement with optimizations for modern CPUs systems. [``BSD-3-Clause``][BSD-3-Clause]
* [Zstandard][51] - Fast, lossless compression algorithm, targeting real-time
  compression scenarios at zlib-level or better compression ratios. [``BSD-3-Clause``][BSD-3-Clause]
* [libzip](https://libzip.org/) - A C library for reading, creating, and modifying zip archives. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [lzo](http://www.oberhumer.com/opensource/lzo/) - Very fast data compression library. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [zlib](http://zlib.net/) - Massively-spiffy yet delicately-unobtrusive compression library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [bzip2](http://www.bzip.org/) - Patent free, high quality data compressor. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [lz4](https://lz4.github.io/lz4/) - Fast Compression algorithm.
* [snappy](https://github.com/google/snappy) - Fast compression library (implementation in C++, native bindings to C).
* [zstd](http://facebook.github.io/zstd/) - Fast real-time compression algorithm [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [brotli](https://github.com/google/brotli) - Generic lossless compression algorithm based on LZ77, Huffman coding and 2nd order context modelling [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [quicklz](http://www.quicklz.com/index.php) - Fast compression library. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [pixz](https://github.com/vasi/pixz) - Pixz (pronounced pixie) is a parallel, indexing version of `xz`. [`2-clause BSD`](https://directory.fsf.org/wiki/License:BSD-2-Clause)
* [Blosc/c-blosc](https://github.com/Blosc/c-blosc) - A blocking, shuffling and loss-less compression library that can be faster than `memcpy()`.
* [Cyan4973/lz4](https://github.com/Cyan4973/lz4) - Extremely Fast Compression algorithm
* [Cyan4973/zstd](https://github.com/Cyan4973/zstd) - Zstandard - Fast and efficient compression algorithm
* [Dead2/zlib-ng](https://github.com/Dead2/zlib-ng) - zlib replacement with optimizations for "next generation" systems.
* [IlyaGrebnov/libbsc](https://github.com/IlyaGrebnov/libbsc) - High performance block-sorting data compression library
* [RoaringBitmap/CRoaring](https://github.com/RoaringBitmap/CRoaring) - Roaring bitmaps in C (and C++)

## Concurrency and Parallelism ##
* [cchan][52] - Small library for channel constructs for inter-thread
  communication. Public domain.
* [checkedthreads][53] - A simple library for parallelism, with built-in
  checking for race conditions. [``BSD-2-Clause``][BSD-2-Clause]
* [ck][54] - Concurrency primitives, safe memory reclamation mechanisms and
  non-blocking data structures. [``BSD-2-Clause``][BSD-2-Clause]
* [FCFS RWLock][55] - First-come first-served Readers/Writers lock for POSIX
  threads. Various licenses, all open source.
* [libconcurrent][56] - Concurrent programming library, using coroutines, for
  C11. [``Zlib``][Zlib]
* [libdill][57] - Library which makes structured concurrent programming easy. [``MIT``][MIT]
* [liburcu][59] - Data synchronization library, which scales linearly with the
  number of cores. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [mill][60] - Go-style concurrency. [``MIT``][MIT]
* [oclkit][61] - Two-file OpenCL wrapper. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [OCL-MLA][62] - OpenCL Mid-Level Abstractions. [``BSD-3-Clause``][BSD-3-Clause]
* [OpenMP][63] - Set of pragmas designed to allow for easy parallelization of
  code. Standard (licensing not applicable).
* [OpenMPI][64] - Message passing interface implementation. [``BSD-3-Clause``][BSD-3-Clause]
* [pth][66] - Portable implementation for non-preemptive priority-based
  scheduling for multiple threads of execution. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [pthreads][67] - POSIX thread library. Standard (no license applicable).
* [TinyCThread][68] - Portable, small implementation of the C11 threads API. [``Zlib``][Zlib]
* [cchan](http://repo.hu/projects/cchan/) - Small library for channel constructs for inter-thread communication. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [ck](http://concurrencykit.org/) - Concurrency primitives, safe memory reclamation mechanisms and non-blocking data structures. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [mill](http://libmill.org/) - Go-style concurrency in C. [`X11`](https://directory.fsf.org/wiki/License:X11)
* [libdill](http://libdill.org/) - Structured concurrency in C. [`X11`](https://directory.fsf.org/wiki/License:X11)
* [MPICH](http://www.mpich.org/) - Another implementation of MPI. [`MPICH licence`](http://git.mpich.org/mpich.git/blob_plain/6aab201f58d71fc97f2c044d250389ba86ac1e3c:/COPYRIGHT)
* [OpenMP](https://www.openmp.org/) - Set of C pragmas designed to allow for easy parallelization of code. [`3-clause BSD`](https://opensource.org/licenses/BSD-3-Clause)
* [OpenMPI](https://github.com/open-mpi/ompi) - Message passing interface implementation. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [pth](https://www.gnu.org/software/pth/) - Portable implementation for non-preemptive priority-based scheduling for multiple threads of execution. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [pthreads](https://en.wikipedia.org/wiki/POSIX_Threads) - The POSIX thread library.
* [SLEPc](https://bitbucket.org/slepc/slepc) - Software library for the solution of large, sparse eigenvalue problems on parallel computers. [`GNU LGPL3`](http://www.gnu.org/licenses/lgpl.html)
* [TinyCThread](https://tinycthread.github.io/) - Portable, small implementation of the C11 threads API. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [cf4ocl](https://fakenmc.github.io/cf4ocl/) - The C Framework for OpenCL; a cross-platform object-oriented framework for developing and benchmarking  [OpenCL](https://www.khronos.org/opencl/) projects. [`GNU LGPL3 (library)`](http://www.gnu.org/licenses/lgpl.html) or [`GNU GPL3 (project code)`](http://www.gnu.org/licenses/gpl.html)
* [Pithikos/C-Thread-Pool](https://github.com/Pithikos/C-Thread-Pool) - A minimal but powerful thread pool in ANSI C

## Crypto ##
Mostly library implementations of well-known cryptographic algorithms or
protocols.
* [GNU SASL][69] - Implementation of the Simple Authentication and Security
  Layer and few common SASL mechanisms. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GnuTLS][70] - Secure communication library, implementing SSL, TLS and DTLS. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libgcrypt][71] - General-purpose cryptography library, with a range of
  available ciphers. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [OpenSSL][72] - Implementation of the SSL and TLS protocols. Also includes a
  cryptography library. [Dual Licensed under the OpenSSL License and the SSLeay License][73].
* [liboqs][74] - Library for quantum-resistant cryptographicl algorithms. [``MIT``][MIT]
* [libsodium][75] - Modern and easy-to-use crypto library. [``MIT``][MIT]
* [libtomcrypt][76] - Fairly comprehensive, modular and portable cryptographic
  toolkit. Public domain.
* [mbed TLS][77] - Another crypto implementation. [``Apache-2.0``][Apache-2.0]
* [MIRACL][78] - Multiprecision Integer and Rational Arithmetic Cryptographic
  Library; an SDK for elliptic curve cryptography. [``AGPL-3.0-or-later``][AGPL-3.0-or-later]
* [retter][79] - Collection of hash functions, ciphers, tools, libraries and
  materials related to cryptography and security. Public domain.
* [s2n][80] - C99 implementation of the TLS/SSL protocols, designed to be
  simple, fast and with security as a priority. [``Apache-2.0``][Apache-2.0]
* [sphlib][81] - Set of implementations of various hash functions, including
  several cryptographic ones. [``MIT``][MIT]
* [trezor-crypto][82] - Heavily optimized crypto algorithms for embedded
  devices. [``MIT``][MIT]
* [GnuTLS](https://www.gnutls.org/) - Secure communication library, implementing SSL, TLS and DTLS. [`GNU LGPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [libgcrypt](https://gnupg.org/related_software/libgcrypt/) - General-purpose cryptography library, with a range of available ciphers. [`GNU LGPL2.1or later (code)`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) and [`GNU GPL2.1 or later (manual and tools)`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [OpenSSL](https://www.openssl.org/) - Implementation of the SSL and TLS protocols, and also includes a cryptography library. [`Dual Licensed under the OpenSSL License and the SSLeay License`](https://www.openssl.org/source/license.html)
* [libsodium](https://download.libsodium.org/doc/) - Modern and easy-to-use crypto library. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [libtomcrypt](https://www.libtom.net/) - Fairly comprehensive, modular and portable cryptographic toolkit. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [mbed TLS](https://tls.mbed.org/) - Another crypto implementation for C. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [libressl](https://www.libressl.org/) - Modernized fork of OpenSSL. [`Various Licenses`](https://cvsweb.openbsd.org/cgi-bin/cvsweb/~checkout~/src/lib/libssl/LICENSE?rev=1.12)
* [jedisct1/libsodium](https://github.com/jedisct1/libsodium) - A modern, portable, easy to use crypto library
* [ARMmbed/mbedtls](https://github.com/ARMmbed/mbedtls) - An open source, portable, easy to use, readable and flexible SSL library
* [B-Con/crypto-algorithms](https://github.com/B-Con/crypto-algorithms) - Basic implementations of standard cryptography algorithms, like AES and SHA-1.
* [CertiVox/MIRACL](https://github.com/CertiVox/MIRACL) - MIRACL Cryptographic SDK: Multiprecision Integer and Rational Arithmetic Cryptographic Library is a C software library that is widely regarded by developers as the gold standard open source SDK for elliptic curve cryptography (ECC).

## Databases ##
* [BerkeleyDB][83] - Library for a high-performance embedded database for
  key-value data. [``AGPL-3.0-only``][AGPL-3.0-only]
* [Groonga][84] - Columnar store with full-text search. [``LGPL-2.1-only``][LGPL-2.1-only]
* [Hiredis][85] - Minimalistic client library for Redis. [``BSD-3-Clause``][BSD-3-Clause]
* [libmongoc][86] - High-performance client library for MongoDB. [``Apache-2.0``][Apache-2.0]
* [LMDB][87] - Ultra-fast, ultra-compact key-value embedded data store. [``OLDAP-2.8``][OLDAP-2.8]
* [PostgreSQL][88] - Powerful object-relational database system. [``PostgreSQL``][PostgreSQL]
* [Redis][89] - Advanced key-value store. [``BSD-3-Clause``][BSD-3-Clause]
* [sophia][90] - Modern, embeddable key-value database. [``BSD-2-Clause``][BSD-2-Clause]
* [sparkey][91] - Simple constant key/value storage library. Designed for
  read-heavy loads with infrequent, large bulk inserts. [``Apache-2.0``][Apache-2.0]
* [SQLite][92] - Self-contained, serverless, zero-configuration, transactional
  SQL database engine. Public domain.
* [UnQLite][93] - Self-contained, serverless, zero-configuration, transactional
  NoSQL engine. [``BSD-2-Clause``][BSD-2-Clause]
* [WhiteDB][94] - Lightweight database library, operating entirely in main
  memory. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [BerkeleyDB](https://www.oracle.com/database/berkeley-db/) - Library for a high-performance embedded database for key-value data. [`GNU AGPLv3`](https://www.gnu.org/licenses/agpl.html)
* [Hiredis](https://github.com/redis/hiredis) - Minimalistic client library for Redis. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [LMDB](https://github.com/LMDB/lmdb) - Ultra-fast, ultra-compact key-value embedded data store. [`OpenLDAP License`](https://directory.fsf.org/wiki/License:OLDAP-2.7)
* [MariaDB](https://mariadb.com/) - Robust, scalable and reliable SQL server, designed to be a drop-in replacement for MySQL. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [mongo-c-driver](http://mongoc.org/) - High-performance client library for [MongoDB](https://www.mongodb.com/). [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [PostgreSQL](https://www.postgresql.org/) - Powerful object-relational database system. [`PostgreSQL licence`](https://opensource.org/licenses/postgresql)
* [recutils](https://www.gnu.org/software/recutils/) - Set of tools and a C library for accessing human-editable, plaintext database files called recfiles. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [Redis](https://redis.io/) - Advanced key-value store. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [sophia](http://sophia.systems/) - Modern, embeddable key-value database. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [SQLite](https://www.sqlite.org/about.html) - Self-contained, serverless, zero-configuration, transactional SQL database engine with a C interface. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [UnQLite](https://unqlite.org/) - Self-contained, serverless, zero-configuration, transactional NoSQL engine with a C interface. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [Akash91/CoSQL](https://github.com/Akash91/CoSQL) - A Co-Relational Key-Value Data Store
* [Amaury/FineDB](https://github.com/Amaury/FineDB) - High-performance nosql database. Written in C, multi-threaded, based on LightningDB and nanomsg.
* [BohuTANG/nessDB](https://github.com/BohuTANG/nessDB) - A very fast transactional key-value, embedded database storage engine.
* [GNOME/libgda](https://github.com/GNOME/libgda) - Libgda is a (relatively small) database access library:
* [Qihoo360/Atlas](https://github.com/Qihoo360/Atlas) - A high-performance and stable proxy for MySQL
* [Softmotions/ejdb](https://github.com/Softmotions/ejdb) - EJDB — Embeddable JSON Database engine
* [Suor/postgresql-json](https://github.com/Suor/postgresql-json) - Extract data from PostgreSQL JSON fields.

## Data Structures ##
* [libhl][58] - Library implementing a thread-safe API to manage a range of data
  structures. Also provides some supporting functions and structures for
  concurrent and lockfree programming. [``LGPL-3.0-only``][LGPL-3.0-only]
* [Collections-C][95] - Library of generic data structures. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [kdtree][96] - Simple library for working with KD-trees. [``BSD-3-Clause``][BSD-3-Clause]
* [libavl][97] - Library containing a range of self-balancing binary trees. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [ds][98] - Common Data Structures and Algorithms. [``MIT``][MIT]
* [igraph][99] - A graph processing library. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [liblfds][100] - Portable lock-free data structure library. Public domain
  (more exactly, whatever license you want).
* [M\*LIB][101] - Library for generic, but typesafe C containers. Implemented as
  header-only. [``BSD-2-Clause``][BSD-2-Clause]
* [offbrand][102] - Collection of generic, reference-counted data structures. [``MIT``][MIT]
* [libsrt][103] - Soft and hard real-time data structures. [``BSD-3-Clause``][BSD-3-Clause].
* [list.h][104] - Implementations for single- and double-linked list functions. [``GPL-3.0-only``][GPL-3.0-only]
* [PackedArray][105] - Random-access array of tightly packed unsigned integers
of any desired width. Has a SIMD-optimized implementation. [``WTFPL``][WTFPL]
* [uthash][106] - Single-file hash table implementation. [``BSD-1-Clause``][BSD-1-Clause]
* [vector.h][107] - Header library for typed lists. [``MIT``][MIT]
* [20centaurifux/datatypes](https://github.com/20centaurifux/datatypes) - A collection of various datatypes in C (linked lists, stack, queue, red-black tree and hash table).
* [2ion/libqueue](https://github.com/2ion/libqueue) - C library providing persistent, named data storage queues
* [Achoulos/Data-Structures](https://github.com/Achoulos/Data-Structures) - Implementation of Data Structures and Sorts in C
* [Blosc/bcolz](https://github.com/Blosc/bcolz) - A columnar data container that can be compressed.
* [ClickerMonkey/CDSL](https://github.com/ClickerMonkey/CDSL) - A data structure library written in C
* [DanielWaterworth/Butterfly](https://github.com/DanielWaterworth/Butterfly) - [DEPRECATED] Butterfly is a C library that implements a very simple 'dynamic' data-type. It could be used, for example, to manipulate JSON data from C. It is distributed under LGPL.
* [Incarnation-p-lee/libds](https://github.com/Incarnation-p-lee/libds) - unified data structure implementation lib of C
* [Krakonos/cutils](https://github.com/Krakonos/cutils) - C utilities and data structures
* [LPD-EPFL/ASCYLIB](https://github.com/LPD-EPFL/ASCYLIB) - ASCYLIB is a concurrent-search data-structure library with over 30 implementantions of linked lists, hash tables, skip lists, and binary search trees.
* [MichaelJWelsh/cdsa](https://github.com/MichaelJWelsh/cdsa) - A library of generic intrusive data structures and algorithms in ANSI C
* [Tarsnap/kivaloo](https://github.com/Tarsnap/kivaloo) - Kivaloo is a collection of utilities which together form a data store associating keys of up to 255 bytes with values of up to 255 bytes.

## Events ##
* [libuv][397] - Cross-platform asynchronous I/O. [``MIT``][MIT]
* [libPhenom][398] - Eventing framework for building high-scalability and
  high-performance systems. [``Apache-2.0``][Apache-2.0]
* [libev][399] - Yet another event loop. [``BSD-2-Clause``][BSD-2-Clause]
* [libevent][400] - Event loop replacement for network servers. [``BSD-3-Clause``][BSD-3-Clause]
* [Lupus/libevfibers](https://github.com/Lupus/libevfibers) - Small C fiber library that uses libev based event loop and libcoro based coroutine context switching.

## FFI ##
Foreign function interfaces, also know as binding interfaces.
* [libffi][404] - Portable foreign-function interface library. [``MIT``][MIT]
* [GNU Libffcall][405] - Collection of libraries for building foreign function
  interfaces. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [dyncall][406] - Another foreign function interface library. [``MIT``][MIT]

## Flow Control and Language Extension ##
* [libCello][429] - Library introducing higher-level programming to C. [``BSD-3-Clause``][BSD-3-Clause]
* [Ragel][430] - DSL for state machines that compiles to C. [``GPL-2.0-only``][GPL-2.0-only]
* [Kitsune][431] - Efficient, general-purpose framework for dynamic software
  updating. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [yasm](http://yasm.tortall.net/) - Yasm Modular Assembler Project. [`2-clause BSD`](https://directory.fsf.org/wiki/License:BSD-2-Clause)
* [P99](http://p99.gforge.inria.fr/) - Suite of macros to implement advanced features like default function arguments, scope-bound resources, etc. (Requires C99) [`Q Public License`](https://tldrlegal.com/license/q-public-license-1.0-(qpl-1.0)#summary)
* [orangeduck/Cello](https://github.com/orangeduck/Cello) - Higher level programming in C
* [CObjectSystem/COS](https://github.com/CObjectSystem/COS) - C Object System
* [H2CO3/Sparkling](https://github.com/H2CO3/Sparkling) - Lightweight extension language
* [LuaDist/lua](https://github.com/LuaDist/lua) - The Lua programming language with CMake based build
* [LuaDist/luajit](https://github.com/LuaDist/luajit) - LuaJIT is JIT compiler for the Lua language.
* [LuaDist/toluapp](https://github.com/LuaDist/toluapp) - tolua++ is an extension of toLua, a tool to integrate C/Cpp code with Lua


## Game Development ##
Engines, libraries and other helpful things specifically for making games.
* [Allegro][170] - Cross-platform, game development and multimedia library. [``Zlib``][Zlib]
* [cglm][171] - Optimized OpenGL/Graphics Math (glm) for C. [``MIT``][MIT]
* [Chipmunk2D][172] - Fast and lightweight 2D game physics library. [``MIT``][MIT]
* [Corange][173] - Game engine in pure C. [``BSD-2-Clause``][BSD-2-Clause]
* [CSFML][174] - Binding for [SFML][175]. [``Zlib``][Zlib]
* [Darkplaces][176] - Modified version of the Quake2 engine. [``GPL-2.0-only``][GPL-2.0-only]
* [Epoxy][177] - Library for handling OpenGL function pointer management. [``MIT``][MIT]
* [Freecell Solver][178] - Set of libraries and command-line programs for
  automatically solving FreeCell and some similar variants of card Solitaire. [``MIT``][MIT]
* [ioquake3][181] - Quake3 engine, freed at last. [``GPL-2.0-only``][GPL-2.0-only]
* [kazmath][182] - Maths library for games. [``BSD-2-Clause``][BSD-2-Clause]
* [libao][183] - Cross-platform audio library with a wide variety of outputs. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [MATHC][184] - Math library for 2D and 3D programming. [``ZLib``][Zlib]
* [Orx][185] - Portable, lightweight, plugin-based, data-driven, 2D-oriented
  game engine. [``Zlib``][Zlib]
* [Quake][186] - Quake engine. [``GPL-2.0-only``][GPL-2.0-only]
* [Quake2][187] - Quake2 engine. [``GPL-2.0-only``][GPL-2.0-only]
* [raylib][188] - Simple library to learn video game programming. [``Zlib``][Zlib]
* [RetroArch][189] - Reference frontend for [libretro][190]. [``GPL-3.0-only``][GPL-3.0-only]
* [SDL2][191] - Cross-platform library designed to provide low-level access to
  audio, keyboard, mouse, joystick and graphics hardware via OpenGL. [``Zlib``][Zlib]
* [sdl-gpu][192] - Library for high-performance, modern 2D graphics. Based on
  SDL. [``MIT``][MIT]
* [SIGIL][193] - Sound, Input and Graphics Integration Library; a simple
  alternative to other libraries for doing all those things. Various licenses,
  all open source.
* [Spearmint][194] - Engine designed for FPS games. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Corange](https://github.com/orangeduck/Corange) - Game engine in pure C. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [Darkplaces](https://icculus.org/twilight/darkplaces/) - Modified version of the Quake2 engine. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [ioquake3](https://ioquake3.org/) - The Quake3 engine, freed at last. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [Orx](http://orx-project.org/) - Portable, lightweight, plugin-based, data-driven, 2D-oriented game engine. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [Quake](https://github.com/id-Software/Quake) - The Quake engine. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [Quake2](https://github.com/id-Software/Quake-2) - The Quake2 engine. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [Spearmint](https://clover.moe/spearmint/) - Engine designed for FPS games. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [Allegro](https://liballeg.org/) - Cross-platform, video game development and multimedia library. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [Chipmunk2D](http://chipmunk-physics.net/) - Fast and lightweight 2D game physics library. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [CSFML](https://www.sfml-dev.org/download/csfml/) - Binding for [SFML](https://www.sfml-dev.org/index.php) in C. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [FreeGLUT](http://freeglut.sourceforge.net/) - Alternative to the OpenGL Utility Toolkit. Allows the creation and management of windows with OpenGL contexts. [`X11`](https://directory.fsf.org/wiki/License:X11)
* [GLFW](https://www.glfw.org/) - Multi-platform library for creating windows with OpenGL contexts. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [libao](https://xiph.org/ao/) - Cross-platform audio library with a wide variety of outputs. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [RetroArch](https://www.libretro.com/) - The reference frontend for [libretro](https://www.libretro.com/). [`GNU GPL3`](http://www.gnu.org/licenses/gpl.html)
* [SDL and SDL2](https://www.libsdl.org/) - Cross-platform development library designed to provide low-level access to audio, keyboard, mouse, joystick and graphics hardware via OpenGL. SDL2 is the most current version. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [raylib](https://www.raylib.com/) - Simple and easy-to-use library to learn videogames programming. [`zlib`](https://directory.fsf.org/wiki/License:Zlib)
* [Gigoteur/UnicornConsole](https://github.com/Gigoteur/UnicornConsole) - Unicorn Console: create quick game !
* [HBehrens/obj2opengl](https://github.com/HBehrens/obj2opengl) - script to convert 3D models of OBJ files to C/C++ float arrays (vertices, faces, texture) compatible with OpenGL ES glDrawArrays compatible with iPhone/iPad
* [HerculesWS/Hercules](https://github.com/HerculesWS/Hercules) - Hercules is a collaborative software development project revolving around the creation of a robust massively multiplayer online role playing game (MMORPG) server package. Written in C, the program is very versatile and provides NPCs, warps and modifications. The project is jointly managed by a group of volunteers located around the world as well as a tremendous community providing QA and support. Hercules is a continuation of the original Athena project.
* [Kazade/kazmath](https://github.com/Kazade/kazmath) - A C math library targeted at games
* [MarilynDafa/Bulllord-Engine](https://github.com/MarilynDafa/Bulllord-Engine) - lightspeed lightweight elegant  game engine in pure c
* [MauriceGit/Cloth_Simulation](https://github.com/MauriceGit/Cloth_Simulation) - Cloth-Visualization via particle-simulation.
* [MauriceGit/Partikel_accelleration_on_GPU](https://github.com/MauriceGit/Partikel_accelleration_on_GPU) - Particle accelleration with OpenGL 4.3, using the compute shader to calculate particle movement on graphics hardware.
* [Olde-Skuul/doom3do](https://github.com/Olde-Skuul/doom3do) - The complete archive for DOOM for the 3DO
* [R4stl1n/cAudio](https://github.com/R4stl1n/cAudio) - 3D Audio Engine Based on Openal
* [RandyGaul/AsciiEngine](https://github.com/RandyGaul/AsciiEngine) - Game engine written in C to create Ascii art games within the Windows console.
* [Tangent128/luasdl2](https://github.com/Tangent128/luasdl2) - A pure C binding of SDL 2.0 for Lua 5.1, Lua 5.2, and LuaJIT.

## Graphics ##
Access to graphical APIs or other graphic rendering libraries.
* [FreeGLUT][179] - Alternative to the OpenGL Utility Toolkit. Allows the
  creation and management of windows with OpenGL contexts. [``X11``][X11]
* [GLFW][180] - Multi-platform library for creating windows with OpenGL
  contexts. [``Zlib``][Zlib]
* [Cairo][196] - 2D graphics library. [``LGPL-2.1-only``][LGPL-2.1-only] or [``MPL-1.1``][205]
* [graphene][197] - Thin layer of graphical data types. [``MIT``][MIT]
* [libcaca][198] - ASCII renderer for terminal-based interfaces. [``WTFPL``][WTFPL]
* [libsixel][199] - Library implementing the SIXEL protocol, allowing beautiful
  graphics in your terminal. [``MIT``][MIT]
* [libxmi][200] - Function library for rasterizing 2D vector
  graphics. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [lightmapper][201] - Single-file library for lightmap baking, using an
  existing OpenGL renderer. Public domain.
* [nanovg][202] - Anti-aliased 2D vector drawing library on top of OpenGL, for
  UI and visualizations. [``Zlib``][Zlib]
* [OpenGL][203] - Industry standard for high-performance graphics, with a
  native C binding. [Various licenses][204].
* [OpenGL](https://www.opengl.org/) - Industry adopted 2D and 3D graphics API. More resources at [awesome-opengl](https://github.com/eug/awesome-opengl).
* [OpenGL ES](https://www.khronos.org/opengles/) - Industry adopted 2D and 3D graphics API for mobile and embedded devices.
* [OpenGL SC](https://www.khronos.org/openglsc/) - Graphic and compute standard for industry requiring system safety certification.
* [Vulkan](https://www.khronos.org/vulkan/) - Explicit graphic and compute API for modern cross-platform development. More resources at [awesome-vulkan](https://github.com/vinjn/awesome-vulkan).
* [Cairo](https://www.cairographics.org/) -2D graphics library. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) or [`MPLv1.1`](https://directory.fsf.org/wiki/License:MPL-1.1)
* [Cogl](https://github.com/rib/cogl-web/wiki) - GPU graphics and utilities API. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [Clutter](https://blogs.gnome.org/clutter/get-it/) - UI library based on OpenGL. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [glfw/glfw](https://github.com/glfw/glfw) - A multi-platform library for OpenGL, OpenGL ES, Vulkan, window and input
* [nigels-com/glew](https://github.com/nigels-com/glew) - The OpenGL Extension Wrangler Library


## GUI ##
* [GTK+][206] - Cross-platform widget toolkit. [``LGPL-2.1-only``][LGPL-2.1-only]
* [IUP][207] - Another cross-platform widget toolkit. [``MIT``][MIT]
* [nuklear][208] - Small, C89, single-header widget toolkit. Public domain.
* [tinyfiledialogs][209] - Single-file library for simple dialogs. Compatible
  with many other toolkits and OSes. [``Zlib``][Zlib]
* [Tk][210] - Basic widget toolkit. Part of Tcl/Tk. [``TCL``][TCL]
* [XForms Toolkit][211] - Widget toolkit designed for the XWindow system. [``LGPL-2.1-only``][LGPL-2.1-only]
* [Glade][415] - RAD tool to enable quick development of GTK+ GUIs. [``GPL-2.0-only``][GPL-2.0-only]
* [vurtun/nuklear](https://github.com/vurtun/nuklear) - A single-header ANSI C gui library

## Hardware Oriented ##
* [libusb][407] - Provides generic access to USB devices. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libimobiledevice][408] - Cross-platform protocol library to communicate
  with iThings. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [cpu\_features][409] - Get CPU features at runtime. [``Apache-2.0``][Apache-2.0]
* [libcoap][423] - Implementation of the [Constrained Application Protocol][424].
  [``GPL-2.0-or-later``][GPL-2.0-or-later] or [``BSD-2-Clause``][BSD-2-Clause]
* [libnfc][438] - Platform-independent Near-Field Communication library. [``LGPL-3.0-only``][LGPL-3.0-only]
* [GTK+](https://www.gtk.org/) - Cross-platform widget toolkit. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [IUP](http://webserver2.tecgraf.puc-rio.br/iup/) - Another cross-platform widget toolkit. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [Tk](http://www.tcl.tk/) - Basic widget toolkit. Part of Tcl/Tk. [`Tcl/Tk License`](http://www.tcl.tk/software/tcltk/license.html)
* [XForms Toolkit](http://xforms-toolkit.org/) - Widget toolkit designed for the XWindow system. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [nuklear](https://github.com/vurtun/nuklear) - Single-header ANSI C gui library. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [libui](https://github.com/andlabs/libui) - Simple and portable (but not inflexible) GUI library. [`MIT`](https://github.com/andlabs/libui/blob/master/LICENSE)
* [LCUI](https://github.com/lc-soft/LCUI/) - Small C library for building user interfaces with C, XML and CSS. [`MIT`](https://github.com/lc-soft/LCUI/blob/develop/LICENSE.TXT)
* [Genymobile/scrcpy](https://github.com/Genymobile/scrcpy) - Display and control your Android device
* [AdysTech/raspy-weather](https://github.com/AdysTech/raspy-weather) - A set of C libraries to gather Temperature and Humidity data from generic DHT11 sensor, store it in a round-robin database and show it in a PHP page.
* [Azure/azure-iot-sdk-c](https://github.com/Azure/azure-iot-sdk-c) - A C99 SDK for connecting devices to Microsoft Azure IoT services
* [Eugnis/spectre-attack](https://github.com/Eugnis/spectre-attack) - Example of using revealed "Spectre" exploit (CVE-2017-5753 and CVE-2017-5715)
* [FoxelSA/libfastcal](https://github.com/FoxelSA/libfastcal) - Fast calibration data access
* [OpenSC/OpenSC](https://github.com/OpenSC/OpenSC) - Open source smart card tools and middleware. PKCS#11/MiniDriver/Tokend
* [OpenSecurityResearch/iclass_dump](https://github.com/OpenSecurityResearch/iclass_dump) - Tools to pull data from HID iClass readers
* [Stephane-D/SGDK](https://github.com/Stephane-D/SGDK) - SGDK: A small, open and free development kit for the Sega Megadrive

## Hashing ##
Hash function implementations for *non*-crypto purposes. Cryptographic hashes
can be found in the Crypto section.
* [CLHash][165] - Library implementing fast CLHash hashing function. Only works
  on Intel Haswell or newer. [``Apache-2.0``][Apache-2.0]
* [HighwayHash][166] - Fast, strong, SIMD-using hash function. Also contains an
  implementation of SipHash. [``Apache-2.0``][Apache-2.0]
* [SpookyHash][167] - Fast hash function. [``BSD-3-Clause``][BSD-3-Clause]
* [t1ha][168] - Fast Positive Hash - a portable, fast hash function. [``BSD-3-Clause``][BSD-3-Clause]
* [xxHash][169] - Fast 32 and 64 bit hashing algorithm. [``BSD-2-Clause``][BSD-2-Clause]
* [GNU gperf][414] - Perfect hash function generator, given a list of strings.
  Outputs C code. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [jwHash](https://github.com/watmough/jwHash) - Fast hashtable implementation. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [xxHash](http://cyan4973.github.io/xxHash/) - Extremely fast non-cryptographic hash algorithm. [`2-clause BSD`](https://directory.fsf.org/wiki/License:BSD-2-Clause)
* [libcrc](https://github.com/PeterScott/murmur3) - Multi platform CRC library. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [murmur](https://github.com/ispc/ispc) - C implementation of MurMur Hashing. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [Cyan4973/xxHash](https://github.com/Cyan4973/xxHash) - Extremely fast non-cryptographic hash algorithm
* [PeterScott/murmur3](https://github.com/PeterScott/murmur3) - Murmur3 hash in C
* [RJ/ketama](https://github.com/RJ/ketama) - C library for consistent hashing, and langauge bindings

## Image Processing and Computer Vision ##
* [ccv][5] - C-based/Cached/Core Computer Vision library; modern computer
  vision. [``BSD-3-Clause``][BSD-3-Clause]
* [libgd][380] - Library for the dynamic creation of images by programmers. [``MIT``][MIT]
* [giflib][381] - Library for reading and writing gif images. [``MIT``][MIT]
* [libimagequant][383] - Small, portable library for high-quality conversion of
  RGBA images to 8-bit indexed colour images. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [libjpeg-turbo][384] - Faster library for reading and writing JPEG files. [Various licences][194]
* [libpng][385] - Official PNG reference library. [``Libpng``][Libpng]
* [libRSVG][386] - Library to render SVG files using Cairo. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libvips][387] - Image processing library. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [mozjpeg][388] - Improved JPEG encoder. [``BSD-3-Clause``][BSD-3-Clause]
* [lodepng][389] - Simple PNG image decoder and encoder, requiring no other
  dependencies. [``BSD-3-Clause``][BSD-3-Clause]
* [libimagequant](https://pngquant.org/lib/) - Small, portable library for high-quality conversion of RGBA images to 8-bit indexed colour images. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [libjpeg-turbo](https://libjpeg-turbo.org/) - Faster library for reading and writing JPEG files. [`Various Licenses`](https://libjpeg-turbo.org/About/License)
* [libpng](http://www.libpng.org) - The official PNG reference library. [`libpng license`](http://www.libpng.org/pub/png/src/libpng-LICENSE.txt)
* [libxmi](https://www.gnu.org/software/libxmi/) - Function library for rasterizing 2D vector graphics. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [mozjpeg](https://github.com/mozilla/mozjpeg) - Improved JPEG encoder. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libccv](http://libccv.org) - Modern Computer Vision Library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [liuliu/ccv](https://github.com/liuliu/ccv) - C-based/Cached/Core Computer Vision Library, A Modern Computer Vision Library
* [MartinMittring/dcraw_exif](https://github.com/MartinMittring/dcraw_exif) - dcraw (Camera RAW format processor) from Dave Coffin with updates, additionally maintain exif data for using it with Agisoft PhotoScan
* [Phildo/pixQL](https://github.com/Phildo/pixQL) - SQL for image processing

## Integrated Debugging ##
* [whereami][390] - One-file library for locating the current executable on the
  file system. [``WTFPL``][WTFPL]
* [zlog][391] - Reliable, pure C logging library. [``LGPL-2.1-only``][LGPL-2.1-only]
* [debug][392] - One-header library for easier 'printf debugging'. [``MIT``][MIT]
* [CException][393] - Implementation of exceptions. [``MIT``][MIT]
* [pblog](https://github.com/google/pblog) - Small, low overhead, structured logging library intended for logging formware events.[`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [0xmalloc/c-log](https://github.com/0xmalloc/c-log) - a fast ,stable and thread-safe log lib(logger) for C/C++ language
* [Celtoys/Remotery](https://github.com/Celtoys/Remotery) - Single C file, Realtime CPU/GPU Profiler with Remote Web Viewer
* [HardySimpson/zlog](https://github.com/HardySimpson/zlog) - A reliable, high-performance, thread safe, flexsible, clear-model, pure C logging library.

## Lexing and Parsing ##
Generic lexers and parsers
* [flex][356] - Fast lexical analyzer generator. [``BSD-2-Clause``][BSD-2-Clause]
* [GNU Bison][357] - General-purpose parser generator that converts an
  annotated context-free grammar into a range of parsers. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [hammer][358] - Parser combinators for binary formats. [``GPL-2.0-only``][GPL-2.0-only]
* [mpc][359] - Parser combinator library. [``BSD-2-Clause``][BSD-2-Clause]
* [re2c][360] - Lexer generator, producing fast lexers, with access to its
  internals. Public domain.
* [MatzeB/cparser](https://github.com/MatzeB/cparser) - C99 parser and frontend for libfirm

## Memory Management ##
* [Boehm GC][212] - Garbage collection for C. Various licenses, all open source.
* [jemalloc][213] - Malloc implementation that emphasizes avoidance of
  fragmentation and scalable concurrency support. [``BSD-2-Clause``][BSD-2-Clause]
* [Lockless Memory Allocator][214] - Efficient memory allocator. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [rpmalloc][215] - Thread-caching, fast memory allocator, naturally aligned on
  32-byte boundaries. Public domain.
* [talloc][216] - Hierarchical, reference-counted memory pool system with
  destructors. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [tlsf][217] - Two-Level Segregated Fit allocator; a general-purpose, dynamic
  memory allocator designed to meet real-time requirements.
  [Up-to-date implementation][218]. [``BSD-3-Clause``][BSD-3-Clause]
* [jemalloc](http://jemalloc.net/) - General purpose malloc(3) implementation that emphasizes fragmentation avoidance and scalable concurrency support, commonly used in production systems. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [dlmalloc](http://g.oswego.edu/pub/misc/malloc.c) - Doug Lea's malloc(3) implementation, useful for academic and research purposes. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [Hoard](http://hoard.org/) - A Fast, Scalable, and Memory-efficient Malloc for Linux, Windows, Mac, and Solaris. [`GNU GPL2`](http://www.gnu.org/licenses/gpl.html)
* [nedmalloc](http://www.nedprod.com/programs/portable/nedmalloc/) - An EXTREMELY FAST portable thread caching malloc(3) implementation written in C. [`GNU GPL2`](http://www.gnu.org/licenses/gpl.html)
* [rpmalloc](https://github.com/rampantpixels/rpmalloc) - Cross platform, lock-free memory allocator. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [CCareaga/heap_allocator](https://github.com/CCareaga/heap_allocator) - A simple heap memory allocator in ~200 lines.

## Multimedia ##
Audio and video processing
* [ApeTagLibs][428] - Library for working with APEv2 tags. [``MIT``][MIT]
* [aubio][219] - Library for audio and music analysis. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [FFMPEG][220] - Complete, cross-platform solution to record, convert and
  stream audio and video. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [GStreamer][221] - Framework for audio and visual media. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libmpv][222] - Music-playing library. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [libsndfile][223] - Library for reading and writing sound files. Supports
  many formats. [``LGPL-2.1-only``][LGPL-2.1-only] or [``LGPL-3.0-only``][LGPL-3.0-only]
* [libsoundio][224] - Library for cross-platform, real-time audio input and
  output. Has a range of back-ends. [``MIT``][MIT]
* [minimp3][225] - Lightweight MP3 decoder single header library. [``CC0-1.0``][CC0-1.0]
* [Soundpipe][226] - Lightweight music DSP library. [``MIT``][MIT]
* [FFMPEG](https://www.ffmpeg.org/) - Complete, cross-platform solution to record, convert and stream audio and video. [`GNU LGPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) or [`GNU GPL2.1 or later (some parts)`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [GStreamer](https://gstreamer.freedesktop.org/) - Framework for audio and visual media. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [lodepng](https://lodev.org/lodepng/) - Simple PNG image decoder and encoder, requiring no other dependencies. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libsoup](https://wiki.gnome.org/action/show/Projects/libsoup?action=show&redirect=LibSoup) - GNOME HTTP client/server library. Uses GObject. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [libmpv](https://mpv.io/) - Music-playing library. Compile with ``./waf configure --disable-cplayer --enable-libmpv-shared`` to not have the music player. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [libsoundio](http://libsound.io/) - Library for cross-platform, real-time audio input and output. Has a range of back-ends. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [AVbin/AVbin](https://github.com/AVbin/AVbin) - AVbin is a C library that provides a thin, cross-platform wrapper around Libav’s video- and audio-decoding functionality, providing long-term binary compatibility for applications and languages that need it.  See also: Pyglet, a python media framework that makes extensive use of AVbin.
* [LnxPrgr3/crossfeed](https://github.com/LnxPrgr3/crossfeed) - Headphone crossfeed filter
* [PaulBatchelor/Soundpipe](https://github.com/PaulBatchelor/Soundpipe) - A lightweight music DSP library.

## Multiple Purpose Libraries ##
* [pal][65] - Optimized library for maths, parallel processing and data
  movement. [``Apache-2.0``][Apache-2.0]
* [APR][154] - Apache Portable Runtime; another library of cross-platform
  utility functions. [``Apache-2.0``][Apache-2.0]
* [C Algorithms][155] - Collection of common algorithms and data structures. [``ISC``][ISC]
* [CPL][156] - The Common Pipeline Library; a set of libraries designed to be a
  comprehensive, efficient and robust software toolkit. [``GPL-2.0-only``][GPL-2.0-only]
* [EFL][157] - Large collection of useful data structures and functions. Various
  licenses, all open source.
* [klib][158] - Small and lightweight implementations of common algorithms and
  data structures. [``MIT``][MIT]
* [libcork][159] - Utility functions and structures, designed for
  resource-constrained systems. Can be embedded. [``BSD-3-Clause``][BSD-3-Clause]
* [libnih][160] - Lightweight library of functions and structures. [``GPL-2.0-only``][GPL-2.0-only]
* [libU][161] - Small library of basic utilities, including memory allocation,
  string manipulation and logging. [``BSD-3-Clause``][BSD-3-Clause]
* [PBL][162] - Large library of utilities, featuring data structures, among
  other things. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [qlibc][163] - Simple and powerful library, designed as a replacement for GLib
  while focusing on being small and light. [``BSD-2-Clause``][BSD-2-Clause]
* [TBOX][164] - Multi-platform library with a large number of capabilities. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [gnulib][425] - Collection of common GNU code. Various licenses, all
  open source.
* [APR](http://apr.apache.org/) - Apache Portable Runtime; another library of cross-platform utility functions. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [C Algorithms](https://fragglet.github.io/c-algorithms/) - Collection of common algorithms and data structures for C. [`ISC`](https://directory.fsf.org/wiki/License:ISC)
* [CPL](http://www.eso.org/sci/software/cpl/) - The Common Pipeline Library; a set of libraries designed to be a comprehensive, efficient and robust software toolkit. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [EFL](https://www.enlightenment.org/) - Large collection of useful data structures and functions.
* [GLib](https://wiki.gnome.org/Projects/GLib) - Library of utility functions and structures, designed to be portable, efficient and powerful. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [GIO](https://developer.gnome.org/gio/) - Modern and easy-to-use VFS API. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [GObject](https://developer.gnome.org/gobject/stable/) - Object-oriented system and object model for C. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [libnih](https://github.com/keybuk/libnih) - Lightweight library of C functions and structures. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [libU](http://www.koanlogic.com/libu/) - Small library of basic utilities, including memory allocation, string manipulation and logging. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [PBL](http://www.mission-base.com/peter/source/) - Large library of utilities, featuring data structures, among other things. [`GNU LGPL2.1 or later (library)`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) or [`GNU GPL2.1 or later (test code)`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [qlibc](http://wolkykim.github.io/qlibc/) - Simple and powerful C library, designed as a replacement for GLib while focusing on being small and light. [`qLib license`](https://github.com/wolkykim/qlibc/blob/master/LICENSE) (similar to [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD))
* [stb](https://github.com/nothings/stb) - Range of single-file libraries for C. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [libsrt](https://faragon.github.io/libsrt.html) - Safe Real-Time library for C. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)

## Networking ##
### DNS ###
* [GNU adns][229] - Advanced, easy-to-use, asynch-capable DNS client library
  and utilities. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [ldns][231] - Library to simplify DNS programming. [``BSD-3-Clause``][BSD-3-Clause]

### HTTP ###
* [http-parser][230] - HTTP request/response parser. [``MIT``][MIT]
* [libsagui][239] - Library for cross-platform HTTP servers. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [lwan][242] - Experimental, scalable, high-performance HTTP server. [``GPL-2.0-only``][GPL-2.0-only]
* [mongoose][243] - Embedded web server. [``GPL-2.0-only``][GPL-2.0-only]
* [libhttpd][234] - Library to add basic web server capabilities to an
  application or embedded device. [``GPL-2.0-only``][GPL-2.0-only]
* [libmicrohttpd][236] - Small library that makes it easy to run an HTTP
  server as part of another application. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libonion][237] - HTTP server library, designed to be easy to use. [``Apache-2.0``][Apache-2.0]
* [nodejs/http-parser](https://github.com/nodejs/http-parser) - http request/response parser for c

### Mail ###
* [LibEtPan][233] - Mail library providing an efficient network for IMAP, SMTP,
  POP and NNTP. [``BSD-3-Clause``][BSD-3-Clause]
* [libvldmail][439] - Email validation library. No external dependencies
  (not even regexps). [``WTFPL``][WTFPL]
* [libquickmail][238] - Library intended to give developers a way to send email
  from their applications. Supports multiple To/Cc/Bcc recipients and
  attachments without size limits. [``GPL-3.0-or-later``][GPL-3.0-or-later]

### Messaging ###
* [NNG][245] - nanomsg-next-generation - lightweight brokerless messaging. [``MIT``][MIT]
* [rabbitmq-c][440] - Client library for [RabbitMQ][229]. [``MIT``][MIT]
* [zproto][370] - Protocol framework for ZeroMQ. [``MIT``][MIT]
* [nanomsg][244] - C-based implementation of ZeroMQ. [``MIT``][MIT]

### Other Networking ###
* [asnlc][227] - Compiler of ASN.1 specifications into C source code. [``BSD-2-Clause``][BSD-2-Clause]
* [CHL][228] - C Hypertext Library - A library for writing for web in C. [``GPL-3.0-only``][GPL-3.0-only]
* [libcurl][232] - Client-side URL transfer library, supporting a wide range of
  formats. [``curl``][curl]
* [libidn][235] - Implementation of the Stringprep, Punycode and IDNA
  specifications. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [LibVNCServer][240] - Cross-platform libraries to implement VNC server and/or
  client functionality. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [oSip][246] - SIP implementation without additional dependencies. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [socket99][247] - C99 wrapper for the BSD sockets API. [``ISC``][ISC]
* [zyre][249] - Framework for proximity-based peer-to-peer applications. [``MPL-2.0``][MPL-2.0]
* [libgss][435] - Generic Security Service. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [asnlc](http://lionet.info/asn1c/compiler.html) - Compiler of ASN.1 specifications into C source code. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [czmq](http://czmq.zeromq.org/) - High-level binding for ZeroMQ. [`MPL2.0`](https://www.gnu.org/licenses/license-list.html#MPL-2.0)
* [GNU adns](https://www.gnu.org/software/adns/) - Advanced, easy-to-use, asynch-capable DNS client library and utilities. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [GNU SASL](https://www.gnu.org/software/gsasl/) - Implementation of the Simple Authentication and Security Layer and a few common SASL mechanism. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [GnuTLS](https://www.gnutls.org/) - Secure communication library, implementing SSL, TLS and DTLS. [`GNU LGPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [gumbo-parser](https://github.com/google/gumbo-parser) - HTML5 parsing library in C99. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [http-parser](https://github.com/nodejs/http-parser) - HTTP request/response parser. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [ldns](https://www.nlnetlabs.nl/projects/ldns/index.html) - Library to simplify DNS programming. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libcurl](https://curl.haxx.se/libcurl/) - Client-side URL transfer library, supporting a wide range of formats. [`curl license`](https://curl.haxx.se/docs/copyright.html)
* [LibEtPan](http://www.etpan.org/) - Mail library providing an efficient network for IMAP, SMTP, POP and NNTP. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libev](http://software.schmorp.de/pkg/libev.html) - Yet another event loop. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [libuv](http://libuv.org/) - Cross-platform asynchronous I/O. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [libevent](http://libevent.org/) - Event loop replacement for network servers. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [libgss](https://www.gnu.org/software/gss/) - Generic Security Service. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [libhttpd](http://www.hughes.com.au/products/libhttpd/) - Library to add basic web server capabilities to an application or embedded device. [`GNU GPL2`](http://www.gnu.org/licenses/gpl.html)
* [libidn](https://www.gnu.org/software/libidn/) - Implementation of the Stringprep, Punycode and IDNA specifications. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [libmicrohttpd](https://www.gnu.org/software/libmicrohttpd/) - Small C library that makes it easy to run an HTTP server as part of another application. [`GNU LGPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [libsagui](https://risoflora.github.io/libsagui/) - Sagui is a cross-platform C library which helps to develop web servers or frameworks. [`GNU LGPL3`](http://www.gnu.org/licenses/lgpl.html)
* [libvldmail](https://github.com/dertuxmalwieder/libvldmail) - Your friendly e-mail address validation library. [`WTFPLv2`](http://www.wtfpl.net/txt/copying/)
* [lwan](https://lwan.ws/) - Experimental, scalable, high-performance HTTP server. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [mongoose](https://cesanta.com/) - Embedded web server for C. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [MQTT-C](https://github.com/LiamBindle/MQTT-C) - Portable MQTT C client for embedded systems and PCs alike. [`MIT`](https://raw.githubusercontent.com/LiamBindle/MQTT-C/master/LICENSE)
* [nanomsg](https://github.com/nanomsg/nanomsg) - C-based implementation of ZeroMQ. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [oSip](https://www.gnu.org/software/osip/) - SIP implementation in C without additional dependencies. [`GNU LGPLv2.1 or later`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [pig](https://github.com/rafael-santiago/pig) - Linux packet crafting tool. [`GPL2`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [s2n](https://github.com/awslabs/s2n) - C99 implementation of the TLS/SSL protocols, designed to be simple, fast and with security as a priority. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [socket99](https://github.com/silentbicycle/socket99) - C99 wrapper for the BSD sockets API. [`ISC`](https://directory.fsf.org/wiki/License:ISC)
* [Tox](https://tox.chat/) - Communication platform, designed to be a Skype-killer. [`GNU GPL3`](http://www.gnu.org/licenses/gpl.html)
* [librg](https://github.com/librg/librg) - Library for building simple and elegant cross-platform mmo client-server solutions. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [dyad](https://github.com/rxi/dyad) - Asynchronous networking library. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [h2o](https://github.com/h2o/h2o/) - Optimized HTTP/1, HTTP/2 high performance server/library. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [51Degrees/Device-Detection](https://github.com/51Degrees/Device-Detection) - THE Fastest and most Accurate device detection for C / PHP / Perl / Python and Node.js - professionally maintained device data
* [uriparser](https://uriparser.github.io) - Strictly RFC 3986-compliant URI parsing and handling library. [``BSD-3-Clause``][BSD-3-Clause]
* [ElementsProject/lightning](https://github.com/ElementsProject/lightning) - c-lightning — a Lightning Network implementation in C
* [FreeRDP/FreeRDP](https://github.com/FreeRDP/FreeRDP) - FreeRDP is a free remote desktop protocol library and clients
* [FreeRDP/Remmina](https://github.com/FreeRDP/Remmina) - The GTK+ Remmina Remote Desktop Client
* [GROX13/BitTorrent](https://github.com/GROX13/BitTorrent) - BitTorrent is a protocol for the practice of peer-to-peer file sharing that is used to distribute large amounts of data over the Internet. BitTorrent is one of the most common protocols for transferring large files, and peer-to-peer networks have been estimated to collectively account for approximately 43% to 70% of all Internet traffic (depending on geographical location) as of February 2009. In November 2004, BitTorrent was responsible for 35% of all Internet traffic. As of February 2013, BitTorrent was responsible for 3.35% of all worldwide bandwidth, more than half of the 6% of total bandwidth dedicated to file sharing.
* [JFreegman/toxic](https://github.com/JFreegman/toxic) - An ncurses-based Tox client
* [LibVNC/libvncserver](https://github.com/LibVNC/libvncserver) - LibVNCServer/LibVNCClient are cross-platform C libraries that allow you to easily implement VNC server or client functionality in your program.
* [Librevault/librevault](https://github.com/Librevault/librevault) - Librevault - Peer-to-peer, decentralized and open source file sync.
* [Netsukuku/netsukuku](https://github.com/Netsukuku/netsukuku) - Revived C-code
* [Tox/toxic](https://github.com/Tox/toxic) - CLI Tox client

### Websockets ###
* [Wslay][248] - WebSocket library. Implements version 13 of the WebSocket
  protocol, as described in RFC 6455. [``MIT``][MIT]
* [libwebsock][241] - Easy-to-use and powerful web socket library. [``LGPL-3.0-only``][LGPL-3.0-only]

--------------------------------------------------------------------------------

## OS Specifics ##
* [attr][401] - Commands for manipulating filesystem extended attributes. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [Caffeine][402] - Library for building daemons and services for Linux and
  FreeBSD systems. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libcox][403] - Library which permits cross-platform system calls and
  standard utilities across different operating systems. [``BSD-2-Clause``][BSD-2-Clause]
* [GNU FreeIPMI][422] - In-band and out-of-band IPMI implementation. [``GPL-3.0-only``][GPL-3.0-only]
* [CRIU][427] - Checkpoint/Restore In Userspace; a software tool (with a C API)
  for 'freezing' a running application to disk, then restoring it. Targeted for
  Linux. [``GPL-2.0-only``][GPL-2.0-only] or [``LGPL-2.1-only``][LGPL-2.1-only]
* [linenoise][433] - Small, self-contained alternative to readline and libedit. [``BSD-2-Clause``][BSD-2-Clause]
* [alsa-lib](http://www.alsa-project.org/main/index.php/Main_Page) - Userspace library to interact with ALSA. [`LGPL2.1`](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.en.html)
* [Leandros/WindowsHModular](https://github.com/Leandros/WindowsHModular) - A modular Windows.h Header. Licensed under Public Domain & MIT.
* [Microsoft/Windows-driver-samples](https://github.com/Microsoft/Windows-driver-samples) - This repo contains driver samples prepared for use with Microsoft Visual Studio and the Windows Driver Kit (WDK). It contains both Universal Windows Driver and desktop-only driver samples.
* [Microsoft/checkedc](https://github.com/Microsoft/checkedc) - Checked C is an extension to C that adds checking to detect or prevent common programming errors such as buffer overruns and out-of-bounds memory accesses.  This repo has a wiki for Checked C, sample code, the specification, and test code.

## Procedural Generation ##
* [heman][382] - Tiny library of image utilities dealing with height maps,
  normal maps, distance fields and the like. [``MIT``][MIT]
* [JCash/voronoi](https://github.com/JCash/voronoi) - A C implementation for creating 2D voronoi diagrams

## Regex ##
* [Onigmo][275] - Fork of Oniguruma, supporting more advanced regexps. [``BSD-2-Clause``][BSD-2-Clause]
* [Oniguruma][276] - Regex library supporting a wide range of encodings, and
  incorporating many security-oriented fixes. [``BSD-2-Clause``][BSD-2-Clause]
* [PCRE][277] - Implementation of regexes identical to that of Perl 5. [``BSD-3-Clause``][BSD-3-Clause]
* [SLRE][278] - Super Light Regular Expression library; a small implementation
  of a subset of Perl regex syntax. [``GPL-2.0-only``][GPL-2.0-only]
* [TRE][279] - POSIX-compliant, feature-full regex library. [``BSD-2-Clause``][BSD-2-Clause]
* [PCRE](http://www.pcre.org/) - Implementation of regexes identical to that of Perl 5. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [regexp4](https://github.com/nasciiboy/recursiveregexpraptor-4) - Simple and complete implementation of regular expressions with its own sintax. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [SLRE](https://github.com/cesanta/slre) - Super Light Regular Expression library; a very small implementation of a subset of Perl regex syntax. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [TRE](https://github.com/laurikari/tre/) - POSIX-compliant, feature-full regex library. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [sregex](https://github.com/openresty/sregex) - Non-backtracking NFA/DFA-based Perl-compatible regex engine library. [`3-clause BSD`](https://opensource.org/licenses/BSD-3-Clause)
* [JazzCore/ctrlp-cmatcher](https://github.com/JazzCore/ctrlp-cmatcher) - CtrlP C matching extension
* [Maxime2/dataparksearch](https://github.com/Maxime2/dataparksearch) - An open source, feature rich search engine.

## Serialization ##
* [binn][280] - Binary serialization format, meant to be compact, fast and
  easy-to-use. [``Apache-2.0``][Apache-2.0]
* [c-capnproto][281] - Implementation of the Cap'n Proto serialization protocol. [``MIT``][MIT]
* [cmp][282] - Implementation of the [MessagePack][283] serialization protocol. [``MIT``][MIT]
* [flatcc][284] - [FlatBuffers][285] compiler and library. [``Apache-2.0``][Apache-2.0]
* [libavro][286] - Implementation of the Avro data serialization system. [``Apache-2.0``][Apache-2.0]
* [mpack][287] - Another implementation of the [MessagePack][283] serialization
  protocol. [``MIT``][MIT]
* [OPIC][288] - Object Persistence in C; a revolutionary serialization
  framework, with matching on-disk and in-memory representations. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [protobuf-c][289] - Implementation of Google Protocol Buffer. [``BSD-2-Clause``][BSD-2-Clause]
* [tpl][290] - Small binary serialization library. [``MIT``][MIT]
* [xdr][291] - External Data Representation; a standard for data serialization.
  Standard (no license applicable).
* [pbc][437] - Protocol buffers library. [``MIT``][MIT]
* [binn](https://github.com/liteserver/binn) - Binary serialization format meant to be compact, fast and easy-to-use. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [c-capnproto](https://github.com/jmckaskill/c-capnproto) - Implementation of the Cap'n Proto serialization protocol. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [cmp](https://github.com/camgunz/cmp) - Implementation of the [MessagePack](https://msgpack.org/) serialization protocol. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [libavro](http://avro.apache.org/docs/current/api/c/index.html#_introduction_to_avro_c) - C implementation of the Avro data serialization system. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [mpack](https://github.com/ludocode/mpack) - Another implementation of the [MessagePack](https://msgpack.org/) serialization protocol. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [netstring-c](https://github.com/liteserver/netstring-c) - Netstring encoder and decoder. [`Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [protobuf-c](https://github.com/protobuf-c/protobuf-c) - Implementation of Google Protocol Buffer in C. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [xdr](https://en.wikipedia.org/wiki/External_Data_Representation) - External Data Representation; a standard for data serialization.
* [ErikDubbelboer/c-pack](https://github.com/ErikDubbelboer/c-pack) - Simple data packing/unpacking in C

## Source Code Collections ##
* [CCAN][292] - Modelled after Perl's CPAN, this is a big collection of code.
  Various licenses, all open source.
* [clib][293] - Something of a package manager. Comes with a
  [bunch of libraries of its own][294]. [``MIT``][MIT]
* [libdjb][295] - Collection of libraries doing various things. (Apparently)
  public domain.
* [mmx][296] - Collection of single-header libraries. Various licenses, all
  open source.
* [par][297] - Bunch of single-file libraries. [``MIT``][MIT]
* [Snippets][298] - Useful code snippets and header-only libraries.
  Public domain.
* [stb][299] - Range of single-file libraries. Public domain.
* [tinyheaders][300] - Collection of header-only libraries, primarily oriented
  toward game development. [``Zlib``][Zlib]
* [CCAN](http://ccodearchive.net/) - Modelled after Perl's CPAN, this is a big collection of C code that does stuff. The full list is [here](http://ccodearchive.net/list.html).
* [clib](https://github.com/clibs/clib) - Something of a package manager for C. Comes with a [bunch of libraries of its own](https://github.com/clibs/clib/wiki/Packages). [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [gnulib](https://www.gnu.org/software/gnulib/) - Collection of common GNU code.
* [libdjb](http://www.fefe.de/djb/) - Collection of libraries doing various things. [`(Apparently) Public Domain`](https://creativecommons.org/share-your-work/public-domain/)
* [BurntSushi/clibs](https://github.com/BurntSushi/clibs) - A smattering of miscellaneous C libraries. Includes sane argument parsing, a thread-safe multi-producer/multi-consumer queue, and implementation of common data structures (hashmaps, vectors and linked lists).
* [RandyGaul/cute_headers](https://github.com/RandyGaul/cute_headers) - Collection of cross-platform one-file C/C++ libraries with no dependencies, primarily used for games

## Special Purpose ##
* [Tulip Indicators][394] - Library of functions for technical analysis of
  financial data. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [libtrading][395] - Implementation of network protocols for communicating
  with exchanges, dark pools and other trading venues. Supports FIX, FIX/FAST
  and many proprietary protocols. [``BSD-2-Clause``][BSD-2-Clause]
* [libpostal][396] - Library for parsing and normalization of street addresses
  around the world. Powered by statistical NLP and open geo data. [``MIT``][MIT]
* [libgeohash][417] - Pure C implementation of the Geohash algorithm. [``BSD-3-Clause``][BSD-3-Clause]
* [AaronJackson/sage-in-c](https://github.com/AaronJackson/sage-in-c) - Simple library written in C for accessing invoices and company data created by Sage Accounts 50.
* [GuillaumeHolley/BloomFilterTrie](https://github.com/GuillaumeHolley/BloomFilterTrie) - A data structure for pan-genome storage
* [Jahor/osm-tools](https://github.com/Jahor/osm-tools) - Tools to operate OpenStreetMap data
* [JayDDee/cpuminer-opt](https://github.com/JayDDee/cpuminer-opt) - Optimized multi algo CPU miner
* [MatthewLM/cbitcoin](https://github.com/MatthewLM/cbitcoin) - A low-level bitcoin library written in standard C.
* [Netflix/dynomite](https://github.com/Netflix/dynomite) - A generic dynamo implementation for different k-v storage engines
* [RhysU/ESIO](https://github.com/RhysU/ESIO) - The ExaScale IO (ESIO) library provides simple, high throughput input and output of structured data sets using parallel HDF5. ESIO is designed to support reading and writing turbulence simulation restart files within C, C++, and modern Fortran applications.
* [TPSully/SRTM2STL](https://github.com/TPSully/SRTM2STL) - Create STL files from SRTM data for the purpose of creating 3D relief maps.

## Standard Libraries ##
Implementations of the C standarts

* [Bionic][301] - Google's standard library, developed for Android. [``BSD-3-Clause``][BSD-3-Clause]
* [cloudlibc][302] - Standard library based on the concept of
  [capability-based security][303]. [``BSD-2-Clause``][BSD-2-Clause]
* [dietlibc][304] - Standard library designed for the smallest possible
  binaries. [``GPL-2.0-only``][GPL-2.0-only]
* [glibc][305] - The GNU C Library; an implementation of the standard library. [``LGPL-2.1-only``][LGPL-2.1-only].
* [musl][306] - Standard library, compatible with POSIX 2008 and C11. Designed
  for static linking. [``MIT``][MIT]
* [PDCLib][307] - The Public Domain C Library. Implements most of C99 and some
  of C11. [``CC0-1.0``][CC0-1.0]
* [uClibc-ng][308] - Small C library for developing embedded systems.
  [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [Bionic](https://github.com/aosp-mirror/platform_bionic) - Google's C standard library, developed for Android. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [dietlibc](http://www.fefe.de/dietlibc/) - C standard library designed for the smallest possible binaries. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [glibc](http://www.gnu.org/software/libc/) - The GNU C Library; an implementation of the C standard library. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [musl](http://www.musl-libc.org/) - Standard C library, compatible with POSIX 2008 and C11. Designed for static linking. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [NuxiNL/cloudlibc](https://github.com/NuxiNL/cloudlibc) - CloudABI's standard C library

## String Manipulation ##
* [bstring][309] - The Better String Library. [``BSD-3-Clause``][BSD-3-Clause]
* [ICU][310] - International Components for Unicode; a library for Unicode
  support. [``ICU``][ICU]
* [levenstein.c][311] - [Levenstein distance][312] algorithm implementation. [``MIT``][MIT].
* [libunistring][313] - Library for manipulating Unicode strings. [``LGPL-3.0-only``][LGPL-3.0-only]
* [libgiconv][314] - Text conversion library. [``LGPL-2.1-only``][LGPL-2.1-only]
* [librope][315] - UTF-8 rope ('heavy' string) library. [``MIT``][MIT]
* [rapidstring][316] - Maybe the fastest string library ever. [``MIT``][MIT]
* [SDS][317] - Simple Dynamic Strings; a library for handling strings in a
  simpler way, but one that is compatible with normal C string functions. [``BSD-2-Clause``][BSD-2-Clause]
* [stmr.c][318] - [Porter Stemmer][319] algorithm implementation. [``MIT``][MIT]
* [utf8.h][320] - Single-header UTF-8 library, designed to mimic C-style string
  functions. Public domain.
* [utf8proc][321] - Library for processing UTF-8 data. [``MIT``][MIT]
* [bstrlib](http://bstring.sourceforge.net/) - The Better String Library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause) and [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [ICU](http://site.icu-project.org/) - International Components for Unicode; a library for Unicode support. [`ICU license`](http://source.icu-project.org/repos/icu/icu/tags/latest/LICENSE)
* [libunistring](https://www.gnu.org/software/libunistring/) - Library for manipulating Unicode strings in C. [`GNU LGPL3`](http://www.gnu.org/licenses/lgpl.html)
* [libgiconv](https://www.gnu.org/software/libiconv/) - Text conversion library. [`GNU LGPL2.1 (library)`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) or [`GNU GPL3 (*iconv* program)`](http://www.gnu.org/licenses/gpl.html)
* [SDS](https://github.com/antirez/sds) - Simple Dynamic Strings; a library for handling C strings in a simpler way, but one that is compatible with normal C string functions. Available via [clib](https://github.com/clibs/clib). [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [shoco](http://ed-von-schleck.github.io/shoco/) - Compressor for small text strings. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [smaz](https://github.com/antirez/smaz) - Efficient string compression library. [`3-clause BSD`](https://directory.fsf.org/wiki/License:BSD-3-Clause)
* [utf8.h](https://github.com/sheredom/utf8.h) - Single header utf8 string functions. [`Unlicense`](http://unlicense.org/)
* [utf8proc](https://github.com/JuliaStrings/utf8proc) - Small, clean library for processing UTF-8 Unicode data. [`License`](https://github.com/JuliaStrings/utf8proc/blob/master/LICENSE.md)
* [JuliaStrings/utf8proc](https://github.com/JuliaStrings/utf8proc) - a clean C library for processing UTF-8 Unicode data

## Structured File Processing ##
Libraries for working wit hspecific filetypes

### Binaries ###
* [bfd][436] - Library for manipulating binary object files. Part of GNU
  binutils. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [libelf][337] - Simple library for parsing ELF files. [``MIT``][MIT]

### CSV ###
* [libcsv][322] - Simple, streaming CSV parser. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]

### JSON ###
* [Jansson][323] - Library for encoding, decoding and manipulating JSON. [``MIT``][MIT]
* [jfes][324] - JSON For Embedded Systems; simple JSON engine without any
  dependencies. [``MIT``][MIT]
* [jsmn][325] - Minimalistic JSON parser. [``MIT``][MIT]
* [json.h][326] - Single-file non-streaming JSON parser. [``Unlicense``][Unlicense]
* [WJElement][327] - Advanced JSON manipulation library, with support for JSON
  Schema. Various licenses, all open source.
* [YAJL][328] - Fast streaming JSON parser library. [``ISC``][ISC]
* [Jansson](http://www.digip.org/jansson/) - C library for encoding, decoding and manipulating JSON. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [jsmn](https://zserge.com/jsmn.html) - Minimalistic JSON parser. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [json-c](https://github.com/json-c/json-c/wiki) - Library for working with JSON. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [parson](https://github.com/kgabis/parson) - Lightweight JSON library written in C. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [WJElement](https://github.com/netmail-open/wjelement/wiki) - Advanced JSON manipulation library, with support for JSON Schema. [`LGPL, any version`](https://github.com/netmail-open/wjelement/)
* [YAJL](https://lloyd.github.io/yajl/) - Fast C JSON streaming parser library. [`ISC`](https://directory.fsf.org/wiki/License:ISC)
* [DaveGamble/cJSON](https://github.com/DaveGamble/cJSON) - Ultralightweight JSON parser in ANSI C

### INI ###
* [inih][329] - Small and simple INI file parser, good for embedded systems. [``BSD-3-Clause``][BSD-3-Clause]
* [iniparser][330] - Parser for .ini files. [``MIT``][MIT]
* [libconfini][331] - Yet another INI parser. [``GPL-3.0-only``][GPL-3.0-only]

### Markdown ###
* [Hoedown][375] - Fully standards-compliant, extension-supporting, UTF-8
  aware, fast Markdown parser. [``MIT``][MIT]
* [libcmark][376] - Library for parsing the CommonMark dialect of
  Markdown. [``BSD-2-Clause``][BSD-2-Clause]
* [Discount][377] - Simple implementation of a Markdown parser. [``BSD-3-Clause``][BSD-3-Clause]
* [cmark][420] - Implementation of the CommonMark, Markdown dialect.
  [Variety of licenses, all open source][421].
* [Orc/discount](https://github.com/Orc/discount) - My C implementation of John Gruber's Markdown markup language

### XML ###
* [Expat][332] - Stream-oriented XML parser. [MIT][MIT]
* [libxml2][333] - Standards-compliant, portable XML parser. [MIT][MIT]
* [mini-xml](https://github.com/michaelrsweet/mxml) - Small XML reading and writing library. No dependencies aside from C standard library. [`GNU LGPL2.1 with static linking exception`](https://github.com/michaelrsweet/mxml/blob/master/COPYING)
* [CastXML/CastXML](https://github.com/CastXML/CastXML) - C-family Abstract Syntax Tree XML Output

### YAML ###
* [libYAML][334] - YAML 1.1 parser and emitter. [``MIT``][MIT]

### Other Filetypes ###
* [libbson][335] - BSON utility library. [``Apache-2.0``][Apache-2.0]
* [libconfuse][336] - Small configuration file parser library. [``ISC``][ISC]
* [libucl][338] - Universal configuration library parser. [``BSD-2-Clause``][BSD-2-Clause]
* [libxo][339] - Allows an application to generate plain text, XML, JSON and
  HTML output using a common set of function calls. The application decides at
  runtime what output style should be produced. [``BSD-2-Clause``][BSD-2-Clause]
* [XLSX I/O][413] - Cross-platform library for reading and writing .xlsx files. [``MIT``][MIT]
* [gumbo-parser][416] - HTML5 parsing library in C99. [``Apache-2.0``][Apache-2.0]
* [hammer](https://github.com/abiggerhammer/hammer) - Parser combinators for binary formats. [`GNU GPL2.1`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [iniparser](https://github.com/ndevilla/iniparser) - Parser for `.ini` files. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [libconfini](https://github.com/madmurphy/libconfini) - Yet another INI parser. [`GNU GPL3 or later`](http://www.gnu.org/licenses/gpl.html)
* [libYAML](https://pyyaml.org/wiki/LibYAML) - YAML 1.1 parser and emitter. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [mpc](https://github.com/orangeduck/mpc) - Parser combinator library. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [libucl](https://github.com/vstakhov/libucl) - Universal configuration library parser. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [StefanKarpinski/odb](https://github.com/StefanKarpinski/odb) - ODB: On-Disk Binary Data Tool

--------------------------------------------------------------------------------

## Testing ##
* [CHEAT][340] - Simple unit testing framework. [``BSD-2-Clause``][BSD-2-Clause]
* [Check][341] - Unit testing framework. [``LGPL-2.1-only``][LGPL-2.1-only]
* [ciut][342] - A modern minimal hassle unit test framework. [``MIT``][MIT]
* [clar][343] - Clear and simple unit testing framework. [``MIT``][MIT]
* [CMock][344] - Mock/stub generator. [``MIT``][MIT]
* [cmocka][345] - Unit testing framework with support for mock objects. [``Apache-2.0``][Apache-2.0]
* [Criterion][346] - KISS, non-intrusive test framework. [``MIT``][MIT]
* [ctest][347] - Yet another unit testing framework. [``Apache-2.0``][Apache-2.0]
* [CUnit][348] - Another unit testing framework. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [greatest][349] - Unit testing library in one file, with no memory allocation. [``MIT``][MIT]
* [minctest][350] - Unit testing microlibrary. [``BSD-3-Clause``][BSD-3-Clause]
* [munit][351] - Small unit testing framework. [``MIT``][MIT]
* [theft][352] - Property-based testing (similar to [Quickcheck][353]). [``MIT``][MIT]
* [Unity][354] - Simple unit testing framework. [``MIT``][MIT]
* [utest][355] - Single-header unit testing library. [``Unlicense``][Unlicense]
* [CHEAT](http://users.jyu.fi/~sapekiis/cheat/) - Very simple unit testing framework. [`FreeBSD`](https://directory.fsf.org/wiki?title=License:FreeBSD)
* [Check](https://libcheck.github.io/check/) - Unit testing framework for C. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [CMock](http://www.throwtheswitch.org/) - Mock/stub generator for C. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [cmocka](https://cmocka.org/) - Unit testing framework with support for mock objects. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [Criterion](https://criterion.readthedocs.io/en/master/) - KISS, non-intrusive C test framework. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [CUnit](http://cunit.sourceforge.net/) - Another unit testing framework for C. [`GNU LGPL2.0`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [Cutest](https://github.com/rafael-santiago/cutest) - Library for unit testing with memory leak detection (Linux, freeBSD and Windows). [`GPL2`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
* [minunit](https://github.com/siu/minunit) - Minimal unit testing framework for C. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [munit](https://nemequ.github.io/munit/) - Small but full-featured unit testing framework for C with no dependencies. [`MIT`](https://raw.githubusercontent.com/atom/atom/master/LICENSE.md)
* [Unity](http://www.throwtheswitch.org/) - Simple unit testing framework for C. [`Expat`](https://directory.fsf.org/wiki/License:Expat)
* [zorgnax/libtap](https://github.com/zorgnax/libtap) - Write tests in C
* [Snaipe/Criterion](https://github.com/Snaipe/Criterion) - A cross-platform C and C++ unit testing framework for the 21th century
* [ThrowTheSwitch/Unity](https://github.com/ThrowTheSwitch/Unity) - Simple Unit Testing for C

## TUI ##
Textual User Interface
* [progressbar][371] - Easy-to-use library for displaying text progress bars. [``BSD-3-Clause``][BSD-3-Clause]
* [netbsd-curses][372] - Simplified and small version of ncurses, with the same
  interface. [``BSD-3-Clause``][BSD-3-Clause]
* [ncurses][373] - Coloured terminal UI library. [``MIT``][MIT]
* [termbox][374] - Library for writing text-based interfaces. [``MIT``][MIT]

## Web Frameworks ##
Comprehensive and integrated solutions for building web application in C.
* [Cloudgizer][361] - Cloudgizer is a tool for building web applications as
  Apache modules, with emphasis on performance, small-footprint, and more
  productive and safer programming in C. [``Apache-2.0``][Apache-2.0]
* [facil.io][362] - Mini-framework for web applications. Includes a fast HTTP
  and Websocket server, and also supports custom protocols. [``MIT``][MIT]
* [KLone][363] - Fully featured, multi-platform, web application development
  framework, targeted especially at embedded systems and appliances. [``BSD-3-Clause``][BSD-3-Clause]
* [Kore][364] - Easy-to-use web application framework for writing scalable
  web APIs in C. [``ISC``][ISC]
* [WAFer][378] - Ultra-light software platform for scalable server-side and
  networking applications (think node.js for C programmers). [``GPL-2.0-only``][GPL-2.0-only]
* [balde](https://balde.rgm.io/) - Microframework for C based on GLib. [`GNU LGPLv2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
* [onion](https://www.coralbits.com/libonion/) - C library to create simple HTTP servers and Web Applications. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [kore](https://kore.io/) - Easy to use, scalable and secure web application framework for writing web APIs in C.
* [klone](http://www.koanlogic.com/klone/) - KLone is a fully-featured, multiplatform, web application development framework.
* [duda](http://duda.io/) - Duda I/O is an event-driven and high performant web services framework written in C. [`Apache 2.0`](https://directory.fsf.org/wiki/License:Apache-2.0)
* [DanielWaterworth/Raphters](https://github.com/DanielWaterworth/Raphters) - [DEPRECATED] A web framework for C.

## Web Service APIs ##
* [twitc][426] - Mini library for interacting with the Twitter OAuth API. [``MIT``][MIT]
* [dajobe/flickcurl](https://github.com/dajobe/flickcurl) - Flickr C API library
* [Cotix/cReddit](https://github.com/Cotix/cReddit) - CLI Reddit client written in C. Oh, crossplatform too!
* [HalosGhost/shaman](https://github.com/HalosGhost/shaman) - A small, native C library and utility to fetch weather
* [PromyLOPh/pianobar](https://github.com/PromyLOPh/pianobar) - Console-based pandora.com player
* [TOTBWF/SteamCurses](https://github.com/TOTBWF/SteamCurses) - A Basic NCurses Client for Steam

[424]: http://coap.technology/

# Uncategorized #
* [tm][432] -  Timer and Timeline Utils for C. [``MIT``][MIT]
* [D-Bus][430] - Interprocess communications bus. [``AFL-2.1``][AFL-2.1] or [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [libgit2](https://libgit2.org/) - Pure C implementation of Git. [`GNU GPL2 only, with a linking exception`](https://github.com/libgit2/libgit2/blob/master/COPYING)
* [Keruspe/GPaste](https://github.com/Keruspe/GPaste) - Clipboard management system
* [Lajnold/falloc](https://github.com/Lajnold/falloc) - falloc creates files of a user-specified size. It uses the posix_fallocate syscall for allocating the right size directly, instead of copying data like the commonly used dd tool does (which, in my opinion, feels like a hack).

# Unsorted #
* [TerryC78/CMU_15213_DataLab](https://github.com/TerryC78/CMU_15213_DataLab) - CMU 15-213 Introduction to Computer Systems
* [Teyras/flowly](https://github.com/Teyras/flowly) - An sFlow data analyzer focused on realtime processing
* [TheAlgorithms/C](https://github.com/TheAlgorithms/C) - All Algorithms implemented in C
* [TheErk/CMake-tutorial](https://github.com/TheErk/CMake-tutorial) - CMake tutorial: beamer presentation and sample code
* [TheWeatherChannel/dClass](https://github.com/TheWeatherChannel/dClass) - Device Classification Engine
* [Themaister/libfmsynth](https://github.com/Themaister/libfmsynth) - A C library which implements an FM synthesizer
* [ThingPulse/esp8266-weather-station-color](https://github.com/ThingPulse/esp8266-weather-station-color) - ESP8266 Weather Station in Color using ILI9341 TFT 240x320 display
* [ThomasAdam/tmux-cvs-archived](https://github.com/ThomasAdam/tmux-cvs-archived) - Git version of tmux (updated hourly from sourceforge CVS) -- NOW ARCHIVED!  DO NOT USE THIS!
* [ThomasAdam/tmux](https://github.com/ThomasAdam/tmux) - Clone of the tmux Git repository.  The master branch contains the latest unreleased code. There are topic branches which may be subject to rebasing, so don't base changes off them.  DO NOT SEND me pull-requests, send patches to tmux-users mailing list instead.
* [ThomasHabets/monotonic_clock](https://github.com/ThomasHabets/monotonic_clock) - Portable C library for getting monotonic time
* [TimAimee/-android-source-code](https://github.com/TimAimee/-android-source-code) - 这是我自己在学习安卓期间，在网上积累下来的源码 ，欢迎交流学习，很多源码已经不能提供具体出处，对作者抱歉，如果有发现自己的代码可以发邮件给我，我会立刻标注上的。
* [TinyCC/tinycc](https://github.com/TinyCC/tinycc) - Mirror from mob branch
* [TouchCode/TouchXML](https://github.com/TouchCode/TouchXML) - Official "clone" of TouchXML from TouchCode
* [TravisWhitaker/FermiShell](https://github.com/TravisWhitaker/FermiShell) - Retrieve, compare, calculate, analyze, graph, simulate, and experiment with chemical data.
* [Tribler/self-compile-Android](https://github.com/Tribler/self-compile-Android) - Autonomous smartphone app. Capable of self-compilation, mutation, and viral spreading. World-first proof-of-principle to bypass Internet kill switches.
* [TulipCharts/tulipindicators](https://github.com/TulipCharts/tulipindicators) - Technical Analysis Indicator Function Library in C
* [UECIDE/UECIDE_data](https://github.com/UECIDE/UECIDE_data) - Cores, boards and compilers for UECIDE
* [UNINETT/mod_auth_mellon](https://github.com/UNINETT/mod_auth_mellon) - An Apache module with a simple SAML 2.0 service provider
* [UWNetworksLab/arrakis](https://github.com/UWNetworksLab/arrakis) - Arrakis public repository.
* [Uncodin/bypass](https://github.com/Uncodin/bypass) - Skip the HTML, Bypass takes markdown and renders it directly on Android and iOS.
* [Unidata/gempak](https://github.com/Unidata/gempak) - Analysis, display, and product generation package for meteorological data.
* [Unidata/netcdf-c](https://github.com/Unidata/netcdf-c) - Official GitHub repository for netCDF-C libraries and utilities.
* [UniversalPrimer/flv-analyzer](https://github.com/UniversalPrimer/flv-analyzer) - Loads an FLV file into sane C data structures and outputs fields as human readable
* [V-E-O/PoC](https://github.com/V-E-O/PoC) - PoC of CVE/Exploit
* [Vidvox/hap-qt-codec](https://github.com/Vidvox/hap-qt-codec) - A QuickTime codec for Hap video
* [Visgean/Zeus](https://github.com/Visgean/Zeus) - NOT MY CODE! Zeus trojan horse - leaked in 2011, I am not the author. I have created this repository to make the access for study as easy as possible.
* [Voluntarynet/Crypt](https://github.com/Voluntarynet/Crypt) - OSX app for drag and drop encryption
* [WeatherGod/BWx](https://github.com/WeatherGod/BWx) - Assorted utilities for dealing with weather related data
* [WhisperSystems/Signal-iOS](https://github.com/WhisperSystems/Signal-iOS) - Free, world-wide, private messaging and phone calls for iPhone.
* [WhisperSystems/curve25519-java](https://github.com/WhisperSystems/curve25519-java) - Pure Java and JNI backed Curve25519 implementation.
* [WhisperSystems/libsignal-protocol-c](https://github.com/WhisperSystems/libsignal-protocol-c) - Signal Protocol C Library
* [Whiteknight/ParrotStore](https://github.com/Whiteknight/ParrotStore) - Storage and data persistance for Parrot VM
* [WickrInc/wickr-crypto-c](https://github.com/WickrInc/wickr-crypto-c) - An implementation of the Wickr Secure Messaging Protocol in C
* [Wilfred/babyc](https://github.com/Wilfred/babyc) - A toy C compiler
* [Wind4/vlmcsd](https://github.com/Wind4/vlmcsd) - KMS Emulator in C (currently runs on Linux including Android, FreeBSD, Solaris, Minix, Mac OS, iOS, Windows with or without Cygwin)
* [WiringPi/WiringPi-Ruby-Legacy](https://github.com/WiringPi/WiringPi-Ruby-Legacy) - Ruby gem of the Arduino wiring-like C library WiringPi
* [WiringPi/WiringPi](https://github.com/WiringPi/WiringPi) - Gordon's Arduino wiring-like WiringPi Library for the Raspberry Pi
* [WizardMac/ReadStat](https://github.com/WizardMac/ReadStat) - Command-line tool (+ C library) for converting SAS, Stata, and SPSS files
* [WojciechMula/pyahocorasick](https://github.com/WojciechMula/pyahocorasick) - Python module (C extension and plain python) implementing Aho-Corasick algorithm
* [WoozleWrangler/ControlPad](https://github.com/WoozleWrangler/ControlPad) - iPhone Controller app for SNES (HD)
* [X0rg/CPU-X](https://github.com/X0rg/CPU-X) - CPU-X is a Free software that gathers information on CPU, motherboard and more.
* [XVilka/cparse](https://github.com/XVilka/cparse) - Parser of C-syntax data definitions, C-syntax function definitions
* [XadillaX/byakuren](https://github.com/XadillaX/byakuren) - 🎭 A theme color extracting library implemented by C.
* [XenonofArcticus/DynamicTrack](https://github.com/XenonofArcticus/DynamicTrack) - Access sources of dynamically-updated data about discrete entities like GPSes, INSes, ADS-B sources.
* [Xfennec/progress](https://github.com/Xfennec/progress) - Linux tool to show progress for cp, rm, dd, ...
* [Xsoda/struct](https://github.com/Xsoda/struct) - pack and unpack packet data like python struct module.
* [Y1ran/Free-VPN-for-Coursera](https://github.com/Y1ran/Free-VPN-for-Coursera) - :key: :unlock:免费开源的科学上网工具
* [Yalir/sfeMovie](https://github.com/Yalir/sfeMovie) - sfeMovie is a simple C++ library that lets you play movies in SFML based applications. It relies on FFmpeg to read medias and remains consistent with SFML's naming conventions. Forum at http://sfemovie.yalir.org/forum/
* [YaroslavLitvinov/Distributed-Sort](https://github.com/YaroslavLitvinov/Distributed-Sort) - Sort data in several processes simultaneously and using zeromq for interprocess communications.
* [Yubico/libu2f-host](https://github.com/Yubico/libu2f-host) - Yubico Universal 2nd Factor (U2F) Host C Library
* [Yubico/yubico-c-client](https://github.com/Yubico/yubico-c-client) - Yubico C client library
* [Yubico/yubico-pam](https://github.com/Yubico/yubico-pam) - Yubico Pluggable Authentication Module (PAM)
* [ZBar/ZBar](https://github.com/ZBar/ZBar) - Clone of the mercurial repository http://zbar.hg.sourceforge.net:8000/hgroot/zbar/zbar
* [ZECTBynmo/node-core-audio](https://github.com/ZECTBynmo/node-core-audio) - Bindings for PortAudio giving JavaScript access to sound card samples (mostly unmaintained)
* [ZSShen/C-Common-Data-Structures](https://github.com/ZSShen/C-Common-Data-Structures) - Uniform C APIs for data structure manipulation
* [Zeex/samp-plugin-crashdetect](https://github.com/Zeex/samp-plugin-crashdetect) - CrashDetect plugin for SA-MP server
* [Zeex/sampgdk](https://github.com/Zeex/sampgdk) - Writing SA-MP gamemodes in C/C++
* [Zeex/subhook](https://github.com/Zeex/subhook) - Simple hooking library for C/C++ (x86 only, 32/64-bit, no dependencies)
* [ZerBea/hcxtools](https://github.com/ZerBea/hcxtools) - Portable solution for capturing wlan traffic and conversion to hashcat formats (recommended by hashcat) and to John the Ripper formats. hcx: h = hash, c = capture, convert and calculate candidates, x = different hashtypes
* [ZhengYang/dc_fdw](https://github.com/ZhengYang/dc_fdw) - PostgreSQL - Document Collection Foreign-data Wrapper (works with 9.1 to 9.3)
* [ZhengYang/odbc_fdw](https://github.com/ZhengYang/odbc_fdw) - PostgreSQL Foreign-data Wrapper for ODBC
* [ZipArchive/ZipArchive](https://github.com/ZipArchive/ZipArchive) - ZipArchive is a simple utility class for zipping and unzipping files on iOS and Mac.
* [a-nikolaev/curseofwar](https://github.com/a-nikolaev/curseofwar) - A Real Time Strategy game for Linux.
* [a0rtega/pafish](https://github.com/a0rtega/pafish) - Pafish is a demonstration tool that employs several techniques to detect sandboxes and analysis environments in the same way as malware families do.
* [a3linux/nagios-amq-perf](https://github.com/a3linux/nagios-amq-perf) - Nagiso fork patched to support post performance data to ActiveMQ
* [a4tunado/mll](https://github.com/a4tunado/mll) - Library used for studying machine learning course at Yandex Data Analysis School.
* [aardappel/lobster](https://github.com/aardappel/lobster) - The Lobster Programming Language
* [aaronstanton/sualft](https://github.com/aaronstanton/sualft) - reconstruction of irregularly sampled seismic data using the Anti-Leakage Fourier Transform (ALFT)
* [abael/amysql](https://github.com/abael/amysql) - High performance( 2.5 times to MySQLDb ) Python  Mysql Driver,   using Python native socket layer.  pure C implemented.
* [abiggerhammer/hammer](https://github.com/abiggerhammer/hammer) - Parser combinators for binary formats, in C. Yes, in C. What? Don't look at me like that.
* [abishekvashok/cmatrix](https://github.com/abishekvashok/cmatrix) - Terminal based "The Matrix" like implementation
* [abrasive/shairport](https://github.com/abrasive/shairport) - Airtunes emulator! Shairport is no longer maintained.
* [abstrakraft/cwiid](https://github.com/abstrakraft/cwiid) - Linux Nintendo Wiimote interface
* [acassen/keepalived](https://github.com/acassen/keepalived) - Keepalived
* [acg/lwpb](https://github.com/acg/lwpb) - Lightweight Protocol Buffers for C and Python
* [acl-dev/acl](https://github.com/acl-dev/acl) - One advanced C/C++ library for Linux, Mac, FreeBSD, Solaris(x86), Windows, Android, IOS
* [acmeism/RosettaCodeData](https://github.com/acmeism/RosettaCodeData) - RosettaCode Data Project
* [acrisci/playerctl](https://github.com/acrisci/playerctl) - 🎧 mpris command-line controller and library for spotify, vlc, audacious, bmp, cmus, and others.
* [adafruit/adafruit-beaglebone-io-python](https://github.com/adafruit/adafruit-beaglebone-io-python) - Adafruit's BeagleBone IO Python Library
* [adamcaudill/ccsrch](https://github.com/adamcaudill/ccsrch) - Cross-platform credit card (PAN) search tool for security assessments
* [addy689/DataStructuresLab](https://github.com/addy689/DataStructuresLab) - Graph Traversal (BFS & DFS), Single Source Shortest Path, Minimum Spanning Tree, RB Trees, B-Trees
* [adenine/ofxFFT_to_OSC](https://github.com/adenine/ofxFFT_to_OSC) - This is an app which uses ofxFFT to then send out OSC data relating to the music being interpreted.
* [adnanozsoy/CUDA_Compression](https://github.com/adnanozsoy/CUDA_Compression) - A GPU-based LZSS compression algorithm, highly tuned for NVIDIA GPGPUs and for streaming data, leveraging the respective strengths of CPUs and GPUs together.
* [adob/print-stmt](https://github.com/adob/print-stmt) - Convenient print statement for C++
* [adobe-flash/crossbridge](https://github.com/adobe-flash/crossbridge) - Welcome to visit the homepage!
* [adobkin/libcapn](https://github.com/adobkin/libcapn) - A simple C Library for interact with the Apple Push Notification Service (APNs)
* [adoxa/ansicon](https://github.com/adoxa/ansicon) - Process ANSI escape sequences for Windows console programs.
* [adrianlopezroche/fdupes](https://github.com/adrianlopezroche/fdupes) - FDUPES is a program for identifying or deleting duplicate files residing within specified directories.
* [adsr/mle](https://github.com/adsr/mle) - flexible terminal-based text editor (C)
* [adtac/fssb](https://github.com/adtac/fssb) - A filesystem sandbox for Linux using syscall intercepts.
* [aerospike/aerospike-client-c](https://github.com/aerospike/aerospike-client-c) - Aerospike C Client
* [aerospike/aerospike-server](https://github.com/aerospike/aerospike-server) - Aerospike Database Server – flash-optimized, in-memory, nosql database
* [agentzh/chunkin-nginx-module](https://github.com/agentzh/chunkin-nginx-module) - HTTP 1.1 chunked-encoding request body support for Nginx
* [aggregateknowledge/postgresql-hll](https://github.com/aggregateknowledge/postgresql-hll) - PostgreSQL extension adding HyperLogLog data structures as a native data type
* [agl/critbit](https://github.com/agl/critbit) - Critbit trees in C
* [agl/ctgrind](https://github.com/agl/ctgrind) - Checking that functions are constant time with Valgrind
* [agl/curve25519-donna](https://github.com/agl/curve25519-donna) - Implementations of a fast Elliptic-curve Diffie-Hellman primitive
* [agordon/datamash](https://github.com/agordon/datamash) - mirror of GNU Datamash
* [aharren/LibComponentLogging-Core](https://github.com/aharren/LibComponentLogging-Core) - A small logging library for Objective-C applications (Mac OS X and iPhone OS/iOS) which provides conditional logging based on log levels and log components. Additionally, different logging strategies can be used, e.g. writing log messages to a file or sending them to the system log, while using the same logging interface.
* [ai-ku/scode](https://github.com/ai-ku/scode) - Sphere embedding (s-code) is a variation of Euclidean embedding of co-occurence data (code).
* [aidansteele/MagicKit](https://github.com/aidansteele/MagicKit) - MagicKit is an Objective-C file identification framework based on libmagic.
* [aidenbell/getdents](https://github.com/aidenbell/getdents) - Simple tool for listing large (millions) numbers of files on Linux systems without causing memory issues. Useful for shell scripting large data stores.
* [aimxhaisse/des](https://github.com/aimxhaisse/des) - C implementation of Data Encryption Standard
* [ajrisi/fsm](https://github.com/ajrisi/fsm) - A finite state machine engine in C - used as a parser for complex data structures
* [akheron/jansson](https://github.com/akheron/jansson) - C library for encoding, decoding and manipulating JSON data
* [akissa/php-couchdb](https://github.com/akissa/php-couchdb) - PHP extension for CouchDB
* [akitaonrails/ObjC_Rubyfication](https://github.com/akitaonrails/ObjC_Rubyfication) - Attempt to make Objective-C more like Ruby
* [alandekok/recli](https://github.com/alandekok/recli) - A re-imagined CLI.  Customizable syntax, help, permissions, data types.
* [alanwoolley/CorsixTH-Android](https://github.com/alanwoolley/CorsixTH-Android) - Port of CorsixTH to Android
* [alawrence/c_LibExifModule](https://github.com/alawrence/c_LibExifModule) - C++ framework module that wraps libexif to pull out EXIF data.
* [alessandrofrancesconi/gimp-plugin-bimp](https://github.com/alessandrofrancesconi/gimp-plugin-bimp) - BIMP. Batch Image Manipulation Plugin for GIMP.
* [alessio9008/PLC-to-STM32F4-communication-through-PC-as-gateway](https://github.com/alessio9008/PLC-to-STM32F4-communication-through-PC-as-gateway) - This project has been made using the STM32F4 accelerometer and a Siemens S7-300 unit. The microcontroller is programmed to send data to a PC by using a serial-port communication; these data are read from a C# program that forward them to the PLC memory. Then, the PLC unit, that recognizes the microcontroller position, moves a mechanical arm.
* [alessio9008/Thingsquare-Contiki-O.S-Porting-STM32F4-Discovery](https://github.com/alessio9008/Thingsquare-Contiki-O.S-Porting-STM32F4-Discovery) - We have ported the Contiki Operating System to STM32F4 platform (http://www.st.com/stm32f4-discovery). We started with the work that was already done on an evaluation board based on STM32L1 platform (STEVAL-IKR001V1, http://www.st.com/web/en/catalog/tools/PF253893). The original project, called "Mist", was created by Thingsquare using Spirit1 radio transceiver (STEVAL-IKR001V8D, http://www.st.com/web/en/catalog/tools/FM116/SC1075/PF258319). We converted the system calls from the original platform to the target platform. We have adapted Spirit1 radio driver in order to work properly on STM32F4. Then, we created a Wireless Sensor Network and collected several communication and performance data.  I worked on it with Daniele Saitta.  To manage the entire work, we used IAR Embedded Workbench (http://www.iar.com/en/products/iar-embedded-workbench/arm/).
* [alexanderb14/cCollections](https://github.com/alexanderb14/cCollections) - lightweight dynamic data structures for C
* [alexanderchuranov/Metaresc](https://github.com/alexanderchuranov/Metaresc) - META data and RESource library for  C language
* [alexbirkett/GPSBabel](https://github.com/alexbirkett/GPSBabel) - Free software for GPS data conversion and transfer
* [alexbw/Netflix-Prize](https://github.com/alexbw/Netflix-Prize) - The code I used to get in the top #150 in the Netflix Prize
* [alexfru/SmallerC](https://github.com/alexfru/SmallerC) - Simple C compiler
* [algernon/libmongo-client](https://github.com/algernon/libmongo-client) - An obsolete library. Don't use it in new projects.
* [ali-rantakari/peg-markdown-highlight](https://github.com/ali-rantakari/peg-markdown-highlight) - C library for Markdown syntax highlighting, using a recursive-descent parser.
* [alibaba/ApsaraCache](https://github.com/alibaba/ApsaraCache) - ApsaraCache is a Redis branch originated from Alibaba Group.
* [alibaba/LVS](https://github.com/alibaba/LVS) - A distribution of Linux Virtual Server with some advanced features. It introduces a new packet forwarding method - FULLNAT other than NAT/Tunneling/DirectRouting, and defense mechanism against synflooding attack - SYNPROXY.
* [alibaba/nginx-http-concat](https://github.com/alibaba/nginx-http-concat) - A Nginx module for concatenating files in a given context: CSS and JS files usually
* [alibaba/tengine](https://github.com/alibaba/tengine) - A distribution of Nginx with some advanced features
* [alibaba/tsar2db](https://github.com/alibaba/tsar2db) - used to store tsar data to mysql
* [alibaba/tsar](https://github.com/alibaba/tsar) - Taobao System Activity Reporter
* [alibashir/pacmonstr](https://github.com/alibashir/pacmonstr) - Tandem Repeat Detection for Long Read Sequence Data
* [allinurl/goaccess](https://github.com/allinurl/goaccess) - GoAccess is a real-time web log analyzer and interactive viewer that runs in a terminal in *nix systems or through your browser.
* [allinurl/gwsocket](https://github.com/allinurl/gwsocket) - fast, standalone, language-agnostic WebSocket server RFC6455 compliant
* [alols/xcape](https://github.com/alols/xcape) - Linux utility to configure modifier keys to act as other keys when pressed and released on their own.
* [alonbl/pkcs11-data](https://github.com/alonbl/pkcs11-data) - PKCS#11 data object manipulator
* [alonho/pytrace](https://github.com/alonho/pytrace) - pytrace is a fast python tracer. it records function calls, arguments and return values. can be used for debugging and profiling.
* [amadvance/snapraid](https://github.com/amadvance/snapraid) - A backup program for disk arrays. It stores parity information of your data and it recovers from up to six disk failures
* [amahule/CoolReader](https://github.com/amahule/CoolReader) - An Android based open e-book reader
* [amaurigabriel/CAD](https://github.com/amaurigabriel/CAD) -  C Algorithms and Data-structures
* [amd/Chromium-WebCL](https://github.com/amd/Chromium-WebCL) - WebCL implementation for Chromium
* [aminroosta/sqlite_modern_cpp](https://github.com/aminroosta/sqlite_modern_cpp) - The C++14 wrapper around sqlite library
* [amitdev/lru-dict](https://github.com/amitdev/lru-dict) - A C extension of a python dict-like LRU container.
* [anael-seghezzi/CToy](https://github.com/anael-seghezzi/CToy) - Interactive C coding environment
* [anatoo/cons](https://github.com/anatoo/cons) - This PHP Extension import cons cell data structure from scheme.
* [andikleen/snappy-c](https://github.com/andikleen/snappy-c) - C port of the snappy compressor
* [andlabs/libui](https://github.com/andlabs/libui) - Simple and portable (but not inflexible) GUI library in C that uses the native GUI technologies of each platform it supports.
* [andreafabrizi/prism](https://github.com/andreafabrizi/prism) - PRISM is an user space stealth reverse shell backdoor, written in pure C.
* [andrewchambers/c](https://github.com/andrewchambers/c) - small self hosting C compiler
* [andrewrk/libsoundio](https://github.com/andrewrk/libsoundio) - C library for cross-platform real-time audio input and output
* [andrewstone/AbqData](https://github.com/andrewstone/AbqData) - Tools to read ABQ Open Data Initiative city gov data
* [ands/lightmapper](https://github.com/ands/lightmapper) - A C/C++ single-file library for drop-in lightmap baking. Just use your existing OpenGL renderer to bounce light!
* [ands/seamoptimizer](https://github.com/ands/seamoptimizer) - A C/C++ single-file library that minimizes the hard transition errors of disjoint edges in lightmaps.
* [andwn/cave-story-md](https://github.com/andwn/cave-story-md) - A fan port of Cave Story for the Sega Mega Drive
* [andygock/avr-uart](https://github.com/andygock/avr-uart) - AVR UART C Library
* [andymcd/cmd-key-happy](https://github.com/andymcd/cmd-key-happy) - Swap cmd and alt keys in Terminal
* [andysworkshop/stm32plus](https://github.com/andysworkshop/stm32plus) - The C++ library for the STM32 F0, F100, F103, F107 and F4 microcontrollers
* [angband/angband](https://github.com/angband/angband) - A free, single-player roguelike dungeon exploration game
* [angel2d/angel2d](https://github.com/angel2d/angel2d) - A cross-platform 2D game prototyping framework based on OpenGL and C++
* [angelortega/mpdm](https://github.com/angelortega/mpdm) - Minimum Profit Data Manager
* [anjos/arithmetic_coding](https://github.com/anjos/arithmetic_coding) - Library to perform arithmetic coding and decoding of text or binary data
* [anoek/android-cairo](https://github.com/anoek/android-cairo) - Android NDK build files to build libcairo
* [anoek/ex-sdl-cairo-freetype-harfbuzz](https://github.com/anoek/ex-sdl-cairo-freetype-harfbuzz) - Example code which uses SDL, cairo, freetype, and harfbuzz to do ttf/otf text layout and rendering
* [anrieff/libcpuid](https://github.com/anrieff/libcpuid) - a small C library for x86 CPU detection and feature extraction
* [ansiboy/ChiTuStore](https://github.com/ansiboy/ChiTuStore) - 开源的电商前端混合 APP
* [ansilove/AnsiLove-C](https://github.com/ansilove/AnsiLove-C) - ANSi / ASCII art to PNG converter in C
* [ansilove/ansilove](https://github.com/ansilove/ansilove) - ANSi / ASCII art to PNG converter in C
* [answer-huang/dSYMTools](https://github.com/answer-huang/dSYMTools) - dSYM analyze
* [ant-media/LibRtmp-Client-for-Android](https://github.com/ant-media/LibRtmp-Client-for-Android) - It is probably the smallest(~60KB, fat version ~300KB) rtmp client for android. It calls librtmp functions over JNI interface
* [ant-streaming/LibRtmp-Client-for-Android](https://github.com/ant-streaming/LibRtmp-Client-for-Android) - It is probably the smallest(~60KB) rtmp client for android. It calls librtmp functions over JNI interface
* [antelopeusersgroup/antelope_contrib](https://github.com/antelopeusersgroup/antelope_contrib) - Contributed code for the Antelope Environmental Monitoring System from BRTT, Inc. (http://www.brtt.com)
* [antirez/disque](https://github.com/antirez/disque) - Disque is a distributed message broker
* [antirez/dump1090](https://github.com/antirez/dump1090) - Dump1090 is a simple Mode S decoder for RTLSDR devices
* [antirez/linenoise](https://github.com/antirez/linenoise) - A small self-contained alternative to readline and libedit
* [antirez/load81](https://github.com/antirez/load81) - SDL based Lua programming environment for kids similar to Codea
* [antirez/lua-cmsgpack](https://github.com/antirez/lua-cmsgpack) - A self contained Lua MessagePack C implementation.
* [antirez/rax](https://github.com/antirez/rax) - A radix tree implementation in ANSI C
* [antirez/redis](https://github.com/antirez/redis) - Redis is an in-memory database that persists on disk. The data model is key-value, but many different kind of values are supported: Strings, Lists, Sets, Sorted Sets, Hashes, HyperLogLogs, Bitmaps.
* [antirez/sds](https://github.com/antirez/sds) - Simple Dynamic Strings library for C
* [antirez/shapeme](https://github.com/antirez/shapeme) - Evolve images using simulated annealing
* [antirez/smaz](https://github.com/antirez/smaz) - Small strings compression library
* [anza/metar](https://github.com/anza/metar) - METAR data fetcher and parser
* [apache/httpd](https://github.com/apache/httpd) - Mirror of Apache HTTP Server
* [apache/incubator-mynewt-core](https://github.com/apache/incubator-mynewt-core) - Mirror of Apache MyNewt Core (Incubating)
* [apache/mynewt-core](https://github.com/apache/mynewt-core) - An OS to build, deploy and securely manage billions of devices
* [aperezdc/ngx-fancyindex](https://github.com/aperezdc/ngx-fancyindex) - Fancy indexes module for the Nginx web server
* [apple/cups](https://github.com/apple/cups) - Official CUPS Sources
* [apple/swift-corelibs-foundation](https://github.com/apple/swift-corelibs-foundation) - The Foundation Project, providing core utilities, internationalization, and OS independence
* [apple/swift-corelibs-libdispatch](https://github.com/apple/swift-corelibs-libdispatch) - The libdispatch Project, (a.k.a. Grand Central Dispatch), for concurrency on multicore hardware
* [applidium/ADZipURLProtocol](https://github.com/applidium/ADZipURLProtocol) - Open static website or access data from a zip archive
* [applidium/Vim](https://github.com/applidium/Vim) - Port of the Vim text editor to the iOS
* [appneta/tcpreplay](https://github.com/appneta/tcpreplay) - Pcap editing and replay tools for *NIX and Windows - Users please download source from
* [appunite/AndroidFFmpeg](https://github.com/appunite/AndroidFFmpeg) - FFmpeg build for android random architectures with example jni
* [aquynh/capstone](https://github.com/aquynh/capstone) - Capstone disassembly/disassembler framework: Core (Arm, Arm64, BPF, EVM, M68K, M680X, MOS65xx, Mips, PPC, Sparc, SystemZ, TMS320C64x, Web Assembly, X86, X86_64, XCore) + bindings.
* [arachsys/containers](https://github.com/arachsys/containers) - Lightweight containers using Linux user namespaces
* [ardagnir/athame](https://github.com/ardagnir/athame) - Full vim for readline (bash, gdb, python, etc)
* [argv0/nbds](https://github.com/argv0/nbds) - C implementations of several scalable non-blocking data structures for x86 and x86-64.
* [arjun024/hide-data-in-ptr](https://github.com/arjun024/hide-data-in-ptr) - how to hide data inside pointers
* [arjun024/mkernel](https://github.com/arjun024/mkernel) - a minimalistic kernel
* [armbrustlab/SEAStAR](https://github.com/armbrustlab/SEAStAR) - SEAStAR is a package of tools supporting the construction of complete analysis pipelines for next-generation (Illumina®, SOLiD™) sequencing data generated from environmental samples.
* [armink/CmBacktrace](https://github.com/armink/CmBacktrace) - Advanced fault backtrace library for ARM Cortex-M series MCU | ARM Cortex-M 系列 MCU 错误追踪库
* [armink/EasyDataManager](https://github.com/armink/EasyDataManager) - A c language advanced framework of data manager. Support static data and dynamic data. Supply easy and simple interface for app.
* [armink/EasyLogger](https://github.com/armink/EasyLogger) - A ultra-lightweight(ROM<1.6K, RAM<0.3k), high-performance C/C++ log library. | 一款超轻量级(ROM<1.6K, RAM<0.3k)、高性能的 C/C++ 日志库
* [armink/struct2json](https://github.com/armink/struct2json) - A fast convert library between the JSON and C structure. Implement structure serialization and deserialization for C. | C 结构体与 JSON 快速互转库，快速实现 C 结构体的序列化及反序列化
* [armon/bloomd](https://github.com/armon/bloomd) - C network daemon for bloom filters
* [armon/hlld](https://github.com/armon/hlld) - C network daemon for HyperLogLogs
* [armon/libart](https://github.com/armon/libart) - Adaptive Radix Trees implemented in C
* [armon/statsite](https://github.com/armon/statsite) - C implementation of statsd
* [arnaudbrejeon/cspec](https://github.com/arnaudbrejeon/cspec) - Behavior driven development in C
* [arnimarj/py-pointless](https://github.com/arnimarj/py-pointless) - A fast and efficient read-only relocatable data structure for JSON like data, with C and Python APIs
* [arrbee/diff-match-patch-c](https://github.com/arrbee/diff-match-patch-c) - C language port of google-diff-match-patch library
* [arut/nginx-rtmp-module](https://github.com/arut/nginx-rtmp-module) - NGINX-based Media Streaming Server
* [as0ler/iphone-dataprotection](https://github.com/as0ler/iphone-dataprotection) - Some useful tools for a iOS Forensics.
* [asadzia/Algorithms-and-Data-Structures](https://github.com/asadzia/Algorithms-and-Data-Structures) - A list of implementations of various algorithms and data structures.
* [asamy/ksm](https://github.com/asamy/ksm) - A really simple and lightweight x64 hypervisor written in C.  Supports VMFUNC, EPTP switching, #VE EPT Violation, VT-x nesting and IDT shadowing.  VMFUNC backward compatibility also supported.
* [asanchez1987/jobcomp-elasticsearch](https://github.com/asanchez1987/jobcomp-elasticsearch) - SLURM jobcomp plugin to index data into an elasticsearch server
* [aseveryn/NLPIR-2013](https://github.com/aseveryn/NLPIR-2013) - Source code and data used in the NLPIR course (Sprint, 2013)
* [ashima/webgl-noise](https://github.com/ashima/webgl-noise) - Procedural Noise Shader Routines compatible with WebGL
* [ashinkarov/trie](https://github.com/ashinkarov/trie) - Simple implementation of trie data structure in C
* [ashwinraghav/Parallel_Open_SSL](https://github.com/ashwinraghav/Parallel_Open_SSL) - Use your idle GPU to encrypt your data. Give your CPU some breathing time!
* [aspotton/xonotic-data-patches](https://github.com/aspotton/xonotic-data-patches) - A clone of xonotic-data plus additional branches
* [asterisk/asterisk](https://github.com/asterisk/asterisk) -  Mirror of the official Asterisk(https://www.asterisk.org) Project repository No pull requests here please.  Use Gerrit:
* [astro/collectd](https://github.com/astro/collectd) - Some personal modifications to collectd, the kick-ass data collector
* [asynclabs/WiShield_user_contrib](https://github.com/asynclabs/WiShield_user_contrib) - WiShield library with user contributed features
* [atduskgreg/Head-Puppet](https://github.com/atduskgreg/Head-Puppet) - Open Frameworks app for distorting a 3D model of my head based on Kinect skeleton tracking data over OSC
* [atduskgreg/Leg-Visualization](https://github.com/atduskgreg/Leg-Visualization) - OF app to visualize leg movement data from Biomechanics and Motor Control of Human Movement by David A. Winter
* [aterrien/forp-PHP-profiler](https://github.com/aterrien/forp-PHP-profiler) - A PHP profiler written in C. forp is a lightweight PHP extension which provides the full call stack of your script, with CPU and memory usage, in a plain PHP Array or JSON output.
* [atg/chocolat-public](https://github.com/atg/chocolat-public) - Public bug tracker for the private chocolat project
* [atgreen/libffi](https://github.com/atgreen/libffi) - A portable foreign-function interface library.
* [atheme/atheme](https://github.com/atheme/atheme) - Atheme IRC Services
* [atheme/charybdis](https://github.com/atheme/charybdis) - an extremely scalable ircd with some cooperation with the ratbox and ircu guys
* [atks/vt](https://github.com/atks/vt) - A tool set for short variant discovery in genetic sequence data.
* [atmatthewat/mdc-encode-decode](https://github.com/atmatthewat/mdc-encode-decode) - Software modem for a specific data burst format
* [atomicobject/heatshrink](https://github.com/atomicobject/heatshrink) - data compression library for embedded/real-time systems
* [atris/JDBC_FDW](https://github.com/atris/JDBC_FDW) - FDW that wraps JDBC for PostgreSQL.It can be used to connect and fetch data from any data source that supports JDBC
* [attractivechaos/kann](https://github.com/attractivechaos/kann) - A lightweight C library for artificial neural networks
* [attractivechaos/klib](https://github.com/attractivechaos/klib) - A standalone and lightweight C library
* [aubio/aubio](https://github.com/aubio/aubio) - a library for audio and music analysis
* [audiohacked/OpenCorsairLink](https://github.com/audiohacked/OpenCorsairLink) - Linux and Mac OS support for the CorsairLink Devices
* [augustl/halt](https://github.com/augustl/halt) - OS where everything is immutable! (Experimental)
* [aurelian/ruby-stemmer](https://github.com/aurelian/ruby-stemmer) - Expose libstemmer_c to Ruby
* [autosportlabs/RaceCapture-Pro_firmware](https://github.com/autosportlabs/RaceCapture-Pro_firmware) - Firmware for RaceCapture-Pro Data Acquisition, control and Telemetry system for motorsports
* [avilleret/laser_drawer](https://github.com/avilleret/laser_drawer) - laser_driver is a pure-data patch to control a Laser projector with a sound card
* [awesomeWM/awesome](https://github.com/awesomeWM/awesome) - awesome window manager
* [aws/amazon-cognito-identity-js](https://github.com/aws/amazon-cognito-identity-js) - Amazon Cognito Identity SDK for JavaScript
* [aws/aws-iot-device-sdk-embedded-C](https://github.com/aws/aws-iot-device-sdk-embedded-C) - SDK for connecting to AWS IoT from a device using embedded C.
* [awslabs/s2n](https://github.com/awslabs/s2n) - s2n : an implementation of the TLS/SSL protocols
* [axiak/pybloomfiltermmap](https://github.com/axiak/pybloomfiltermmap) - Fast Python Bloom Filter using Mmap
* [axoltl/HubCap](https://github.com/axoltl/HubCap) - ChromeCast HubCap exploit
* [b-k/21st-Century-Examples](https://github.com/b-k/21st-Century-Examples) - Examples for _21st Century C_ by Ben Klemens
* [b-k/apophenia](https://github.com/b-k/apophenia) - A C library for statistical and scientific computing
* [b4n/ctags](https://github.com/b4n/ctags) - Git mirror of Exuberant CTags SVN (http://ctags.sourceforge.net/), with additional feature branches
* [b4winckler/macvim](https://github.com/b4winckler/macvim) - Vim - the text editor - for Mac OS X
* [b4winckler/vim](https://github.com/b4winckler/vim) - Mirror of the Vim Mercurial repository
* [babelouest/ulfius](https://github.com/babelouest/ulfius) - Web Framework to build REST APIs, Webservices or any HTTP endpoint in C language. Can stream large amount of data, integrate JSON data with Jansson, and create websocket services
* [bagder/c-ares](https://github.com/bagder/c-ares) - c-ares is a C library for asynchronous DNS requests
* [bagder/curl](https://github.com/bagder/curl) - Curl is a tool and libcurl is a library for transferring data with URL syntax, supporting FTP, FTPS, HTTP, HTTPS, GOPHER, TFTP, SCP, SFTP, TELNET, DICT, LDAP, LDAPS, FILE, IMAP, SMTP, POP3, RTSP and RTMP. libcurl offers a myriad of powerful features
* [bagder/spindly](https://github.com/bagder/spindly) - a portable C library for SPDY transport (DEAD project!)
* [bahbka/pebble-my-data](https://github.com/bahbka/pebble-my-data) - Pebble watches application to show only your own data, prepared on your own server.
* [baiduwearable/duband](https://github.com/baiduwearable/duband) - duband1.0 对应的公版版本为 1.0
* [baina/biyifei](https://github.com/baina/biyifei) - The general flight data cloud acceleration system design
* [baiwei0427/PIAS](https://github.com/baiwei0427/PIAS) - Information-Agnostic Flow Scheduling for Commodity Data Centers
* [baiwei0427/XPath](https://github.com/baiwei0427/XPath) - Explicit Path Control in Commodity Data Centers
* [balabit/syslog-ng](https://github.com/balabit/syslog-ng) - syslog-ng is an enhanced log daemon, supporting a wide range of input and output methods: syslog, unstructured text, queueing, SQL & NoSQL.
* [balde/balde](https://github.com/balde/balde) - A microframework for C based on GLib and bad intentions.
* [bananita/MBFaker](https://github.com/bananita/MBFaker) - Objective-C fake data generator
* [bang590/JSPatch](https://github.com/bang590/JSPatch) - JSPatch bridge Objective-C and Javascript using the Objective-C runtime. You can call any Objective-C class and method in JavaScript by just including a small engine. JSPatch is generally used to hotfix iOS App.
* [banister/binding_of_caller](https://github.com/banister/binding_of_caller) - Retrieve the binding of a method's caller in MRI 1.9.2+
* [barankurtulusozan/Algorithms-and-Data-Structures](https://github.com/barankurtulusozan/Algorithms-and-Data-Structures) - Introduction To Algorithms and Data Structures
* [bartobri/bmenu](https://github.com/bartobri/bmenu) - A generic terminal menu written in C.
* [baruch/libwire](https://github.com/baruch/libwire) - User space threading (aka coroutines) library for C resembling GoLang and goroutines
* [baskerville/bspwm](https://github.com/baskerville/bspwm) - A tiling window manager based on binary space partitioning
* [baskerville/sxhkd](https://github.com/baskerville/sxhkd) - Simple X hotkey daemon
* [bauerca/gridfloat](https://github.com/bauerca/gridfloat) - Slice and dice USGS elevation data from the command line.
* [baupetit/VisuScaterredData](https://github.com/baupetit/VisuScaterredData) - projet de visualisation
* [bbu/simple-interpreter](https://github.com/bbu/simple-interpreter) - A hackable and extensible lexer, parser and interpreter for a minimalistic, imperative, C-like language.
* [bcmpinc/dagdb](https://github.com/bcmpinc/dagdb) - small database for storing semi-structured data
* [bcopeland/em_misc](https://github.com/bcopeland/em_misc) - external memory data structure playground
* [beaups/SamsungCID](https://github.com/beaups/SamsungCID) - Change the CID in Samsung eMMC
* [beave/barnyard2-extra](https://github.com/beave/barnyard2-extra) - Barnyard2 with "Extra Data" support and other enhancements.
* [beave/nfdump-1.6.10p1-sagan](https://github.com/beave/nfdump-1.6.10p1-sagan) - Modified version of Nfdump which allows Sagan to analyze netflow data in real time
* [bedops/bedops](https://github.com/bedops/bedops) - :microscope: BEDOPS: high-performance genomic feature operations
* [begeekmyfriend/CuckooFilter](https://github.com/begeekmyfriend/CuckooFilter) - Substitute for bloom filter.
* [begeekmyfriend/bplustree](https://github.com/begeekmyfriend/bplustree) - A minimal but extreme fast B+ tree indexing structure demo for billions of key-value storage
* [begeekmyfriend/leetcode](https://github.com/begeekmyfriend/leetcode) - LeetCode in pure C
* [belangeo/pyo](https://github.com/belangeo/pyo) - Python DSP module - ajaxsoundstudio.com
* [bellbind/node-v4l2camera](https://github.com/bellbind/node-v4l2camera) - node module for capturing an image from USB(UVC) webcam on linux.
* [benblazak/ergodox-firmware](https://github.com/benblazak/ergodox-firmware) - firmware for the ergoDOX keyboard
* [bendmorris/pybioclim](https://github.com/bendmorris/pybioclim) - A Python interface to BIOCLIM climate data. Data files included in package.
* [benhoyt/inih](https://github.com/benhoyt/inih) - Simple .INI file parser in C, good for embedded systems
* [benhoyt/scandir](https://github.com/benhoyt/scandir) - Better directory iterator and faster os.walk(), now in the Python 3.5 stdlib
* [benmills/robotskirt](https://github.com/benmills/robotskirt) - A node wrapper for the awesome C markdown parser, sundown.
* [benoitc/http-parser](https://github.com/benoitc/http-parser) - HTTP request/response parser for python in C
* [beoran/chipmunk](https://github.com/beoran/chipmunk) - Bindings to Chipmunk 5.3.4 with extra features for use with Ruby 1.8.x and 1.9.x. Version 5.4.3.4 released on rubygems. Just a gem install chipmunk should work, even on windows! -- Developers wanted to take over this project!!!
* [bettio/AtomVM](https://github.com/bettio/AtomVM) - Tiny Erlang VM
* [bfulgham/WinCairoRequirements](https://github.com/bfulgham/WinCairoRequirements) - Source archive of the build requirements for the WinCairo port of WebKit
* [bg111/asterisk-chan-dongle](https://github.com/bg111/asterisk-chan-dongle) - Automatically exported from code.google.com/p/asterisk-chan-dongle
* [bgamari/data-logger](https://github.com/bgamari/data-logger) - An autonomous data logging firmware for the MC HCK development board
* [bianster/mysqlfs](https://github.com/bianster/mysqlfs) - MySQLfs is Linux userspace filesystem which stores data in a MySQL database. It uses FUSE to interface with the kernel.
* [bigclean/structure](https://github.com/bigclean/structure) - Several languages of data structure practice
* [billhsu/cashew](https://github.com/billhsu/cashew) - Freestyle 3D sketching app.
* [billiob/terminology](https://github.com/billiob/terminology) - The best terminal emulator based on the Enlightenment Foundation Libraries
* [billvb/cfe](https://github.com/billvb/cfe) - This framework is used as the basis for the flight software for satellite data systems and instruments, but can be used on other embedded systems.
* [binaryage/asepsis](https://github.com/binaryage/asepsis) - a solution for .DS_Store pollution
* [binchewer/power_fixer](https://github.com/binchewer/power_fixer) - OSX command line utility that attempts to restore pre-Mavericks power button behavior. Written in C.
* [bindecy/HugeDirtyCowPOC](https://github.com/bindecy/HugeDirtyCowPOC) - A POC for the Huge Dirty Cow vulnerability (CVE-2017-1000405)
* [bingmann/disk-filltest](https://github.com/bingmann/disk-filltest) - Simple program to detect bad disks by filling them with random data.
* [biomood/LuaSerial](https://github.com/biomood/LuaSerial) - A Lua library in C for sending/receving data from Arduino
* [bitcoin-core/secp256k1](https://github.com/bitcoin-core/secp256k1) - Optimized C library for EC operations on curve secp256k1
* [bitcoin/secp256k1](https://github.com/bitcoin/secp256k1) - Optimized C library for EC operations on curve secp256k1
* [bitcraze/crazyflie-firmware](https://github.com/bitcraze/crazyflie-firmware) - The main firmware for the Crazyflie Nano Quadcopter.
* [bither/bither-android-lib](https://github.com/bither/bither-android-lib) - Bither Android Library
* [bitlbee/bitlbee-facebook](https://github.com/bitlbee/bitlbee-facebook) - Facebook protocol plugin for BitlBee
* [bitlbee/bitlbee-steam](https://github.com/bitlbee/bitlbee-steam) - Steam protocol plugin for BitlBee
* [bitlbee/bitlbee](https://github.com/bitlbee/bitlbee) - An IRC to other chat networks gateway :bee:
* [bitly/dablooms](https://github.com/bitly/dablooms) - scaling, counting, bloom filter library
* [bitly/simplehttp](https://github.com/bitly/simplehttp) - a family of libraries and daemons for building scalable web infrastructure
* [bitrig/bitrig](https://github.com/bitrig/bitrig) - Bitrig base system repository.
* [bjoernknafla/amp](https://github.com/bjoernknafla/amp) - C portable low-level assemblies for parallelism and threading
* [bjoernknafla/peak](https://github.com/bjoernknafla/peak) - Parallelism exploration assembly kit. C toolkit to experiment with task- and data-parallelism.
* [bkrpub/EngineRoom](https://github.com/bkrpub/EngineRoom) - EngineRoom is a toolkit addressing basic, recurring needs when using C based languages.  The most prominent (and mature) component is LogPoints,  a logging facility designed to provide comfort to developers working on applications of all sizes. EngineRoom is primarily targeted at Objective-C developers on Mac OS X and iOS with some support for C on GNU/Linux and Solaris.
* [bl0b/tinyap](https://github.com/bl0b/tinyap) - One build to parse them all. A GLR-like parsing engine where the grammar is actually data. And you can augment the grammar at runtime. Also provides a framework to walk the resulting ASTs. C API and commandline frontend available.
* [bl0ckeduser/new-bpf-tools](https://github.com/bl0ckeduser/new-bpf-tools) - subset-of-C compiler targeting 32-bit x86
* [blacksmithlabs/NetworkRecorder](https://github.com/blacksmithlabs/NetworkRecorder) - An app to record targeted network traffic data of other apps using iptables.
* [blankwall/MacDBG](https://github.com/blankwall/MacDBG) - Simple easy to use C and python debugging framework for OSX
* [blechschmidt/massdns](https://github.com/blechschmidt/massdns) - A high-performance DNS stub resolver for bulk lookups in C
* [blitz/xplot](https://github.com/blitz/xplot) - Plot tcptrace data
* [blodow/realtime_urdf_filter](https://github.com/blodow/realtime_urdf_filter) - ROS package that can filter geometry defined in URDF models from Kinect depth images. Can also preprocess data for the OpenNI tracker, to remove backgrounds, robots etc.
* [bloomberg/comdb2](https://github.com/bloomberg/comdb2) - Bloomberg's distributed RDBMS
* [blucia0a/CTraps-gcc](https://github.com/blucia0a/CTraps-gcc) - Last Writer Slicing: data provenance tracking for concurrent program debugging & analysis
* [bluesmoon/pngtocss](https://github.com/bluesmoon/pngtocss) - Read in a gradient from a png file and spit out CSS for it
* [boazsegev/c-server-tools](https://github.com/boazsegev/c-server-tools) - Write network services in C using dynamic protocols such as HTTP and Websockets
* [boazsegev/facil.io](https://github.com/boazsegev/facil.io) - Your high performance web application C framework
* [boazsegev/iodine](https://github.com/boazsegev/iodine) - Iodine - HTTP / Websocket Server & EventMachine alternative for Ruby MRI - a kqueue/epoll C extension
* [bodgit/graphite-amqp-tools](https://github.com/bodgit/graphite-amqp-tools) - A set of tools for getting Graphite data in and out of AMQP message brokers
* [bonemurmurer/simplebonjour](https://github.com/bonemurmurer/simplebonjour) - pure-data external providing simple bonjour service name discovery and port resolution
* [bonzini/qboot](https://github.com/bonzini/qboot) - Minimal x86 firmware for booting Linux kernels
* [boothj5/profanity](https://github.com/boothj5/profanity) - Ncurses based XMPP client
* [borgbackup/borg](https://github.com/borgbackup/borg) - Deduplicating archiver with compression and authenticated encryption.
* [borland667/btier](https://github.com/borland667/btier) - Btier is a tiered storage that automatically moves frequently accessible data to fast(er) device.
* [bovine/datapipe](https://github.com/bovine/datapipe) - Network TCP port forwarding
* [boyerjohn/rapidstring](https://github.com/boyerjohn/rapidstring) - Maybe the fastest string library ever.
* [bpudream/pat](https://github.com/bpudream/pat) - Data Structure (中国大学MOOC-陈越、何钦铭-数据结构)
* [brackeen/glfm](https://github.com/brackeen/glfm) - OpenGL ES and input for iOS, tvOS, Android, and WebGL
* [brandenburg/sched-trace-tools](https://github.com/brandenburg/sched-trace-tools) - Some tools for working with LITMUS^RT sched_trace data.
* [breckinloggins/libuseful](https://github.com/breckinloggins/libuseful) - A collection of useful data structures, algorithms, and utilities for C programming
* [breckinloggins/ngtemplate](https://github.com/breckinloggins/ngtemplate) - ngtemplate - A template engine written in C designed to be syntax-compatible with Google CTemplate
* [brendan-rius/c-jwt-cracker](https://github.com/brendan-rius/c-jwt-cracker) - JWT brute force cracker written in C
* [brendangregg/Dump2PNG](https://github.com/brendangregg/Dump2PNG) - Visualize file data as a PNG
* [brenns10/lsh](https://github.com/brenns10/lsh) - Simple shell implementation.  Tutorial here ->
* [brg-liuwei/ngx_kafka_module](https://github.com/brg-liuwei/ngx_kafka_module) - nginx kafka module, send post log data to kafka cluster
* [brho/plan9](https://github.com/brho/plan9) - UC Berkeley release of Plan 9 under the GPLv2
* [brianmario/bzip2-ruby](https://github.com/brianmario/bzip2-ruby) - Original libbz2 ruby C bindings from Guy Decoux, with some new love
* [brianmario/escape_utils](https://github.com/brianmario/escape_utils) - Faster string escaping routines for your ruby apps
* [brianmario/yajl-ruby](https://github.com/brianmario/yajl-ruby) - A streaming JSON parsing and encoding library for Ruby (C bindings to yajl)
* [brong/cyrus-imapd](https://github.com/brong/cyrus-imapd) - My git clone of the Cyrus CVS repository
* [browndeer/coprthr](https://github.com/browndeer/coprthr) - The CO-PRocessing THReads (COPRTHR) SDK - latest release is v1.6.1 (Freewill)
* [bruceg/sqldjbdns](https://github.com/bruceg/sqldjbdns) - An authoritative DNS server that pulls its data directly from a set of SQL tables
* [bryansum/ijam](https://github.com/bryansum/ijam) - A collaborative music application for the iPhone utilizing Pure Data.
* [bryansum/pdlib](https://github.com/bryansum/pdlib) - An open source port of Pure Data to the iPhone
* [bsdphk/Ntimed](https://github.com/bsdphk/Ntimed) - Network time synchronization software, NTPD replacement.
* [bsmulders/CaptureTheData](https://github.com/bsmulders/CaptureTheData) - Vehicle data logging, parsing and analysis using C, PHP, JavaScript (Ext JS 4)
* [buaazp/zimg](https://github.com/buaazp/zimg) - A lightweight and high performance image storage and processing system.
* [bumptech/stud](https://github.com/bumptech/stud) - The Scalable TLS Unwrapping Daemon
* [burke/monkeysupport](https://github.com/burke/monkeysupport) - [abandoned] C extensions monkeypatching ActiveSupport for improved perfomance
* [burtonsamograd/sxc](https://github.com/burtonsamograd/sxc) - sxc is an 'S-Expression C' transpiler for generating C code using macros written in Common Lisp
* [bus1/dbus-broker](https://github.com/bus1/dbus-broker) - Linux D-Bus Message Broker
* [buserror/simavr](https://github.com/buserror/simavr) - simavr is a lean, mean and hackable AVR simulator for linux & OSX
* [bvdberg/ctest](https://github.com/bvdberg/ctest) - ctest is a unit test framework for software written in C.
* [bwalex/tc-play](https://github.com/bwalex/tc-play) - Free and simple TrueCrypt Implementation based on dm-crypt
* [bwhite/hadoopy](https://github.com/bwhite/hadoopy) - Python MapReduce library written in Cython. Visit us in #hadoopy on freenode.  See the link below for documentation and tutorials.
* [bwlewis/lazy.frame](https://github.com/bwlewis/lazy.frame) - Lazy person's file-backed data frame
* [c9s/Pux](https://github.com/c9s/Pux) - A High Performance PHP Router. PHP Router re-design
* [c9s/r3](https://github.com/c9s/r3) - libr3 is a high-performance path dispatching library. It compiles your route paths into a prefix tree (trie). By using the constructed prefix trie in the start-up time, you may dispatch your routes with efficiency
* [cadwallion/spinel](https://github.com/cadwallion/spinel) - A free and open source game engine using mruby and C/C++
* [cahirwpz/amigaos-cross-toolchain](https://github.com/cahirwpz/amigaos-cross-toolchain) - AmigaOS cross compiler for Linux / MacOSX / Windows
* [caisah/Sedgewick-algorithms-in-c-exercises-and-examples](https://github.com/caisah/Sedgewick-algorithms-in-c-exercises-and-examples) - Examples and exercises from Algorithms in C, Parts 1-4: Fundamentals, Data Structures, Sorting, Searching by Robert Sedgewick book
* [caisonglu/cachemaster](https://github.com/caisonglu/cachemaster) - Cachemaster is similar to VMTOUCH, but with more functions. Such as kick page cache, warmup/readahead data, lock data in mem, stat page cache, stat page cache in realtime mode, by file or directory~ Personally, I think the most usefule function is real-time-statistic of page cache. You can see the page cache thrashing when kernel do page reclaiming.
* [caius/fio](https://github.com/caius/fio) - Mirror of git://brick.kernel.dk/data/git/fio.git
* [calleerlandsson/pick](https://github.com/calleerlandsson/pick) - A fuzzy search tool for the command-line
* [calvinwilliams/cocker](https://github.com/calvinwilliams/cocker) - Container Engine
* [calvinwilliams/tcpdaemon](https://github.com/calvinwilliams/tcpdaemon) - Tcpdaemon is similar to the xinetd TCP daemon, which is under the particular process model of TCP connection management, docking with the customer communication data protocol layer and application processing module on runtime or compile linking, construct TCP server quickly.
* [camgunz/cmp](https://github.com/camgunz/cmp) - An implementation of the MessagePack serialization format in C / msgpack.org[C]
* [canboat/canboat](https://github.com/canboat/canboat) - CAN Boat provides NMEA 2000 and NMEA 0183 utilities. It contains a NMEA 2000 PGN decoder, can read and write N2K messages.
* [canonizer/libgpuvm](https://github.com/canonizer/libgpuvm) - library which simplifies host-GPU data transfer using userspace pagefault handling
* [caomaocao/micro-camera](https://github.com/caomaocao/micro-camera) - The mircocamera driven by a STM32 chip and its PC client. The microcamera captures a photo and then converts it to JPEG or BMP formet.     Finally , the camera sent image  data to PC by 485 serial-ports
* [careermonk/DataStructuresAndAlgorithmsMadeEasy](https://github.com/careermonk/DataStructuresAndAlgorithmsMadeEasy) - Data Structures And Algorithms Made Easy
* [carld/micro-lisp](https://github.com/carld/micro-lisp) - 🎄A very small Lisp programming language 😀that used to be under 200 lines of C🎄
* [carlj/CJAMacros](https://github.com/carlj/CJAMacros) - Macro collection for daily usage
* [carljv/Will_it_Python](https://github.com/carljv/Will_it_Python) - Translating R Data Analyses to Python
* [carlosgs/Cyclone-PCB-Factory](https://github.com/carlosgs/Cyclone-PCB-Factory) - Cyclone (Circuit Cloner) is a CNC mill intended for PCB manufacturing.
* [carp-lang/Carp](https://github.com/carp-lang/Carp) - A statically typed lisp, without a GC, for high performance applications
* [caseyscarborough/keylogger](https://github.com/caseyscarborough/keylogger) - A no-frills keylogger for Mac OS X.
* [catalinii/minisatip](https://github.com/catalinii/minisatip) - minisatip is an SATIP server for linux using local DVB-S2, DVB-C, DVB-T or ATSC cards
* [cbgbt/DataStructures](https://github.com/cbgbt/DataStructures) - A data structures library written in C.
* [cbsd/cbsd](https://github.com/cbsd/cbsd) - Yet one more wrapper around jail, bhyve and XEN on FreeBSD platform. For more information please visit website
* [cbsheng/tinyhttpd](https://github.com/cbsheng/tinyhttpd) - tinyhttpd的详细注释版，十分适合入门者学习的一个项目
* [cbuchner1/CudaMiner](https://github.com/cbuchner1/CudaMiner) - a CUDA accelerated litecoin mining application based on pooler's CPU miner
* [cbuchner1/ccminer](https://github.com/cbuchner1/ccminer) - Christian Buchner's & Christian H.'s CUDA miner project
* [cc65/cc65](https://github.com/cc65/cc65) - cc65 - a freeware C compiler for 6502 based systems —
* [ccore/ccore](https://github.com/ccore/ccore) - A cross platform low level game development library
* [ccore/ccore_rewrite](https://github.com/ccore/ccore_rewrite) - A cross platform low level game development library
* [ccpalettes/the-c-programming-language-second-edition-solutions](https://github.com/ccpalettes/the-c-programming-language-second-edition-solutions) - Solutions for all exercises in the book "The C Programming Language - Second Edition"(referred to as K&R, after its authors' initials) by Brian W. Kernighan and Dennis M. Ritchie.
* [ccxvii/mujs](https://github.com/ccxvii/mujs) - An embeddable Javascript interpreter in C.
* [cdkamat/hammerspace](https://github.com/cdkamat/hammerspace) - Senior Year (BE Computer Engg.) Undergraduate project - Data Deduplication for the TUX 3 Linux File System
* [celery/librabbitmq](https://github.com/celery/librabbitmq) - Python bindings to librabbitmq-c
* [celluloid-player/celluloid](https://github.com/celluloid-player/celluloid) - A simple GTK+ frontend for mpv
* [celluloid/nio4r](https://github.com/celluloid/nio4r) - New IO for Ruby
* [cengek/CKDatastruct](https://github.com/cengek/CKDatastruct) - The using of data structure in C from our class
* [centaurean/density](https://github.com/centaurean/density) - Superfast compression library
* [ceph/ceph-client](https://github.com/ceph/ceph-client) - Ceph kernel client
* [cesanta/fossa](https://github.com/cesanta/fossa) - Async non-blocking multi-protocol networking library for C/C++
* [cesanta/frozen](https://github.com/cesanta/frozen) - JSON parser and generator for C/C++ with scanf/printf like interface. Targeting embedded systems.
* [cesanta/mjs](https://github.com/cesanta/mjs) - Embedded JavaScript engine for C/C++
* [cesanta/mongoose-os](https://github.com/cesanta/mongoose-os) - Mongoose OS - an IoT Firmware Development Framework. Supported microcontrollers: ESP32, ESP8266, CC3220, CC3200, STM32F4, STM32L4, STM32F7. Amazon AWS IoT, Microsoft Azure, Google IoT Core integrated. Code in C or JavaScript.
* [cesanta/mongoose](https://github.com/cesanta/mongoose) - Embedded web server for C/C++
* [cesanta/slre](https://github.com/cesanta/slre) - Super Light Regexp engine for C/C++
* [cesanta/smart.js](https://github.com/cesanta/smart.js) - Embedded Javascript engine for C/C++ with networking, file, database and device interfaces
* [cesanta/v7](https://github.com/cesanta/v7) - Embedded JavaScript engine for C/C++
* [cfengine/core](https://github.com/cfengine/core) - CFEngine Community
* [cgaebel/pipe](https://github.com/cgaebel/pipe) - A simple thread-safe FIFO in C.
* [cgdb/cgdb](https://github.com/cgdb/cgdb) - Console front-end to the GNU debugger
* [chadjoan/C-Survival-Kit](https://github.com/chadjoan/C-Survival-Kit) - A set of useful functions, data structures, and macros aimed at allowing more expressive and reliable C code.  Portability targets are OpenVMS and Linux.
* [chadjoan/sleep-waffle](https://github.com/chadjoan/sleep-waffle) - A reimplementation of the Zeo Raw Data Library with less restrictive (Boost) licensing and written in C with a non-threaded polling-event model.  And a silly name.
* [chadwickbureau/chadwick](https://github.com/chadwickbureau/chadwick) - Chadwick tools for manipulating baseball data
* [chaelim/HAMT](https://github.com/chaelim/HAMT) - Hash Array Mapped Trie (C++ Templates)
* [chameco/Solid](https://github.com/chameco/Solid) - A minimalist interpreted language, with a clean object model and a tiny VM.
* [chaoslawful/ccard-lib](https://github.com/chaoslawful/ccard-lib) - C library for estimating cardinality in streams for which it is infeasible to store all events in memory
* [chaoslawful/tcc](https://github.com/chaoslawful/tcc) - track of Tiny C Compiler
* [charleyw/cordova-plugin-alipay](https://github.com/charleyw/cordova-plugin-alipay) - Cordova支付宝插件，cordova alipay plugin
* [charliegerard/Epoc.js](https://github.com/charliegerard/Epoc.js) - Node.js addon for the Emotiv C++ SDK
* [charliesome/jsos](https://github.com/charliesome/jsos) - An operating system written in JavaScript
* [charybdis-ircd/charybdis](https://github.com/charybdis-ircd/charybdis) - Scalable IRCv3.2 server for large, community-oriented networks
* [checkpoint-restore/criu](https://github.com/checkpoint-restore/criu) - Checkpoint/Restore tool
* [chelyaev/ffmpeg-tutorial](https://github.com/chelyaev/ffmpeg-tutorial) - A set of tutorials that demonstrates how to write a video player based on FFmpeg
* [chengjiaming/JSPatch---comment](https://github.com/chengjiaming/JSPatch---comment) - JSPatch 是一套牛逼的 hotfix 框架，可利用 js 脚本修复线上 bug，但是作者 bang 没写注释，阅读源代码后，我添加了部分注释，想快速理解源码的同学可以参考。
* [chenkovsky/ngram](https://github.com/chenkovsky/ngram) - efficient data structure for storing ngram.
* [chenlonggang/Adaptive-CSA](https://github.com/chenlonggang/Adaptive-CSA) - Adaptive CSA, is data-aware,can select the best coding-method for each block
* [chentao0707/QrCodeScan](https://github.com/chentao0707/QrCodeScan) - Android手机客户端二维码扫描
* [cherokee/webserver](https://github.com/cherokee/webserver) - Cherokee Web Server
* [chitika/cberl](https://github.com/chitika/cberl) - NIF based Erlang bindings for Couchbase
* [chmduquesne/sharebox-fs](https://github.com/chmduquesne/sharebox-fs) - C rewrite of sharebox
* [chmduquesne/xmppipe](https://github.com/chmduquesne/xmppipe) - This program allows to pipe data through an xmpp tunnel
* [chneukirchen/cwm](https://github.com/chneukirchen/cwm) - portable version of OpenBSD's cwm(1) window manager
* [chneukirchen/rdd](https://github.com/chneukirchen/rdd) - random data dumper
* [chneukirchen/rs](https://github.com/chneukirchen/rs) - rs(1) — reshape a data array (from OpenBSD)
* [chobits/ngx_http_proxy_connect_module](https://github.com/chobits/ngx_http_proxy_connect_module) - A forward proxy module for CONNECT request handling
* [chocolate-doom/chocolate-doom](https://github.com/chocolate-doom/chocolate-doom) - Chocolate Doom is a Doom source port that is minimalist and historically accurate.
* [chokepoint/CryptHook](https://github.com/chokepoint/CryptHook) - TCP/UDP symmetric encryption tunnel wrapper
* [chokepoint/azazel](https://github.com/chokepoint/azazel) - Azazel is a userland rootkit based off of the original LD_PRELOAD technique from Jynx rootkit.  It is more robust and has additional features, and focuses heavily around anti-debugging and anti-detection.
* [chrisforbes/libaof](https://github.com/chrisforbes/libaof) - Age Of Empires Data Format Parsers
* [chrisjmccormick/word2vec_commented](https://github.com/chrisjmccormick/word2vec_commented) - Commented (but unaltered) version of original word2vec C implementation.
* [chrismoos/hash-ring](https://github.com/chrismoos/hash-ring) - C hash ring library
* [chriso/bitset](https://github.com/chriso/bitset) - A compressed bitset with supporting data structures and algorithms
* [chronomex/1600bpi-tape](https://github.com/chronomex/1600bpi-tape) - Tool to recover data from analog recordings of 1970s data tape
* [chucknthem/Data-structures-algorithms](https://github.com/chucknthem/Data-structures-algorithms) - Collection of Data structures, algorithms and interesting bits of code.
* [chutsu/cog](https://github.com/chutsu/cog) - C common library containing common data structures, sorting algorithms and utility functions
* [cinder/Cinder-Kinect](https://github.com/cinder/Cinder-Kinect) - Kinect support for Cinder
* [cinder/Cinder](https://github.com/cinder/Cinder) - Cinder is a community-developed, free and open source library for professional-quality creative coding in C++.
* [cioc/functionalC](https://github.com/cioc/functionalC) - Not because it is good, but because we can...
* [circonus-labs/fq](https://github.com/circonus-labs/fq) - F@#$*&%Q (Message queue that is fast, brokered, in C and gets out of your way)
* [cirosantilli/cpp-cheat](https://github.com/cirosantilli/cpp-cheat) - C, C++, POSIX and Linux system programming minimal examples. Asserts used wherever possible. Hello worlds for cool third party libraries and build systems. Cheatsheets, tutorials and mini-projects.
* [cirosantilli/linux-kernel-module-cheat](https://github.com/cirosantilli/linux-kernel-module-cheat) - The perfect emulation setup to study and modify the Linux kernel, kernel modules, QEMU and gem5. Highly automated. Thoroughly documented. GDB and KGDB just work. Powered by Buildroot. "Tested" in Ubuntu 18.04 host, x86 and ARM guests with kernel v4.18.
* [cisco-system-traffic-generator/trex-core](https://github.com/cisco-system-traffic-generator/trex-core) - trex-core site
* [cisco/thor](https://github.com/cisco/thor) - Thor Video Codec
* [citiususc/BigBWA](https://github.com/citiususc/BigBWA) - Approaching the Burrows-Wheeler Aligner to Big Data Technologies
* [citra-emu/citra](https://github.com/citra-emu/citra) - A Nintendo 3DS Emulator
* [citusdata/citus](https://github.com/citusdata/citus) - Scalable PostgreSQL for multi-tenant and real-time analytics workloads
* [citusdata/cstore_fdw](https://github.com/citusdata/cstore_fdw) - Columnar store for analytics with Postgres, developed by Citus Data. Check out the mailing list at https://groups.google.com/forum/#!forum/cstore-users or join our slack channel at https://slack.citusdata.com
* [citusdata/json_fdw](https://github.com/citusdata/json_fdw) - PostgreSQL extension which implements a Foreign Data Wrapper (FDW) for JSON files.
* [citusdata/mongo_fdw](https://github.com/citusdata/mongo_fdw) - PostgreSQL foreign data wrapper for MongoDB
* [citusdata/pg_cron](https://github.com/citusdata/pg_cron) - Run periodic jobs in PostgreSQL
* [citusdata/pg_shard](https://github.com/citusdata/pg_shard) - PostgreSQL extension to scale out real-time reads and writes. Check out the mailing list at https://groups.google.com/group/pg_shard-users or read the docs at http://citusdata.com/docs/pg-shard
* [citusdata/postgres_vectorization_test](https://github.com/citusdata/postgres_vectorization_test) - Vectorized executor to speed up PostgreSQL
* [civetweb/civetweb](https://github.com/civetweb/civetweb) - Embedded C/C++ web server
* [cjac/cmusphinx](https://github.com/cjac/cmusphinx) - CMU Sphinx - Speech Recognition Toolkit
* [cksystemsteaching/selfie](https://github.com/cksystemsteaching/selfie) - An educational software system of a tiny self-compiling C compiler, a tiny self-executing RISC-V emulator, and a tiny self-hosting RISC-V hypervisor.
* [clMathLibraries/clBLAS](https://github.com/clMathLibraries/clBLAS) - a software library containing BLAS functions written in OpenCL
* [clMathLibraries/clRNG](https://github.com/clMathLibraries/clRNG) - an OpenCL based software library containing random number generation functions
* [clarkds/Benchmark-Results](https://github.com/clarkds/Benchmark-Results) - this is benchmarking data for arm cortex A8 and A9's
* [clarkgrubb/data-tools](https://github.com/clarkgrubb/data-tools) - File format conversion tools
* [clawoo/AsteroidsCocos2D-x](https://github.com/clawoo/AsteroidsCocos2D-x) - An Asteroids game implemented in Cocos2D-x
* [cleanflight/cleanflight](https://github.com/cleanflight/cleanflight) - Clean-code version of the baseflight flight controller firmware
* [clear-code/cutter](https://github.com/clear-code/cutter) - An easy to write and debug unit testing framework for C and C++.
* [clibs/buffer](https://github.com/clibs/buffer) - Tiny C string library
* [clibs/clib](https://github.com/clibs/clib) - C package manager-ish
* [clibs/commander](https://github.com/clibs/commander) - Commander option parser ported to C - simple API, auto-generated --help
* [clibs/dumpasn1](https://github.com/clibs/dumpasn1) - Display the contents of ASN.1 encoded data
* [clibs/flag](https://github.com/clibs/flag) - Go-style flag parsing for C
* [clibs/hash](https://github.com/clibs/hash) - C hash implementation based on khash
* [clibs/list](https://github.com/clibs/list) - C doubly linked list
* [closeio/ciso8601](https://github.com/closeio/ciso8601) - Fast ISO8601 date time parser for Python written in C
* [cloudflare/cloudflare-blog](https://github.com/cloudflare/cloudflare-blog) - Cloudflare Blog code samples
* [cloudflare/keyless](https://github.com/cloudflare/keyless) - CloudFlare's Keyless SSL Server Reference Implementation
* [cloudflare/lua-resty-json](https://github.com/cloudflare/lua-resty-json) - json lib for lua and C
* [cloudflare/lua-upstream-cache-nginx-module](https://github.com/cloudflare/lua-upstream-cache-nginx-module) - Nginx module for ngx_lua to provide Lua API to inspect upstream http cache meta-data
* [cloudius-systems/osv](https://github.com/cloudius-systems/osv) - OSv, a new operating system for the cloud.
* [cloudozer/ling](https://github.com/cloudozer/ling) - Erlang on Xen
* [cloudwu/atomdict](https://github.com/cloudwu/atomdict) - A data structure for data exchange between multi lua states.
* [cloudwu/coroutine](https://github.com/cloudwu/coroutine) - A asymmetric coroutine library for C.
* [cloudwu/cstring](https://github.com/cloudwu/cstring) - A simple C string lib
* [cloudwu/lua-db](https://github.com/cloudwu/lua-db) - A database shared data among multi-states .
* [cloudwu/mptun](https://github.com/cloudwu/mptun) - Multi-path Tunnel
* [cloudwu/pbc](https://github.com/cloudwu/pbc) - A protocol buffers library for C
* [cloudwu/skynet](https://github.com/cloudwu/skynet) - A lightweight online game framework
* [cloudwu/sproto](https://github.com/cloudwu/sproto) - Yet another protocol library like google protocol buffers , but simple and fast.
* [cloudyourcar/minmea](https://github.com/cloudyourcar/minmea) - a lightweight GPS NMEA 0183 parser library in pure C
* [clowwindy/ChinaDNS](https://github.com/clowwindy/ChinaDNS) - Protect yourself against DNS poisoning in China.
* [clowwindy/ShadowVPN](https://github.com/clowwindy/ShadowVPN) - Removed according to regulations.
* [cmatsuoka/libxmp](https://github.com/cmatsuoka/libxmp) - Libxmp is a library that renders module files to PCM data.
* [cmus/cmus](https://github.com/cmus/cmus) - Small, fast and powerful console music player for Unix-like operating systems.
* [cmusphinx/pocketsphinx](https://github.com/cmusphinx/pocketsphinx) - PocketSphinx is a lightweight speech recognition engine, specifically tuned for handheld and mobile devices, though it works equally well on the desktop
* [cni/pdr](https://github.com/cni/pdr) - CNI Peripheral Data Reader (PDR)
* [cnlohr/channel3](https://github.com/cnlohr/channel3) - ESP8266 Analog Broadcast Television Interface
* [cnlohr/colorchord](https://github.com/cnlohr/colorchord) - Chromatic Sound to Light Conversion System
* [cnlohr/wificompositer](https://github.com/cnlohr/wificompositer) - Various tools I used to collect and composite data from a wifi device into an image.
* [cockpit-project/cockpit](https://github.com/cockpit-project/cockpit) - There's code a goin' on
* [cocos2d/cocos2d-frame](https://github.com/cocos2d/cocos2d-frame) - Player and "stub" for cocos2d
* [codahale/bcrypt-ruby](https://github.com/codahale/bcrypt-ruby) - bcrypt-ruby is a Ruby binding for the OpenBSD bcrypt() password hashing algorithm, allowing you to easily store a secure hash of your users' passwords.
* [code-mancers/rbkit](https://github.com/code-mancers/rbkit) - A new profiler for Ruby. With a GUI
* [codebox/bitmeteros](https://github.com/codebox/bitmeteros) - BitMeter OS - a cross-platform bandwidth monitor
* [codeman38/zvbi2raw](https://github.com/codeman38/zvbi2raw) - A quick-and-dirty tool for capturing vertical blanking interval data using libzvbi
* [codeplea/genann](https://github.com/codeplea/genann) - simple neural network library in ANSI C
* [codeprepper/data-structures](https://github.com/codeprepper/data-structures) - arrays, linked lists, stacks and queues
* [coderaven/B-Tree](https://github.com/coderaven/B-Tree) - B-Tree Implementation in C. A project in Data Structures.
* [codinghead/nmea-module](https://github.com/codinghead/nmea-module) - Module to enable decoding of NMEA data from GPS receivers.
* [cofyc/argparse](https://github.com/cofyc/argparse) - Command-line arguments parsing library.
* [cofyc/dnscrypt-wrapper](https://github.com/cofyc/dnscrypt-wrapper) - This is dnscrypt wrapper (server-side dnscrypt proxy), which helps to add dnscrypt support to any name resolver.
* [coins11/data-structures-and-algorithms](https://github.com/coins11/data-structures-and-algorithms) - Data Structures and Algorithms
* [colindean/optar](https://github.com/colindean/optar) - OPTical ARchiver - highly compressed 2D barcode for paper or film archiving of digital data
* [collectd/collectd](https://github.com/collectd/collectd) - The system statistics collection daemon. Please send Pull Requests here!
* [colmap/colmap](https://github.com/colmap/colmap) - COLMAP - Structure-from-Motion and Multi-View Stereo
* [comex/data](https://github.com/comex/data) - the green eyed monster
* [comex/frash](https://github.com/comex/frash) - yeah I'm getting tired of the long description
* [comex/substitute](https://github.com/comex/substitute) - A free runtime modification library.
* [commoncrawl/commoncrawl](https://github.com/commoncrawl/commoncrawl) - CommonCrawl Project Repository
* [commonmark/cmark](https://github.com/commonmark/cmark) - CommonMark parsing and rendering library and program in C
* [commonsguy/cwac-anddown](https://github.com/commonsguy/cwac-anddown) - CWAC AndDown: Markdown Utility Library
* [compiler-dept/speck](https://github.com/compiler-dept/speck) - A small unit testing framework for C
* [conch/disco](https://github.com/conch/disco) - Automatic perspective DIStortion COrrection using accelerometer data
* [concurrencykit/ck](https://github.com/concurrencykit/ck) - Concurrency primitives, safe memory reclamation mechanisms and non-blocking (including lock-free) data structures designed to aid in the research, design and implementation of high performance concurrent systems developed in C99+.
* [confluentinc/bottledwater-pg](https://github.com/confluentinc/bottledwater-pg) - Change data capture from PostgreSQL into Kafka
* [confluentinc/confluent-kafka-python](https://github.com/confluentinc/confluent-kafka-python) - Confluent's Apache Kafka Python client
* [conformal/cyphertite](https://github.com/conformal/cyphertite) - A high-security scalable solution for online backups.
* [conghui/algorithms-in-c](https://github.com/conghui/algorithms-in-c) - Exercise of the book Algorithms In C, Part 1-4, Fundamentals, Data Strcuture, Sorting, Searching, written by  Robert Sedgewick
* [contiki-ng/contiki-ng](https://github.com/contiki-ng/contiki-ng) - Contiki-NG: The OS for Next Generation IoT Devices
* [contiki-os/contiki](https://github.com/contiki-os/contiki) - The official git repository for Contiki, the open source OS for the Internet of Things
* [coocox/cox](https://github.com/coocox/cox) - CoX is an peripherals library with a unified standard interface specially for ARM Cortex M.
* [coolstar/RecordMyScreen](https://github.com/coolstar/RecordMyScreen) - Record the display even on non-jailbroken iPhones.
* [coolwanglu/quantile-alg](https://github.com/coolwanglu/quantile-alg) - Algorithms for finding quantiles of a data stream
* [coolwanglu/vim.js](https://github.com/coolwanglu/vim.js) - JavaScript port of Vim
* [cooperative-computing-lab/cctools](https://github.com/cooperative-computing-lab/cctools) - The Cooperative Computing Tools (cctools) enable large scale distributed computations to harness hundreds to thousands of machines from clusters, clouds, and grids.
* [coova/coova-chilli](https://github.com/coova/coova-chilli) - CoovaChilli is an open-source software access controller for captive portal hotspots.
* [coreboot/coreboot](https://github.com/coreboot/coreboot) - github mirror of coreboot.org's master repository
* [coreutils/coreutils](https://github.com/coreutils/coreutils) - upstream mirror
* [corks/corc.ds](https://github.com/corks/corc.ds) - A data structure library written in C.
* [cornet/ccze](https://github.com/cornet/ccze) - ccze
* [cornetp/eagle-owl](https://github.com/cornetp/eagle-owl) - Data acquisition from an OWL CM160 +USB device on linux platforms
* [corosync/corosync](https://github.com/corosync/corosync) - The Corosync Cluster Engine
* [corporateshark/Android-NDK-Game-Development-Cookbook](https://github.com/corporateshark/Android-NDK-Game-Development-Cookbook) - Android NDK Game Development Cookbook
* [cos120/captcha_crack](https://github.com/cos120/captcha_crack) - 选字验证码破解，试验过网易和极验，破解率99
* [coturn/coturn](https://github.com/coturn/coturn) - coturn TURN server project
* [couchbase/Android-Couchbase](https://github.com/couchbase/Android-Couchbase) - The android build for humans.
* [couchbase/couchbase-lite-android](https://github.com/couchbase/couchbase-lite-android) - Lightweight, embedded, syncable NoSQL database engine for Android.
* [couchbase/couchbase-ruby-client](https://github.com/couchbase/couchbase-ruby-client) - Couchbase Ruby client library (official) built atop libcouchbase
* [couchbase/libcouchbase](https://github.com/couchbase/libcouchbase) - The couchbase client for C.
* [couchbaselabs/Android-Couchbase](https://github.com/couchbaselabs/Android-Couchbase) - The android build for humans.
* [couchbaselabs/couchstore](https://github.com/couchbaselabs/couchstore) - couchbase storage file library
* [cr-marcstevens/sha1collisiondetection](https://github.com/cr-marcstevens/sha1collisiondetection) - Library and command line tool to detect SHA-1 collision in a file
* [crash-utility/crash](https://github.com/crash-utility/crash) - Linux kernel crash utility
* [crass/lessfs](https://github.com/crass/lessfs) - lessfs - An inline data deduplicating filesystem
* [creaceed/CeedMath](https://github.com/creaceed/CeedMath) - Computer graphics math library for Mac & iOS
* [credativ/informix_fdw](https://github.com/credativ/informix_fdw) - Foreign Data Wrapper for Informix Databases
* [criticalstack/libevhtp](https://github.com/criticalstack/libevhtp) - Create extremely-fast and secure embedded HTTP servers with ease.
* [crmulliner/adbi](https://github.com/crmulliner/adbi) - Android Dynamic Binary Instrumentation Toolkit
* [crocodella/MongooseWrapper](https://github.com/crocodella/MongooseWrapper) - An Objective-C Mongoose wrapper emulating Java servlets
* [crosg/idCreator](https://github.com/crosg/idCreator) - 这是一个id生成器，主要为互联网的各种业务生成id（也就是数据库主键）。该id生成器生成的id主要被用来做数据路由之用。和Albianj2配合，可以快速而简单的搭建完整的分布式业务系统！
* [crosslife/OpenBird](https://github.com/crosslife/OpenBird) - Flappy Bird in cocos2dx
* [crozone/SpectrePoC](https://github.com/crozone/SpectrePoC) - Proof of concept code for the Spectre CPU exploit.
* [cs3157/recitations](https://github.com/cs3157/recitations) - Recitation notes for cs3157, the C systems programming course with a narrative
* [cs50/libcs50](https://github.com/cs50/libcs50) - CS50 Library for C
* [csete/gpredict](https://github.com/csete/gpredict) - Gpredict satellite tracking application
* [csound/csound](https://github.com/csound/csound) - Main repository for Csound
* [cstack/db_tutorial](https://github.com/cstack/db_tutorial) - Writing a sqlite clone from scratch in C
* [cstavish/c_data_structs](https://github.com/cstavish/c_data_structs) - singly/doubly linked list and hash table implementations...more to come
* [ctz/cifra](https://github.com/ctz/cifra) - A collection of cryptographic primitives targeted at embedded use.
* [cuber/ngx_http_google_filter_module](https://github.com/cuber/ngx_http_google_filter_module) - Nginx Module for Google Mirror
* [cuberite/cuberite](https://github.com/cuberite/cuberite) - A performant C++ Minecraft compatible game server
* [cuckoobox/cuckoomon](https://github.com/cuckoobox/cuckoomon) - Cuckoo Sandbox Monitor Component
* [cuckoosandbox/cuckoomon](https://github.com/cuckoosandbox/cuckoomon) - DEPRECATED - replaced with "monitor"
* [cucumber/cucumber](https://github.com/cucumber/cucumber) - Cucumber monorepo - polyglot home for Cucumber building blocks
* [cudpp/cudpp](https://github.com/cudpp/cudpp) - CUDA Data Parallel Primitives Library
* [cundong/SmartAppUpdates](https://github.com/cundong/SmartAppUpdates) - Android应用增量更新
* [cvmfs/cvmfs](https://github.com/cvmfs/cvmfs) - The CernVM File System
* [cvxgrp/scs](https://github.com/cvxgrp/scs) - C package that solves convex cone problems via operator splitting
* [cvxopt/cvxopt](https://github.com/cvxopt/cvxopt) - CVXOPT -- Python Software for Convex Optimization
* [cxong/cdogs-sdl](https://github.com/cxong/cdogs-sdl) - Classic overhead run-and-gun game
* [cxong/tinydir](https://github.com/cxong/tinydir) - Lightweight, portable and easy to integrate C directory and file reader
* [cyassl/cyassl](https://github.com/cyassl/cyassl) - Please use wolfSSL now instead: https://github.com/wolfSSL/wolfssl . CyaSSL is a small, fast, portable implementation of TLS/SSL for embedded devices to the cloud.
* [cybergarage/mupnp](https://github.com/cybergarage/mupnp) - mUPnP for C is a development package for UPnP™ developers. CyberLink controls these protocols automatically, and supports to create your devices and control points quickly.
* [cybergarage/mupnpc](https://github.com/cybergarage/mupnpc) - mUPnP for C is a development package for UPnP™ developers. CyberLink controls these protocols automatically, and supports to create your devices and control points quickly.
* [cypresssemiconductorco/PSoC-4-BLE](https://github.com/cypresssemiconductorco/PSoC-4-BLE) - PSoC 4 BLE is an easy-to-use, ARM® Cortex™-M0 based, single-chip solution which integrates programmable analog front ends, programmable digital peripherals, CapSense® technology for touch-sensing, and a Bluetooth® LE (Low Energy) or Bluetooth Smart radio.
* [cyring/CoreFreq](https://github.com/cyring/CoreFreq) - CoreFreq is a CPU monitoring software designed for the 64-bits Processors.
* [cyrus-and/prof](https://github.com/cyrus-and/prof) - Self-contained C/C++ profiler library for Linux
* [cyrusimap/cyrus-imapd](https://github.com/cyrusimap/cyrus-imapd) - Cyrus IMAP is an email, contacts and calendar server
* [czarrar/cwas-paper](https://github.com/czarrar/cwas-paper) - Scripts to analyze data and generate figures for the CWAS paper
* [cznic/cc](https://github.com/cznic/cc) - Package CC is a C99 compiler front end.
* [cztomczak/cef2go](https://github.com/cztomczak/cef2go) - Go lang bindings for the Chromium Embedded Framework (CEF)
* [dake/openVP](https://github.com/dake/openVP) - Voice Print Recognition in C language.
* [dalerank/caesaria-game](https://github.com/dalerank/caesaria-game) - Caesar III (Open source remake)
* [dalibo/hypopg](https://github.com/dalibo/hypopg) - Hypothetical Indexes for PostgreSQL
* [damellis/attiny](https://github.com/damellis/attiny) - ATtiny microcontroller support for the Arduino IDE
* [damiannz/ofxPd_damians](https://github.com/damiannz/ofxPd_damians) - Pure Data addon for openFrameworks
* [danghvu/mod_dumpost](https://github.com/danghvu/mod_dumpost) - Small and lightweight Apache module to log POST data of a HTTP request
* [danielfrg/word2vec](https://github.com/danielfrg/word2vec) - Python interface to Google word2vec
* [danielwaterworth/Raphters](https://github.com/danielwaterworth/Raphters) - [DEPRECATED] A web framework for C.
* [danomatika/PdParty](https://github.com/danomatika/PdParty) - (work-in-progress) Run your Pure Data patches on iOS with native GUIs emulated
* [danomatika/ofxPd](https://github.com/danomatika/ofxPd) - (maintained) a Pure Data addon for OpenFrameworks using libpd
* [daoluan/decode-memcached](https://github.com/daoluan/decode-memcached) - memcached 源码剖析注释
* [dariomanesku/cmftStudio](https://github.com/dariomanesku/cmftStudio) - cmftStudio - GUI counterpart for:
* [dariomanesku/cmft](https://github.com/dariomanesku/cmft) - Cross-platform open-source command-line cubemap filtering tool.
* [darius/ichbins](https://github.com/darius/ichbins) - A tiny self-hosting Lisp-to-C compiler
* [darkk/redsocks](https://github.com/darkk/redsocks) - transparent redirector of any TCP connection to proxy
* [darkstalker/dbc_browser](https://github.com/darkstalker/dbc_browser) - quick and dirty web DBC browser for WoW spell data
* [darktable-org/darktable](https://github.com/darktable-org/darktable) - darktable main repository
* [darthstroyer/005tools](https://github.com/darthstroyer/005tools) - Open-source software for extracting save data from Nintendo DS, DSi and 3DS game cards
* [darwin-on-arm/xnu](https://github.com/darwin-on-arm/xnu) - Porting the Darwin kernel to the AArch64/ARMv7/ARMv6-A architectures.
* [dasuxullebt/tddp](https://github.com/dasuxullebt/tddp) - Trivial Data Deduplication
* [dave-andersen/cudapts](https://github.com/dave-andersen/cudapts) - An Nvidia-based miner for the Protoshares (PTS) cryptocurrency
* [daveho/EasySandbox](https://github.com/daveho/EasySandbox) - really simple sandboxing of untrusted C programs using Linux SECCOMP
* [davidar/c-hashtable](https://github.com/davidar/c-hashtable) - Git mirror of the hash table data structure in C by Christopher Clark
* [davidcranor/Thinner-Client](https://github.com/davidcranor/Thinner-Client) - This project implements an STM32F based thin client which can send and receive data over serial, read a PS/2 keyboard, and display the contents of a 480x240 framebuffer on an NTSC television.
* [davidfstr/rdiscount](https://github.com/davidfstr/rdiscount) - Discount (For Ruby) Implementation of John Gruber's Markdown
* [davidh-ssec/polar2grid](https://github.com/davidh-ssec/polar2grid) - Tools for reading, remapping, and writing satellite instrument data.
* [davidmoreno/onion](https://github.com/davidmoreno/onion) - C library to create simple HTTP servers and Web Applications.
* [davidreynolds/algorithms](https://github.com/davidreynolds/algorithms) - A repository of assorted algorithms and data structures.
* [davidsblog/rCPU](https://github.com/davidsblog/rCPU) - Remote CPU monitoring webserver
* [davisp/python-spidermonkey](https://github.com/davisp/python-spidermonkey) - Python/JavaScript bridge module, making use of Mozilla's spidermonkey JavaScript implementation.
* [dawnbreaks/mysql2redis](https://github.com/dawnbreaks/mysql2redis) -    A high performance mysql udf  to sync the newly modified/inserted data from mysql to redis cache.
* [dbalmain/ferret](https://github.com/dbalmain/ferret) - Ferret: the extensible information retrieval library for ruby.
* [dbartolini/crown](https://github.com/dbartolini/crown) - The flexible game engine.
* [dbohdan/s2png](https://github.com/dbohdan/s2png) - Store data of any kind inside PNG images.
* [dbro/csvquote](https://github.com/dbro/csvquote) - Enables common unix utlities like cut, awk, wc, head to work correctly with csv data containing delimiters and newlines
* [dcjones/quip](https://github.com/dcjones/quip) - Compressing next-generation sequencing data with extreme prejudice.
* [dcreager/libcork](https://github.com/dcreager/libcork) - A simple, easily embeddable cross-platform C library
* [dcreager/libpush](https://github.com/dcreager/libpush) - An arrow-based parser combinator library for C
* [dcshi/Mysync](https://github.com/dcshi/Mysync) - Mysync is an MySQL binlog Parser. With it, you can sync mysql data to any other servers, such as redis, mc, sphinx and so on
* [deactivated/collectd-write-zmq](https://github.com/deactivated/collectd-write-zmq) - a collectd plugin that writes data via zeromq
* [deadbits/InsecureProgramming](https://github.com/deadbits/InsecureProgramming) - mirror of gera's insecure programming examples | http://community.coresecurity.com/~gera/InsecureProgramming/
* [deanmao/node-chimera](https://github.com/deanmao/node-chimera) - A new kind of headless webkit integration for nodejs; a great alternative to phantomjs.
* [debrouxl/tilp-libticables](https://github.com/debrouxl/tilp-libticables) - TILP (formerly GtkTiLink) can transfer data between Texas Instruments scientific calculators and a computer. It works with all link cables (parallel, serial, Black/Gray/Silver/Direct Link) and it supports the TI-Z80 series (73..86), the TI-68k series (89, 92+, V200, 89T) and the Nspire series (Nspire Clickpad / Touchpad / CX, both CAS and non-CAS)
* [debrouxl/tilp-linkguide](https://github.com/debrouxl/tilp-linkguide) - TILP (formerly GtkTiLink) can transfer data between Texas Instruments scientific calculators and a computer. It works with all link cables (parallel, serial, Black/Gray/Silver/Direct Link) and it supports the TI-Z80 series (73..86), the TI-68k series (89, 92+, V200, 89T) and the Nspire series (Nspire Clickpad / Touchpad / CX, both CAS and non-CAS)
* [debrouxl/tilp](https://github.com/debrouxl/tilp) - TILP (formerly GtkTiLink) can transfer data between Texas Instruments scientific calculators and a computer. It works with all link cables (parallel, serial, Black/Gray/Silver/Direct Link) and it supports the TI-Z80 series (73..86), the TI-68k series (89, 92+, V200, 89T) and the Nspire series (Nspire Clickpad / Touchpad / CX, both CAS and non-CAS)
* [deep011/redis-cluster-tool](https://github.com/deep011/redis-cluster-tool) - A convenient and useful tool for redis cluster.
* [deepwater82/bismark_data_transmit](https://github.com/deepwater82/bismark_data_transmit) - data transmit using cURL
* [defuse/crackstation-hashdb](https://github.com/defuse/crackstation-hashdb) - CrackStation.net's Lookup Table Implementation.
* [defuse/swatd](https://github.com/defuse/swatd) - Run a script when one or more sensors fail.
* [deltachat/deltachat-core](https://github.com/deltachat/deltachat-core) - Delta.Chat C-Library with e2e chat-over-email functionality & Python bindings
* [demerphq/Data-Undump](https://github.com/demerphq/Data-Undump) - Perl extension for securely and quickly deserializing simple Data::Dumper dumps
* [demorest/guppi_daq](https://github.com/demorest/guppi_daq) - Data acquisition software primarily for the GUPPI pulsar backend.
* [demorest/psrfits_utils](https://github.com/demorest/psrfits_utils) - Utility library for working with search- and fold-mode PSRFITS pulsar data files.
* [derekmolloy/boneCV](https://github.com/derekmolloy/boneCV) - Beaglebone Webcam and OpenCV Examples Repository
* [derpston/linux-rpi-audi-dis](https://github.com/derpston/linux-rpi-audi-dis) - Linux kernel module for sending data to the DIS LCD in an Audi car from a Raspberry Pi.
* [devsisters/libquic](https://github.com/devsisters/libquic) - QUIC, a multiplexed stream transport over UDP
* [dewoods/greenplum-json-formatter](https://github.com/dewoods/greenplum-json-formatter) - Greenplum extension for reading and writing JSON data
* [dfm/acor](https://github.com/dfm/acor) - Estimate the autocorrelation time of time-series data very quickly
* [dgvncsz0f/lift](https://github.com/dgvncsz0f/lift) - Implementation of some data structures in C
* [dhbikoff/Generic-C-Library](https://github.com/dhbikoff/Generic-C-Library) - A library of generic data structures in C
* [dhoerl/PhotoScrollerNetwork](https://github.com/dhoerl/PhotoScrollerNetwork) - Awesomely fast enhanced version of Apple's PhotoScroller, also pulls images from network.
* [dhoerl/htmlcxx](https://github.com/dhoerl/htmlcxx) - a simple non-validating css1 and html parser written in C++ tuned for iOS and Mac
* [dhuertas/AES](https://github.com/dhuertas/AES) - AES algorithm implementation in C
* [dianping/camel](https://github.com/dianping/camel) - camel: soft load balance(slb) middle ware - control nginx servers by portal and api.
* [diegocr/netcat](https://github.com/diegocr/netcat) - NetCat for Windows
* [digidotcom/xbee_ansic_library](https://github.com/digidotcom/xbee_ansic_library) - A collection of portable ANSI C code for communicating with Digi International's XBee wireless radio modules in API mode.
* [dimkr/szl](https://github.com/dimkr/szl) - A lightweight, embeddable scripting language
* [dinhviethoa/libetpan](https://github.com/dinhviethoa/libetpan) - Mail Framework for C Language
* [diwu/CCB-X-Reader](https://github.com/diwu/CCB-X-Reader) - This C++ class helps processing CocosBuilder(ccb) files for your Cocos2d-X project.
* [dizballanze/hashtable](https://github.com/dizballanze/hashtable) - Async hash table server in C
* [djcb/mu](https://github.com/djcb/mu) - maildir indexer/searcher + emacs mail client + guile bindings
* [djhworld/gomeboycolor](https://github.com/djhworld/gomeboycolor) - Gameboy Color emulator
* [dlundquist/sniproxy](https://github.com/dlundquist/sniproxy) - Proxies incoming HTTP and TLS connections based on the hostname contained in the initial request of the TCP session.
* [dmage/co2mon](https://github.com/dmage/co2mon) - CLI for MasterKit CO2 Monitor
* [dminor/skip-quadtree](https://github.com/dminor/skip-quadtree) - Implementation of the skip quadtree and compressed quadtree data structures.
* [dmw/caffeine](https://github.com/dmw/caffeine) - C Application Framework
* [doches/progressbar](https://github.com/doches/progressbar) - An easy-to-use C library for displaying text progress bars.
* [docileninja/ctf_import](https://github.com/docileninja/ctf_import) - Run basic functions from stripped binaries cross platform
* [docopt/docopt.c](https://github.com/docopt/docopt.c) - C-code generator for docopt language.
* [dogriffiths/HeadFirstC](https://github.com/dogriffiths/HeadFirstC) - Source code for the book Head First C, by O'Reilly Media
* [dokan-dev/dokany](https://github.com/dokan-dev/dokany) - User mode file system library for windows with FUSE Wrapper
* [dolaameng/pysax](https://github.com/dolaameng/pysax) - python implementation of SAX (Symbolic Aggregate Approximation) for time series data
* [domoran/DriveDOORS](https://github.com/domoran/DriveDOORS) - An efficient data Interface to IBM Rational DOORS
* [dorimanx/exfat-nofuse](https://github.com/dorimanx/exfat-nofuse) - Android ARM Linux non-fuse read/write kernel driver for exFat and VFat Android file systems
* [dosgo/ngrok-c](https://github.com/dosgo/ngrok-c) - ngrok client for c language,Due to the use of GO ngrok language development, porting to embedded devices some inconvenience, such as openwrt, so use C language rewrite a client. Very mini, the need to support polarssl library.
* [douban/beansdb](https://github.com/douban/beansdb) - Yet anonther distributed key-value storage system from Douban Inc.
* [douban/greenify](https://github.com/douban/greenify) - Make blocking C library work with gevent
* [dougbradbury/cslim](https://github.com/dougbradbury/cslim) - Fitnesse Slim implementation in C
* [douglascrockford/DEC64](https://github.com/douglascrockford/DEC64) - Decimal floating point
* [douglascrockford/JSMin](https://github.com/douglascrockford/JSMin) - JavaScript Minification Filter
* [douzzer/megaqueue](https://github.com/douzzer/megaqueue) - lightweight high performance streaming data kernel
* [dovecot/core](https://github.com/dovecot/core) - Dovecot mail server
* [dpage/redis_fdw](https://github.com/dpage/redis_fdw) - A PostgreSQL foreign data wrapper for Redis
* [dpfau/quagga](https://github.com/dpfau/quagga) - Library for automated ROI extraction from calcium imaging data
* [dpryan79/MethIndelRealigner](https://github.com/dpryan79/MethIndelRealigner) - A local realigner around InDels for MethylSeq data
* [draco2003/freebsd-database-riak](https://github.com/draco2003/freebsd-database-riak) - FreeBSD port for riak support
* [dreamsxin/cphalcon7](https://github.com/dreamsxin/cphalcon7) - Phalcon7 - Web framework for PHP7.x 高性能PHP7框架
* [drh/cii](https://github.com/drh/cii) - C Interfaces and Implementations
* [drh/lcc](https://github.com/drh/lcc) - The lcc retargetable ANSI C compiler
* [droe/sslsplit](https://github.com/droe/sslsplit) - Transparent SSL/TLS interception
* [dropbox/miniutf](https://github.com/dropbox/miniutf) - A C++ library for basic Unicode manipulation.
* [drotiro/postpic](https://github.com/drotiro/postpic) - PostPic is an extension for the open source dbms PostgreSQL that enables image processing inside the database, like PostGIS does for spatial data. It adds the new 'image' type to the SQL, and several functions to process images and to extract their attributes.
* [drvink/epanos](https://github.com/drvink/epanos) - ElectroPaint Automatic No-source Object reaSsembler (a MIPS to C decompiler)
* [dryman/opic](https://github.com/dryman/opic) - Fast serialization framework for C
* [dtb/algorithms-and-data-structures](https://github.com/dtb/algorithms-and-data-structures) - Wherein I fill in the gaps in my programming knowledge
* [dtrace4linux/linux](https://github.com/dtrace4linux/linux) - dtrace for linux - kernel driver and userland tools
* [duckythescientist/obfuscatedLife](https://github.com/duckythescientist/obfuscatedLife) - Conway's Game of Life in 9 lines of C
* [dunst-project/dunst](https://github.com/dunst-project/dunst) - Lightweight and customizable notification daemon
* [dutc/generators](https://github.com/dutc/generators) - Generators for Stream Data Processing, or Generator Showcase Showdown
* [dvidelabs/flatcc](https://github.com/dvidelabs/flatcc) - FlatBuffers Compiler and Library in C for C
* [dvorka/hstr](https://github.com/dvorka/hstr) - Bash and zsh shell history suggest box - easily view, navigate, search and manage your command history.
* [dxjia/ffmpeg-commands-executor-library](https://github.com/dxjia/ffmpeg-commands-executor-library) - execute ffmpeg commands through a jni shared library.
* [dxjia/ffmpeg-compile-shared-library-for-android](https://github.com/dxjia/ffmpeg-compile-shared-library-for-android) - 移植ffmpeg到android，编译可用于jni调用的so库.
* [dynup/kpatch](https://github.com/dynup/kpatch) - kpatch - dynamic kernel patching
* [dyu/ffi-overhead](https://github.com/dyu/ffi-overhead) - comparing the c ffi (foreign function interface) overhead on various programming languages
* [eaccelerator/eaccelerator](https://github.com/eaccelerator/eaccelerator) - eAccelerator PHP opcode cache
* [eam/libcrange](https://github.com/eam/libcrange) - Range parsing library for managing sets of hostnames, ips, clusters, roles and other operational data.
* [earthquake/chw00t](https://github.com/earthquake/chw00t) - chw00t - Unices chroot breaking tool
* [easydatawarehousing/easy2oracle](https://github.com/easydatawarehousing/easy2oracle) - Easy-To-Oracle is a data integration tool. It can pull data from databases like Microsoft SQL Server, MySQL, Sybase, SQLite, Presto (Hadoop) and Excel directly into your Oracle 10g/11g/12c database
* [eatnumber1/goal](https://github.com/eatnumber1/goal) - g()()()()('al') → "gooooal"
* [ebassi/graphene](https://github.com/ebassi/graphene) - A thin layer of graphic data types
* [eclipse/paho.mqtt.c](https://github.com/eclipse/paho.mqtt.c) - paho.mqtt.c
* [eclipse/paho.mqtt.embedded-c](https://github.com/eclipse/paho.mqtt.embedded-c) - paho.mqtt.embedded-c
* [eclipse/wakaama](https://github.com/eclipse/wakaama) - Eclipse Wakaama (formerly liblwm2m) is an implementation of the Open Mobile Alliance's LightWeight M2M protocol (LWM2M).
* [edenhill/librdkafka](https://github.com/edenhill/librdkafka) - The Apache Kafka C/C++ library
* [editorconfig/editorconfig-core-c](https://github.com/editorconfig/editorconfig-core-c) - EditorConfig core library written in C (for use by plugins supporting EditorConfig parsing)
* [edoko/AIR-Kernel_ICS](https://github.com/edoko/AIR-Kernel_ICS) - AIR Kernel for ICS (r_data / edoko)
* [edorfaus/TEMPered](https://github.com/edorfaus/TEMPered) - C library and program for reading the TEMPer family of thermometer and hygrometer devices.
* [eduard-permyakov/permafrost-engine](https://github.com/eduard-permyakov/permafrost-engine) - An OpenGL 3.3 RTS game engine written in C
* [eduardsui/tlse](https://github.com/eduardsui/tlse) - Single C file TLS 1.2/1.3 implementation, using tomcrypt as crypto library
* [edussx/database](https://github.com/edussx/database) - B+tree database
* [eeertekin/bbcp](https://github.com/eeertekin/bbcp) - Securely and quickly copy data from source to target.
* [efelix/lua-cjson](https://github.com/efelix/lua-cjson) - Fast JSON parsing and encoding support for Lua
* [eggheads/eggdrop](https://github.com/eggheads/eggdrop) - The Eggdrop IRC Bot
* [einsteinx2/libSub](https://github.com/einsteinx2/libSub) - Internal library used by iSub, encapsulates the data model and audio engine. Licensed under the GPL3.
* [ejoy/ejoy2d](https://github.com/ejoy/ejoy2d) - A 2D Graphics Engine for Mobile Game
* [ejurgensen/forked-daapd](https://github.com/ejurgensen/forked-daapd) - Linux/FreeBSD DAAP (iTunes) and MPD media server with support for AirPlay devices (multiroom), Apple Remote (and compatibles), Chromecast, Spotify and internet radio.
* [eleme/corvus](https://github.com/eleme/corvus) - A fast and lightweight Redis Cluster Proxy for Redis 3.0
* [elliotwoods/ARDrone-GStreamer-test](https://github.com/elliotwoods/ARDrone-GStreamer-test) - Test of reading video data from ARDrone using GStreamer (cross-platform code, win32 project)
* [ellson/graphviz](https://github.com/ellson/graphviz) - Graph Visualization Tools
* [elua/elua](https://github.com/elua/elua) - eLua Project on GitHub
* [elvismt/slope](https://github.com/elvismt/slope) - A library to create charts from raw data using cairo. Can be shown in GtkDrawingArea
* [emacsattic/doxymacs](https://github.com/emacsattic/doxymacs) - Code to efficiently read/write XML data with Elisp --- IN ATTIC BECAUSE: import problems
* [embedthis/appweb](https://github.com/embedthis/appweb) - Appweb Embedded Web Server
* [embox/embox](https://github.com/embox/embox) - Modular and configurable OS kernel for embedded applications
* [emeau/itrace](https://github.com/emeau/itrace) - hook objc_msgSend to trace Objective-C method callz
* [emgram769/lighthouse](https://github.com/emgram769/lighthouse) - A simple scriptable popup dialog to run on X.
* [emilk/wfc](https://github.com/emilk/wfc) - A C++ port of Wave Function Collapse Tiling
* [emptyhua/baidu_pcs_cli](https://github.com/emptyhua/baidu_pcs_cli) - 百度个人云存储API命令行工具
* [emrainey/OpenCL-Environment](https://github.com/emrainey/OpenCL-Environment) - A series of utilities aimed at making OpenCL easier to use. Includes clCompiler which generates both binary outputs and precompiled headers which can be used in conjunction with clEnvironment. clQuery allows you to print all known information about a OpenCL data type. clPid, clYUV clImgFilter are all examples of how to use the utilities to create a compile time kernel make it a dependency in you makefiles and then use the clEnvironment to call your kernel.
* [emsec/ChameleonMini](https://github.com/emsec/ChameleonMini) - The ChameleonMini is a versatile contactless smartcard emulator compliant to NFC. To support our project, buy it here: https://shop.kasper.it. For further information see the Getting Started Page https://rawgit.com/emsec/ChameleonMini/master/Doc/Doxygen/html/_page__getting_started.html or the Wiki tab above.
* [emweb/wt](https://github.com/emweb/wt) - Wt, C++ Web Toolkit
* [encog/encog-c](https://github.com/encog/encog-c) - The Encog project for C/C++
* [energinet/datalogger-client](https://github.com/energinet/datalogger-client) - Energinet Datalogger
* [energinet/datalogger-server](https://github.com/energinet/datalogger-server) - rpserver.cgi
* [eos-org/datastructures](https://github.com/eos-org/datastructures) - PHP extensions for classes supporting common datastructures
* [epico/libibuspinyin-compat](https://github.com/epico/libibuspinyin-compat) - compatible files for ibus-pinyin and libpinyin integration.
* [ericfischer/datamaps](https://github.com/ericfischer/datamaps) - Indexes points and lines and generates map tiles to display them
* [ericfischer/geotools](https://github.com/ericfischer/geotools) - Tools for working with geographic data
* [ericmandel/funtools](https://github.com/ericmandel/funtools) - A "minimal buy-in" FITS library and utility package for astronomical data analysis
* [erikd/libsndfile](https://github.com/erikd/libsndfile) - A C library for reading and writing sound files containing sampled audio data..
* [erikfrey/bashreduce](https://github.com/erikfrey/bashreduce) - mapreduce in bash
* [erikkaashoek/Comskip](https://github.com/erikkaashoek/Comskip) - A free commercial detector
* [eriksvedang/Carp](https://github.com/eriksvedang/Carp) - a statically typed lisp, without a GC, for high performance applications
* [erimatnor/libckit](https://github.com/erimatnor/libckit) - A kit of C-based utilities and data structures.
* [esden/ppm_to_spektrum_encoder](https://github.com/esden/ppm_to_spektrum_encoder) - An atmega based board converting standard servo data to spektrum satellite serial protocol for use with Paparazzi
* [esheldon/meds](https://github.com/esheldon/meds) - Python and C libraries to work with Multi Epoch Data Structures
* [esneider/debug](https://github.com/esneider/debug) - Debugging like a sir (in C)
* [esnme/ultrajson](https://github.com/esnme/ultrajson) - Ultra fast JSON decoder and encoder written in C with Python bindings
* [esnme/ultramysql](https://github.com/esnme/ultramysql) - A fast MySQL driver written in pure C/C++ for Python. Compatible with gevent through monkey patching.
* [espruino/Espruino](https://github.com/espruino/Espruino) - The Espruino JavaScript interpreter - Official Repo
* [ethz-asl/asctec_mav_framework](https://github.com/ethz-asl/asctec_mav_framework) - Framework for data aquisition and position control to be used with the highlevel processor of Ascending Technologies helicopters
* [etlegacy/etlegacy](https://github.com/etlegacy/etlegacy) - ET: Legacy is based on the source code of the Wolfenstein: Enemy Territory which was released under the GPLv3 license. The main goal of this project is to fix bugs, remove old dependencies and make it playable on all major operating systems while still remaining compatible with the ET 2.60b version and as many of its mods as possible.
* [etmc/lemon](https://github.com/etmc/lemon) - Lemon is an MPI parallel I/O library that is intended to allow for efficient parallel I/O of both binary and metadata on massively parallel architectures. Data is stored in the SciDAC Lattice QCD Interchange Message Encapsulation format, that allows for storing large blocks of binary data and corresponding metadata in the same file.
* [etolabo/kumofs](https://github.com/etolabo/kumofs) - kumofs is a scalable and highly available distributed key-value store.
* [eudoxia0/magma](https://github.com/eudoxia0/magma) - Extending C with cmacro
* [evan/memcached](https://github.com/evan/memcached) - A Ruby interface to the libmemcached C client
* [evanmiller/ProjCL](https://github.com/evanmiller/ProjCL) - Crazy-fast map projections and geodesic calculations
* [evanmiller/nginx_circle_gif](https://github.com/evanmiller/nginx_circle_gif) - Serve 68,000 round corners per second
* [everettjf/AppleTrace](https://github.com/everettjf/AppleTrace) - Objective C message tracing tool for iOS/macOS
* [eweitnauer/minstreamer](https://github.com/eweitnauer/minstreamer) - Simple audio (n to n) and video (1 to n) streaming in C using libgstreamer.
* [examplecode/mproxy](https://github.com/examplecode/mproxy) - c 语言实现的一个最小的http代理，支持翻墙
* [exosite-garage/arduino_http_post](https://github.com/exosite-garage/arduino_http_post) - Demo of Arduino hardware sending data to the cloud.  It is a simple web based monitoring example for Arduino - really easy to put values captured by Arduino online .
* [explosion/lightnet](https://github.com/explosion/lightnet) - 🌓 Bringing pjreddie's DarkNet out of the shadows #yolo
* [ext/datapack](https://github.com/ext/datapack) - Testing compression and storage of data inside executable
* [f9micro/f9-kernel](https://github.com/f9micro/f9-kernel) - An efficient and secure microkernel built for ARM Cortex-M cores, inspired by L4
* [fabianishere/brainfuck](https://github.com/fabianishere/brainfuck) - Brainfuck interpreter written in C
* [fabiensanglard/chocolate_duke3D](https://github.com/fabiensanglard/chocolate_duke3D) - chocolate Duke Nukem,3D
* [face/MongooseDaemon](https://github.com/face/MongooseDaemon) - An objective-c wrapper for embedding the mongoose http web server in iPhone apps
* [facebook/360-Capture-SDK](https://github.com/facebook/360-Capture-SDK) - A developer focused sample SDK that allows game and virtual Reality devs to be able to easily and quickly integrate 360 photo/video capture capability into their game apps.
* [facebook/css-layout](https://github.com/facebook/css-layout) - A subset of CSS (specifically flex-box) re-implemented as a stand alone project for use primarily on mobile. Used by react-native
* [facebook/fb-adb](https://github.com/facebook/fb-adb) - A better shell for Android devices
* [facebook/fishhook](https://github.com/facebook/fishhook) - A library that enables dynamically rebinding symbols in Mach-O binaries running on iOS.
* [facebook/flashcache](https://github.com/facebook/flashcache) - A general purpose, write-back block cache for Linux.
* [facebook/liblogfaf](https://github.com/facebook/liblogfaf) - A library that logs messages using non-blocking UDP datagrams.
* [facebook/libphenom](https://github.com/facebook/libphenom) - An eventing framework for building high performance and high scalability systems in C.
* [facebook/watchman](https://github.com/facebook/watchman) - Watches files and records, or triggers actions, when they change.
* [facebookresearch/SparseConvNet](https://github.com/facebookresearch/SparseConvNet) - Submanifold sparse convolutional networks
* [falconindy/expac](https://github.com/falconindy/expac) - alpm data extraction utility
* [falkTX/Cadence](https://github.com/falkTX/Cadence) - Collection of tools useful for audio production
* [fanchy/fflib](https://github.com/fanchy/fflib) - FFLib is a lightweight c++ framework.FFlib is mainly designed for game server developing. But some components in FFLib is in common use. For example socket&net module, log module, thread&lock, tools for performance & memory leak check.用于分布式程序的c++类库，封装了socket、rpc、lua、CQRS框架、算法等组件，适于SNS、WEBGAME、MMO后台程序， about C++,linux socket,lua,rpc,broker,cqrs,timer,log libary
* [fancycode/MemoryModule](https://github.com/fancycode/MemoryModule) - Library to load a DLL from memory.
* [fanglingsu/vimb](https://github.com/fanglingsu/vimb) - Vimb - the vim like browser is a webkit based web browser that behaves like the vimperator plugin for the firefox and usage paradigms from the great editor vim. The goal of vimb is to build a completely keyboard-driven, efficient and pleasurable browsing-experience.
* [faragon/libsrt](https://github.com/faragon/libsrt) - libsrt is a C library for writing fast and safe C code, faster. It provides string, vector, bit set, set, map, hash set, and hash map handling. Suitable for soft and hard real-time. Allows both heap and stack allocation.  *BETA* (API still can change: suggestions are welcome)
* [farsightsec/dnstable](https://github.com/farsightsec/dnstable) - encoding format, library, and utilities for passive DNS data
* [fastos/fastsocket](https://github.com/fastos/fastsocket) - Fastsocket is a highly scalable socket and its underlying networking implementation of Linux kernel. With the straight linear scalability, Fastsocket can provide extremely good performance in multicore machines. In addition, it is very easy to use and maintain. As a result, it has been deployed in the production environment of SINA.
* [fcitx/fcitx](https://github.com/fcitx/fcitx) - A Flexible Input Method Framework
* [feeley/gambit](https://github.com/feeley/gambit) - Gambit is an efficient implementation of the Scheme programming language.
* [felipec/msn-pecan](https://github.com/felipec/msn-pecan) - MSN Messenger library in C
* [felis/Arduino_Camera_Control](https://github.com/felis/Arduino_Camera_Control) - PTP, Camera-specific layers to work with Arduino USB Host Shield
* [felixangell/mac](https://github.com/felixangell/mac) - virtual machine in c
* [felselva/mathc](https://github.com/felselva/mathc) - Pure C math library for 2D and 3D programming.
* [ferreiradaselva/mathc](https://github.com/ferreiradaselva/mathc) - Pure C math library for 2D and 3D programming
* [ffi/ffi](https://github.com/ffi/ffi) - Ruby FFI
* [fi01/CVE-2015-3636](https://github.com/fi01/CVE-2015-3636) - PoC code for 32 bit Android OS
* [fictorial/logstore](https://github.com/fictorial/logstore) - experimental data storage engine for arbitrary data for POSIX systems with spinning hard disks
* [fileability/Ingredients](https://github.com/fileability/Ingredients) - A Cocoa documentation viewer.
* [fileability/chocolat-public](https://github.com/fileability/chocolat-public) - Public bug tracker for the private chocolat project
* [fileability/self-ml](https://github.com/fileability/self-ml) - A human data language
* [firmianay/CTF-All-In-One](https://github.com/firmianay/CTF-All-In-One) - 一本 CTF 书
* [fiveruns/memcache-client](https://github.com/fiveruns/memcache-client) - Seattle.rb's memcache-client 1.5.0 with fixes
* [fjz13/Cocos2d-x-ParticleEditor-for-Windows](https://github.com/fjz13/Cocos2d-x-ParticleEditor-for-Windows) - A FREE WINDOWS cocos2d particle editor Upgraded to Cocos2dx 2.12，and support saving texture into plist。  Welcome any suggestions,or join me.  Jack Fu(傅建钊） fjz13@live.cn QQ:2722937652  http://weibo.com/u/1847201447
* [fletcher/MultiMarkdown-4](https://github.com/fletcher/MultiMarkdown-4) - C implementation of MultiMarkdown; almost complete rewrite of MMD 3 (which was aka "peg-multimarkdown").
* [flightcrank/ratio-boost](https://github.com/flightcrank/ratio-boost) - This program spoofs or fakes the amount of data torrent clients report to private torrent trackers in order to maintain a good ratio of data uploads to downloads, which they require.
* [floooh/chips](https://github.com/floooh/chips) - 8-bit chip and system emulators in standalone C headers
* [floooh/sokol](https://github.com/floooh/sokol) - minimal cross-platform standalone C headers
* [flori/amatch](https://github.com/flori/amatch) - Approximate String Matching library
* [fluent/fluent-bit](https://github.com/fluent/fluent-bit) - Fast and Lightweight Log processor and forwarder for Linux, BSD and OSX
* [fluent/nginx-fluentd-module](https://github.com/fluent/nginx-fluentd-module) - Nginx module for Fluentd data collector
* [fmahnke/orxCraft](https://github.com/fmahnke/orxCraft) - Experimental data configuration editor for the Orx/Scroll game engine. C++
* [fmela/libdict](https://github.com/fmela/libdict) - C library of key-value data structures with an object-oriented interface.
* [fnordware/AdobeWebM](https://github.com/fnordware/AdobeWebM) - WebM plug-ins for Adobe programs
* [fogleman/Craft](https://github.com/fogleman/Craft) - A simple Minecraft clone written in C using modern OpenGL (shaders).
* [foldedtoad/PebblePointer](https://github.com/foldedtoad/PebblePointer) - Sending Pebble Watch accelerometer data to an Android app -- See wiki
* [fomy/destor](https://github.com/fomy/destor) - An experimental platform for chunk-level data deduplication. Key words: DDFS, Sparse Index, Extreme Binning, SiLo, Sample Index, BLC; CBR, CFL, CAP, HAR; ASM, OPT; GC, Cumulus
* [fontforge/fontforge](https://github.com/fontforge/fontforge) - Free (libre) font editor for Windows, Mac OS X and GNU+Linux
* [fontforge/libuninameslist](https://github.com/fontforge/libuninameslist) - A library with a large (sparse) array mapping each unicode code point to the annotation data for it provided in http://www.unicode.org/Public/UNIDATA/NamesList.txt
* [foool/Z-code](https://github.com/foool/Z-code) - A family of XOR erasure codes with optimal repair bandwidth for a single data node failure
* [forhappy/cpy-leveldb](https://github.com/forhappy/cpy-leveldb) - python bingding for leveldb using c api
* [fragglet/c-algorithms](https://github.com/fragglet/c-algorithms) - A library of common data structures and algorithms written in C.
* [fragglet/yoctolisp](https://github.com/fragglet/yoctolisp) - Tiny Scheme-like Lisp interpreter written in a weekend
* [franckverrot/git_fdw](https://github.com/franckverrot/git_fdw) - PostgreSQL Git Foreign Data Wrapper
* [franckverrot/holycorn](https://github.com/franckverrot/holycorn) - PostgreSQL multi-purpose Ruby data wrapper
* [franko/regress-pro](https://github.com/franko/regress-pro) - Spectroscopic Ellipsometry and Reflectometry data analysis
* [freaklabs/chibiArduino](https://github.com/freaklabs/chibiArduino) - A lightweight 802.15.4 wireless protocol stack for Arduino
* [freddiev4/DailyProgrammerChallenges](https://github.com/freddiev4/DailyProgrammerChallenges) - External Repo of Challenges from r/dailyprogrammer
* [fredrik-johansson/arb](https://github.com/fredrik-johansson/arb) - C library for arbitrary-precision interval arithmetic
* [fredrikbk/libpack](https://github.com/fredrikbk/libpack) - Library that packs/serializes or unpacks/deserializes user-defined data layouts. The data layouts are specified using datatypes similar to MPI Datatypes. The library compiles the datatypes into efficient vectorized pack/unpack code at commit time using an LLVM-based online compiler.
* [freebsd/crochet](https://github.com/freebsd/crochet) - Build FreeBSD images for RaspberryPi, BeagleBone, PandaBoard, and others.
* [freebsd/freebsd](https://github.com/freebsd/freebsd) - FreeBSD src tree
* [freebsd/pkg](https://github.com/freebsd/pkg) - Package management tool for FreeBSD. Help at #pkgng on Freenode or pkg@FreeBSD.org
* [freefoote/gpscorrelate](https://github.com/freefoote/gpscorrelate) - Abandoned C program to match GPS tracks to photographs, and store the matches in the EXIF data in the photographs.
* [freels/ruby_trie](https://github.com/freels/ruby_trie) - Native C implementation of a trie data structure.
* [freifunk-gluon/gluon](https://github.com/freifunk-gluon/gluon) - a modular framework for creating OpenWrt-based firmwares for wireless mesh nodes
* [freshcode/MFMathLib](https://github.com/freshcode/MFMathLib) - A mathematical library providing basic math operations on data types from 8-bits to 1024-bits with overflow/underflow tracking.
* [freshplanet/ANE-Chartboost](https://github.com/freshplanet/ANE-Chartboost) - Air Native Extension for Chartboost (iOS + Android)
* [frida/frida-core](https://github.com/frida/frida-core) - Frida core library intended for static linking into bindings
* [fritz0705/libf](https://github.com/fritz0705/libf) - Library to make programming simpler and cleaner (and slower, because I was too lazy to implement usable data structures)
* [frobware/cmd-key-happy](https://github.com/frobware/cmd-key-happy) - Swap cmd and alt keys in Terminal (useful when running emacs over ssh)
* [frodosens/fsnet](https://github.com/frodosens/fsnet) - 一个c+ruby支持分布式部署开源的网络游戏库
* [fubarwrangler/datastruct](https://github.com/fubarwrangler/datastruct) - A silly project to code some data structures to help brush up on my C
* [fukuchi/libqrencode](https://github.com/fukuchi/libqrencode) - QR Code encoding library
* [fusijie/Airplane_3.0](https://github.com/fusijie/Airplane_3.0) - Wechat Airplane C++ version, powered by Cocos2d-x 3.0 stable version.
* [fuzxxl/memf](https://github.com/fuzxxl/memf) - Portable scanf/printf-like functions to marshal binary data
* [fw42/nfportscan](https://github.com/fw42/nfportscan) - Tool for analyzing Cisco netflow data in order to automatically detect portscans
* [fygrave/moloch_zmq](https://github.com/fygrave/moloch_zmq) - ZMQ data explort plugin for Moloch
* [gabomdq/SDL_GameControllerDB](https://github.com/gabomdq/SDL_GameControllerDB) - A community sourced database of game controller mappings to be used with SDL2 Game Controller functionality
* [gabriel/yajl-objc](https://github.com/gabriel/yajl-objc) - Objective-C bindings for YAJL (Yet Another JSON Library) C library
* [galkahana/PDF-Writer](https://github.com/galkahana/PDF-Writer) - High performance library for creating, modiyfing and parsing PDF files in C++
* [gallir/concurrencia](https://github.com/gallir/concurrencia) - Códigos fuente del libro "Principios y algoritmos de concurrencia"
* [gallir/concurrencia_source_samples](https://github.com/gallir/concurrencia_source_samples) - Códigos fuente del libro "Principios y algoritmos de concurrencia"
* [gamefreak/Athena](https://github.com/gamefreak/Athena) - Data editor for Xsera, Antares, and Ares
* [gamelinux/passivedns](https://github.com/gamelinux/passivedns) - A network sniffer that logs all DNS server replies for use in a passive DNS setup
* [gameoverhack/ofxOpenNI](https://github.com/gameoverhack/ofxOpenNI) - Wrapper for OpenNI, NITE and SensorKinect
* [ganglia/monitor-core](https://github.com/ganglia/monitor-core) - Ganglia Monitoring core
* [garrynewman/GWEN](https://github.com/garrynewman/GWEN) - GWEN - GUI Without Extravagant Nonsense
* [garthz/pdwiringPi](https://github.com/garthz/pdwiringPi) - Pure Data (pd) external for hardware I/O on a Raspberry Pi using wiringPi.
* [gbishop/cython-hidapi](https://github.com/gbishop/cython-hidapi) - Python wrapper for the hidapi (not active, use one of the forks)
* [gcesarmza/curl-android-ios](https://github.com/gcesarmza/curl-android-ios) - Static libcurl to be used in Android and iOS apps. Build scripts included. No Android source required
* [gdbinit/ExtractMachO](https://github.com/gdbinit/ExtractMachO) - IDA plugin to extract Mach-O binaries located in the disassembly or data
* [gdbinit/onyx-the-black-cat](https://github.com/gdbinit/onyx-the-black-cat) - Kernel extension to disable anti-debug tricks and other useful XNU "features"
* [ge-ne/bibtool](https://github.com/ge-ne/bibtool) - BibTool is a tool for manipulating BibTeX data bases. BibTeX provides a mean to integrate citations into LaTeX documents. BibTool allows the manipulation of BibTeX files which goes beyond the possibilities -- and intentions -- of BibTeX.
* [geany/geany](https://github.com/geany/geany) - A fast and lightweight IDE
* [geertj/cgreenlet](https://github.com/geertj/cgreenlet) - Coroutines for C/C++
* [gentilkiwi/kekeo](https://github.com/gentilkiwi/kekeo) - A little toolbox to play with Microsoft Kerberos in C
* [gentilkiwi/mimikatz](https://github.com/gentilkiwi/mimikatz) - A little tool to play with Windows security
* [gentoo/eudev](https://github.com/gentoo/eudev) - Repository for eudev development
* [geocommons/geocoder](https://github.com/geocommons/geocoder) - Modular Street Address Geocoder
* [geoffgarside/cocoagit](https://github.com/geoffgarside/cocoagit) - An Objective-C/Foundation implementation of the Git version control software.
* [geon/gloss](https://github.com/geon/gloss) - A bidirectional path tracer written in C.
* [ggasoftware/indigo](https://github.com/ggasoftware/indigo) - Indigo: a cheminformatics toolkit. Bingo: RDBMS data cartridge for Oracle, MS SQL Server, and PostgreSQL
* [ggobi/ggobi](https://github.com/ggobi/ggobi) - High dimensional data vis
* [ggounot/BnfData](https://github.com/ggounot/BnfData) - Android Application: Auteurs et œuvres
* [ggreer/the_silver_searcher](https://github.com/ggreer/the_silver_searcher) - A code-searching tool similar to ack, but faster.
* [ghosert/VimProject](https://github.com/ghosert/VimProject) - All about my vim projects
* [ghostrong/algorithm](https://github.com/ghostrong/algorithm) - Data Structure and Algorithms
* [ghughes/fruitstrap](https://github.com/ghughes/fruitstrap) - Install and debug iPhone apps from the command line, without using Xcode
* [gianlucabertani/Objective-Zip](https://github.com/gianlucabertani/Objective-Zip) - An object-oriented friendly wrapper library for ZLib and MiniZip, in Objective-C for iOS and OS X
* [gibranfp/Sampled-MinHashing](https://github.com/gibranfp/Sampled-MinHashing) - MinHash-based clustering for binary and weighted dyadic data (e.g. bag of words).
* [gilbo/cork](https://github.com/gilbo/cork) - 3D Boolean / CSG Library
* [giltene/wrk2](https://github.com/giltene/wrk2) - A constant throughput, correct latency recording variant of wrk
* [ging/licode](https://github.com/ging/licode) - Open Source Communication Provider based on WebRTC and Cloud technologies
* [gingerBill/gb](https://github.com/gingerBill/gb) - gb single-file public domain libraries for C & C++
* [ginsweater/gif-h](https://github.com/ginsweater/gif-h) - Simple C++ one-header library for the creation of animated GIFs from image data.
* [git-mirror/nginx](https://github.com/git-mirror/nginx) - A mirror of the nginx SVN repository.
* [git/git](https://github.com/git/git) - Git Source Code Mirror - This is a publish-only repository and all pull requests are ignored. Please follow Documentation/SubmittingPatches procedure for any of your improvements.
* [githole/Live-Coder](https://github.com/githole/Live-Coder) - Live Coder is a realtime GLSL editor/viewer mainly for demosceners.
* [github/brubeck](https://github.com/github/brubeck) - A Statsd-compatible metrics aggregator
* [gittup/tup](https://github.com/gittup/tup) - Tup is a file-based build system.
* [gjedeer/tuntox](https://github.com/gjedeer/tuntox) - Tunnel TCP connections over the Tox protocol
* [gkaindl/ambi-tv](https://github.com/gkaindl/ambi-tv) - a flexible ambilight clone for embedded linux
* [gleicon/leveldb_engine](https://github.com/gleicon/leveldb_engine) - memcached leveldb engine - stores data on leveldb
* [gleu/sqlite_fdw](https://github.com/gleu/sqlite_fdw) - Foreign Data Wrapper for sqlite
* [glock45/iOS-Hierarchy-Viewer](https://github.com/glock45/iOS-Hierarchy-Viewer) - iOS Hierarchy viewer - View and Coredata debugging made easy
* [glouw/tinn](https://github.com/glouw/tinn) - The tiny neural network library
* [gluster/glusterfs](https://github.com/gluster/glusterfs) - Gluster Filesystem - (this is only a public mirror)
* [glyptodon/guacamole-server](https://github.com/glyptodon/guacamole-server) - The server-side, native components that form the Guacamole proxy.
* [gnea/grbl](https://github.com/gnea/grbl) - An open source, embedded, high performance g-code-parser and CNC milling controller written in optimized C that will run on a straight Arduino
* [gnemoug/data_structure](https://github.com/gnemoug/data_structure) - 关于各种数据结构和算法的一些收录
* [gnome-mpv/gnome-mpv](https://github.com/gnome-mpv/gnome-mpv) - A simple GTK+ frontend for mpv
* [gnosek/nginx-upstream-fair](https://github.com/gnosek/nginx-upstream-fair) - The fair load balancer module for nginx
* [gnu-mcu-eclipse/eclipse-plugins](https://github.com/gnu-mcu-eclipse/eclipse-plugins) - The GNU MCU Eclipse plug-ins for ARM & RISC-V C/C++ developers
* [gnudennis/ds_c](https://github.com/gnudennis/ds_c) - Data Structure In C
* [go-vgo/robotgo](https://github.com/go-vgo/robotgo) - RobotGo, Go Native cross-platform GUI automation
* [gogotanc/DataStructures](https://github.com/gogotanc/DataStructures) - Data Structures and Algorithm Analysis in C
* [goj/coreutils](https://github.com/goj/coreutils) - fork of GNU coreutils package
* [gokhankici/orc_fdw](https://github.com/gokhankici/orc_fdw) - PostgreSQL extension which implements a Foreign Data Wrapper (FDW) for ORC files.
* [golang-ui/nuklear](https://github.com/golang-ui/nuklear) - This project provides Go bindings for nuklear.h — a small ANSI C GUI library.
* [google/capsicum-linux](https://github.com/google/capsicum-linux) - Linux kernel with Capsicum support
* [google/clspv](https://github.com/google/clspv) - Clspv is a prototype compiler for a subset of OpenCL C to Vulkan compute shaders
* [google/cpu_features](https://github.com/google/cpu_features) - A cross platform C99 library to get cpu features at runtime.
* [google/cronutils](https://github.com/google/cronutils) - utilities to assist running batch processing jobs
* [google/eddystone](https://github.com/google/eddystone) - Specification for Eddystone, an open beacon format from Google
* [google/google-ctf](https://github.com/google/google-ctf) - Google CTF
* [google/honggfuzz](https://github.com/google/honggfuzz) - Security oriented fuzzer with powerful analysis options. Supports evolutionary, feedback-driven fuzzing based on code coverage (software- and hardware-based)
* [google/ios-webkit-debug-proxy](https://github.com/google/ios-webkit-debug-proxy) - A DevTools proxy (WebKit Remote Debugging Protocol) for iOS devices (Safari Remote Web Inspector).
* [google/ktsan](https://github.com/google/ktsan) - ThreadSanitizer for Linux kernel, a fast data race detector
* [google/latency-benchmark](https://github.com/google/latency-benchmark) - Tests web browser input latency and jank
* [google/snappy-start](https://github.com/google/snappy-start) - Tool for launching a Linux process from a snapshot
* [google/upb](https://github.com/google/upb) - a small protobuf implementation in C
* [gopro/cineform-sdk](https://github.com/gopro/cineform-sdk) - The GoPro® CineForm video codec SDK.
* [gosexy/canvas](https://github.com/gosexy/canvas) - Image manipulation library based on ImageMagick's MagickWand, for Go.
* [gosu/gosu](https://github.com/gosu/gosu) - 2D game development library for Ruby and C++
* [gozfree/libraries](https://github.com/gozfree/libraries) - Basic libraries all written in c by gozfree, including network, event, config, log, hash, ipc, rpc, mem,  and so on
* [gparmer/Composite](https://github.com/gparmer/Composite) - A component-based OS
* [grahamedgecombe/nginx-ct](https://github.com/grahamedgecombe/nginx-ct) - Certificate Transparency module for nginx.
* [grahamking/Key-Value-Polyglot](https://github.com/grahamking/Key-Value-Polyglot) - A basic key-value store, repeated in C, Go, Python (basic, gevent, and diesel), Ruby (event machine), Java, Scala, Haskell, and NodeJS.
* [graphitemaster/gmqcc](https://github.com/graphitemaster/gmqcc) - An Improved Quake C Compiler
* [graphitemaster/incbin](https://github.com/graphitemaster/incbin) - Include binary files in C/C++
* [graphitemaster/lambdapp](https://github.com/graphitemaster/lambdapp) - Anonymous functions in C
* [graphitemaster/libintrusive](https://github.com/graphitemaster/libintrusive) - Intrusive data structures for C
* [grbl/grbl](https://github.com/grbl/grbl) - An open source, embedded, high performance g-code-parser and CNC milling controller written in optimized C that will run on a straight Arduino
* [greghaynes/Afproto](https://github.com/greghaynes/Afproto) - Serial data framing protocol
* [gregvirgin/libcork](https://github.com/gregvirgin/libcork) - A simple, easily embeddable cross-platform C library
* [greiman/ChibiOS-Arduino](https://github.com/greiman/ChibiOS-Arduino) - ChibiOS/RT 3.0.3 for Arduino AVR, Due, and Teensy 3.x
* [grimfang4/sdl-gpu](https://github.com/grimfang4/sdl-gpu) - A library for high-performance, modern 2D graphics with SDL written in C.
* [grizzlin/sylvanas](https://github.com/grizzlin/sylvanas) - Data Aggregation Girl.
* [grobian/carbon-c-relay](https://github.com/grobian/carbon-c-relay) - Enhanced C implementation of Carbon relay, aggregator and rewriter
* [groonga/groonga](https://github.com/groonga/groonga) - An embeddable fulltext search engine. Groonga is the successor project to Senna.
* [grpc/grpc](https://github.com/grpc/grpc) - The C based gRPC (C++, Node.js, Python, Ruby, Objective-C, PHP, C#)
* [grrrwaaa/maxcpp](https://github.com/grrrwaaa/maxcpp) - C++ templates for Max/MSP objects
* [grundprinzip/bitcompressedvector](https://github.com/grundprinzip/bitcompressedvector) - Provide a container for integral data types that applies light-weight bit compression
* [grz0zrg/fbg](https://github.com/grz0zrg/fbg) - Lightweight C 2D graphics API agnostic library with parallelism support
* [gsliepen/tinc](https://github.com/gsliepen/tinc) - a VPN daemon
* [guardianproject/libsqlfs](https://github.com/guardianproject/libsqlfs) - a library that implements a POSIX style filesystem on top of an SQLite database
* [guaxiao/renderer.gua](https://github.com/guaxiao/renderer.gua) - Software 3D Renderer in C++ on Windows, OSX and Linux or other popular flavors of Unix that SDL supports
* [guedes/ldap_fdw](https://github.com/guedes/ldap_fdw) - A LDAP Foreign Data Wrapper for PostgreSQL
* [guilleiguaran/xv6](https://github.com/guilleiguaran/xv6) - mirror of the source code of the Xv6 operating system
* [guillermocalvo/exceptions4c](https://github.com/guillermocalvo/exceptions4c) - :bomb: An exception handling framework for C
* [guodong/dbd](https://github.com/guodong/dbd) - Distributed block device, used for cloud computing environment or big data storage base.
* [guokr/gkseg](https://github.com/guokr/gkseg) - Yet another Chinese word segmentation package based on character-based tagging heuristics and CRF algorithm
* [guomeizhou/data_structure](https://github.com/guomeizhou/data_structure) - 数据结构
* [gurnec/HashCheck](https://github.com/gurnec/HashCheck) - HashCheck Shell Extension for Windows with added SHA2, SHA3, and multithreading; originally from code.kliu.org
* [gwaldron/osgearth](https://github.com/gwaldron/osgearth) - A free open source C++ geospatial toolkit.
* [gwik/ffmpeg-ruby](https://github.com/gwik/ffmpeg-ruby) - Ruby interface to the ffmpeg C library. It is able to extract images from videos but do not allow to encode full video.
* [h2non/semver.c](https://github.com/h2non/semver.c) - semantic version parser and serializer written in ANSI C
* [h2o/h2o](https://github.com/h2o/h2o) - H2O - the optimized HTTP/1, HTTP/2 server
* [h2o/picohttpparser](https://github.com/h2o/picohttpparser) - tiny HTTP parser written in C (used in HTTP::Parser::XS et al.)
* [h2o/picotls](https://github.com/h2o/picotls) - TLS 1.3 implementation in C (master supports RFC8446 as well as draft-26, -27, -28)
* [h5md/VMD-h5mdplugin](https://github.com/h5md/VMD-h5mdplugin) - This plugin enables VMD to display data stored in h5 files that are structured according to the H5MD specifications (http://nongnu.org/h5md/)
* [haad/proxychains](https://github.com/haad/proxychains) - proxychains - a tool that forces any TCP connection made by any given application to follow through proxy like TOR or any other SOCKS4, SOCKS5 or HTTP(S) proxy.  Supported auth-types: "user/pass" for SOCKS4/5, "basic" for HTTP.
* [haakonnessjoen/MAC-Telnet](https://github.com/haakonnessjoen/MAC-Telnet) - Open source MAC Telnet client and server for connecting to Microtik RouterOS routers and Posix machines via MAC address.
* [hacatu/haclib](https://github.com/hacatu/haclib) - A utility library providing data types C should have been made with such as vectors and sequences, mostly as macros.
* [hach-que/configd](https://github.com/hach-que/configd) - Generates configuration files in /etc based on YAML data and XSLT transformations.
* [hackedteam/core-linux](https://github.com/hackedteam/core-linux) - RCS Agent for Linux
* [hackgnar/ble_ctf](https://github.com/hackgnar/ble_ctf) - A Bluetooth low energy capture the flag
* [hackingtype1/cgm-pebble](https://github.com/hackingtype1/cgm-pebble) - pebble watch-face or app to display cgm data
* [haf/System.Data.SQLite](https://github.com/haf/System.Data.SQLite) - A mirror to the official https://system.data.sqlite.org site which uses Fossil for their SCM, and configured to be buildable on mono.
* [haiwen/ccnet](https://github.com/haiwen/ccnet) - Ccnet is a framework for writing networked applications in C.
* [haiwen/seafile](https://github.com/haiwen/seafile) - Open source cloud storage with file encryption and group sharing, and emphasis on reliability and high performance.
* [halayli/lthread](https://github.com/halayli/lthread) - lthread, a multicore enabled coroutine library written in C
* [haldean/x6502](https://github.com/haldean/x6502) - Yet another 6502 emulator that one day dreams of being an Atari 2600.
* [halfninja/android-ffmpeg-x264](https://github.com/halfninja/android-ffmpeg-x264) - INACTIVE, UNSUPPORTED - Android Videokit - basic FFMPEG+X264 build for Android. Pull requests gratefully accepted.
* [hanzz/libtransport](https://github.com/hanzz/libtransport) - Create C++ transports easily
* [happyfish100/fastdfs](https://github.com/happyfish100/fastdfs) - FastDFS is an open source high performance distributed file system (DFS). It's major functions include: file storing, file syncing and file accessing, and design for high capacity and load balance.
* [happyfish100/fastdht](https://github.com/happyfish100/fastdht) - FastDHT is a high performance distributed hash table (DHT) which based key value pairs. It can store mass key value pairs such as filename mapping, session data and user related data.
* [happyfish100/libfastcommon](https://github.com/happyfish100/libfastcommon) - c common functions library extracted from my open source project FastDFS. this library is very simple and stable.  functions including: string, logger, chain, hash, socket, ini file reader, base64 encode / decode, url encode / decode, fast timer, skiplist, object pool etc. detail info please see the c header files.
* [happykevins/cocos2dx-ext](https://github.com/happykevins/cocos2dx-ext) - Extensions for Cocos2dx: Dynamic Font Management, HTML Widget, Powerful Asset Management...
* [happypeter/tata](https://github.com/happypeter/tata) - tinylion data
* [haproxy/haproxy](https://github.com/haproxy/haproxy) - Mirror of haproxy repository
* [harbour/core](https://github.com/harbour/core) - Portable, xBase compatible programming language and environment
* [harnold/generic-c](https://github.com/harnold/generic-c) - A library of generic data structures and algorithms for C, in the spirit of the STL
* [hashcat/hashcat](https://github.com/hashcat/hashcat) - World's fastest and most advanced password recovery utility
* [haskell-crypto/cryptonite](https://github.com/haskell-crypto/cryptonite) - lowlevel set of cryptographic primitives for haskell
* [havlenapetr/FFMpeg](https://github.com/havlenapetr/FFMpeg) - this is port of ffmpeg for android (this is app, but in future i will do android lib from it and then system will be able to convert videos automatically)
* [haywire/haywire](https://github.com/haywire/haywire) - Haywire is an asynchronous HTTP server framework written in C that's built using the event loop based libuv platform layer that node.js is built on top of.
* [hcarty/ocaml-hdf](https://github.com/hcarty/ocaml-hdf) - Library for reading/writing HDF4 data and reading NetCDF data
* [hdevalence/wordgen](https://github.com/hdevalence/wordgen) - let's play with google ngrams data
* [hdm/juniper-cve-2015-7755](https://github.com/hdm/juniper-cve-2015-7755) - Notes, binaries, and related information from analysis of the CVE-2015-7755 & CVE-2015-7756 issues within Juniper ScreenOS
* [heewa/pipestats](https://github.com/heewa/pipestats) - Stats about data being piped.
* [heimir-sverrisson/jdbc2_fdw](https://github.com/heimir-sverrisson/jdbc2_fdw) - JDBC Foreign Data Wrapper for PostgreSQL
* [hellerve/e](https://github.com/hellerve/e) - A dead simple editor
* [henrypp/chrlauncher](https://github.com/henrypp/chrlauncher) - Small and very fast portable launcher and updater for Chromium.
* [hexchat/hexchat](https://github.com/hexchat/hexchat) - GTK+ IRC client -
* [hfiref0x/CVE-2015-1701](https://github.com/hfiref0x/CVE-2015-1701) - Win32k LPE vulnerability used in APT attack
* [hfiref0x/TDL](https://github.com/hfiref0x/TDL) - Driver loader for bypassing Windows x64 Driver Signature Enforcement
* [hfiref0x/UACME](https://github.com/hfiref0x/UACME) - Defeating Windows User Account Control
* [hfiref0x/UPGDSED](https://github.com/hfiref0x/UPGDSED) - Universal PatchGuard and Driver Signature Enforcement Disable
* [hfiref0x/VBoxHardenedLoader](https://github.com/hfiref0x/VBoxHardenedLoader) - VirtualBox VM detection mitigation loader
* [hfiref0x/WinObjEx64](https://github.com/hfiref0x/WinObjEx64) - Windows Object Explorer 64-bit
* [hhetter/smbtatools](https://github.com/hhetter/smbtatools) - Tools to query the SMB traffic analyzer data base
* [hibara/AttacheCase](https://github.com/hibara/AttacheCase) - file/folder encryption software for Windows ( C++Builder2010 Project Files )
* [hillegass/BNRPersistence](https://github.com/hillegass/BNRPersistence) - A set of classes which use Tokyo Cabinet to save and load Objective-C objects
* [hishamhm/htop](https://github.com/hishamhm/htop) - htop is an interactive text-mode process viewer for Unix systems. It aims to be a better 'top'.
* [hit9/todo.c](https://github.com/hit9/todo.c) - Command line lightweight todo tool with readable storage , written in C.
* [hmng/jsonrpc-c](https://github.com/hmng/jsonrpc-c) - JSON-RPC in C (server only for now)
* [hnes/libaco](https://github.com/hnes/libaco) - A blazing fast and lightweight C asymmetric coroutine library  💎 ⛅🚀⛅🌞
* [holmium/dnsforwarder](https://github.com/holmium/dnsforwarder) - Just a DNS utility.
* [horchi/linux-p4d](https://github.com/horchi/linux-p4d) - Deamon which fetch sensor data of the 'Lambdatronic s3200' and store to a MySQL database
* [hoxnox/rawsock_recv_example](https://github.com/hoxnox/rawsock_recv_example) - SOCK_RAW IPPROTO_UDP socket data transmission example
* [hoytech/vmtouch](https://github.com/hoytech/vmtouch) - Portable file system cache diagnostics and control
* [hp09d/SAE-Baja-Data-Acquisition](https://github.com/hp09d/SAE-Baja-Data-Acquisition) - Senior Design project year 2014-2015
* [hpc/dtcmp](https://github.com/hpc/dtcmp) - Datatype Compare (DTCMP) Library for sorting and ranking distributed data using MPI
* [hpc/scr](https://github.com/hpc/scr) - SCR caches checkpoint data in storage on the compute nodes of a Linux cluster to provide a fast, scalable checkpoint / restart capability for MPI codes.
* [hpjansson/chafa](https://github.com/hpjansson/chafa) - 📺🗿 Terminal graphics for the 21st century.
* [hpricot/hpricot](https://github.com/hpricot/hpricot) - Hpricot has ended. Please consider an alternative like nokogiri.
* [hroptatyr/dateutils](https://github.com/hroptatyr/dateutils) - nifty command line date and time utilities; fast date calculations and conversion in the shell
* [hroptatyr/gandalf](https://github.com/hroptatyr/gandalf) - serve time series from rolled-out text data, part of the army of unserding services
* [hroptatyr/glod](https://github.com/hroptatyr/glod) - Grokking lots of data
* [hroptatyr/uterus](https://github.com/hroptatyr/uterus) - universal tick encoder library to efficiently transport huge amounts of tick data
* [hrydgard/native](https://github.com/hrydgard/native) - NOTE: DEPRECATED! No longer used in PPSSPP! Various C++ utility code: OpenGL ES, JSON, etc, portable to Android.
* [htacg/tidy-html5](https://github.com/htacg/tidy-html5) - The granddaddy of HTML tools, with support for modern standards
* [huacnlee/rucaptcha](https://github.com/huacnlee/rucaptcha) - This is a Captcha gem for Rails Application. No dependencies. No ImageMagick, No RMagick.
* [huangz1990/annotated_redis_source](https://github.com/huangz1990/annotated_redis_source) - 带有详细注释的 Redis 2.6 源码
* [huangz1990/redis-3.0-annotated](https://github.com/huangz1990/redis-3.0-annotated) - 带有详细注释的 Redis 3.0 代码（annotated Redis 3.0 source code）。
* [hughsie/fwupd](https://github.com/hughsie/fwupd) - A simple daemon to allow session software to update firmware
* [hugsy/proxenet](https://github.com/hugsy/proxenet) - The REAL^WONLY Hacker-Friendly proxy for web application pentests.
* [hvdieren/swan](https://github.com/hvdieren/swan) - Data-flow driven work-stealing scheduler
* [hyPiRion/c-rrb](https://github.com/hyPiRion/c-rrb) - RRB-tree implemented as a library in C.
* [hyPiRion/persistencia](https://github.com/hyPiRion/persistencia) - Repository with implementations to understand persistent data structures.
* [hyPiRion/roulette-tree](https://github.com/hyPiRion/roulette-tree) - Data structure for efficient fitness-proportionate selection.
* [hyperic/sigar](https://github.com/hyperic/sigar) - System Information Gatherer And Reporter
* [hyperrealm/libconfig](https://github.com/hyperrealm/libconfig) - C/C++ library for processing configuration files
* [hzeller/gmrender-resurrect](https://github.com/hzeller/gmrender-resurrect) - Resource efficient UPnP/DLNA renderer, optimal for Raspberry Pi, CuBox or a general MediaServer. Fork of GMediaRenderer to add some features to make it usable.
* [i-rinat/apulse](https://github.com/i-rinat/apulse) - PulseAudio emulation for ALSA
* [i-rinat/freshplayerplugin](https://github.com/i-rinat/freshplayerplugin) - ppapi2npapi compatibility layer
* [i-saint/DynamicPatcher](https://github.com/i-saint/DynamicPatcher) - Runtime C++ Editing
* [i3/i3](https://github.com/i3/i3) - A better tiling and dynamic window manager
* [iMoreApps/ffmpeg-avplayer-for-ios](https://github.com/iMoreApps/ffmpeg-avplayer-for-ios) - A tiny but powerful video player framework for iOS developers.
* [iTyran/SushiCrush](https://github.com/iTyran/SushiCrush) - SushiCrush
* [iafonov/cosmonaut](https://github.com/iafonov/cosmonaut) - Fast web server & micro framework implemented in C. Just for fun.
* [iafonov/multipart-parser-c](https://github.com/iafonov/multipart-parser-c) - Http multipart parser implemented in C
* [ibarwick/firebird_fdw](https://github.com/ibarwick/firebird_fdw) - A PostgreSQL foreign data wrapper (FDW) for Firebird
* [ibc/em-udns](https://github.com/ibc/em-udns) - An async DNS resolver for EventMachine based on udns C library
* [ice799/memprof](https://github.com/ice799/memprof) - A Ruby gem for memory profiling
* [id-Software/DOOM-iOS](https://github.com/id-Software/DOOM-iOS) - DOOM Classic for iOS Source Release
* [id-Software/DOOM](https://github.com/id-Software/DOOM) - DOOM Open Source Release
* [id-Software/Quake-2](https://github.com/id-Software/Quake-2) - Quake 2 GPL Source Release
* [id-Software/Quake-III-Arena](https://github.com/id-Software/Quake-III-Arena) - Quake III Arena GPL Source Release
* [id-Software/Quake](https://github.com/id-Software/Quake) - Quake GPL Source Release
* [id-Software/Wolf3D-iOS](https://github.com/id-Software/Wolf3D-iOS) - Wolfenstein 3D for iOS Source Release
* [ideawu/c1000k](https://github.com/ideawu/c1000k) - A tool to test if you OS supports 1 million connections(c1000k)
* [ideawu/icomet](https://github.com/ideawu/icomet) - A C1000K comet/push server built with C++, for web and mobile app
* [iem-projects/pd-iemrtp](https://github.com/iem-projects/pd-iemrtp) - RTP support for Pure Data
* [ifsnop/reader_network](https://github.com/ifsnop/reader_network) - A package of utilities to record and work with multicast radar data in ASTERIX format. (radar as in air navigation surveillance).
* [igorsobreira/iclib](https://github.com/igorsobreira/iclib) - Library with useful C data structures
* [igraph/igraph](https://github.com/igraph/igraph) - Library for the analysis of networks
* [igrr/esp32-cam-demo](https://github.com/igrr/esp32-cam-demo) - Demo for working with a camera on ESP32
* [igrr/esptool-ck](https://github.com/igrr/esptool-ck) - ESP8266 build/flash helper tool by Christian Klippel
* [iiordanov/remote-desktop-clients](https://github.com/iiordanov/remote-desktop-clients) - VNC, RDP, SPICE, and oVirt/RHEV/Proxmox Clients for Android and Blackberry 10
* [ileben/ShivaVG](https://github.com/ileben/ShivaVG) - OpenGL based ANSI C implementation of the OpenVG standard.
* [illumos/illumos-gate](https://github.com/illumos/illumos-gate) - Community developed and maintained version of the OS/Net consolidation
* [imankulov/wav2rtp](https://github.com/imankulov/wav2rtp) - wav2rtp is a simple tool intended to convert speech data from wav files to RTP data stream
* [imatix/zguide](https://github.com/imatix/zguide) - Learning and Using ØMQ
* [immobiliare/sfs](https://github.com/immobiliare/sfs) - Asynchronous Filesystem Replication
* [imneme/pcg-c-basic](https://github.com/imneme/pcg-c-basic) - PCG — Minimal C Implementation
* [imneme/pcg-c](https://github.com/imneme/pcg-c) - PCG — C Implementation
* [indrajithi/Audio-Visualizer](https://github.com/indrajithi/Audio-Visualizer) - Audio Visualizer in C++ using OpenGL
* [indutny/bud](https://github.com/indutny/bud) - Bud - The TLS Terminator
* [infincia/Cardrand](https://github.com/infincia/Cardrand) - This is a simple demonstration of two things, pulling random entropy out of a hardware smart card, and feeding that data into the Linux kernel pool using an ioctl call. Makes it possible for any Linux system to have a real hardware random number generator
* [infofarmer/hashtypes](https://github.com/infofarmer/hashtypes) - sha1, md5 and other data types for PostgreSQL
* [innoying/iOS-DataProtection](https://github.com/innoying/iOS-DataProtection) - Tools to manipulate and use iOS data protection features.
* [inspirit/CaptureDevice](https://github.com/inspirit/CaptureDevice) - Adobe Air Native Extension for video capturing from cameras
* [intel-iot-devkit/how-to-code-samples](https://github.com/intel-iot-devkit/how-to-code-samples) - These applications are code sample exercises using the Intel IoT Developer Kit, Intel Edison board or Intel IoT Gateway, sensors, actuators, cloud platforms, and APIs.
* [intel-iot-devkit/mraa](https://github.com/intel-iot-devkit/mraa) - Linux Library for low speed IO Communication in C with bindings for C++, Python, Node.js & Java. Supports generic io platforms, as well as Intel Edison, Intel Joule, Raspberry Pi and many more.
* [intel/cc-oci-runtime](https://github.com/intel/cc-oci-runtime) - OCI (Open Containers Initiative) compatible runtime for Intel® Architecture
* [intel/intel-cmt-cat](https://github.com/intel/intel-cmt-cat) - User space software for Intel(R) Resource Director Technology
* [intellectualheaven/ceed](https://github.com/intellectualheaven/ceed) - A tiny x86 compiler with ELF and PE target
* [io7m/coreland-lua-ada-load](https://github.com/io7m/coreland-lua-ada-load) - Load data from Lua into Ada data structures
* [ioerror/tlsdate](https://github.com/ioerror/tlsdate) - secure parasitic rdate replacement
* [ionescu007/SpecuCheck](https://github.com/ionescu007/SpecuCheck) - SpecuCheck is a Windows utility for checking the state of the software mitigations and hardware against  CVE-2017-5754 (Meltdown), CVE-2017-5715 (Spectre v2), CVE-2018-3260 (Foreshadow), and CVE-2018-3639 (Spectre v4)
* [ipa320/cob_extern](https://github.com/ipa320/cob_extern) - The cob_extern stack contains third party libraries needed for operating Care-O-bot. The packages are downloaded from the manufactorers website and not changed in any way.
* [ircmaxell/php-ndata](https://github.com/ircmaxell/php-ndata) - NData PECL extension for dealing with native data types
* [irssi/irssi](https://github.com/irssi/irssi) - The client of the future
* [irtimmer/moonlight-embedded](https://github.com/irtimmer/moonlight-embedded) - Gamestream client for embedded systems
* [irungentoo/toxcore](https://github.com/irungentoo/toxcore) - The future of online communications.
* [irvined1982/loguino](https://github.com/irvined1982/loguino) - Logiuno, an arduino based data aquisition tool
* [iscsi-osx/iSCSIInitiator](https://github.com/iscsi-osx/iSCSIInitiator) - iSCSI Initiator for macOS
* [isislab/CSAW-CTF-2016-Quals](https://github.com/isislab/CSAW-CTF-2016-Quals) - Repo for CSAW CTF 2016 Quals challenges
* [iskra/jsonx](https://github.com/iskra/jsonx) - JSONX is an Erlang library for efficient decode and encode JSON, written in C.
* [island-org/island](https://github.com/island-org/island) - Lightweight and low-level creative coding toolkits in C.
* [isti757/DataNetwork](https://github.com/isti757/DataNetwork) - Data network project. This was a project at Saarland University of the Course Data Networks. The project implements some ideas of OSI protocol stack. The code runs using the CNET network simulator  (http://www.csse.uwa.edu.au/cnet/), however the project is easily separable and can run on real networks as well.  Please see the design folder for tex file and generate a pdf with the entire desciption of the project.  The project is written in C and is portable.
* [it4e/CHL](https://github.com/it4e/CHL) - C Hypertext Library - A library for writing web applications in C
* [itkz/librtmp](https://github.com/itkz/librtmp) - RTMP server and client written by C
* [itod/panthro](https://github.com/itod/panthro) - A implementation of XPath 3.0 in Objective-C/Cocoa
* [iunderstand/SWE](https://github.com/iunderstand/SWE) - SWE Toolkit. Learning Semantic Word Embeddings based on Ordinal Knowledge Constraints. A general framework to incorporate semantic knowledge into the popular data-driven learning process of word vectors. Applications including word similarity, sentence completion, etc. ACL-2015 long paper, Beijing, China
* [ivansafrin/CS3113](https://github.com/ivansafrin/CS3113) - NYU CS3113 [Intro To Game Programming]
* [ivmai/bdwgc](https://github.com/ivmai/bdwgc) - The Boehm-Demers-Weiser conservative C/C++ Garbage Collector (libgc, bdwgc, boehm-gc)
* [ixty/xarch_shellcode](https://github.com/ixty/xarch_shellcode) - Cross Architecture Shellcode in C
* [jabberd2/jabberd2](https://github.com/jabberd2/jabberd2) - JabberD XMPP Server
* [jackeylu/mysql2redis](https://github.com/jackeylu/mysql2redis) - A UDF(user defined functions) plugin for MySQL, which can be used for pushing data to Redis
* [jackmitch/libsoc](https://github.com/jackmitch/libsoc) - libsoc: C library for interfacing with common SoC peripherals through generic kernel interfaces
* [jacob-carlborg/dstep](https://github.com/jacob-carlborg/dstep) - A tool for converting C and Objective-C headers to D modules
* [jacobdufault/cquery](https://github.com/jacobdufault/cquery) - Low-latency language server supporting multi-million line C++ code-bases, powered by libclang. Works in any editor with language server support (vscode, emacs, vim, etc).
* [jagt/clumsy](https://github.com/jagt/clumsy) - clumsy makes your network condition on Windows significantly worse, but in a controlled and interactive manner.
* [jaimz/core_ds](https://github.com/jaimz/core_ds) - Simple C data structure library
* [jakogut/tinyflock](https://github.com/jakogut/tinyflock) - A simple, high-performance, threaded, and interactive flocking demo written in C with GLFW.
* [jakogut/tinyvm](https://github.com/jakogut/tinyvm) - TinyVM is a small, fast, lightweight virtual machine written in pure ANSI C.
* [jalvesaq/VimCom](https://github.com/jalvesaq/VimCom) - *Deprecated* package used to intermediate the communication between Vim and R
* [jalvesaq/colorout](https://github.com/jalvesaq/colorout) - Colorize R output on terminal emulators
* [jamezilla/ats](https://github.com/jamezilla/ats) - ATS is a spectral modeling system based on a sinusoidal plus critical-band noise decomposition. Psychoacoustic processing informs the system's sinusoidal tracking and noise modeling algorithms. Perceptual Audio Coding (PAC) techniques such as Signal-to-Mask Ratio (SMR) evaluation are used to achieve perceptually accurate sinusoidal tracking. SMR values are also used as a psychoacoustic metric to determine the perceptual relevance of partials during analysis data postprocessing. The system's noise component is modeled using Bark-scale frequency warping and sub-band noise energy evaluation. Noise energy at the sub-bands is then distributed on a frame-by-frame basis among the partials resulting in a compact hybrid representation based on noise modulated sinusoidal trajectories.
* [jamplus/jamplus](https://github.com/jamplus/jamplus) - Jamplus is a generic code and data build system derived from the original Perforce version of Jam
* [janet-lang/janet](https://github.com/janet-lang/janet) - A dynamic language and bytecode vm
* [jangaraj/Zabbix-Docker-Monitoring](https://github.com/jangaraj/Zabbix-Docker-Monitoring) - :whale: Monitoring of Docker containers (LXC/systemd Docker supported) - Zabbix template and Zabbix C module
* [japeq/bencode-tools](https://github.com/japeq/bencode-tools) - bencode-tools is a collection of tools for manipulating bencoded data.
* [jaredly/codetalker](https://github.com/jaredly/codetalker) - A succinct, pythonic parser + translator solution
* [jarikomppa/soloud](https://github.com/jarikomppa/soloud) - Free, easy, portable audio engine for games
* [jarun/dslib](https://github.com/jarun/dslib) - A library of handy data structures
* [jaseg/matelight](https://github.com/jaseg/matelight) - Show text and gifs on mate crates. Uses C code orchestrated from Python via ctypes.
* [jashmenn/apriori](https://github.com/jashmenn/apriori) - A ruby/c extension to Christian Borgelt's apriori item-set implementation
* [jasonmaclafferty/String](https://github.com/jasonmaclafferty/String) - A dynamic string data type implementation for C.
* [jasonmc/forked-daapd](https://github.com/jasonmc/forked-daapd) - A re-write of the firefly media server (mt-daapd). It's released under GPLv2+. Please note that this git repository is a mirror of the official one at git://git.debian.org/~jblache/forked-daapd.git
* [jb55/hearthstone-cardxml](https://github.com/jb55/hearthstone-cardxml) - Hearthstone xml card data extractor
* [jbaiter/jpegtran-cffi](https://github.com/jbaiter/jpegtran-cffi) - Fast, (mostly) lossless JPEG transformations with Python
* [jbangert/trapcc](https://github.com/jbangert/trapcc) - Computing with traps
* [jbenjore/Clone-Data](https://github.com/jbenjore/Clone-Data) - Simple and fast data cloning
* [jbenjore/Internals-GraphArenas](https://github.com/jbenjore/Internals-GraphArenas) - Chart a map of where perl locates data
* [jberthold/packman](https://github.com/jberthold/packman) - Evaluation-orthogonal serialisation of Haskell data, as a library
* [jbremer/darm](https://github.com/jbremer/darm) - A light-weight and efficient disassembler written in C for the ARMv7 instruction set.
* [jbruchon/jdupes](https://github.com/jbruchon/jdupes) - A powerful duplicate file finder and an enhanced fork of 'fdupes'.
* [jbuchbinder/statsd-c](https://github.com/jbuchbinder/statsd-c) - C port of Etsy's statsd
* [jbush001/NyuziProcessor](https://github.com/jbush001/NyuziProcessor) - GPGPU processor core, implemented in SystemVerilog.
* [jcline/fuse-google-drive](https://github.com/jcline/fuse-google-drive) - A fuse filesystem wrapper for Google Drive.
* [jcloudpub/speedy](https://github.com/jcloudpub/speedy) - a distributed docker image storage
* [jcupitt/libvips](https://github.com/jcupitt/libvips) - A fast image processing library with low memory needs.
* [jdduke/three_cpp](https://github.com/jdduke/three_cpp) - A port of three.js to C++
* [jdp/ephemeron](https://github.com/jdp/ephemeron) - where transient data makes itself useful
* [jduck/asus-cmd](https://github.com/jduck/asus-cmd) - ASUS Router infosvr UDP Broadcast root Command Execution
* [jduck/canhazaxs](https://github.com/jduck/canhazaxs) - A tool for enumerating the access to entries in the file system of an Android device.
* [jduck/challack](https://github.com/jduck/challack) - Proof-of-concept exploit code for CVE-2016-5696
* [jech/polipo](https://github.com/jech/polipo) - The Polipo caching HTTP proxy
* [jedisct1/Pincaster](https://github.com/jedisct1/Pincaster) - A fast persistent nosql database with a HTTP/JSON interface, not only for geographical data.
* [jedisct1/dnscrypt-proxy](https://github.com/jedisct1/dnscrypt-proxy) - A tool for securing communications between a client and a DNS resolver
* [jedisct1/libhydrogen](https://github.com/jedisct1/libhydrogen) - A lightweight, secure, easy-to-use crypto library suitable for constrained environments.
* [jedwing/CHMLib](https://github.com/jedwing/CHMLib) - Library for reading Microsoft ITSS/CHM format files.
* [jeff-1amstudios/restful-doom](https://github.com/jeff-1amstudios/restful-doom) - HTTP+JSON API hosted inside the 1993 DOOM engine!
* [jelathro/C](https://github.com/jelathro/C) - C Programming Projects
* [jenswilly/AVR-enc28j60-pachube](https://github.com/jenswilly/AVR-enc28j60-pachube) - AVR Libc-based project for ATmega328/-168 sending data to Pachube using an ENC28J60 with the Tuxgraphics TCP library.
* [jeremy-w/objc-zmq](https://github.com/jeremy-w/objc-zmq) - Objective-C binding for ZeroMQ.
* [jeroenooms/curl](https://github.com/jeroenooms/curl) - A Modern and Flexible Web Client for R
* [jeromekelleher/msprime](https://github.com/jeromekelleher/msprime) - A reimplementation of Hudson's classical ms simulator for modern data sets.
* [jgamblin/Mirai-Source-Code](https://github.com/jgamblin/Mirai-Source-Code) - Leaked Mirai Source Code for Research/IoC Development Purposes
* [jgarzik/cpuminer](https://github.com/jgarzik/cpuminer) - CPU miner for bitcoin
* [jgarzik/picocoin](https://github.com/jgarzik/picocoin) - A bitcoin library in C, SPV wallet & more.
* [jgeboski/purple-facebook](https://github.com/jgeboski/purple-facebook) - Facebook protocol plugin for libpurple
* [jgm/cmark](https://github.com/jgm/cmark) - CommonMark parsing and rendering library and program in C
* [jgm/peg-markdown](https://github.com/jgm/peg-markdown) - An implementation of markdown in C, using a PEG grammar
* [jhawthorn/fzy](https://github.com/jhawthorn/fzy) - :mag: A better fuzzy finder
* [jianfengye/nginx-1.0.14_comment](https://github.com/jianfengye/nginx-1.0.14_comment) - nginx源码中文注释版
* [jimenezrick/patch-AuthenticAMD](https://github.com/jimenezrick/patch-AuthenticAMD) - Utility to patch binaries generated by the Intel C++ Compiler to get the maximum performance on AMD CPUs
* [jimon/osx_app_in_plain_c](https://github.com/jimon/osx_app_in_plain_c) - A simple showcase how to create a simple OS X app in plain C without any Objective-C
* [jimstudt/ook-decoder](https://github.com/jimstudt/ook-decoder) - Ook-decoder reads On-Off Keying radio data commonly used in the 433MHz ISM bands using a software defined radio (SDR).
* [jjgod/vim-cocoa](https://github.com/jjgod/vim-cocoa) - A compact Cocoa port for Vim.
* [jkff/scrunch](https://github.com/jkff/scrunch) - Stream cruncher - data stream algorithms
* [jklmnn/imagejs](https://github.com/jklmnn/imagejs) - Small tool to package javascript into a valid image file.
* [jknotzke/GoldenEmbedGPS](https://github.com/jknotzke/GoldenEmbedGPS) - Embedded Firmware for the Sparkfun Package Tracker which will log ANT+ data
* [jknotzke/GoldenEmbed](https://github.com/jknotzke/GoldenEmbed) - Embedded Firmware for the Sparkfun Logomatic V2 which will log ANT+ data
* [jkramer/shell-fm](https://github.com/jkramer/shell-fm) - Lightweight console-based radio player for Last.FM radio streams.
* [jlamarche/iOS-OpenGLES-Stuff](https://github.com/jlamarche/iOS-OpenGLES-Stuff) - Various scripts, utils, and code examples for OpenGL ES programming for iOS
* [jlapeyre/PDL-IO-Matlab](https://github.com/jlapeyre/PDL-IO-Matlab) - Reading and writing matlab format data files for the perl data language.
* [jlblancoc/suitesparse-metis-for-windows](https://github.com/jlblancoc/suitesparse-metis-for-windows) - CMake scripts for painless usage of SuiteSparse+METIS from Visual Studio and the rest of Windows/Linux/OSX IDEs supported by CMake
* [jllodra/ncdump-json](https://github.com/jllodra/ncdump-json) - Modified ncdump to output data in json format
* [jmasters/gbt-pipeline](https://github.com/jmasters/gbt-pipeline) - The Green Bank Telescope data analysis pipeline
* [jmcejuela/Levenshtein-MySQL-UDF](https://github.com/jmcejuela/Levenshtein-MySQL-UDF) - General Levenshtein algorithm and k-bounded levenshtein distance in linear time and constant space. Implementation in C as a MySQL UDF
* [jmckaskill/luaffi](https://github.com/jmckaskill/luaffi) - Standalone FFI library for calling C functions from lua. Compatible with the luajit FFI interface.
* [jmcnamara/libxlsxwriter](https://github.com/jmcnamara/libxlsxwriter) - A C library for creating Excel XLSX files.
* [jnz/q3vm](https://github.com/jnz/q3vm) - Q3VM - Embeddable bytecode virtual machine/interpreter for C-language input
* [joan2937/pigpio](https://github.com/joan2937/pigpio) - pigpio is a C library for the Raspberry which allows control of the General Purpose Input Outputs (GPIO).
* [jobovy/extreme-deconvolution](https://github.com/jobovy/extreme-deconvolution) - Density estimation using Gaussian mixtures in the presence of noisy, heterogeneous and incomplete data
* [joewalnes/tinytest](https://github.com/joewalnes/tinytest) - A tiny unit-testing framework for C
* [johnj/llds](https://github.com/johnj/llds) - Low-Level Data Structure - efficient data structures, and fast data access in the 2.6/3.0 kernel
* [johnkerl/miller](https://github.com/johnkerl/miller) - Miller is like sed, awk, cut, join, and sort for name-indexed data such as CSV
* [jonas/tig](https://github.com/jonas/tig) - Text-mode interface for git
* [jonashaag/bjoern](https://github.com/jonashaag/bjoern) - A screamingly fast Python 2/3 WSGI server written in C.
* [jonls/redshift](https://github.com/jonls/redshift) - Redshift adjusts the color temperature of your screen according to your surroundings. This may help your eyes hurt less if you are working in front of the screen at night.
* [jonmarimba/OpenCV-iOS](https://github.com/jonmarimba/OpenCV-iOS) - OpenCV Xcode project for iOS build
* [jonpe960/ufsm](https://github.com/jonpe960/ufsm) - UML Statechart library in C and XMI importer
* [jonstewart/foremost](https://github.com/jonstewart/foremost) - Foremost is a console program to recover files based on their headers, footers, and internal data structures. c.f., http://foremost.sourceforge.net/
* [jordansissel/xdotool](https://github.com/jordansissel/xdotool) - fake keyboard/mouse input, window management, and more
* [jorisvink/kore](https://github.com/jorisvink/kore) - An easy to use, scalable and secure web application framework for writing web APIs in C. || This is a read-only mirror, please see https://kore.io/mail and https://kore.io/source for information on how to contribute via the mailing lists.
* [josephg/librope](https://github.com/josephg/librope) - UTF-8 rope library for C
* [joshdk/libmap](https://github.com/joshdk/libmap) - A map (data structure) library written in c
* [jourlin/WebCrawler](https://github.com/jourlin/WebCrawler) - An academic open source and open data web crawler
* [joyent/http-parser](https://github.com/joyent/http-parser) - http request/response parser for c
* [joyent/illumos-kvm-cmd](https://github.com/joyent/illumos-kvm-cmd) - qemu-kvm for illumos-kvm
* [joyent/libuv](https://github.com/joyent/libuv) - Go to
* [joyent/smartos-live](https://github.com/joyent/smartos-live) - For more information, please see http://smartos.org/  For any questions that aren't answered there, please join the SmartOS discussion list: http://smartos.org/smartos-mailing-list/
* [joyent/v8plus](https://github.com/joyent/v8plus) - Node.js native add-ons in C
* [jp9000/OBS](https://github.com/jp9000/OBS) - Open Broadcaster Software
* [jp9000/obs-studio](https://github.com/jp9000/obs-studio) - OBS
* [jpbruyere/vkvg](https://github.com/jpbruyere/vkvg) - Vulkan vector drawing, try to stay close to cairo api
* [jpiper/pyDNase](https://github.com/jpiper/pyDNase) - Python module for the easy handling and analysis of DNase-seq data
* [jpmens/mqtt-chronos](https://github.com/jpmens/mqtt-chronos) - Periodically submit time/date-related data to an MQTT broker
* [jpmens/powerdns-datacheck](https://github.com/jpmens/powerdns-datacheck) - MySQL UDF to check data in PowerDNS tables
* [jpountz/lz4-java](https://github.com/jpountz/lz4-java) - LZ4 compression for Java
* [jpr5/ngrep](https://github.com/jpr5/ngrep) - ngrep strives to provide most of GNU grep's common features, applying them to the network layer. ngrep is a pcap-aware tool that will allow you to specify extended regular expressions to match against data payloads of packets.
* [jrd730/WordFinder](https://github.com/jrd730/WordFinder) - a data structure that specializes in rapidly finding valid anagrams of strings
* [jrfoell/campfire-libpurple](https://github.com/jrfoell/campfire-libpurple) - A Campfire protocol plugin for libpurple (Pidgin)
* [jrudolph/java-direct-data-store](https://github.com/jrudolph/java-direct-data-store) - An experiment to dump Java objects into a memory-mapped data store accessible without (de)serialization
* [jserv/amacc](https://github.com/jserv/amacc) - Small C Compiler generating ELF executable for Arm architecture
* [jserv/facebooc](https://github.com/jserv/facebooc) - Yet another Facebook clone written in C
* [json-c/json-c](https://github.com/json-c/json-c) - https://github.com/json-c/json-c is the official code repository for json-c.  See the wiki for release tarballs for download.  API docs at http://json-c.github.io/json-c/
* [jssjr/collectd-write_graphite](https://github.com/jssjr/collectd-write_graphite) - Graphite output plugin for collectd
* [jstasiak/asterisk-chan-dongle](https://github.com/jstasiak/asterisk-chan-dongle) - Mirror of SVN-based "asterisk's huawei 3g dongle channel driver" project with my Asterisk 10 and 11 compatibility patches (asterisk10 and asterisk11 branches)
* [jstjohn/SimSeq](https://github.com/jstjohn/SimSeq) - An illumina paired-end and mate-pair short read simulator. This project attempts to model as many of the quirks that exist in Illumina data as possible. Some of these quirks include the potential for chimeric reads, and non-biotinylated fragment pull down in mate-pair libraries . Additionally the program provides the ability to model both site and base specific error, and scripts are provided to train this error model on real datasets. My hope in creating this program is to generate as realistic data as possible to assist in assessing the accuracy of genome assembly tools.
* [jsvennevid/filearchive](https://github.com/jsvennevid/filearchive) - File archive library allowing for easy creation and access to data stored inside a container through a simple API.
* [jtauber/cleese](https://github.com/jtauber/cleese) - an operating system in Python
* [jtsiomb/c11threads](https://github.com/jtsiomb/c11threads) - Trivial C11 threads.h implementation over POSIX threads.
* [jtsiomb/kdtree](https://github.com/jtsiomb/kdtree) - A simple C library for working with KD-Trees
* [juanmirocks/Levenshtein-MySQL-UDF](https://github.com/juanmirocks/Levenshtein-MySQL-UDF) - General Levenshtein algorithm and k-bounded levenshtein distance in linear time and constant space. Implementation in C as a MySQL UDF
* [juliettef/IconFontCppHeaders](https://github.com/juliettef/IconFontCppHeaders) - C, C++ headers and C# classes for icon fonts: Font Awesome, Fork Awesome, Material Design, Material Design icons, Kenney game icons and Ionicons
* [julycoding/The-Art-Of-Programming-By-July](https://github.com/julycoding/The-Art-Of-Programming-By-July) - 此为《编程之法：面试和算法心得》一书2014年6月老版本的原型，最新完整纸质版于2015年9月上市！
* [justinmeza/lci](https://github.com/justinmeza/lci) - A LOLCODE interpreter written in C.
* [justjkk/gtfs2pgrouting](https://github.com/justjkk/gtfs2pgrouting) - Import GTFS data into Postgresql database for use by pgrouting
* [juuso/keychaindump](https://github.com/juuso/keychaindump) - A proof-of-concept tool for reading OS X keychain passwords
* [jvimal/perfiso_10g](https://github.com/jvimal/perfiso_10g) - Network Performance Isolation for Data Centres.   WIP: stay tuned!
* [jvirkki/libbloom](https://github.com/jvirkki/libbloom) - A simple and small bloom filter implementation in plain C.
* [jvirtanen/dada](https://github.com/jvirtanen/dada) - Generate tabular text data
* [jwasham/practice-c](https://github.com/jwasham/practice-c) - Part of my daily plan for studying C.
* [jwerle/fs.c](https://github.com/jwerle/fs.c) - File system API much like Node's fs module
* [jwerle/progress.c](https://github.com/jwerle/progress.c) - Progress display lib for c
* [jwiegley/git-scripts](https://github.com/jwiegley/git-scripts) - A bunch of random scripts I've either written, downloaded or clipped from #git.
* [jwilberding/bcp](https://github.com/jwilberding/bcp) - Broadcast Copy
* [jwise/ndfslave](https://github.com/jwise/ndfslave) - Tools to pull data off of a NAND flash chip using a Digilent Nexys-2 board.
* [jwmatthys/kalman-pd](https://github.com/jwmatthys/kalman-pd) - Simple control rate Kalman filter for Pure Data
* [jwr/msp430_usi_i2c](https://github.com/jwr/msp430_usi_i2c) - I2C for the MSP430 using the USI module
* [jyr/MNPP](https://github.com/jyr/MNPP) - Mac + Nginx + Percona + PHP a high performance web server in a one-click installer
* [k-takata/Onigmo](https://github.com/k-takata/Onigmo) - Onigmo is a regular expressions library forked from Oniguruma.
* [k7f/PureData](https://github.com/k7f/PureData) - branching clone of git://pure-data.git.sourceforge.net/gitroot/pure-data/pure-data
* [kablaa/CTF-Workshop](https://github.com/kablaa/CTF-Workshop) - Challenges for Binary Exploitation Workshop
* [kafka399/TwsMongo](https://github.com/kafka399/TwsMongo) - TwsMongo is an example of integration between Mongodb and InteractiveBrokers.com API v.9.66 written in C++. The goal of this application to save high frequency data in Mongodb database.
* [kaitanie/ruby-cernlib](https://github.com/kaitanie/ruby-cernlib) - Ruby interface to the legacy CERNLIB data analysis libraries
* [kanoi/cgminer-binaries](https://github.com/kanoi/cgminer-binaries) - cgminer binary downloads for AntMiner, Fedora 18 x86_64, RPi ARM_32, Xubuntu 11.04 x86_64
* [karelia/CurlHandle](https://github.com/karelia/CurlHandle) - Cocoa Class wrapping libcurl
* [karelzak/mutt-kz](https://github.com/karelzak/mutt-kz) - mutt with notmuch support and another improvements...
* [karlstav/cava](https://github.com/karlstav/cava) - Console-based Audio Visualizer for Alsa
* [karrenberg/wfvopencl](https://github.com/karrenberg/wfvopencl) - IMPORTANT NOTICE: This implementation is long outdated. The latest wfvopencl will be made publicly available with the new libwfv implementation. WFVOpenCL is an OpenCL driver for CPUs on the basis of LLVM. This driver employs Whole-Function Vectorization (WFV) in addition to multi-threading to fully exploit the available data-parallelism by executing as many kernel instances in parallel as possible.
* [karthick18/inception](https://github.com/karthick18/inception) - Inception movie explained programmatically
* [kavu/cocoa-go](https://github.com/kavu/cocoa-go) - A simple PoC example of calling Go from Cocoa and vice versa.
* [kazuho/picogc](https://github.com/kazuho/picogc) - a tiny, portable, precise, mark-and-sweep GC in C++
* [kbranigan/cJSON](https://github.com/kbranigan/cJSON) - I did not write this code, but I like it.
* [kbranigan/pow](https://github.com/kbranigan/pow) - C datastore/cache for MySQL data
* [kbranigan/tubes](https://github.com/kbranigan/tubes) - A series of programs intended for manipulating and handling various data
* [kdeforche/wt](https://github.com/kdeforche/wt) - Wt, C++ Web Toolkit
* [keendreams/keen](https://github.com/keendreams/keen) - Keen Dreams on Greenlight!
* [keenerd/jshon](https://github.com/keenerd/jshon) - Jshon is a JSON parser designed for maximum convenience within the shell.
* [keenlabs/KeenClient-iOS](https://github.com/keenlabs/KeenClient-iOS) - Official iOS client for the Keen IO API. Build analytics features directly into your iOS apps.
* [keeshux/basic-blockchain-programming](https://github.com/keeshux/basic-blockchain-programming) - Sample code from my blog series "Basic blockchain programming".
* [kehribar/usbSerial_benchmark](https://github.com/kehribar/usbSerial_benchmark) - Usb serial data transfer speed calculator & integrity checker
* [kehribar/xmega_ov7670](https://github.com/kehribar/xmega_ov7670) - OV7670 image sensor data capture with Atxmega32E5 without using external FIFO
* [kellabyte/Haywire](https://github.com/kellabyte/Haywire) - Haywire is an asynchronous HTTP server framework written in C that's built using the event loop based libuv platform layer that node.js is built on top of.
* [kelly/node-i2c](https://github.com/kelly/node-i2c) - Node.js native bindings for i2c-dev. Plays well with Raspberry Pi and Beaglebone.
* [kennytm/iphone-private-frameworks](https://github.com/kennytm/iphone-private-frameworks) - Headers for private frameworks or undocumented interfaces of iPhoneOS 3.x or before (4.x is not supported yet).
* [ketoo/NoahGameFrame](https://github.com/ketoo/NoahGameFrame) - A fast, scalable, distributed game server framework for C++, include actor library, network library,can be used as a  real time multiplayer game engine ( MMO RPG ), which support C#/Lua script/ Unity3d, and plan to support Cocos2dx, FlashAir client access.
* [kev009/Concurrency-Kit](https://github.com/kev009/Concurrency-Kit) - Concurrency primitives and lock-less data structures
* [kev009/cii](https://github.com/kev009/cii) - libcii ported to Autotools/libtool - D. R. Hanson's C Interfaces and Implementations
* [kev009/craftd](https://github.com/kev009/craftd) - kev009 development repo.  Canonical repo @ craftd/craftd (see project URL)
* [kevinbirch/kanabo](https://github.com/kevinbirch/kanabo) - query JSON/YAML data with JSONPath
* [kevinlawler/kona](https://github.com/kevinlawler/kona) - Open-source implementation of the K programming language
* [kevsmith/erlz](https://github.com/kevsmith/erlz) - Erlang wrapper for the fastlz (LZO-like) data compression library
* [kfish/libfishsound](https://github.com/kfish/libfishsound) - A simple programming interface for decoding and encoding audio data using Xiph.org codecs (FLAC, Speex and Vorbis)
* [kframework/c-semantics](https://github.com/kframework/c-semantics) - Semantics of C in K
* [kgabis/parson](https://github.com/kgabis/parson) - Lightweight JSON library written in C.
* [kholia/dedrop](https://github.com/kholia/dedrop) - Looking inside the (Drop) box. Security Analysis of Dropbox. Updated WOOT '13 paper and other goodies.
* [kiibohd/controller](https://github.com/kiibohd/controller) - Kiibohd Controller
* [kinect-team-3/unifying-sensor-api](https://github.com/kinect-team-3/unifying-sensor-api) - Sensor API for data transport
* [kineme/KinectTools](https://github.com/kineme/KinectTools) - Quartz Composer plugin that retrieves color and depth image data from the Xbox Kinect.
* [kitsune-dsu/kitsune-core](https://github.com/kitsune-dsu/kitsune-core) - Kitsune runtime, driver, ktcc, xfgen, documentation, and test suite.
* [kivy/python-for-android](https://github.com/kivy/python-for-android) - Turn your Python application into an Android APK - Build your own python and extension
* [kiyo-masui/bitshuffle](https://github.com/kiyo-masui/bitshuffle) - Filter for improving compression of typed binary data.
* [kklis/proxy](https://github.com/kklis/proxy) - TCP proxy in ANSI C
* [kkos/oniguruma](https://github.com/kkos/oniguruma) - regular expression library
* [klange/nyancat](https://github.com/klange/nyancat) - Nyancat in your terminal, rendered through ANSI escape sequences. This is the source for the Debian package `nyancat`.
* [klange/toaruos](https://github.com/klange/toaruos) - A completely-from-scratch hobby operating system: bootloader, kernel, drivers, C library, and userspace including a composited graphical UI, dynamic linker, syntax-highlighting text editor, network stack, etc.
* [kljensen/Gemoda](https://github.com/kljensen/Gemoda) - A generic motif discovery algorithm for sequential data
* [kmcallister/embedded-breakpoints](https://github.com/kmcallister/embedded-breakpoints) - Embed GDB breakpoints in C source code
* [kmike/datrie](https://github.com/kmike/datrie) - Fast, efficiently stored Trie for Python. Uses libdatrie.
* [kmussel/Moment](https://github.com/kmussel/Moment) - Natural Language Date Parser Using Lex/Yacc/C
* [knopwob/dunst](https://github.com/knopwob/dunst) - lightweight and customizable notification daemon
* [knossos-project/knossos](https://github.com/knossos-project/knossos) - KNOSSOS is a software tool for the visualization and annotation of 3D image data and was developed for the rapid reconstruction of neural morphology and connectivity.
* [ko1/allocation_tracer](https://github.com/ko1/allocation_tracer) - Add ObjectSpace::AllocationTracer module.
* [koanlogic/libu](https://github.com/koanlogic/libu) - LibU is a multiplatform utility library written in C, with APIs for handling memory allocation, networking and URI parsing, string manipulation, debugging, and logging in a very compact way, plus many other miscellaneous tasks
* [kohler/gifsicle](https://github.com/kohler/gifsicle) - Gifsicle is a suite of programs for manipulating GIF images and animations.
* [kohsuke/com4j](https://github.com/kohsuke/com4j) - Type-safe Java/COM binding
* [kokke/tiny-AES-c](https://github.com/kokke/tiny-AES-c) - Small portable AES128/192/256 in C
* [kokke/tiny-AES128-C](https://github.com/kokke/tiny-AES128-C) - Small portable AES128/192/256 in C
* [korczis/foremost](https://github.com/korczis/foremost) - Foremost is a console program to recover files based on their headers, footers, and internal data structures. This process is commonly referred to as data carving. Foremost can work on image files, such as those generated by dd, Safeback, Encase, etc, or directly on a drive. The headers and footers can be specified by a configuration file or you can use command line switches to specify built-in file types. These built-in types look at the data structures of a given file format allowing for a more reliable and faster recovery.  Originally developed by the United States Air Force Office of Special Investigations and The Center for Information Systems Security Studies and Research , foremost has been opened to the general public. We welcome any comments, suggestions, patches, or feedback you have on this program. Please direct all correspondence to namikus@users.sf.net.
* [koron/cmigemo](https://github.com/koron/cmigemo) - C/Migemo
* [kosma/minmea](https://github.com/kosma/minmea) - a lightweight GPS NMEA 0183 parser library in pure C
* [kovidgoyal/html5-parser](https://github.com/kovidgoyal/html5-parser) - Fast C based HTML 5 parsing for python
* [kovidgoyal/kitty](https://github.com/kovidgoyal/kitty) - A cross-platform, fast, feature full, GPU based terminal emulator
* [kozyraki/phoenix](https://github.com/kozyraki/phoenix) - an API and runtime environment for data processing with MapReduce for shared-memory multi-core & multiprocessor systems.
* [kr/beanstalkd](https://github.com/kr/beanstalkd) - Beanstalk is a simple, fast work queue.
* [krakjoe/SIMD](https://github.com/krakjoe/SIMD) - Simple Instructions, Multiple Data
* [krakjoe/apcu](https://github.com/krakjoe/apcu) - APCu - APC User Cache
* [krakjoe/phpdbg](https://github.com/krakjoe/phpdbg) - The Interactive PHP Debugger
* [krakjoe/pthreads](https://github.com/krakjoe/pthreads) - Threading for PHP - Share Nothing, Do Everything :)
* [krallin/tini](https://github.com/krallin/tini) - A tiny but valid `init` for containers
* [krieger-od/whdd](https://github.com/krieger-od/whdd) - HDD diagnostic and data recovery tool for Linux
* [kripken/BananaBread](https://github.com/kripken/BananaBread) - BananaBread is a C++ 3D game engine that runs on the web using JavaScript+WebGL+HTML
* [kripken/emscripten](https://github.com/kripken/emscripten) - Emscripten: An LLVM-to-JavaScript Compiler
* [kripken/lua.vm.js](https://github.com/kripken/lua.vm.js) - The Lua VM, on the Web
* [kristapsdz/acme-client](https://github.com/kristapsdz/acme-client) - secure ACME client
* [kroitor/gjk.c](https://github.com/kroitor/gjk.c) - Gilbert-Johnson-Keerthi (GJK) collision detection algorithm in 200 lines of clean plain C
* [kroki/XProbes](https://github.com/kroki/XProbes) - Explicit probes (XProbes) - static user space probes with natural data access.
* [kronihias/dbap](https://github.com/kronihias/dbap) - Distance Based Amplitude Panning externals for Pure Data
* [kronihias/espeak](https://github.com/kronihias/espeak) - pure data external to synthesize text to an array with espeak library
* [kronihias/smpte-](https://github.com/kronihias/smpte-) - Pure Data/Max (flext) external for generating or decoding ltc audio timecode.
* [krutin/psoc_data_acquisition](https://github.com/krutin/psoc_data_acquisition) - Data Acquisition using usbuart of Cypress PSoC. Developed using Tinychip Axios 1.0
* [kscz/n_stress](https://github.com/kscz/n_stress) - Linux network stress tester - attempts to send and receive data over a network as fast as possible and confirm integrity of the data
* [ksheedlo/kmdata](https://github.com/ksheedlo/kmdata) - Data structures for C programmers, by C programmers.
* [ktap/ktap](https://github.com/ktap/ktap) - A lightweight script-based dynamic tracing tool for Linux
* [kuba--/zip](https://github.com/kuba--/zip) - A portable, simple zip library written in C
* [kurtisthompson/Algorithms](https://github.com/kurtisthompson/Algorithms) - Random assortment of Interesting data structures and/or algorithms and academic work
* [kwgoodman/bottleneck](https://github.com/kwgoodman/bottleneck) - Fast NumPy array functions written in C
* [kyle-github/libplctag](https://github.com/kyle-github/libplctag) - This library provides a portable and simple API for accessing PLC data over Ethernet and serial links.
* [kylemcdonald/ofxCcv](https://github.com/kylemcdonald/ofxCcv) - libccv addon for openFrameworks
* [lacker/ikalman](https://github.com/lacker/ikalman) - An iPhone-friendly Kalman filter written in C.
* [laijs/userspace-rcu](https://github.com/laijs/userspace-rcu) - Laijs-maintained  Userspace-RCU tree for concurrent data struct(cds) changes
* [lalongooo/VideoCompressor](https://github.com/lalongooo/VideoCompressor) - Video compressor based in the Telegram for Android app source code.
* [larmel/lacc](https://github.com/larmel/lacc) - A simple, self-hosting C compiler
* [larsbrinkhoff/httptunnel](https://github.com/larsbrinkhoff/httptunnel) - Creates a bidirectional virtual data path tunnelled in HTTP requests.
* [laruence/taint](https://github.com/laruence/taint) - Taint is a PHP extension, used for detecting XSS codes
* [laruence/yac](https://github.com/laruence/yac) - A fast shared memory user data cache for PHP
* [laruence/yaconf](https://github.com/laruence/yaconf) - A PHP Persistent Configurations Container
* [laruence/yaf](https://github.com/laruence/yaf) - Fast php framework written in c, built in php extension
* [laruence/yar](https://github.com/laruence/yar) - Light, concurrent RPC framework for PHP & C
* [lastpass/lastpass-cli](https://github.com/lastpass/lastpass-cli) - LastPass command line interface tool
* [laurenz/oracle_fdw](https://github.com/laurenz/oracle_fdw) - PostgreSQL extension that provides a Foreign Data Wrapper for easy and efficient access to Oracle databases, including pushdown of WHERE conditions as well as comprehensive EXPLAIN and ANALYZE support.
* [laverdet/node-fibers](https://github.com/laverdet/node-fibers) - Fiber/coroutine support for v8 and node.
* [lavoiesl/osx-cpu-temp](https://github.com/lavoiesl/osx-cpu-temp) - Outputs current CPU temperature for OSX
* [lawrancej/CompilerKit](https://github.com/lawrancej/CompilerKit) - Compiler construction library in C.
* [lbrito1/cstuff](https://github.com/lbrito1/cstuff) - Algorithms & data structures in C
* [lc-soft/LCUI](https://github.com/lc-soft/LCUI) - A small C library for building user interfaces with C, XML and CSS.
* [lcastelli/chdb](https://github.com/lcastelli/chdb) - A fast read-only memory mapped hash-table for PHP
* [ldc-developers/ldc](https://github.com/ldc-developers/ldc) - The LLVM-based D compiler.
* [leaflabs/libmaple](https://github.com/leaflabs/libmaple) - [INACTIVE] C and C++ library for STM32 ARM Cortex-M3 development boards.
* [learnopengles/airhockey](https://github.com/learnopengles/airhockey) - Repository for "Developing a Simple Game of Air Hockey Using C++ and OpenGL ES 2 for Android, iOS, and the Web", located at http://www.learnopengles.com/developing-a-simple-game-of-air-hockey-using-c-and-opengl-es-2-for-android-ios-and-the-web/
* [leecarraher/CardinalityShiftClustering](https://github.com/leecarraher/CardinalityShiftClustering) - MOVED -- https://github.com/wilseypa/rphash -- Ongoing research into communication minimizing parallel data clustering for an LSH accelerated random projection mean-shift algorithm.
* [leecbaker/datareftool](https://github.com/leecbaker/datareftool) - Dataref Tool for X-Plane plugin development
* [lefcha/imapfilter](https://github.com/lefcha/imapfilter) - IMAP mail filtering utility
* [lemire/Code-used-on-Daniel-Lemire-s-blog](https://github.com/lemire/Code-used-on-Daniel-Lemire-s-blog) - This is a repository for the code posted on my blog
* [lemire/clhash](https://github.com/lemire/clhash) - C library implementing the ridiculously fast CLHash  hashing function
* [lemire/simdcomp](https://github.com/lemire/simdcomp) - A simple C library for compressing lists of integers using binary packing
* [lennylxx/leetcode](https://github.com/lennylxx/leetcode) - Pure C solution for LeetCode
* [leonindy/camel](https://github.com/leonindy/camel) - camel: soft load balance(slb) midware - control nginx servers by portal and api.
* [lericson/pylibmc](https://github.com/lericson/pylibmc) - A Python wrapper around the libmemcached interface from TangentOrg.
* [letoram/arcan](https://github.com/letoram/arcan) - Arcan - [Display Server, Multimedia Framework, Game Engine] -> "Desktop Engine"
* [lexborisov/Modest](https://github.com/lexborisov/Modest) - Modest is a fast HTML renderer implemented as a pure C99 library with no outside dependencies.
* [lexborisov/myhtml](https://github.com/lexborisov/myhtml) - Fast C/C++ HTML 5 Parser. Using threads.
* [lfittl/libpg_query](https://github.com/lfittl/libpg_query) - C library for accessing the PostgreSQL parser outside of the server environment
* [lfos/calcurse](https://github.com/lfos/calcurse) - A text-based calendar and scheduling application
* [lgfischer/dcel](https://github.com/lgfischer/dcel) - A DCEL implementation, described in details in http://leonardofischer.com/dcel-data-structure-c-plus-plus-implementation/
* [lgsonic/mysqlIncSync](https://github.com/lgsonic/mysqlIncSync) - A mysql incremental synchronization tool which can parse mysql row-format binlog and process the incremental data
* [lh3/bioawk](https://github.com/lh3/bioawk) - BWK awk modified for biological data
* [lh3/bwa](https://github.com/lh3/bwa) - Burrow-Wheeler Aligner for pairwise alignment between DNA sequences
* [lh3/naivepca](https://github.com/lh3/naivepca) - Naive PCA for genotype data
* [liamoc/learn-you-an-agda](https://github.com/liamoc/learn-you-an-agda) - Learn you an Agda (and achieve enlightenment)
* [liballeg/allegro5](https://github.com/liballeg/allegro5) - The official Allegro 5 git repository. Pull requests welcome!
* [libamqp/libamqp](https://github.com/libamqp/libamqp) - libamqp is a C client for the AMQP 1.0 protocol
* [libarchive/libarchive](https://github.com/libarchive/libarchive) - Multi-format archive and compression library
* [libass/libass](https://github.com/libass/libass) - libass is a portable subtitle renderer for the ASS/SSA (Advanced Substation Alpha/Substation Alpha) subtitle format.
* [libav/c99-to-c89](https://github.com/libav/c99-to-c89) - Tool to convert C99 code to MSVC-compatible C89
* [libav/libav](https://github.com/libav/libav) - Libav github mirror, clone of git://git.libav.org/libav
* [libcheck/check](https://github.com/libcheck/check) - A unit testing framework for C
* [libertyernie/goombasav](https://github.com/libertyernie/goombasav) - Extract/replace Game Boy SRAM data stored in Goomba/Goomba Color SRAM
* [libexpat/libexpat](https://github.com/libexpat/libexpat) - :herb: Expat library: Fast streaming XML parser written in C; in the process of migrating from SourceForge to GitHub
* [libfirm/cparser](https://github.com/libfirm/cparser) - C99 parser and frontend for libfirm
* [libfirm/libfirm](https://github.com/libfirm/libfirm) - graph based intermediate representation and backend for optimising compilers
* [libgdx/fbx-conv](https://github.com/libgdx/fbx-conv) - Command line utility using the FBX SDK to convert FBX/Collada/Obj files to a custom text/binary format for static, keyframed and skinned meshes.
* [libgit2/libgit2](https://github.com/libgit2/libgit2) - The Library
* [libgit2/php-git](https://github.com/libgit2/php-git) - PHP bindings for libgit2
* [libgit2/pygit2](https://github.com/libgit2/pygit2) - Python bindings for libgit2
* [libgit2/rugged](https://github.com/libgit2/rugged) - ruby bindings to libgit2
* [libharu/libharu](https://github.com/libharu/libharu) - libharu - free PDF library
* [libical/libical](https://github.com/libical/libical) - Libical is an Open Source implementation of the iCalendar protocols and protocol data units.
* [libimobiledevice/libimobiledevice](https://github.com/libimobiledevice/libimobiledevice) - A cross-platform protocol library to communicate with iOS devices
* [libopencm3/libopencm3](https://github.com/libopencm3/libopencm3) - Open Source ARM cortex m microcontroller library
* [libpd/libpd](https://github.com/libpd/libpd) - Pure Data embeddable audio synthesis library
* [libressl-portable/portable](https://github.com/libressl-portable/portable) - LibreSSL Portable itself. This includes the build scaffold and compatibility layer that builds portable LibreSSL from the OpenBSD source code.
* [libretro/RetroArch](https://github.com/libretro/RetroArch) - Cross-platform, sophisticated frontend for the libretro API. Licensed GPLv3.
* [libretro/common-shaders](https://github.com/libretro/common-shaders) - Collection of commonly used Cg shaders. These shaders are usable by either HLSL and/or Cg runtime compilers. The cg2glsl script will translate most of these into GLSL shaders.
* [libssh2/libssh2](https://github.com/libssh2/libssh2) - the SSH library
* [libtom/libtomcrypt](https://github.com/libtom/libtomcrypt) - LibTomCrypt is a fairly comprehensive, modular and portable cryptographic toolkit that provides developers with a vast array of well known published block ciphers, one-way hash functions, chaining modes, pseudo-random number generators, public key cryptography and a plethora of other routines.
* [libtom/libtommath](https://github.com/libtom/libtommath) - LibTomMath is a free open source portable number theoretic multiple-precision integer library written entirely in C.
* [libtom/tomsfastmath](https://github.com/libtom/tomsfastmath) - TomsFastMath is a fast public domain, open source, large integer arithmetic library written in portable ISO C.
* [libtrading/libtrading](https://github.com/libtrading/libtrading) - Libtrading, an ultra low-latency trading connectivity library for C and C++.
* [libusb/libusb](https://github.com/libusb/libusb) - A cross-platform library to access USB devices
* [libuv/libuv](https://github.com/libuv/libuv) - Cross-platform asychronous I/O
* [lichuang/qnode](https://github.com/lichuang/qnode) - qnode(cute node) - C + Lua + Actor Model = Erlang-like system
* [licstar/compare](https://github.com/licstar/compare) - compare embedding
* [lidaof/methylQA](https://github.com/lidaof/methylQA) - methylation sequence data quality assessment tool
* [limccn/Cocoa-Charts](https://github.com/limccn/Cocoa-Charts) - Open-source iPhone/iPad graph/chart framework includes line chart,stick chart,candlestick chart,pie chart,spider-web chart etc. Based on iOS graph SDK, Using native Objective-c Codes
* [limingth/NCCL](https://github.com/limingth/NCCL) - New Concept C Language
* [limpkin/mooltipass](https://github.com/limpkin/mooltipass) - Github repository dedicated to the mooltipass project
* [lincomatic/Colorduino](https://github.com/lincomatic/Colorduino) - Colorduino Interface Library for Arduino
* [linkedin/datacl](https://github.com/linkedin/datacl) - A collection of efficient utilities for a data scientist.
* [linklayer/cantact-fw](https://github.com/linklayer/cantact-fw) - Firmware source files for the CANtact tool
* [linleyh/liberation-circuit](https://github.com/linleyh/liberation-circuit) - Trapped in a hostile computer system, you must make a way out - RTS/coding game
* [linux-can/can-utils](https://github.com/linux-can/can-utils) - Linux-CAN / SocketCAN user space applications
* [linux-nvme/nvme-cli](https://github.com/linux-nvme/nvme-cli) - NVMe management command line interface.
* [linux-rdma/rdma-core](https://github.com/linux-rdma/rdma-core) - RDMA core userspace libraries and daemons
* [linux-test-project/ltp](https://github.com/linux-test-project/ltp) - Linux Test Project
* [linuxmint/Cinnamon](https://github.com/linuxmint/Cinnamon) - A Linux Desktop featuring a traditional layout, built from modern technology and introducing brand new innovative features.
* [linuxmint/nemo](https://github.com/linuxmint/nemo) - File browser for Cinnamon
* [linyiqun/Redis-Code](https://github.com/linyiqun/Redis-Code) - redis键值数据库源码分析
* [lioncash/ExtractData](https://github.com/lioncash/ExtractData) - An extraction tool for visual novels. Originally developed by Yuu.
* [lionsoul2014/friso](https://github.com/lionsoul2014/friso) - High performance chinese tokenizer with both GBK and UTF-8 charset support developed by ANSI C
* [lionsoul2014/ip2region](https://github.com/lionsoul2014/ip2region) - Ip2region is a offline IP location library with accuracy rate of 99.9% and 0.0x millseconds searching performance. DB file is less then 5Mb with all ip address stored. binding for Java,PHP,C,Python,Nodejs,Golang,C#,lua. Binary,B-tree,Memory searching algorithm
* [lip6-lisp/data-plane](https://github.com/lip6-lisp/data-plane) - OpenLISP data plane
* [litehelpers/Cordova-sqlite-storage](https://github.com/litehelpers/Cordova-sqlite-storage) - A Cordova/PhoneGap plugin to open and use sqlite databases on Android/iOS/Windows Universal(8.1)/Amazon Fire-OS/WP(7/8) with HTML5/Web SQL API
* [littlevgl/lvgl](https://github.com/littlevgl/lvgl) - Graphics library to create an embedded GUI with easy-to-use graphical elements, beautiful visual effects and low memory footprint. It offers anti-aliasing, opacity, and animations using only one frame buffer.
* [liudf0716/apfree_wifidog](https://github.com/liudf0716/apfree_wifidog) - Apfree WiFidog is an  efficient captive portal solution for wireless router which with embeded linux(LEDE/Openwrt) system.
* [liudf0716/xkcptun](https://github.com/liudf0716/xkcptun) - xkcptun is kcp tunnel for OpenWRT&LEDE, implemented in c language
* [liuliu/ndqi](https://github.com/liuliu/ndqi) - Non-structural Data Query Interface
* [liuluheng/levmu](https://github.com/liuluheng/levmu) - Based on redis protocol, storing data in leveldb, using muduo for communication
* [livioso/datastructures-in-C](https://github.com/livioso/datastructures-in-C) - Implementation of a some data structures in C for educational purposes. For example featuring a trie implementation in C (inspired by DAS84 "a bit of C") or a XOR linked list.
* [liyuming1978/NativeLibCompression](https://github.com/liyuming1978/NativeLibCompression) - The native library compression sdk is given to solve the apk size problem. It is easy to integrate and will get max 50% size decreasing. Not only sdk, a Java tool for package is provided to convert normal apk to compressed apk.  MIT Licence, you can use any where
* [ljianhui/Data-Structure](https://github.com/ljianhui/Data-Structure) - 这个库的内容大多为数据结构及其具体实现代码，还包含一些基本的算法！
* [ljmocic/PJISP](https://github.com/ljmocic/PJISP) - Programming Languages and Data Structures
* [lkarsten/libvmod-cookie](https://github.com/lkarsten/libvmod-cookie) - A Varnish module for simpler use of the cookie header.
* [lloyd/yajl](https://github.com/lloyd/yajl) - A fast streaming JSON parsing library in C.
* [llvm-mirror/compiler-rt](https://github.com/llvm-mirror/compiler-rt) - Mirror of official compiler-rt git repository located at http://llvm.org/git/compiler-rt.  Updated every five minutes.
* [lneto/luadata](https://github.com/lneto/luadata) - Lua data library
* [locasto/libdisorder](https://github.com/locasto/libdisorder) - A simple C library for entropy measurement of byte streams and other data.
* [lopter/lightsd](https://github.com/lopter/lightsd) - A daemon with a JSON-RPC API to control your light bulbs
* [lotabout/write-a-C-interpreter](https://github.com/lotabout/write-a-C-interpreter) - Write a simple interpreter of C. Inspired by c4 and largely based on it.
* [louiswins/RB-Tree](https://github.com/louiswins/RB-Tree) - An implementation of the Red-Black Tree data structure.
* [lp/ObjCHiredis](https://github.com/lp/ObjCHiredis) - Hiredis with Objective-C Interface
* [lp/pdtest](https://github.com/lp/pdtest) - Pure Data testing external
* [lp/puredis](https://github.com/lp/puredis) - Pure-Data Redis External
* [lpabon/cmockery2](https://github.com/lpabon/cmockery2) - Reviving cmockery unit test framework from Google
* [lpan/viw](https://github.com/lpan/viw) - VI Worsened, a lightweight and fun VI clone.
* [lpereira/lwan](https://github.com/lpereira/lwan) - Experimental, scalable, high performance HTTP server
* [lpsantil/rt0](https://github.com/lpsantil/rt0) - A minimal C runtime for Linux i386 & x86_64
* [lqez/npk](https://github.com/lqez/npk) - neat package system written in C
* [lqs/crabdb](https://github.com/lqs/crabdb) - CrabDB - a fast, flexible and space-effective database.
* [lsalzman/enet](https://github.com/lsalzman/enet) - ENet reliable UDP networking library
* [lthiery/SPI-Py](https://github.com/lthiery/SPI-Py) - Hardware SPI as a C Extension for Python
* [lua/lua](https://github.com/lua/lua) - Unofficial git history of Lua releases
* [luarpro/BitmapDataQRCodeScanner](https://github.com/luarpro/BitmapDataQRCodeScanner) - Flash AIR Native Extension:  QRCode reader/decoder which accept BitmapData, therefore you can design your own scanner UI, adding overlay image, without launch  fullscreen native Camera UI
* [lubyk/lubyk](https://github.com/lubyk/lubyk) - Open source patcher for multimedia projects: glue all this midi, DMX, neural networks, opengl stuff into a fast C++ core with Lua scriptable objects.
* [lucasb-eyer/heatmap](https://github.com/lucasb-eyer/heatmap) - High performance C heatmap generation library. Supposed to be wrapped by higher-level languages.
* [lucasjones/cpuminer-multi](https://github.com/lucasjones/cpuminer-multi) - Multi-algo CPUMiner & Reference Cryptonote Miner (JSON-RPC 2.0)
* [ludocode/mpack](https://github.com/ludocode/mpack) - MPack - A C encoder/decoder for the MessagePack serialization format / msgpack.org[C]
* [luke-jr/bfgminer](https://github.com/luke-jr/bfgminer) - Modular ASIC/FPGA miner written in C, featuring overclocking, monitoring, fan speed control and remote interface capabilities.
* [lukeredpath/libPusher](https://github.com/lukeredpath/libPusher) - An Objective-C interface to Pusher (pusherapp.com)
* [lukeweber/webrtc-jingle-client](https://github.com/lukeweber/webrtc-jingle-client) - Webrtc audio + jingle protocol brought to IOS and Android.
* [lumpyzhu/nmscc](https://github.com/lumpyzhu/nmscc) - nmscc is a library of C++14 components designed for for scientific computation.
* [luohaha/CSpider](https://github.com/luohaha/CSpider) - A scalable and convenient crawler framework in C:).
* [lvzixun/Clang-Complete](https://github.com/lvzixun/Clang-Complete) - a auto complete plugin for sublimetext3
* [lwfinger/rtl8188eu](https://github.com/lwfinger/rtl8188eu) - Repository for stand-alone RTL8188EU driver.
* [lwfinger/rtlwifi_new](https://github.com/lwfinger/rtlwifi_new) - A repo for the newest Realtek rtlwifi codes.
* [lxc/lxc](https://github.com/lxc/lxc) - LXC - Linux Containers
* [lxc/lxcfs](https://github.com/lxc/lxcfs) - FUSE filesystem for LXC
* [lyda/tz](https://github.com/lyda/tz) - Historical archive of the zoneinfo project.  Generated from the original data with the tz-history-scripts.
* [lyjdamzwf/chaos](https://github.com/lyjdamzwf/chaos) - c++ 网络事件库
* [lyosha/ctags-go](https://github.com/lyosha/ctags-go) - Go support for exuberant ctags
* [lz4/lz4](https://github.com/lz4/lz4) - Extremely Fast Compression algorithm
* [m-schmoock/lcpp](https://github.com/m-schmoock/lcpp) - A Lua C PreProcessor
* [m0nad/Diamorphine](https://github.com/m0nad/Diamorphine) - LKM rootkit for Linux Kernels 2.6.x/3.x/4.x (x86 and x86_64)
* [m0wfo/cups](https://github.com/m0wfo/cups) - Ruby bridge to CUPS API
* [m8rge/cwebsocket](https://github.com/m8rge/cwebsocket) - cWebsocket is lightweight websocket server library
* [mabl/ChibiOS](https://github.com/mabl/ChibiOS) - Mirror of the ChibiOS SVN repository (updated every 10 minutes)
* [machinezone/tcpkali](https://github.com/machinezone/tcpkali) - Fast multi-core TCP and WebSockets load generator.
* [maciejczyzewski/hashbase](https://github.com/maciejczyzewski/hashbase) - A fast, efficient on-disk/in-memory database with many different kind of data structures. :floppy_disk:
* [maciejczyzewski/retter](https://github.com/maciejczyzewski/retter) - A collection of hash functions, ciphers, tools, libraries, and materials related to cryptography. :closed_lock_with_key:
* [mackron/dr_libs](https://github.com/mackron/dr_libs) - A collection of public domain single-file libraries for C/C++.
* [mackyle/sqlite](https://github.com/mackyle/sqlite) - Unofficial git mirror of SQLite sources (see link for build instructions)
* [macmade/ClangKit](https://github.com/macmade/ClangKit) - ClangKit provides an Objective-C frontend to LibClang. Source tokenization, diagnostics and fix-its are actually implemented.
* [macournoyer/tinyrb](https://github.com/macournoyer/tinyrb) - The tiny and fast (subset of) Ruby VM that loves you like you are
* [madeye/gaeproxy](https://github.com/madeye/gaeproxy) - GAEProxy for Android
* [madeye/proxydroid](https://github.com/madeye/proxydroid) - Global Proxy for Android
* [madhur/android-chat-starter](https://github.com/madhur/android-chat-starter) - A starter project for Android chat application
* [madler/zlib](https://github.com/madler/zlib) - A massively spiffy yet delicately unobtrusive compression library.
* [madnoda/stm32f4-glcd-logger](https://github.com/madnoda/stm32f4-glcd-logger) - Data Logger with LCD
* [magellannh/rtl-wx](https://github.com/magellannh/rtl-wx) - RTL-Wx logs data from 433Mhz wireless sensors using an RTL-SDR dongle.  The Wiki has some screenshots of the results
* [magnumripper/JohnTheRipper](https://github.com/magnumripper/JohnTheRipper) - This is the official repo for the Jumbo version of John the Ripper. The "bleeding-jumbo" branch (default) is based on 1.8.0-Jumbo-1 (but we are literally several thousands of commits ahead of it).
* [magnuskarlsson/SDLogger](https://github.com/magnuskarlsson/SDLogger) - Open Hardware Data Logger
* [mainroach/crabby](https://github.com/mainroach/crabby) - A texture compression algorithm for sprite sheets that allows decompression on the GPU during rendering.
* [majn/telegram-purple](https://github.com/majn/telegram-purple) - Adds support for Telegram to Pidgin, Adium, Finch and other Libpurple based messengers.
* [makefu/skytraq-datalogger](https://github.com/makefu/skytraq-datalogger) - configuration and download tool for GPS data loggers based on Skytraq Venus 5 and 6 chipsets
* [malbrain/Btree-source-code](https://github.com/malbrain/Btree-source-code) - A working project for High-concurrency B-tree source code in C
* [mamedev/mame](https://github.com/mamedev/mame) - MAME - Multiple Arcade Machine Emulator
* [mar-file-system/marfs](https://github.com/mar-file-system/marfs) - MarFS provides a scalable near-POSIX file system by using one or more POSIX file systems as a scalable metadata component and one ore more data stores (object, file, etc) as a scalable data component. Our initial implementation will use GPFS file systems as the metadata component and Scality and EMC ECS ViPR object stores as the data component.
* [marcelloceschia/chan-datacard](https://github.com/marcelloceschia/chan-datacard) - clone of https://code.google.com/p/asterisk-chan-dongle/ with asterisk 11 branch
* [marcobambini/gravity](https://github.com/marcobambini/gravity) - Gravity Programming Language
* [marekweb/datastructs-c](https://github.com/marekweb/datastructs-c) - Arraylist and Hashtable implementation in C
* [marforic/imagemagick_lib_iphone](https://github.com/marforic/imagemagick_lib_iphone) - Scripts and instructions to compile ImageMagick as a static library to use in any iOS project
* [mariadb-corporation/MaxScale](https://github.com/mariadb-corporation/MaxScale) - A content aware, plug-able proxy server.           Discuss @: maxscale@googlegroups.com
* [mariokonrad/grib](https://github.com/mariokonrad/grib) - GRIB data access
* [mariusae/heapster](https://github.com/mariusae/heapster) - production heap profiling for the JVM.  compatible with google-perftools.
* [markjasonanderson/wiegand-linux](https://github.com/markjasonanderson/wiegand-linux) - Linux driver for reading wiegand data from GPIO. Tested  for ARM 9G20 (linux stamp)
* [marssaxman/startc](https://github.com/marssaxman/startc) - minimal freestanding C library for bare-metal i386 development
* [martanne/vis](https://github.com/martanne/vis) - A vi-like editor based on Plan 9's structural regular expressions
* [martincohen/Punity](https://github.com/martincohen/Punity) - A tiny game engine in C.
* [martinezjavier/ldd3](https://github.com/martinezjavier/ldd3) - Linux Device Drivers 3 examples updated to work in recent kernels
* [martinh/libconfuse](https://github.com/martinh/libconfuse) - Small configuration file parser library for C.
* [masterzen/nginx-upload-progress-module](https://github.com/masterzen/nginx-upload-progress-module) - Nginx module implementing an upload progress system, that monitors RFC1867 POST uploads as they are transmitted to upstream servers.
* [mate-desktop/caja](https://github.com/mate-desktop/caja) - Caja, the file manager for the MATE desktop
* [matianfu/FUNK](https://github.com/matianfu/FUNK) - a c continuation library inspired by Adam Dunkel's ProtoThread.
* [matildah/fastcat](https://github.com/matildah/fastcat) - netcat-like thing that uses the linux syscall splice(2) to avoid overhead from copying data from kernelspace/userspace
* [matricks/teeworlds](https://github.com/matricks/teeworlds) - A retro multiplayer shooter
* [matsumoto-r/ngx_mruby](https://github.com/matsumoto-r/ngx_mruby) - ngx_mruby - A Fast and Memory-Efficient Web Server Extension Mechanism Using Scripting Language mruby for nginx
* [mattbornski/cdf](https://github.com/mattbornski/cdf) - A Python package which handles files in NASA Common Data Format
* [mattconnolly/ZipArchive](https://github.com/mattconnolly/ZipArchive) - zip archive processing for Cocoa - iPhone and OS X
* [matteobertozzi/blog-code](https://github.com/matteobertozzi/blog-code) - Blog Code
* [matteobertozzi/carthage](https://github.com/matteobertozzi/carthage) - Pure C Data Structure and Utils
* [mattfoster/matlab-interpolation-toolkit](https://github.com/mattfoster/matlab-interpolation-toolkit) - A matlab toolkit for interpolating scattered data in interesting ways.
* [mattgodbolt/zindex](https://github.com/mattgodbolt/zindex) - Create an index on a compressed text file
* [matthijskooijman/arduino-lmic](https://github.com/matthijskooijman/arduino-lmic) - LoraWAN-in-C library, adapted to run under the Arduino environment
* [mattiasgustavsson/libs](https://github.com/mattiasgustavsson/libs) - Single-file public domain libraries for C/C++
* [mattjr/structured](https://github.com/mattjr/structured) - Tools for the Generation and Visualization of Large-scale Three-dimensional Reconstructions from Image Data.
* [mattn/go-sqlite3](https://github.com/mattn/go-sqlite3) - sqlite3 driver for go that using database/sql
* [mattsta/crcspeed](https://github.com/mattsta/crcspeed) - This make CRC be fast.  Included implementations: CRC-64-Jones and CRC-16-CCITT
* [mattt/MsgPackSerialization](https://github.com/mattt/MsgPackSerialization) - MsgPack Serialization for Objective-C
* [matz/streem](https://github.com/matz/streem) - prototype of stream based programming language
* [maximeh/tesla](https://github.com/maximeh/tesla) - Grab data from an OWL-CM160 and generate graph using RRD
* [maxmind/geoip-api-c](https://github.com/maxmind/geoip-api-c) - GeoIP Legacy C API
* [maxmind/libmaxminddb](https://github.com/maxmind/libmaxminddb) - C library for the MaxMind DB file format
* [mback2k/wireshark-amf](https://github.com/mback2k/wireshark-amf) - Wireshark dissector for the Action Message Format data protocol and representation
* [mbebenita/Broadway](https://github.com/mbebenita/Broadway) - A JavaScript H.264 decoder.
* [mbeddr/mbeddr.core](https://github.com/mbeddr/mbeddr.core) - The mbeddr core. An extensible C
* [mbedmicro/CMSIS-DAP](https://github.com/mbedmicro/CMSIS-DAP) - Interface Firmware providing USB CMSIS-DAP for debugging, USB MSD for programming, USB Serial for communication.
* [mbedmicro/mbed](https://github.com/mbedmicro/mbed) - mbed libraries and tools
* [mbornet-hl/hl](https://github.com/mbornet-hl/hl) - Highlight (colorize) text data using regular expressions
* [mbrazeau/Morphy](https://github.com/mbrazeau/Morphy) - Phylogenetic analysis of morphological data
* [mbrossard/threadpool](https://github.com/mbrossard/threadpool) - A simple C Thread pool implementation
* [mbykov/diglossa.data](https://github.com/mbykov/diglossa.data) - texts for diglossa.org
* [mcandre/qc](https://github.com/mcandre/qc) - qc - A C port of the QuickCheck unit test framework
* [mchck/mchck](https://github.com/mchck/mchck) - MC HCK, the small and cheap microcontroller board!
* [mchochlov/Gnucash](https://github.com/mchochlov/Gnucash) - Data model unit testing - GSoC 2011
* [mclap/tdsproxy](https://github.com/mclap/tdsproxy) - tabular data stream (TDS) proxy server
* [mcxiaoke/dsaac](https://github.com/mcxiaoke/dsaac) - Learn Data Structures and Algorithm Analysis in C
* [mdaines/viz.js](https://github.com/mdaines/viz.js) - A hack to put GraphViz on the web.
* [mdirolf/nginx-gridfs](https://github.com/mdirolf/nginx-gridfs) - Nginx module for serving files from MongoDB's GridFS
* [meetecho/janus-gateway](https://github.com/meetecho/janus-gateway) - Janus WebRTC Gateway
* [meganz/sdk](https://github.com/meganz/sdk) - MEGA C++ SDK
* [megous/megatools](https://github.com/megous/megatools) - Open-source command line tools and C library (libmega) for accessing Mega.co.nz cloud storage.
* [memcached/memcached](https://github.com/memcached/memcached) - memcached development tree
* [memo/ofxMSAInterpolator](https://github.com/memo/ofxMSAInterpolator) - C++ openFrameworks addon with a set of template classes for doing various types of interpolations on data with any number of dimensions. You can feed the system an arbitrary number of data, then resample at any resolution, or ask for the value at any percentage along the data. Input data can be floats (for 1D splines, Vec2f (for 2D splines), Vec3f (for 3D splines), or even matrices, or custom data types (e.g. biped pose). Demo at www.memo.tv/msainterpolator
* [memononen/nanovg](https://github.com/memononen/nanovg) - Antialiased 2D vector drawing library on top of OpenGL for UI and visualizations.
* [mempodippy/vlany](https://github.com/mempodippy/vlany) - Linux LD_PRELOAD rootkit (x86 and x86_64 architectures)
* [menudoproblema/libemqtt](https://github.com/menudoproblema/libemqtt) - Embedded C client library for the MQTT protocol
* [messense/data-structure-learning](https://github.com/messense/data-structure-learning) - 数据结构学习，作业代码
* [metadave/erln8](https://github.com/metadave/erln8) - A sneaky Erlang version manager, v1 (C version)
* [methodmissing/rbczmq](https://github.com/methodmissing/rbczmq) - Ruby extension that wraps the official high level ZeroMQ C API ( http://czmq.zeromq.org/ )
* [mevdschee/2048.c](https://github.com/mevdschee/2048.c) - Console version of the game "2048" for GNU/Linux
* [mfragkoulis/PiCO_QL](https://github.com/mfragkoulis/PiCO_QL) - SQL query interface to C++ collections and C data structures. Also configurable as a loadable Linux kernel module and an extension to Valgrind tools.
* [mgalloy/ridl](https://github.com/mgalloy/ridl) - Really Interactive Data Language
* [mgba-emu/mgba](https://github.com/mgba-emu/mgba) - mGBA Game Boy Advance Emulator
* [mgp/redis-types](https://github.com/mgp/redis-types) - Library of the Redis data types
* [mhogomchungu/zuluCrypt](https://github.com/mhogomchungu/zuluCrypt) - zuluCrypt is a front end to cryptsetup and tcplay and it allows easy management of encrypted block devices
* [mhroth/tinyosc](https://github.com/mhroth/tinyosc) - A minimal Open Sound Control (OSC) library written in vanilla C.
* [miao1007/Openwrt-NetKeeper](https://github.com/miao1007/Openwrt-NetKeeper) - [C/C++] Run Netkeeper on OpenWrt Device
* [micahpearlman/MonkVG](https://github.com/micahpearlman/MonkVG) - MonkVG is an OpenVG 1.1 like vector graphics API implementation optimized for game use currently using an OpenGL ES backend that should be compatible with any HW that supports OpenGL ES 2.0 which includes most iOS and Android devices.
* [michaeldv/pit](https://github.com/michaeldv/pit) - The project manager from hell (integrates with Git)
* [michaeltyson/TPCircularBuffer](https://github.com/michaeltyson/TPCircularBuffer) - A simple, fast circular buffer implementation
* [microbuilder/LPC1114CodeBase](https://github.com/microbuilder/LPC1114CodeBase) - Open Source SW Library for NXP's LPC1114 ARM Cortex M0 MCU
* [microbuilder/LPC11U_LPC13U_CodeBase](https://github.com/microbuilder/LPC11U_LPC13U_CodeBase) - Open source code base for ARM Cortex M3 LPC1347 or Cortex M0 LPC11U37/LPC11U24 MCUs
* [microbuilder/LPC1343CodeBase](https://github.com/microbuilder/LPC1343CodeBase) - Generic GCC-based library for the ARM Cortex-M3 LPC1343
* [microbuilder/LPC810_CodeBase](https://github.com/microbuilder/LPC810_CodeBase) - Open source code base for the ARM Cortex M0+ LPC810 family from NXP
* [micronucleus/micronucleus](https://github.com/micronucleus/micronucleus) - ATTiny usb bootloader with a strong emphasis on bootloader compactness.
* [micropython/micropython](https://github.com/micropython/micropython) - MicroPython - a lean and efficient Python implementation for microcontrollers and constrained systems
* [mid-kid/CakesForeveryWan](https://github.com/mid-kid/CakesForeveryWan) - A CFW for the 3DS.
* [miezuit/php-base85](https://github.com/miezuit/php-base85) - A PHP extension to encode/decode data with base85.
* [mikebmcl/N3888_RefImpl](https://github.com/mikebmcl/N3888_RefImpl) - Reference Implementations of ISO C++ P0267
* [mikedlowis/data-structures](https://github.com/mikedlowis/data-structures) - A collection of data structures implemented in C to be included in multiple projects.
* [mikelhernaez/qvz](https://github.com/mikelhernaez/qvz) - A Lossy compressor for Quality Scores in Genomic Data
* [mikeryan/crackle](https://github.com/mikeryan/crackle) - Crack and decrypt BLE encryption
* [mikewest/nginx-static-etags](https://github.com/mikewest/nginx-static-etags) - Nginx doesn't generate etags for static content.  I'd like it to.  Let's see if I can remember some C from college.
* [mil/foo-wm](https://github.com/mil/foo-wm) - A minimal window manager that organizes windows in a tree data structure, provides a socket to send commands to, and nothing more.
* [mindboards/ev3sources](https://github.com/mindboards/ev3sources) - LEGO MINDSTORMS EV3 source code
* [mingzhao/dm-cache](https://github.com/mingzhao/dm-cache) - Generic block-level cache utility based on Linux device mapper framework
* [minix3/minix](https://github.com/minix3/minix) - MINIX 3 (mirror)
* [mintomic/mintomic](https://github.com/mintomic/mintomic) - [deprecated] For native C atomics, see Turf instead
* [minusinf/opengl_dataviewer](https://github.com/minusinf/opengl_dataviewer) - A simple OpenGL xyzw dataviewer
* [miohtama/python-Levenshtein](https://github.com/miohtama/python-Levenshtein) - The Levenshtein Python C extension module contains functions for fast computation of Levenshtein distance and string similarity
* [miracl/MIRACL](https://github.com/miracl/MIRACL) - MIRACL Cryptographic SDK: Multiprecision Integer and Rational Arithmetic Cryptographic Library is a C software library that is widely regarded by developers as the gold standard open source SDK for elliptic curve cryptography (ECC).
* [mirek/CoreSQLite3](https://github.com/mirek/CoreSQLite3) - Core SQLite3 for iOS and OSX. Fast. Clean. Powerful...
* [mirek/CoreWebSocket](https://github.com/mirek/CoreWebSocket) - Web Socket Server and Client Library for iOS and OSX. Follows Core Foundation API style.
* [mirek/YAML.framework](https://github.com/mirek/YAML.framework) - Proper YAML support for Objective-C. Based on recommended libyaml.
* [mischasan/aho-corasick](https://github.com/mischasan/aho-corasick) - A-C implementation in "C". Tight-packed (interleaved) state-transition matrix -- as fast as it gets, as small as it gets.
* [mist64/hvdos](https://github.com/mist64/hvdos) - hvdos, a simple DOS emulator based on the OS X Hypervisor.framework
* [mist64/pucrunch](https://github.com/mist64/pucrunch) - pucrunch, an Optimizing Hybrid LZ77 RLE Data Compression Program for C64/C128/VIC-20/Plus4
* [mist64/xhyve](https://github.com/mist64/xhyve) - xhyve, a lightweight OS X virtualization solution
* [mit-carbon/Flat-Combining](https://github.com/mit-carbon/Flat-Combining) - Traditional data-structure designs, whether lock-based or lock-free, provide parallelism via fine grained synchronization among threads. Flat Combining is a new, efficient synchronization paradigm based on coarse locking.
* [mjg59/mei-amt-check](https://github.com/mjg59/mei-amt-check) - Check whether AMT is enabled and provisioned under Linux
* [mjording/ttyrec](https://github.com/mjording/ttyrec) - ttyrec is a tty recorder. Recorded data can be played back with the included ttyplay command. ttyrec is just a derivative of script command for recording timing information with microsecond accuracy as well. It can record emacs -nw, vi, lynx, or any programs running on tty.
* [mklong/libngx](https://github.com/mklong/libngx) - static library about nginx core data structure include array,buf,hash,list,queue ,tree,string and memory pool
* [mkoppanen/php-zmq](https://github.com/mkoppanen/php-zmq) - ZeroMQ for PHP
* [mkorenkov/ipad_charge](https://github.com/mkorenkov/ipad_charge) - charge Apple devices under Ubuntu Linux
* [mkottman/AndroLua](https://github.com/mkottman/AndroLua) - Lua and LuaJava ported to Android
* [mkottman/acpi_call](https://github.com/mkottman/acpi_call) - A linux kernel module that enables calls to ACPI methods through /proc/acpi/call. Now with support for Integer, String and Buffer parameters.
* [mlaurijsse/linux-mpu9150](https://github.com/mlaurijsse/linux-mpu9150) - 9-axis data fusion for Linux-based systems using the InvenSense MPU-9150 IMU
* [mlin/ocaml-bgzf](https://github.com/mlin/ocaml-bgzf) - OCaml library for BGZF, a gunzip-compatible format allowing random access to the uncompressed data
* [mlongob/Linux-Kernel-Hack](https://github.com/mlongob/Linux-Kernel-Hack) - Minimal Hacks to the Linux Kernel to gather data about machine utilization
* [mltframework/mlt](https://github.com/mltframework/mlt) - MLT Multimedia Framework
* [mm2/Little-CMS](https://github.com/mm2/Little-CMS) - A free, open source, CMM engine. It provides fast transforms between ICC profiles.
* [mmadry/st-hmp](https://github.com/mmadry/st-hmp) - Implementation of the Spatio-Temporal Hierarchical Matching Pursuit (ST-HMP) descriptor presented in the paper: M. Madry, L. Bo, D. Kragic, D. Fox, "ST-HMP: Unsupervised Spatio-Temporal Feature Learning for Tactile Data". In ICRA, 2014 (Download: http://www.nada.kth.se/~madry/publications/madry2014ICRA.pdf).
* [mmb/vmod_dgram](https://github.com/mmb/vmod_dgram) - Varnish VMOD to send data over UDP from VCL.
* [mmin18/WaxPatch](https://github.com/mmin18/WaxPatch) - Dynamically load a lua script to change the behavior of your iOS application.
* [mnacos/pg51g](https://github.com/mnacos/pg51g) - a data diff toolkit for PostgreSQL
* [moai/moai-beta](https://github.com/moai/moai-beta) - WARNING: This repository has been deprecated. Please update and submit all pull requests to moai-dev
* [mobile-web-messaging/MQTTKit](https://github.com/mobile-web-messaging/MQTTKit) - MQTT Objective-C client for iOS
* [mobius3/tweeny](https://github.com/mobius3/tweeny) - A modern C++ tweening library
* [moc-/datastructure](https://github.com/moc-/datastructure) - exercise of datastructure
* [mofaph/csapp](https://github.com/mofaph/csapp) - Computer Systems: A Programmer's Perspective
* [mofarrell/p2pvc](https://github.com/mofarrell/p2pvc) - A point to point color terminal video chat.
* [mogenson/USBTempLogger](https://github.com/mogenson/USBTempLogger) - A two component USB temperature data logger made from a PIC16F1455
* [moinakg/pcompress](https://github.com/moinakg/pcompress) - A Parallelized Data Deduplication and Compression utility
* [moneymanagerex/moneymanagerex](https://github.com/moneymanagerex/moneymanagerex) - Money Manager Ex is an easy to use, money management application built with wxWidgets
* [mongodb/libbson](https://github.com/mongodb/libbson) - ARCHIVED - libbson has moved to https://github.com/mongodb/mongo-c-driver/tree/master/src/libbson
* [mongodb/mongo-c-driver-legacy](https://github.com/mongodb/mongo-c-driver-legacy) - C Driver for MongoDB
* [mongodb/mongo-c-driver](https://github.com/mongodb/mongo-c-driver) - A high-performance MongoDB driver for C
* [mongrel2/mongrel2](https://github.com/mongrel2/mongrel2) - The Mongrel2 Web Server Project
* [monitoringartist/Zabbix-Docker-Monitoring](https://github.com/monitoringartist/Zabbix-Docker-Monitoring) - :whale: Monitoring of Docker containers (LXC/systemd Docker supported) - Zabbix template and Zabbix C module
* [monitoringartist/zabbix-docker-monitoring](https://github.com/monitoringartist/zabbix-docker-monitoring) - :whale: Docker/Kubernetes/Mesos/Marathon/Chronos/LXC/LXD/Swarm container monitoring - Docker image, Zabbix template and C module
* [monkey/duda](https://github.com/monkey/duda) - Duda I/O is an event-driven and high performant web services framework which exposes a friendly C API
* [monkey/monkey](https://github.com/monkey/monkey) - Monkey HTTP Server
* [mono/libgdiplus](https://github.com/mono/libgdiplus) - C-based implementation of the GDI+ API
* [monome/libmonome](https://github.com/monome/libmonome) - makes writing applications for Monomes easy.
* [moonlight-stream/moonlight-android](https://github.com/moonlight-stream/moonlight-android) - GameStream client for Android
* [moonlight-stream/moonlight-chrome](https://github.com/moonlight-stream/moonlight-chrome) - GameStream client for ChromeOS
* [moonlight-stream/moonlight-pc](https://github.com/moonlight-stream/moonlight-pc) - GameStream client for Windows/OS X/Linux
* [moonpolysoft/cherly](https://github.com/moonpolysoft/cherly) - Cherly (sher-lee) is an in-VM caching library for Erlang.
* [moosefs/moosefs](https://github.com/moosefs/moosefs) - MooseFS – Open Source, Petabyte, Fault-Tolerant, Highly Performing, Scalable Network Distributed File System
* [mopemope/meinheld](https://github.com/mopemope/meinheld) - meinheld is a high performance asynchronous WSGI Web Server (based on picoev)
* [moqod/ios-qr-code-encoder](https://github.com/moqod/ios-qr-code-encoder) - This is an Objective-C library that helps to easily convert a UIImage with a QR-code from NSString with just one line of code.
* [morhetz/gruvbox-contrib](https://github.com/morhetz/gruvbox-contrib) - Ports of the gruvbox colorscheme
* [mortdeus/legacy-cc](https://github.com/mortdeus/legacy-cc) - The earliest versions of the very first c compiler known to exist in the wild written by the late legend himself dmr.
* [mortie/snow](https://github.com/mortie/snow) - A testing library for C.
* [moyix/panda](https://github.com/moyix/panda) - Platform for Architecture-Neutral Dynamic Analysis
* [mozilla-services/ios-sync-client](https://github.com/mozilla-services/ios-sync-client) - A standalone iOS client for Firefox Sync
* [mozilla-services/lua_sandbox](https://github.com/mozilla-services/lua_sandbox) - Generic Lua sandbox for dynamic data analysis
* [mozilla/firefox-ios](https://github.com/mozilla/firefox-ios) - Firefox for iOS
* [mozilla/mozjpeg](https://github.com/mozilla/mozjpeg) - Improved JPEG encoder.
* [mpc-hc/mpc-hc](https://github.com/mpc-hc/mpc-hc) - MPC-HC's main repository.  For support use our Trac: https://trac.mpc-hc.org/
* [mptre/pick](https://github.com/mptre/pick) - A fuzzy search tool for the command-line
* [mpx/lua-cjson](https://github.com/mpx/lua-cjson) - Lua CJSON is a fast JSON encoding/parsing module for Lua
* [mreiferson/php-wkhtmltox](https://github.com/mreiferson/php-wkhtmltox) - PHP bindings for libwkhtmltox
* [mridgers/clink](https://github.com/mridgers/clink) - Bash's powerful command line editing in cmd.exe
* [mrkn/ruby-odbc](https://github.com/mrkn/ruby-odbc) - Extension library to use ODBC data sources from Ruby.
* [mrnugget/data_structures](https://github.com/mrnugget/data_structures) - Implementations of common data structures in C
* [mruby/mruby](https://github.com/mruby/mruby) - Lightweight Ruby
* [msanders/autopy](https://github.com/msanders/autopy) - A simple, cross-platform GUI automation toolkit for Python.
* [msettles/rSFFreader](https://github.com/msettles/rSFFreader) - R packages for flow gram based sequence data Roche 454 and Ion Torrent
* [msgpack/msgpack-objectivec](https://github.com/msgpack/msgpack-objectivec) - MessagePack serializer implementation for Objective-C / msgpack.org[Objective-C]
* [msgpack/msgpack-ruby](https://github.com/msgpack/msgpack-ruby) - MessagePack implementation for Ruby / msgpack.org[Ruby]
* [msteinbeck/tinyspline](https://github.com/msteinbeck/tinyspline) - ANSI C library for NURBS, B-Splines, and Bézier curves with interfaces for C++, C#, D, Java, Lua, Octave, PHP, Python, R, and Ruby
* [mstiehr-dev/data_dedup](https://github.com/mstiehr-dev/data_dedup) - designed to store a lot of (likely redundant) data for backup purpose. Restore specific files as well.
* [msysgit/msysgit](https://github.com/msysgit/msysgit) - msysGit has been superseded by Git for Windows 2.x
* [mtodd/geoip](https://github.com/mtodd/geoip) - Ruby C binding to Maxmind GeoIP Library
* [mtoyoda/sl](https://github.com/mtoyoda/sl) - SL(1): Cure your bad habit of mistyping
* [mubix/post-exploitation](https://github.com/mubix/post-exploitation) - Post Exploitation Collection
* [muennich/sxiv](https://github.com/muennich/sxiv) - Simple X Image Viewer
* [mulle-nat/mulle-allocator](https://github.com/mulle-nat/mulle-allocator) - 🔄 Flexible C memory allocation scheme with leak checking
* [multipath-tcp/mptcp](https://github.com/multipath-tcp/mptcp) - Linux Kernel implementation of MultiPath TCP
* [multiwii/baseflight](https://github.com/multiwii/baseflight) - 32 bit fork of the MultiWii RC flight controller firmware
* [munificent/mark-sweep](https://github.com/munificent/mark-sweep) - A simple mark-sweep garbage collector in C
* [munificent/wren](https://github.com/munificent/wren) - The Wren Programming Language
* [mupen64plus/mupen64plus-core](https://github.com/mupen64plus/mupen64plus-core) - Core module of the Mupen64Plus project
* [muvarov/daq-odp](https://github.com/muvarov/daq-odp) - OpenDataPlane.org (ODP) Data Acquisition module for Snort.
* [mvp/uhubctl](https://github.com/mvp/uhubctl) - uhubctl - USB hub per-port power control
* [mw55309/c_fast5](https://github.com/mw55309/c_fast5) - C code to extract data from fast5 files
* [mwarning/KadNode](https://github.com/mwarning/KadNode) - P2P DNS with content key, crypto key and PKI support. DynDNS alternative.
* [myafer/OpenSSLApplication](https://github.com/myafer/OpenSSLApplication) - iOS Object-C OC swift RSA加密
* [mysqludf/lib_mysqludf_json](https://github.com/mysqludf/lib_mysqludf_json) - A UDF library of functions to map relational data to the JSON format.
* [mzhaom/trunk](https://github.com/mzhaom/trunk) - Make bazel an out of box solution for C++/Java developers
* [n1ckfg/recKinect](https://github.com/n1ckfg/recKinect) - Utility for recording raw Kinect data; much faster than Processing but binary output must be remapped
* [n64dev/cen64](https://github.com/n64dev/cen64) - Cycle-Accurate Nintendo 64 Emulator
* [naelstrof/maim](https://github.com/naelstrof/maim) - maim (make image) takes screenshots of your desktop. It has options to take only a region, and relies on slop to query for regions. maim is supposed to be an improved scrot.
* [naelstrof/slop](https://github.com/naelstrof/slop) - slop (Select Operation) is an application that queries for a selection from the user and prints the region to stdout.
* [naemon/naemon-core](https://github.com/naemon/naemon-core) - Networks, Applications and Event Monitor
* [naev/naev](https://github.com/naev/naev) - Naev is a 2d action/rpg space game that combines elements from the action, rpg and simulation genres.
* [naftaliharris/lazysort](https://github.com/naftaliharris/lazysort) - A partially and lazily sorted list data structure for Python
* [nanomsg/nanomsg](https://github.com/nanomsg/nanomsg) - nanomsg library
* [nanopb/nanopb](https://github.com/nanopb/nanopb) - Protocol Buffers with small code size
* [napsy/libhelper](https://github.com/napsy/libhelper) - General functions and data structures for C
* [naraing/dsLib](https://github.com/naraing/dsLib) - An algorithm library with core data-sttructures and common algortihm implementations on those data structures
* [nasa/XPlaneConnect](https://github.com/nasa/XPlaneConnect) - The X-Plane Communications Toolbox is a research tool used to interact with the X-Plane flight simulator
* [nashvail/Data-Structures](https://github.com/nashvail/Data-Structures) - Includes implementation of common data structures along with specific algorithmic operations.
* [nategri/nematoduino](https://github.com/nategri/nematoduino) - Arduino UNO-compatible robotic simulation of the C. elegans nematode
* [natehardison/data-structures](https://github.com/natehardison/data-structures) - A bunch of data structure implementations, just for fun.
* [nathanleclaire/algorithms_and_data_structures](https://github.com/nathanleclaire/algorithms_and_data_structures) - Want to learn more fundamentals of Comp Sci and get some practice writing C, C++, and Java.
* [navit-gps/navit](https://github.com/navit-gps/navit) - The open source (GPL v2) turn-by-turn navigation software for many OS
* [nayuki/QR-Code-generator](https://github.com/nayuki/QR-Code-generator) - High-quality QR Code generator library in Java, JavaScript, Python, C++, C.
* [nbs-system/naxsi](https://github.com/nbs-system/naxsi) - NAXSI is an open-source, high performance, low rules maintenance WAF for NGINX
* [nbs-system/snuffleupagus](https://github.com/nbs-system/snuffleupagus) - Security module for php7 - Killing bugclasses and virtual-patching the rest!
* [ncbi/osiris](https://github.com/ncbi/osiris) - OSIRIS is a public domain quality assurance software package that facilitates the assessment of multiplex short tandem repeat (STR) DNA profiles based on laboratory-specific protocols.  OSIRIS evaluates the raw electrophoresis data contained in .fsa or .hid files using an independently derived mathematically-based sizing algorithm.  OSIRIS currently supports ABI capillary analytical platforms and numerous commercially available marker kits including all CODIS-compliant kits as well as those favored by biomedical laboratories.
* [nccgroup/Cyber-Defence](https://github.com/nccgroup/Cyber-Defence) - Information released publicly by NCC Group's Cyber Defence team
* [ndreynolds/flathead](https://github.com/ndreynolds/flathead) - A toy JavaScript interpreter written in C
* [nebneuron/clique-top](https://github.com/nebneuron/clique-top) - Topological data analysis tools for cross correlation matrices
* [nec-postgres/tdeforpg](https://github.com/nec-postgres/tdeforpg) - PostgreSQL Transparent Data Encryption tool development
* [ned14/nedmalloc](https://github.com/ned14/nedmalloc) - An EXTREMELY FAST portable thread caching malloc implementation written in C for multiple threads without lock contention based on dlmalloc. Optimised for x86 and x64. Compatible with C++. Can patch itself into existing binaries on Windows.
* [neilalexander/sigmavpn](https://github.com/neilalexander/sigmavpn) - Light-weight, secure and modular VPN solution which makes use of NaCl encryption (also available for Android using jnacl in "sigmavpn-android")
* [neiljpeterson/Data-Structures-II-Assignments-COSC-3100](https://github.com/neiljpeterson/Data-Structures-II-Assignments-COSC-3100) - Just a repo for me to share homework with classmates. Nothing interesting here.
* [nelhage/reptyr](https://github.com/nelhage/reptyr) - Reparent a running program to a new terminal
* [nesbox/tic.computer](https://github.com/nesbox/tic.computer) - 🐛 Public TIC-80 issues tracker
* [netmail-open/wjelement](https://github.com/netmail-open/wjelement) - advanced, flexible JSON manipulation in C
* [netsniff-ng/netsniff-ng](https://github.com/netsniff-ng/netsniff-ng) - A Swiss army knife for your daily Linux network plumbing.
* [neurodroid/cryptonite](https://github.com/neurodroid/cryptonite) - EncFS and TrueCrypt on Android
* [neutrinolabs/xrdp](https://github.com/neutrinolabs/xrdp) - xrdp: an open source RDP server
* [newaetech/chipwhisperer](https://github.com/newaetech/chipwhisperer) - ChipWhisperer - the complete open-source toolchain for side-channel power analysis and glitching attacks
* [nfc-tools/libnfc](https://github.com/nfc-tools/libnfc) - Platform independent Near Field Communication (NFC) library
* [nfs-ganesha/nfs-ganesha](https://github.com/nfs-ganesha/nfs-ganesha) - NFS-Ganesha is an NFSv3,v4,v4.1 fileserver that runs in user mode on most UNIX/Linux systems
* [nginx/nginx-releases](https://github.com/nginx/nginx-releases) - * NOTE: This repository has been retired *. Complete (unofficial) history of nginx releases.  Please note that this repository is unofficial and pull requests have no chance of being merged. The proper way to submit changes to nginx is via the nginx development mailing list, see http://nginx.org/en/docs/contributing_changes.html.
* [ngircd/ngircd](https://github.com/ngircd/ngircd) - Free, portable and lightweight Internet Relay Chat server
* [ngtcp2/ngtcp2](https://github.com/ngtcp2/ngtcp2) - ngtcp2 project is an effort to implement IETF QUIC protocol
* [ngwese/AF_MacTypeUtil](https://github.com/ngwese/AF_MacTypeUtil) - Utility functions for interacting with Mac OS X Carbon data types.
* [nickbjohnson4224/rhombus](https://github.com/nickbjohnson4224/rhombus) - a hobby operating system written in C
* [nickdesaulniers/bf_interpreter_jit_compiler](https://github.com/nickdesaulniers/bf_interpreter_jit_compiler) - Teach myself about interpreters, JITs, and compilers using the Brainfuck language as the toy language
* [nicklockwood/FastCoding](https://github.com/nicklockwood/FastCoding) - A faster and more flexible binary file format replacement for NSCoding, Property Lists and JSON
* [nicknassar/cosby](https://github.com/nicknassar/cosby) - A TI99/4a data cassette interface software modem and practical example of signal processing with the infamous FFT
* [nicolasff/river](https://github.com/nicolasff/river) - A simple “comet” server in C, streaming data to web clients
* [nicolasff/webdis](https://github.com/nicolasff/webdis) - A Redis HTTP interface with JSON output
* [niftylight/niftyled](https://github.com/niftylight/niftyled) - library designed to provide an abstract interface for LED/lighting hardware to easily control it using pixel data.
* [nightscout/cgm-pebble-splitscreen](https://github.com/nightscout/cgm-pebble-splitscreen) - Pebble app to view data from two nightscout servers .
* [nigma/pywt](https://github.com/nigma/pywt) - We're moving. Please visit https://github.com/PyWavelets
* [nikhilm/uvbook](https://github.com/nikhilm/uvbook) - An Introduction to libuv
* [nikki93/cgame](https://github.com/nikki93/cgame) - some ideas involving games and C
* [niklasfrykholm/nflibs](https://github.com/niklasfrykholm/nflibs) - A collection of interoperable minimalistic C libraries
* [nil-zhang/php-beanstalk](https://github.com/nil-zhang/php-beanstalk) - A php c extension beanstalkd client, multi-server support, high performance, using libbeanstalkclient.
* [ninia/jep](https://github.com/ninia/jep) - Embed Python in Java
* [nitrogenlogic/cliserver](https://github.com/nitrogenlogic/cliserver) - A sample libevent-based network socket server that presents a simple command line interface to multiple connecting clients.
* [nitrogenlogic/kinradar](https://github.com/nitrogenlogic/kinradar) - Displays a pseudocolor ASCII-art radar-like view of Kinect depth data.
* [njh/mqtt-sn-tools](https://github.com/njh/mqtt-sn-tools) - Command line tools written in C for the MQTT-SN (MQTT For Sensor Networks) protocol
* [nlsandler/write_a_c_compiler](https://github.com/nlsandler/write_a_c_compiler) - Test suite to help you write your own C compiler
* [nmathewson/Libevent](https://github.com/nmathewson/Libevent) - Nick's public libevent repository.  The official repository is at         git://levent.git.sourceforge.net/gitroot/levent/libevent
* [nodemcu/nodemcu-firmware](https://github.com/nodemcu/nodemcu-firmware) - lua based interactive firmware for mcu like esp8266
* [nohbdy/libtorchlight2](https://github.com/nohbdy/libtorchlight2) - Library and tools for extracting data from the PAK archives used in the game 'Torchlight 2'
* [noporpoise/BitArray](https://github.com/noporpoise/BitArray) - C bit array structs and methods
* [noporpoise/madcrowlib](https://github.com/noporpoise/madcrowlib) - Common C data structure macros
* [noporpoise/seq_file](https://github.com/noporpoise/seq_file) - Library for Reading Bioinformatic Sequence Data in C
* [notandy/ympd](https://github.com/notandy/ympd) - Standalone MPD Web GUI written in C, utilizing Websockets and Bootstrap/JS
* [nothings/stb](https://github.com/nothings/stb) - stb single-file public domain libraries for C/C++
* [notro/fbtft](https://github.com/notro/fbtft) - Linux Framebuffer drivers for small TFT LCD display modules
* [notsecure/uTox](https://github.com/notsecure/uTox) - Lightweight Tox client
* [npmccallum/deo](https://github.com/npmccallum/deo) - A service for binding data to networks
* [nrj/objective-curl](https://github.com/nrj/objective-curl) - Curl bindings for Objective-C.
* [nsf/termbox](https://github.com/nsf/termbox) - Library for writing text-based user interfaces
* [nspire-emus/firebird](https://github.com/nspire-emus/firebird) - Third-party multi-platform emulator of the ARM-based TI-Nspire™ calculators
* [nst/BatteryChart](https://github.com/nst/BatteryChart) - Drawing iPhone Battery Charge / Discharge
* [ntamas/plfit](https://github.com/ntamas/plfit) - Fitting power-law distributions to empirical data, according to the method of Clauset, Shalizi and Newman
* [ntpeters/SimpleLogger](https://github.com/ntpeters/SimpleLogger) - Basic logger for C and C++ projects
* [ntruchsess/arduino_uip](https://github.com/ntruchsess/arduino_uip) - UIPEthernet: A plugin-replacement of the stock Arduino Ethernet library for ENC28J60 shields and breakout boards. Full support for persistent (streaming) TCP-connections and UDP (Client and Server each), ARP, ICMP, DHCP and DNS. Build around Adam Dunkels uIP Stack.
* [nuko-yokohama/neo4j_fdw](https://github.com/nuko-yokohama/neo4j_fdw) - Graph Database Foreign Data Wrapper for PostgreSQL
* [numpy/numpy](https://github.com/numpy/numpy) - Numpy main repository
* [nurupo/vlc-pause-click-plugin](https://github.com/nurupo/vlc-pause-click-plugin) - Plugin for VLC that pauses/plays video on mouse click
* [nviennot/tmate](https://github.com/nviennot/tmate) - Instant Terminal Sharing
* [oNaiPs/droidVncServer](https://github.com/oNaiPs/droidVncServer) - VNC server for Android devices.
* [oap/ekf-angles](https://github.com/oap/ekf-angles) - Extended Kalman Filter for Accelerometer and Gyro data
* [obdev/v-usb](https://github.com/obdev/v-usb) - A Firmware-Only USB implementation for Atmel's AVR Microcontrollers
* [obgm/libcoap](https://github.com/obgm/libcoap) - A CoAP (RFC 7252) implementation in C
* [ocaml-bytes/ocamlcc](https://github.com/ocaml-bytes/ocamlcc) - OCaml bytecode to C compiler
* [ocornut/imgui_club](https://github.com/ocornut/imgui_club) - Nice things to use along dear imgui
* [octalmage/robotjs](https://github.com/octalmage/robotjs) - Node.js Desktop Automation.
* [odus/odus](https://github.com/odus/odus) - ODUS, a PHP module to improve performance/data size of serialization/unserialization.
* [oetiker/rrdtool-1.x](https://github.com/oetiker/rrdtool-1.x) - RRDtool 1.x - Round Robin Database
* [ofTheo/ofxKinect](https://github.com/ofTheo/ofxKinect) - legacy openFrameworks wrapper for the xbox kinect (OF pre-0.8.0+ only) - ofxKinect is now included and is being maintained in OF releases
* [offensive-security/exploit-database](https://github.com/offensive-security/exploit-database) - The official Exploit Database repository
* [offensive-security/kali-nethunter](https://github.com/offensive-security/kali-nethunter) - Kali Linux NetHunter
* [oggy/looksee](https://github.com/oggy/looksee) - Supercharged method introspection in IRB
* [ohler55/oj](https://github.com/ohler55/oj) - Optimized JSON
* [ohler55/ox](https://github.com/ohler55/ox) - Ruby Optimized XML Parser
* [okamstudio/godot](https://github.com/okamstudio/godot) - Godot Game Engine
* [okbob/plpgsql_check](https://github.com/okbob/plpgsql_check) - plpgsql_check is next generation of plpgsql_lint. It allows to check source code by explicit call plpgsql_check_function.
* [okbob/pspg](https://github.com/okbob/pspg) - Unix pager designed for work with tables. Designed for PostgreSQL, but MySQL is supported too.
* [okws/sfslite](https://github.com/okws/sfslite) - SFSlite C++ development libraries
* [olajep/rpi-cecd](https://github.com/olajep/rpi-cecd) - Temporary remote control HDMI-CEC hack for OpenElec on Raspberry Pi
* [oleganza/CoreBitcoin](https://github.com/oleganza/CoreBitcoin) - Awesome Bitcoin toolkit for ObjC and Swift
* [olevole/cbsd](https://github.com/olevole/cbsd) - Yet one more wrapper around FreeBSD jail and bhyve. For more information please visit website
* [olibc/olibc](https://github.com/olibc/olibc) - Another C Library optimized for Embedded Linux
* [olilarkin/wdl-ol](https://github.com/olilarkin/wdl-ol) - Enhanced version of Cockos' iPlug - A simple-to-use C++ framework for developing cross platform audio plugins and targeting multiple plugin APIs with the same code. VST / VST3 / Audiounit / RTAS / AAX (Native) formats supported. NOTE: THIS IS OBSOLETE, PLEASE SEE IPLUG2:
* [olofsj/GLMap](https://github.com/olofsj/GLMap) - An OpenGL ES 2.0 renderer for Openstreetmap data
* [olofsj/Whichway](https://github.com/olofsj/Whichway) - C library for flexible (bike, foot, car) routing in road networks from Openstreetmap data.
* [olso4539/HSDMPi](https://github.com/olso4539/HSDMPi) - High Speed Data Monitor for Raspberry Pi
* [oneoo/alilua-coevent-module](https://github.com/oneoo/alilua-coevent-module) - epoll base coroutine module
* [oneoo/alilua](https://github.com/oneoo/alilua) - epoll/kqueue+lua based web server
* [open-io/oio-sds](https://github.com/open-io/oio-sds) - OpenIO Software Defined Storage, Flexible + Smart + Fast
* [open-mpi/hwloc](https://github.com/open-mpi/hwloc) - Hardware locality (hwloc)
* [open-mpi/ompi](https://github.com/open-mpi/ompi) - Open MPI main development repository
* [open-quantum-safe/liboqs](https://github.com/open-quantum-safe/liboqs) - C library for quantum-resistant cryptographic algorithms.
* [open62541/open62541](https://github.com/open62541/open62541) - Open source implementation of OPC UA (OPC Unified Architecture) aka IEC 62541 licensed under Mozilla Public License v2.0
* [openantz/antz](https://github.com/openantz/antz) - immersive data visualization
* [opencb/hpg-variant](https://github.com/opencb/hpg-variant) - A complete suite of tools to work with genomic variation data, from VCF tools to variant profiling or genomic statistics
* [opencomputeproject/OCP-Networking-Project-Community-Contributions](https://github.com/opencomputeproject/OCP-Networking-Project-Community-Contributions) - WARNING: This repository will hold software contributions that are being worked on collaboratively by the OCP Networking Community. Code in this repository has not yet been approved and accepted by the OCP Incubation Committee.  Software in this repository should be not be used on production machines and should be treated as you would any Alpha/Beta release or any software that is in development.
* [opendp/dpdk-odp](https://github.com/opendp/dpdk-odp) - Open data plane on dpdk, TCP/IP stack for dpdk.
* [openfaux/openfaux-client](https://github.com/openfaux/openfaux-client) - Browser add-on for encrypting and masking internet traffic.
* [openglbook/openglbook.com](https://github.com/openglbook/openglbook.com) - The source code for http://openglbook.com/
* [openglsuperbible/sb6code](https://github.com/openglsuperbible/sb6code) - Source code for OpenGL SupeBible 6th Edition examples
* [openglsuperbible/sb7code](https://github.com/openglsuperbible/sb7code) - Source code and supporting material for the 7th Edition of OpenGL SuperBible
* [openj/core](https://github.com/openj/core) - there are failing tests.  please find any bugs you may have introduced, fix and submit.
* [openjudge/sandbox](https://github.com/openjudge/sandbox) - The sandbox libraries (libsandbox & pysandbox) are an open-source suite of software components for C/C++ and Python developers to create automated profiling tools and watchdog programs. The API's are designed for executing and instrumenting simple (single process) tasks, featuring policy-based behavioral auditing, resource quota, and statistics collecting.
* [openlink/virtuoso-opensource](https://github.com/openlink/virtuoso-opensource) - Virtuoso is a scalable cross-platform server that combines Relational, Graph, and Document Data Management with Web Application Server and Web Services Platform functionality.
* [openresty/drizzle-nginx-module](https://github.com/openresty/drizzle-nginx-module) - an nginx upstream module that talks to mysql and drizzle by libdrizzle
* [openresty/echo-nginx-module](https://github.com/openresty/echo-nginx-module) - An Nginx module for bringing the power of "echo", "sleep", "time" and more to Nginx's config file
* [openresty/lua-upstream-nginx-module](https://github.com/openresty/lua-upstream-nginx-module) - Nginx C module to expose Lua API to ngx_lua for Nginx upstreams
* [openresty/redis2-nginx-module](https://github.com/openresty/redis2-nginx-module) - Nginx upstream module for the Redis 2.0 protocol
* [openresty/sregex](https://github.com/openresty/sregex) - A non-backtracking NFA/DFA-based Perl-compatible regex engine matching on large data streams
* [openslide/openslide](https://github.com/openslide/openslide) - C library for reading virtual slide images
* [openvenues/libpostal](https://github.com/openvenues/libpostal) - A C library for parsing/normalizing street addresses around the world. Powered by statistical NLP and open geo data.
* [openvswitch/ovs](https://github.com/openvswitch/ovs) - Open vSwitch
* [openworm/sibernetic](https://github.com/openworm/sibernetic) - This is a C++/OpenCL implementation of the PCISPH algorithm supplemented with a set of biomechanics related features applied to C. elegans locomotion
* [openwrt-mirror/openwrt](https://github.com/openwrt-mirror/openwrt) - Mirror of the OpenWRT repository
* [openyou/libomron](https://github.com/openyou/libomron) - Libraries for accessing data from Omron medical devices
* [openzfsonosx/zfs](https://github.com/openzfsonosx/zfs) - OpenZFS on OS X
* [opsengine/cpulimit](https://github.com/opsengine/cpulimit) - CPU usage limiter for Linux
* [opsxcq/exploit-CVE-2017-7494](https://github.com/opsxcq/exploit-CVE-2017-7494) - SambaCry exploit and vulnerable container (CVE-2017-7494)
* [oracle/python-cx_Oracle](https://github.com/oracle/python-cx_Oracle) - Python interface to Oracle Database conforming to the Python DB API 2.0 specification.
* [orangeduck/Corange](https://github.com/orangeduck/Corange) - Pure C Game Engine
* [orangeduck/LuaAutoC](https://github.com/orangeduck/LuaAutoC) - Automagically use C Functions and Structs with the Lua API
* [orangeduck/json2c](https://github.com/orangeduck/json2c) - Convert JSON to C data literals
* [orangeduck/mpc](https://github.com/orangeduck/mpc) - A Parser Combinator library for C
* [orangeduck/ptest](https://github.com/orangeduck/ptest) - DRY Microtesting Framework for C
* [orangeduck/tgc](https://github.com/orangeduck/tgc) - A Tiny Garbage Collector for C
* [orangejulius/cs_fundamentals](https://github.com/orangejulius/cs_fundamentals) - simple implementations of common data structures/algorithms
* [orlp/ed25519](https://github.com/orlp/ed25519) - Portable C implementation of Ed25519, a high-speed high-security public-key signature system.
* [orsonwang/Taiwan_CDC_RI](https://github.com/orsonwang/Taiwan_CDC_RI) - Reference implementation of Taiwan's citizen digital certificate
* [osdba/qpipe](https://github.com/osdba/qpipe) - Across the network of pipe tools, data sent through a pipe to another host, providing a reliable transmission function.
* [ossc-db/pg_bulkload](https://github.com/ossc-db/pg_bulkload) - High speed data loading utility for PostgreSQL
* [ossec/ossec-hids](https://github.com/ossec/ossec-hids) - OSSEC is an Open Source Host-based Intrusion Detection System that performs log analysis, file integrity checking, policy monitoring, rootkit detection, real-time alerting and active response.
* [osxfuse/fuse](https://github.com/osxfuse/fuse) - C-based FUSE for OS X API
* [osxfuse/sshfs](https://github.com/osxfuse/sshfs) - File system based on the SSH File Transfer Protocol
* [otto-de/trackrdrd](https://github.com/otto-de/trackrdrd) - The Tracking Log Reader demon reads from the shared memory log of a running instance of Varnish, aggregates data logged in a specific format for requests and ESI subrequests, and forwards the data to a messaging system (such as ActiveMQ or Kafka).
* [ottypes/libot](https://github.com/ottypes/libot) - A minimal C library for operational transform
* [paladin-t/my_basic](https://github.com/paladin-t/my_basic) - Lightweight BASIC interpreter written in standard C in dual files. Aimed to be embeddable, extendable and portable.
* [pangweiwei/slua](https://github.com/pangweiwei/slua) - Fastest Unity lua binding via static code generating.
* [paparazzi/paparazzi](https://github.com/paparazzi/paparazzi) - Paparazzi is a free and open-source hardware and software project for unmanned (air) vehicles. This is the main software repository.
* [papplampe/virgo](https://github.com/papplampe/virgo) - Virtual desktops for Windows
* [parallella/pal](https://github.com/parallella/pal) - An optimized C library for math, parallel processing and data movement
* [parrot/parrot](https://github.com/parrot/parrot) - Parrot Virtual Machine
* [particle-iot/device-os](https://github.com/particle-iot/device-os) - Device OS (Firmware) for Particle Devices
* [particle-iot/firmware](https://github.com/particle-iot/firmware) - Device OS (Firmware) for Particle Devices
* [patjak/bcwc_pcie](https://github.com/patjak/bcwc_pcie) - Reverse engineered Linux driver for the Broadcom 1570 PCIe webcam
* [paulasmuth/fyrehose](https://github.com/paulasmuth/fyrehose) - message broker for JSON data streams
* [paulasmuth/libsmatrix](https://github.com/paulasmuth/libsmatrix) - thread-safe sparse matrix data structure
* [paulfitz/coopy](https://github.com/paulfitz/coopy) - distributed spreadsheets with intelligent merges
* [paulhoux/Cinder-Samples](https://github.com/paulhoux/Cinder-Samples) - Sample applications for the Cinder framework
* [paulreimer/ofxWebUI-poco](https://github.com/paulreimer/ofxWebUI-poco) - A jquery-mobile web page which generates HTML5 form controls (from a protobuf-gwt generated description file) for exchanging protocol buffer-encoded data with an openFrameworks app.
* [payden/libwebsock](https://github.com/payden/libwebsock) - C library for easy WebSockets server.
* [pbatard/libwdi](https://github.com/pbatard/libwdi) - Windows Driver Installer library for USB devices
* [pbatard/rufus](https://github.com/pbatard/rufus) - The Reliable USB Formatting Utility
* [pbhogan/scrypt](https://github.com/pbhogan/scrypt) - A Ruby gem with native C extension for the scrypt password hashing algorithm.
* [pbrady/fastcache](https://github.com/pbrady/fastcache) - C implementation of Python 3 lru_cache
* [pcdavid/data-structures](https://github.com/pcdavid/data-structures) - Sample implementations of classical data structures in C.
* [pchote/falloutviewer](https://github.com/pchote/falloutviewer) - A tool for viewing and extracting files from Fallout 2 data archives
* [pcostesi/c-data-structures](https://github.com/pcostesi/c-data-structures) - Simple Data Structures
* [pd-l2ork/pd](https://github.com/pd-l2ork/pd) - L2Ork version of Pure-Data real-time digital signal processing language developed and maintained at DISIS, Virginia Tech
* [pd-projects/pd-double](https://github.com/pd-projects/pd-double) - a dev fork of pure-data.git for working on 64-bit double-precision support
* [pdpdds/CGSF](https://github.com/pdpdds/CGSF) - Online Game Server Platform
* [pebble-examples/cards-example](https://github.com/pebble-examples/cards-example) - Pebble Draw Commands example with a cards based app
* [pepe2k/u-boot_mod](https://github.com/pepe2k/u-boot_mod) - U-Boot 1.1.4 modification for routers
* [perfaram/xLine](https://github.com/perfaram/xLine) - Getting OSX hardware data/params through command line
* [performancecopilot/pcp](https://github.com/performancecopilot/pcp) - Performance Co-Pilot
* [perl11/potion](https://github.com/perl11/potion) - _why the lucky stiff's little language (the official repo... until _why returns)
* [peterburk/stackoverflowlocal](https://github.com/peterburk/stackoverflowlocal) - Scripts for locally hosting and searching a compressed StackOverflow data dump
* [petermichaux/royal-scheme](https://github.com/petermichaux/royal-scheme) - Royal Scheme will eventually grow to be a real, usable, embeddable Scheme implemented in ANSI C.
* [petewarden/c_hashmap](https://github.com/petewarden/c_hashmap) - A simple string hashmap in C
* [petropavel13/pg_rrule](https://github.com/petropavel13/pg_rrule) - RRULE data type for PostgreSQL
* [pez2001/razer_chroma_drivers](https://github.com/pez2001/razer_chroma_drivers) - A collection of Linux drivers for Razer Chroma devices, it supports all lighting modes and includes a daemon for advanced effects + gui configuration app
* [pflarr/dns_parse](https://github.com/pflarr/dns_parse) - A fast parser for DNS pcap data.
* [pforemski/libpjf](https://github.com/pforemski/libpjf) - A C library of data structures with tools (based on libasn)
* [pfq/PFQ](https://github.com/pfq/PFQ) - Functional Networking Framework for Multi-Core Architectures
* [pfultz2/Cloak](https://github.com/pfultz2/Cloak) - A mini-preprocessor library to demostrate the recursive capabilites of the preprocessor
* [pgRouting/pgrouting](https://github.com/pgRouting/pgrouting) - Repository contains pgRouting library. Development branch is "develop", stable branch is "master"
* [pgbackrest/pgbackrest](https://github.com/pgbackrest/pgbackrest) - Reliable PostgreSQL Backup & Restore
* [pgbovine/CDE](https://github.com/pgbovine/CDE) - CDE: Code, Data, and Environment packaging for Linux
* [pgbovine/OnlinePythonTutor](https://github.com/pgbovine/OnlinePythonTutor) - Visualize Python, Java, JavaScript, TypeScript, Ruby, C, and C++ code execution in your Web browser
* [pgbovine/opt-cpp-backend](https://github.com/pgbovine/opt-cpp-backend) - C and C++ visualizer backend for Online Python Tutor
* [phadej/igbinary](https://github.com/phadej/igbinary) - Igbinary is a drop in replacement for the standard php serializer.  Check https://github.com/igbinary/igbinary for the freshest version
* [phalcon/cphalcon](https://github.com/phalcon/cphalcon) - Web framework delivered as a C-extension for PHP
* [phalcon/zephir](https://github.com/phalcon/zephir) - Zephir is a compiled high level language aimed to the creation of C-extensions for PHP
* [philburk/pforth](https://github.com/philburk/pforth) - Portable Forth in C
* [philipl/pifs](https://github.com/philipl/pifs) - πfs - the data-free filesystem!
* [philippe44/AirConnect](https://github.com/philippe44/AirConnect) - Use AirPlay to stream to UPnP/Sonos & Chromecast devices
* [philwieland/openrail](https://github.com/philwieland/openrail) - Open Rail Data Processing
* [phlowy/splunk-phlow](https://github.com/phlowy/splunk-phlow) - This is an application for consuming netflow v5,7,9 data using NFDUMP, iNotify, Binary-ASCII coverter, and Splunk!
* [phoboslab/jsmpeg-vnc](https://github.com/phoboslab/jsmpeg-vnc) - A low latency, high framerate screen sharing server for Windows and client for browsers
* [phonegap/phonegap-plugin-contentsync](https://github.com/phonegap/phonegap-plugin-contentsync) - Download and cache remotely hosted content
* [phonegap/phonegap-plugin-fast-canvas](https://github.com/phonegap/phonegap-plugin-fast-canvas) - Fast, 2D, mostly-HTML5-canvas-compatible rendering surface for Android.
* [php-memcached-dev/php-memcached](https://github.com/php-memcached-dev/php-memcached) - memcached extension based on libmemcached library
* [php/pecl-database-pdo_user](https://github.com/php/pecl-database-pdo_user) - Userspace driver for PDO
* [php/php-src](https://github.com/php/php-src) - The PHP Interpreter
* [phpredis/phpredis](https://github.com/phpredis/phpredis) - A PHP extension for Redis
* [pi-hole/FTL](https://github.com/pi-hole/FTL) - The Pi-hole FTL engine
* [pi8027/libdatastruct](https://github.com/pi8027/libdatastruct) - libdatastruct is an ANSI C library for abstract data types.
* [pikelang/Pike](https://github.com/pikelang/Pike) - Pike is a dynamic programming language with a syntax similar to Java and C. It is simple to learn, does not require long compilation passes and has powerful built-in data types allowing simple and really fast data manipulation.
* [pimoroni/unicorn-hat](https://github.com/pimoroni/unicorn-hat) - C library, C example and Python wrapper for driving ws2812 pixels from the Raspberry Pi
* [pipelinedb/pipelinedb](https://github.com/pipelinedb/pipelinedb) - The Streaming SQL Database
* [pixelnerve/BlockOpenNI](https://github.com/pixelnerve/BlockOpenNI) - A c++ wrapper for OpenNI.
* [pjotrp/biolib](https://github.com/pjotrp/biolib) - BioLib brings together a set of opensource libraries written in C/C++ and makes them available for all Bio* languages
* [pkieltyka/stash](https://github.com/pkieltyka/stash) - Steganography application that hides data within a bitmap image
* [pkmital/StickFigureOSC](https://github.com/pkmital/StickFigureOSC) - Streams PrimeSense NITE's Skeleton Data via OSC (XCode Project)
* [pkmital/pkmColorBlobTracker](https://github.com/pkmital/pkmColorBlobTracker) - track overhead using color and map tracked points to a new geometry using a homography transformation and calibration routine - some example test videos are provided in the bin/data directory of an overhead capture.  The tracking transformation is useful for when you need a defined metric space of your tracking parameters, or need to account for different user heights in tracking their paths in a space.
* [pkrumins/bithacks.h](https://github.com/pkrumins/bithacks.h) - bithacks.h is a C header file containing useful bit manipulation macros
* [pkrumins/node-base64](https://github.com/pkrumins/node-base64) - A base64 encoding and decoding C++ module for node.js that actually works! (node now has it's own base64 encoding, see docs!)
* [pkrumins/node-png](https://github.com/pkrumins/node-png) - A nodejs C++ module that given a buffer with RGB or RGBA values creates a PNG image (in memory).
* [planetbeing/iphonelinux](https://github.com/planetbeing/iphonelinux) - Port Linux to the iPhone
* [planetbeing/xpwn](https://github.com/planetbeing/xpwn) - A cross-platform custom NOR firmware loader and custom IPSW generator for the iPhone
* [plashchynski/str2hex](https://github.com/plashchynski/str2hex) - Data formats convertion utility
* [plusvic/yara](https://github.com/plusvic/yara) - The pattern matching swiss knife
* [pmq20/ruby-compiler](https://github.com/pmq20/ruby-compiler) - Ahead-of-time (AOT) Compiler designed for Ruby, that just works.
* [pmwkaa/sophia](https://github.com/pmwkaa/sophia) - modern emeddable key-value database
* [pn2200/g3data](https://github.com/pn2200/g3data) - Grab graph data, a program for extracting data from graphs
* [pocoproject/poco](https://github.com/pocoproject/poco) - The POCO C++ Libraries are powerful cross-platform C++ libraries for building network- and internet-based applications that run on desktop, server, mobile, IoT, and embedded systems.
* [pod2g/sendrawpdu](https://github.com/pod2g/sendrawpdu) - CLI tool to send raw SMS PDU data to the iPhone 4 baseband
* [popoffka/i3lock](https://github.com/popoffka/i3lock) - i3lock is a simple screen locker like slock. This repo contains a patched version of i3lock which displays additional data on the lock screen, such as current time (like this: http://nn.lv/3y1s).
* [pornel/dssim](https://github.com/pornel/dssim) - Image similarity comparison simulating human perception (multiscale SSIM in C)
* [pornel/giflossy](https://github.com/pornel/giflossy) - Lossy GIF compressor
* [pornel/pngquant](https://github.com/pornel/pngquant) - Lossy PNG compressor — pngquant command and libimagequant library
* [pornin/CTTK](https://github.com/pornin/CTTK) - Constant-Time Toolkit
* [postgis/postgis](https://github.com/postgis/postgis) - PostGIS spatial database extension to PostgreSQL
* [postgres/postgres](https://github.com/postgres/postgres) - Mirror of the official PostgreSQL GIT repository. Note that this is just a *mirror* - we don't work with pull requests on github. To contribute, please see http://wiki.postgresql.org/wiki/Submitting_a_Patch
* [posva/catimg](https://github.com/posva/catimg) - :squirrel: Insanely fast image printing in your terminal
* [powturbo/TurboRLE](https://github.com/powturbo/TurboRLE) - Fastest Run Length Encoding
* [pozorvlak/libtap](https://github.com/pozorvlak/libtap) - Testing library for C, implementing the Test Anything Protocol. Written by Nik Clayton.
* [pramsey/pgsql-ogr-fdw](https://github.com/pramsey/pgsql-ogr-fdw) - PostgreSQL foreign data wrapper for OGR
* [preshing/CompareIntegerMaps](https://github.com/preshing/CompareIntegerMaps) - Generates benchmark data for two different data structures, then renders some graphs.
* [prideout/par](https://github.com/prideout/par) - single-file C libraries from Philip Allan Rideout
* [priitj/whitedb](https://github.com/priitj/whitedb) - WhiteDB memory database
* [pritambaral/hostapd-rtl871xdrv](https://github.com/pritambaral/hostapd-rtl871xdrv) - Hostapd driver for RTL8188{C|CU|CUS} wifi chips.
* [probablycorey/seriously](https://github.com/probablycorey/seriously) - The Objective-C HTTP library that Apple should have created, seriously.
* [probablycorey/wax](https://github.com/probablycorey/wax) - Wax is now being maintained by alibaba
* [processhacker/processhacker](https://github.com/processhacker/processhacker) - A free, powerful, multi-purpose tool that helps you monitor system resources, debug software and detect malware.
* [processhacker2/processhacker2](https://github.com/processhacker2/processhacker2) - A free, powerful, multi-purpose tool that helps you monitor system resources, debug software and detect malware.
* [processhacker2/processhacker](https://github.com/processhacker2/processhacker) - A free, powerful, multi-purpose tool that helps you monitor system resources, debug software and detect malware.
* [processone/oneteam](https://github.com/processone/oneteam) - OneTeam XMPP multi-platform client. This is a Mozilla / XUL based platform, developed mostly in Javascript and C++ XPCOM.
* [proftpd/proftpd](https://github.com/proftpd/proftpd) - ProFTPD source code
* [programmingthomas/ObjectiveGumbo](https://github.com/programmingthomas/ObjectiveGumbo) - An Objective-C wrapper with utility functions around Gumbo for easy HTML5 parsing in Cocoa and Cocoa Touch
* [project-imas/security-check](https://github.com/project-imas/security-check) - Application level, attached debug detect and jailbreak checking
* [projectNe10/Ne10](https://github.com/projectNe10/Ne10) - An open optimized software library project for the ARM® Architecture
* [proot-me/PRoot](https://github.com/proot-me/PRoot) - chroot, mount --bind, and binfmt_misc without privilege/setup for Linux
* [propublica/simple-tiles](https://github.com/propublica/simple-tiles) - Simple tile generation for maps.
* [psankar/simplefs](https://github.com/psankar/simplefs) - A simple, kernel-space, on-disk filesystem from the scratch
* [pseudomuto/c-data-structures](https://github.com/pseudomuto/c-data-structures) - A simple library of data structures for C
* [psgroove/psgroove](https://github.com/psgroove/psgroove) - PSGroove
* [psobot/ipsumcrypt](https://github.com/psobot/ipsumcrypt) - A small C program to embed binary data into the whitespace between words.
* [psychs/cocoaoniguruma](https://github.com/psychs/cocoaoniguruma) - Objective-C binding of Oniguruma regular expression engine
* [pudongqi/My_Compiler](https://github.com/pudongqi/My_Compiler) - An open-source projects about how to develop a compiler
* [puffnfresh/toggle-osx-shadows](https://github.com/puffnfresh/toggle-osx-shadows) - Tiny tool to toggle window shadows on OS X
* [pure-data/pure-data](https://github.com/pure-data/pure-data) - Pure Data - tracking Miller's SourceForge git repository (also used by libpd)
* [pusher/libPusher](https://github.com/pusher/libPusher) - An Objective-C interface to Pusher | owner=@TomKemp
* [pvaret/rtl8192cu-fixes](https://github.com/pvaret/rtl8192cu-fixes) - Realtek 8192 chipset driver, ported to kernel 3.11.
* [pyca/pynacl](https://github.com/pyca/pynacl) - Python binding to the Networking and Cryptography (NaCl) library
* [pygame/pygame](https://github.com/pygame/pygame) - pygame (the library) is a Free and Open Source python programming language library for making multimedia applications like games built on top of the excellent SDL library. C, Python, Native, OpenGL.
* [pyknite/catwm](https://github.com/pyknite/catwm) - catwm is a very simple tiling window manager
* [pysam-developers/pysam](https://github.com/pysam-developers/pysam) - Pysam is a Python module for reading and manipulating SAM/BAM/VCF/BCF files. It's a lightweight wrapper of the htslib C-API, the same one that powers samtools, bcftools, and tabix.
* [python-greenlet/greenlet](https://github.com/python-greenlet/greenlet) - Lightweight in-process concurrent programming
* [q3k/gm_datapack](https://github.com/q3k/gm_datapack) - A binary Lua module for Garry's Mod to tell when a datapack is created.
* [qayshp/TestDisk](https://github.com/qayshp/TestDisk) - TestDisk is powerful free data recovery software!
* [qemu/qemu](https://github.com/qemu/qemu) - Official QEMU mirror
* [qianshanhai/fastwiki](https://github.com/qianshanhai/fastwiki) - Fast offline data reader
* [qiq/Czech-morphology](https://github.com/qiq/Czech-morphology) - Czech morphology library, using data files compatible with PDT 2.0
* [qmk/qmk_firmware](https://github.com/qmk/qmk_firmware) - keyboard controller firmware for Atmel AVR and ARM USB families
* [qris/iptables](https://github.com/qris/iptables) - Modified iptables binary for firewall data gathering via JSON
* [quantcast/qfs](https://github.com/quantcast/qfs) - Quantcast File System
* [quartzjer/js0n](https://github.com/quartzjer/js0n) - Flexible Zero-Footprint JSON Parser in C
* [qubodup/freedink-data](https://github.com/qubodup/freedink-data) - freedink-data sound additions. see http://www.freedink.org/ (not my project)
* [questor/ringbuffer](https://github.com/questor/ringbuffer) - simple ringbuffer with possibility to get all data and/or only updates
* [r-medina/ll](https://github.com/r-medina/ll) - Thread safe linked list data structure for C
* [r03ert0/CoactivationMap.app](https://github.com/r03ert0/CoactivationMap.app) - Interactive viewer for the Brain Coactivation Map data
* [r0nk/corvus](https://github.com/r0nk/corvus) - Genetic BF programming
* [rabbitmq/rabbitmq-c](https://github.com/rabbitmq/rabbitmq-c) - The official rabbitmq-c sources have moved to:
* [rackerlabs/boot.rackspace.com](https://github.com/rackerlabs/boot.rackspace.com) - Multiple Operating System Installer via iPXE
* [radare/radare2](https://github.com/radare/radare2) - unix-like reverse engineering framework and commandline tools security
* [radareorg/r2con](https://github.com/radareorg/r2con) - Radare Congress Stuff
* [radarsat1/plhm](https://github.com/radarsat1/plhm) - A library and command-line front-end for acquiring data from Polhemus motion tracking devices.
* [radfordneal/LDPC-codes](https://github.com/radfordneal/LDPC-codes) - Software for Low Density Parity Check codes
* [radif/SIPHON-SIP-Client-that-actually-compiles](https://github.com/radif/SIPHON-SIP-Client-that-actually-compiles) - SIPHON SIP VOIP Client that actually compiles and runs on ios5 non-jailbroken phones. Works on the device and simulator! (GPL). Here is the original repository: http://code.google.com/p/siphon/
* [radiofreejohn/cfastread](https://github.com/radiofreejohn/cfastread) - Implementation of the Spritz reading method for command line files
* [rafael-santiago/pig](https://github.com/rafael-santiago/pig) - A Linux packet crafting tool
* [rahpaere/dc](https://github.com/rahpaere/dc) - Power grid data collector.
* [rainkid/dataserv](https://github.com/rainkid/dataserv) - dataserv
* [rajatkhanduja/Benchmarks](https://github.com/rajatkhanduja/Benchmarks) - Some programs to test the performance of two (or more) methods to achieve the same thing. It could be two (or more) data structures or two (or more) algorithms to solve the same problem
* [ramonza/libcoro](https://github.com/ramonza/libcoro) - Lightweight C coroutines (derived from http://software.schmorp.de/pkg/libcoro.html)
* [rampantpixels/foundation_lib](https://github.com/rampantpixels/foundation_lib) - Cross-platform public domain foundation library in C providing basic support data types and functions to write applications and games in a platform-independent fashion.
* [rampantpixels/rpmalloc](https://github.com/rampantpixels/rpmalloc) - Public domain cross platform lock free thread caching 32-byte aligned memory allocator implemented in C
* [randrew/layout](https://github.com/randrew/layout) - Single-file library for calculating 2D UI layouts using stacking boxes. Compiles as C99 or C++.
* [raphydaphy/Q-Operating-System](https://github.com/raphydaphy/Q-Operating-System) - Q OS is a versatile operating system designed with the new features of 64 bit "long mode" CPU's in mind that focuses on making everything as simple as possible for the end user
* [raspberrypi/maynard](https://github.com/raspberrypi/maynard) - Desktop environment for Wayland
* [raspberrypi/userland](https://github.com/raspberrypi/userland) - Source code for ARM side libraries for interfacing to Raspberry Pi GPU.
* [raspofabs/dodsrc](https://github.com/raspofabs/dodsrc) - Source for the Data-Oriented Design book
* [rathena/rathena](https://github.com/rathena/rathena) - rAthena is an open-source cross-platform MMORPG server.
* [rayh/kvo-block-binding](https://github.com/rayh/kvo-block-binding) - Use blocks to observe Objective-C properties using KVO
* [raysan5/raylib](https://github.com/raysan5/raylib) - A simple and easy-to-use library to enjoy videogames programming
* [razpeitia/data-structures](https://github.com/razpeitia/data-structures) - Stack, Queue, Binary Tree
* [rcr/rirc](https://github.com/rcr/rirc) - A terminal IRC client in C
* [rdub/smallfile](https://github.com/rdub/smallfile) - Security tool to create a large number of small (FS blocksize or less) files full of random data, in an effort to sanitize filesystem freespace and journal.
* [readium/readium-sdk](https://github.com/readium/readium-sdk) - A C++ ePub renderer SDK
* [reagent/http](https://github.com/reagent/http) - Simple HTTP client in C
* [realtalk/cve-2013-2094](https://github.com/realtalk/cve-2013-2094) - original cve-2013-2094 exploit and a rewritten version for educational purposes
* [rebol/rebol](https://github.com/rebol/rebol) - Source code for the Rebol interpreter
* [recp/cglm](https://github.com/recp/cglm) - 📽 Highly Optimized Graphics Math (glm) for C
* [redBorder/n2kafka](https://github.com/redBorder/n2kafka) - Tool that listen on a given port and throw all data received to a kafka topic
* [redbo/cloudfuse](https://github.com/redbo/cloudfuse) - Filesystem (fuse) implemented on Mosso's Cloud Files
* [redbrain/cython-book](https://github.com/redbrain/cython-book) - Learning Cython packtpub.com code examples.
* [redis/hiredis](https://github.com/redis/hiredis) - Minimalistic C client for Redis >= 1.2
* [redjack/libcork](https://github.com/redjack/libcork) - A simple, easily embeddable cross-platform C library
* [redxu/sihook](https://github.com/redxu/sihook) - source insight 3.X tabs plugin in c language
* [reeze/php-ext-embed](https://github.com/reeze/php-ext-embed) - Write your PHP extension with C and PHP!
* [regehr/ub-canaries](https://github.com/regehr/ub-canaries) - collection of C/C++ programs that try to get compilers to exploit undefined behavior
* [reicast/reicast-emulator](https://github.com/reicast/reicast-emulator) - Reicast is a multiplatform Sega Dreamcast emulator
* [remicollet/pecl-json-c](https://github.com/remicollet/pecl-json-c) - JSON-C wrapper
* [remis-thoughts/native-hdfs-fuse](https://github.com/remis-thoughts/native-hdfs-fuse) - C HDFS FUSE implementation, no libhdfs
* [rentzsch/MagicHat](https://github.com/rentzsch/MagicHat) - Objective-C Binary Documentation Tool. Think classdump with a hyperlinked GUI.
* [rentzsch/mach_inject](https://github.com/rentzsch/mach_inject) - interprocess code injection for Mac OS X
* [rentzsch/mach_star](https://github.com/rentzsch/mach_star) - code injection and function overriding for Mac OS X
* [rentzsch/markdownlive](https://github.com/rentzsch/markdownlive) - Purpose-built Markdown Editor for Mac OS X with Live Preview
* [rentzsch/stressdrive](https://github.com/rentzsch/stressdrive) - tool to completely fill a drive with random data and ensure it can be entirely correctly read back
* [reorg/pg_repack](https://github.com/reorg/pg_repack) - Reorganize tables in PostgreSQL databases with minimal locks
* [replay/ngx_http_consistent_hash](https://github.com/replay/ngx_http_consistent_hash) - a module which enables the nginx to use the same consistent hashing distribution for memcache servers as the php memcache module
* [reprappro/RepRapFirmware](https://github.com/reprappro/RepRapFirmware) - OO C++ RepRap Firmware
* [res0nat0r/tsunami-udp](https://github.com/res0nat0r/tsunami-udp) -  A fast user-space file transfer protocol that uses TCP control and UDP data for transfer over very high speed long distance networks (≥ 1 Gbps and even 10 GE), designed to provide more throughput than possible with TCP over the same networks.
* [residuum/PuRestJson](https://github.com/residuum/PuRestJson) - PuREST JSON is a library for connecting Puredata (Pd) to HTTP services  and encoding and decoding JSON data.
* [retme7/CVE-2014-4322_poc](https://github.com/retme7/CVE-2014-4322_poc) - Gain privileges:system -> root,as a part of  https://github.com/retme7/CVE-2014-7911_poc
* [retuxx/tinyspline](https://github.com/retuxx/tinyspline) - ANSI C library for NURBS, B-Splines, and Bézier curves with wrappers for C++11, C#, Java, Lua, PHP, Python, and Ruby
* [reverbrain/eblob](https://github.com/reverbrain/eblob) - Eblob is an append-only low-level IO library, which saves data in blob files. Created as low-level backend for elliptics
* [reverbrain/smack](https://github.com/reverbrain/smack) - Low-level IO storage which packs data into sorted (zlib/bzip2/snappy compressed) blobs
* [revolutionary/zergRush](https://github.com/revolutionary/zergRush) - Android 2.2 / 2.3 local root
* [rfjakob/cshatag](https://github.com/rfjakob/cshatag) - Detect silent data corruption under Linux using checksums in extended attributes
* [rfk/tnetstring](https://github.com/rfk/tnetstring) - data serialization using typed netstrings
* [rflynn/imgmin](https://github.com/rflynn/imgmin) - Lossy image optimization
* [rg3/bcrypt](https://github.com/rg3/bcrypt) - bcrypt password hash C library
* [rgantt/compsci.c](https://github.com/rgantt/compsci.c) - data structures, algorithms, and musings in C
* [rgerganov/footswitch](https://github.com/rgerganov/footswitch) - Command-line utility for PCsensor foot switch
* [rhomobile/rhodes](https://github.com/rhomobile/rhodes) - The Rhodes framework is a platform for building locally executing, device-optimized mobile applications for all major smartphone devices.
* [ricardo-rendoncepeda/mtl2opengl](https://github.com/ricardo-rendoncepeda/mtl2opengl) - A perl script for converting .obj and .mtl data files into arrays compatible with OpenGL ES on iOS devices
* [richarddurbin/pbwt](https://github.com/richarddurbin/pbwt) - Implementation of Positional Burrows-Wheeler Transform for genetic data
* [richgel999/miniz](https://github.com/richgel999/miniz) - miniz: Single C source file zlib-replacement library, originally from code.google.com/p/miniz
* [richox/comprox](https://github.com/richox/comprox) - An experimental lossless data compression program with high compression ratio.
* [ridiculousfish/cdecl-blocks](https://github.com/ridiculousfish/cdecl-blocks) - The venerable cdecl, with Apple blocks support
* [riolet/WAFer](https://github.com/riolet/WAFer) - WAFer is a C language-based software platform for scalable server-side and networking applications. Think node.js for C programmers.
* [riolet/nope.c](https://github.com/riolet/nope.c) - nope.c is a C language-based software platform for scalable server-side and networking applications. Think node.js for C programmers.
* [riolet/rix](https://github.com/riolet/rix) - Rix language combines the power of C language and the convenience of a high level language
* [rjsikarwar/gpu_compression](https://github.com/rjsikarwar/gpu_compression) - Nine Light weight Schemes to Compress and Decompress the data of Database Using GPU and also a planer
* [rmagick-temp/rmagick](https://github.com/rmagick-temp/rmagick) - An interface to the ImageMagick and GraphicsMagick image processing libraries.
* [rmccullagh/como-lang-ng](https://github.com/rmccullagh/como-lang-ng) - A programming language prototype implemented in C with an AST, Compiler, and  Virtual Machine \@TODO Garbage Collection
* [rmitton/rjm](https://github.com/rmitton/rjm) - Various single-file C libraries.
* [rmtheis/tess-two](https://github.com/rmtheis/tess-two) - Fork of Tesseract Tools for Android.
* [rnorris/viking](https://github.com/rnorris/viking) - Viking is a free/open source program to manage GPS data (including GPX and KML files). You can import and plot tracks, routes and waypoints, show OpenStreetMaps (OSM), Bing Aerial and other maps, generate Mapnik maps, geotag images, make new tracks, routes and waypoints, see real-time GPS position, etc.  It is written mostly in C with the GTK+ 2 toolkit and some C++.
* [robertdavidgraham/cve-2015-5477](https://github.com/robertdavidgraham/cve-2015-5477) - PoC exploit for CVE-2015-5477 BIND9 TKEY assertion failure
* [robertdavidgraham/heartleech](https://github.com/robertdavidgraham/heartleech) - Demonstrates the "heartbleed" problem using full OpenSSL stack
* [robertdavidgraham/isowall](https://github.com/robertdavidgraham/isowall) - This is a mini-firewall that completely isolates a target device from the local network.
* [robertdavidgraham/masscan](https://github.com/robertdavidgraham/masscan) - TCP port scanner, spews SYN packets asynchronously, scanning entire Internet in under 5 minutes.
* [robertdavidgraham/robdns](https://github.com/robertdavidgraham/robdns) - A fast DNS server based on C10M principles
* [robm/dzen](https://github.com/robm/dzen) - Dzen is a general purpose messaging, notification and menuing program for X11.
* [robmccoll/graphdb-testing](https://github.com/robmccoll/graphdb-testing) - Benchmarking various graph databases, engines, datastructures, and data stores.
* [roboterclubaachen/xpcc](https://github.com/roboterclubaachen/xpcc) - The C++ microcontroller framework xpcc for AVR and Cortex-M
* [robotmedia/RMStore](https://github.com/robotmedia/RMStore) - A lightweight iOS library for In-App Purchases
* [robotpy/robotpy-crio](https://github.com/robotpy/robotpy-crio) - Obsolete. Python 3 port for cRIO for use in the FIRST Robotics Competition (FRC)
* [robrix/RXPreprocessing](https://github.com/robrix/RXPreprocessing) - A variety of utilities for the C preprocessor.
* [robwhess/opensift](https://github.com/robwhess/opensift) - Open-Source SIFT Library
* [rockdaboot/mget](https://github.com/rockdaboot/mget) - Multithreaded metalink/file/website downloader (like Wget) and C library
* [rofl0r/libulz](https://github.com/rofl0r/libulz) - a collection of useful functions and data structures to create C apps faster. focus on simplicity, ability to statically link and minimal binary size.
* [rofl0r/proxychains-ng](https://github.com/rofl0r/proxychains-ng) - proxychains ng (new generation) - a preloader which hooks calls to sockets in dynamically linked programs and redirects it through one or more socks/http proxies. continuation of the unmaintained proxychains project.
* [romanbsd/fast-stemmer](https://github.com/romanbsd/fast-stemmer) - Fast Porter stemmer based on a C version of the algorithm
* [rothlab/chromozoom](https://github.com/rothlab/chromozoom) - ChromoZoom is a fast, fluid web-based genome browser
* [rougier/freetype-gl](https://github.com/rougier/freetype-gl) - OpenGL text using one vertex buffer, one texture and FreeType
* [roundsheep/rpp](https://github.com/roundsheep/rpp) - RPP is a new programming language combined with C++ and LISP
* [roysjosh/xbee-comm](https://github.com/roysjosh/xbee-comm) - XBee communication libraries and utilities
* [rpetrich/untrackerd](https://github.com/rpetrich/untrackerd) - Continuously clean up locationd's history data
* [rpm-software-management/hawkey](https://github.com/rpm-software-management/hawkey) - This is hawkey, library providing simplified C and Python API to libsolv. Hawkey project is obsoleted.
* [rsms/sol](https://github.com/rsms/sol) - A sunny little virtual machine
* [rspamd/rspamd](https://github.com/rspamd/rspamd) - Rapid spam filtering system.
* [rsta2/circle](https://github.com/rsta2/circle) - A C++ bare metal environment for Raspberry Pi with USB (32 and 64 bit)
* [rsta2/uspi](https://github.com/rsta2/uspi) - A bare metal USB driver for Raspberry Pi written in C
* [rswier/c4](https://github.com/rswier/c4) - C in four functions
* [rswier/swieros](https://github.com/rswier/swieros) - A tiny hand crafted CPU emulator, C compiler, and Operating System
* [rsyslog/rsyslog](https://github.com/rsyslog/rsyslog) - a Rocket-fast SYStem for LOG processing
* [rubenspessoa/LocData-P1](https://github.com/rubenspessoa/LocData-P1) - Projeto de Programação 1.
* [ruby/curses](https://github.com/ruby/curses) - Ruby binding for curses, ncurses, and PDCurses.  Formerly part of the ruby standard library.
* [ruby/psych](https://github.com/ruby/psych) - A libyaml wrapper for Ruby
* [rui314/9cc](https://github.com/rui314/9cc) - A Small C Compiler
* [rui314/minilisp](https://github.com/rui314/minilisp) - A readable lisp in less than 1k lines of C
* [rustyrussell/bitcoin-iterate](https://github.com/rustyrussell/bitcoin-iterate) - Simple fast iterator to extract data from bitcoind's blockchain files.
* [rustyrussell/ccan](https://github.com/rustyrussell/ccan) - The C Code Archive Network
* [rvoicilas/inotify-tools](https://github.com/rvoicilas/inotify-tools) -   inotify-tools is a C library and a set of command-line programs for Linux providing a simple interface to inotify.
* [rweichler/cylinder](https://github.com/rweichler/cylinder) - iOS homescreen page transitions in Lua
* [rwos/gti](https://github.com/rwos/gti) - a git launcher :-)
* [rxi/dyad](https://github.com/rxi/dyad) - Asynchronous networking for C
* [rxi/log.c](https://github.com/rxi/log.c) - A simple logging library implemented in C99
* [rxi/lovedos](https://github.com/rxi/lovedos) - A framework for making 2D DOS games in Lua
* [rxi/map](https://github.com/rxi/map) - A type-safe hash map implementation for C
* [rxi/vec](https://github.com/rxi/vec) - A type-safe dynamic array implementation for C
* [rxin/db-benchmarks](https://github.com/rxin/db-benchmarks) - Collection of some database benchmarks, along with tools to parallelize the data generation.
* [ryanb/rmov](https://github.com/ryanb/rmov) - Ruby wrapper for the QuickTime C API.
* [ryandotsmith/queue_lkls](https://github.com/ryandotsmith/queue_lkls) - A lock-free, non-blocking queue data structure.
* [ryanmjacobs/c](https://github.com/ryanmjacobs/c) - Compile and execute C "scripts" in one go!
* [ryd/chaosvpn](https://github.com/ryd/chaosvpn) - Config generator for chaos vpn
* [s-matyukevich/raspberry-pi-os](https://github.com/s-matyukevich/raspberry-pi-os) - Learning operating system development using Linux kernel and Raspberry Pi
* [s-u/iotools](https://github.com/s-u/iotools) - High-performance I/O tools to run distributed R jobs seamlessly on Hadoop and handle chunk-wise data processing
* [sackmotion/motion](https://github.com/sackmotion/motion) - Motion, a software motion detector
* [saelo/cve-2014-0038](https://github.com/saelo/cve-2014-0038) - Linux local root exploit for CVE-2014-0038
* [saghul/pycares](https://github.com/saghul/pycares) - Python interface for c-ares
* [saghul/pyuv](https://github.com/saghul/pyuv) - Python interface for libuv
* [sahib/glyr](https://github.com/sahib/glyr) - Glyr is a music related metadata searchengine, both with commandline interface and C API
* [sahib/rmlint](https://github.com/sahib/rmlint) - Extremely fast tool to remove duplicates and other lint from your filesystem
* [sainteos/tmxparser](https://github.com/sainteos/tmxparser) - C++ library for parsing the maps generated by the Map Editor called Tiled.
* [samdeane/xcode-unicode-formatter](https://github.com/samdeane/xcode-unicode-formatter) - Xcode data view plugin for formatting 16-bit and 32-bit unicode strings
* [samdmarshall/SDMMobileDevice](https://github.com/samdmarshall/SDMMobileDevice) - MobileDevice Implementation
* [samop/Polar-Flowlink-linux](https://github.com/samop/Polar-Flowlink-linux) - Development of interface for Polar FT60 HRM for Linux. It was tested with FT80 and it didn't work, due to different command set. I will need physical access to the watch to be able to devise a solution for other HRMs. Simple one page web interface that can be run on local machine and mimics polarpersonaltrainer is also included (see screenshot) but needs lots of polishing. Please note it is a work in progress. This early version pulls down all data except for weekly training program.
* [samrushing/irken-compiler](https://github.com/samrushing/irken-compiler) - Irken is a statically typed variant of Scheme.  Or a lisp-like variant of ML.
* [samtools/htslib](https://github.com/samtools/htslib) - C library for high-throughput sequencing data formats
* [samtools/samtools](https://github.com/samtools/samtools) - Tools (written in C using htslib) for manipulating next-generation sequencing data
* [samuellab/InterProcess](https://github.com/samuellab/InterProcess) - A compact C library to share data between processes on Windows. Fast. Simple
* [samyk/pwnat](https://github.com/samyk/pwnat) - pwnat punches holes in firewalls and NATs allowing any numbers of clients behind NATs to directly connect to a server behind a different NAT with no 3rd party, port forwarding, DMZ or spoofing involved
* [saprykin/plibsys](https://github.com/saprykin/plibsys) - Highly portable C system library: threads and synchronization primitives, sockets (TCP, UDP, SCTP), IPv4 and IPv6, IPC, hash functions (MD5, SHA-1, SHA-2, SHA-3, GOST), binary trees (RB, AVL) and more. Native code performance.
* [sass/sassc](https://github.com/sass/sassc) - libsass command line driver
* [satellogic/canopus](https://github.com/satellogic/canopus) - Canopus framework and flight computer software for CubeBug cubesat platform
* [sbinet/go-clang](https://github.com/sbinet/go-clang) - CGo bindings to the C-api of libclang.
* [scallopedllama/nerorip](https://github.com/scallopedllama/nerorip) - Rips data out of nero archives
* [sch3m4/libntoh](https://github.com/sch3m4/libntoh) - User-friendly C Library to perform TCP streams reassembly and IPv4/6 defragmentation
* [schweikert/fping](https://github.com/schweikert/fping) - High performance ping tool
* [sciguy14/MSP430-Wireless-Weather-Station](https://github.com/sciguy14/MSP430-Wireless-Weather-Station) - A Remote MSP430 monitors temperature, light, and humidity and sends the data to a local UART-USB MSP430.  A processing script graphs the data in real time on a computer.
* [scottcgi/Mojoc](https://github.com/scottcgi/Mojoc) - A cross-platform, open-source, pure C  game engine for mobile game.
* [scottellis/snapx](https://github.com/scottellis/snapx) - Stream data from a v4l2 camera and periodically save image. Testing app.
* [scottransom/psrfits2psrfits](https://github.com/scottransom/psrfits2psrfits) - Convert 16-bit PSRFITS search-mode data to 4- or 8-bit PSRFITS data
* [scrapinghub/mdr](https://github.com/scrapinghub/mdr) - A python library detect and extract listing data from HTML page.
* [scytulip/nrf51-back-rec](https://github.com/scytulip/nrf51-back-rec) - NRF51822 Firmware for Background Data Recording
* [sdegutis/mjolnir](https://github.com/sdegutis/mjolnir) - Lightweight automation and productivity app for OS X
* [sdhand/x11fs](https://github.com/sdhand/x11fs) - A tool for manipulating X windows
* [sdiehl/pycraig](https://github.com/sdiehl/pycraig) - Python library for scraping data from Craigslist
* [sdroege/snippets](https://github.com/sdroege/snippets) - Some algorithms and data structures
* [seL4/seL4](https://github.com/seL4/seL4) - The seL4 microkernel
* [sean-/postgresql-varint](https://github.com/sean-/postgresql-varint) - Data type for PostgreSQL that encodes integers using variable width encoding in order to save space
* [seanmiddleditch/libtelnet](https://github.com/seanmiddleditch/libtelnet) - Simple RFC-complient TELNET implementation as a C library.
* [seanooi/iOS-WebP](https://github.com/seanooi/iOS-WebP) - Google's WebP image format decoder and encoder for iOS
* [searchdaimon/enterprise-search](https://github.com/searchdaimon/enterprise-search) - An open source search engine for corporate data and websites.
* [seastorm/PuttyRider](https://github.com/seastorm/PuttyRider) - Hijack Putty sessions in order to sniff conversation and inject Linux commands.
* [sebnow/data_structures](https://github.com/sebnow/data_structures) - A collection of data structures, written in C.
* [seemoo-lab/nexmon](https://github.com/seemoo-lab/nexmon) - The C-based Firmware Patching Framework for Broadcom/Cypress WiFi Chips that enables Monitor Mode, Frame Injection and much more
* [seenaburns/stag](https://github.com/seenaburns/stag) - Streaming bar graphs. For stats and stuff.
* [sektioneins/SUIDGuard](https://github.com/sektioneins/SUIDGuard) - SUIDGuard - a TrustedBSD Kernel Extension that adds mitigations to protect SUID/SGID processes a bit more
* [selkhateeb/hardlink](https://github.com/selkhateeb/hardlink) - a simple command-line utility that implements hardlinks on Mac OsX
* [semmerson/NOAAPORT](https://github.com/semmerson/NOAAPORT) - The Unidata NOAAPORT package captures broadcast UDP packets from a DVB-S or DVB-S2 receiver listening to the NOAAPORT satellite broadcast, creates data-products from the UDP packets, and inserts those data-products into an LDM product-queue.
* [seppo0010/rlite](https://github.com/seppo0010/rlite) - self-contained, serverless, zero-configuration, transactional redis-compatible database engine. rlite is to Redis what SQLite is to SQL.
* [septag/darkhammer](https://github.com/septag/darkhammer) - darkHAMMER is a lightweight, open-source, multiplatform game engine. written in C (C99) language, supports python and C# bindings and lua scripts. Runs on windows and linux
* [servalproject/batphone](https://github.com/servalproject/batphone) - The Serval Mesh app for Android.  EXPERIMENTAL SOFTWARE.
* [session-replay-tools/tcpburn](https://github.com/session-replay-tools/tcpburn) - The most powerful tool for stress testing of Internet server applications
* [session-replay-tools/tcpcopy](https://github.com/session-replay-tools/tcpcopy) - An online request replication tool, also a tcp stream replay tool, fit for real testing, performance testing, stability testing, stress testing, load testing, smoke testing, etc
* [seth/crio](https://github.com/seth/crio) - Prototype R package providing C-level utils for streaming data processing
* [seth/rdict](https://github.com/seth/rdict) - R dictionary data type
* [sevenler/Uninstall_Statics](https://github.com/sevenler/Uninstall_Statics) - Android 统计 应用 自身被 卸载 Android Statistics application is uninstalled
* [sgminer-dev/sgminer](https://github.com/sgminer-dev/sgminer) - Scrypt GPU miner
* [shadeslayer/libnice](https://github.com/shadeslayer/libnice) - Libnice is an implementation of the IETF's Interactive Connectivity Establishment (ICE) standard (RFC 5245) and the Session Traversal Utilities for NAT (STUN) standard (RFC 5389).  It provides a GLib-based library, libnice and a Glib-free library, libstun as well as GStreamer elements.  ICE is useful for applications that want to establish peer-to-peer UDP data streams. It automates the process of traversing NATs and provides security against some attacks. It also allows applications to create reliable streams using a TCP over UDP layer.  Existing standards that use ICE include Session Initiation Protocol (SIP) and XMPP Jingle.
* [shadowsocks/ChinaDNS](https://github.com/shadowsocks/ChinaDNS) - Protect yourself against DNS poisoning in China.
* [shadowsocks/shadowsocks-android](https://github.com/shadowsocks/shadowsocks-android) - A Shadowsocks client for Android
* [shannah/Java-Objective-C-Bridge](https://github.com/shannah/Java-Objective-C-Bridge) - A thin bridge that allows for two-way communication from Java to Objective-C.
* [shantzu/ClipIt](https://github.com/shantzu/ClipIt) - ClipIt clipboard manager for GTK+
* [sharelatex/clsi-sharelatex](https://github.com/sharelatex/clsi-sharelatex) - A web api for compiling LaTeX documents in the cloud
* [sharvil/flingfd](https://github.com/sharvil/flingfd) - A tiny library to send file descriptors across processes
* [shaunlebron/blinky](https://github.com/shaunlebron/blinky) - Exploring peripheral vision in games (using Quake)
* [shawnclovie/cocos2dx-LuaProxy](https://github.com/shawnclovie/cocos2dx-LuaProxy) - LuaProxy for cocos2d-x, include CocosBuilder support for lua, and other cocos2d-extension support for lua, and easy to use function.
* [sheepdog/sheepdog](https://github.com/sheepdog/sheepdog) - Distributed Storage System for QEMU
* [shenfeng/tiny-web-server](https://github.com/shenfeng/tiny-web-server) - a tiny web server in C, for daily use.
* [sheredom/json.h](https://github.com/sheredom/json.h) - json parser for C and C++
* [sheredom/process.h](https://github.com/sheredom/process.h) - A simple one header solution to launching processes and interacting with them for C and C++.
* [sheredom/utf8.h](https://github.com/sheredom/utf8.h) - single header utf8 string functions for C and C++
* [shinh/maloader](https://github.com/shinh/maloader) - mach-o loader for linux
* [shiziwen/nagios-status2txt](https://github.com/shiziwen/nagios-status2txt) - nagios enhancement to get service data as plain text
* [shoes/shoes](https://github.com/shoes/shoes) - a tiny graphical app kit for ruby
* [shtrom/xkeyboard-config](https://github.com/shtrom/xkeyboard-config) - Mirror of FreeDesktop.org's XKB data with local branches
* [shuLhan/vos](https://github.com/shuLhan/vos) - Vos is a program to process formatted data, i.e. CSV data. Vos is designed to process a large input file, a file where their size is larger than the size of memory, and can be tuned to adapt with your machine environment.
* [sickill/stderred](https://github.com/sickill/stderred) - stderr in red
* [siddhant3s/cs215](https://github.com/siddhant3s/cs215) - My Third Semester, Data Structure Lab programs
* [siddontang/libtnet](https://github.com/siddontang/libtnet) - libtnet is a tiny high performance c++ network lib, like tornado
* [siemens/jailhouse](https://github.com/siemens/jailhouse) - Linux-based partitioning hypervisor
* [siganakis/tny](https://github.com/siganakis/tny) - Tiny data structures that pack a punch!
* [signal11/hidapi](https://github.com/signal11/hidapi) - A Simple library for communicating with USB and Bluetooth HID devices on Linux, Mac, and Windows.
* [signalapp/libsignal-protocol-c](https://github.com/signalapp/libsignal-protocol-c) - Signal Protocol C Library
* [silentbicycle/greatest](https://github.com/silentbicycle/greatest) - A C testing library in 1 file. No dependencies, no dynamic allocation. ISC licensed.
* [silentbicycle/theft](https://github.com/silentbicycle/theft) - property-based testing for C: generate input to find obscure bugs, then reduce to minimal failing input
* [simondlevy/BreezySLAM](https://github.com/simondlevy/BreezySLAM) - Simple, efficient, open-source package for Simultaneous Localization and Mapping in Python, Matlab,  Java, and C++
* [simondlevy/TinyEKF](https://github.com/simondlevy/TinyEKF) - Lightweight C/C++ Extended Kalman Filter with Python for prototyping
* [simonyiszk/csdr](https://github.com/simonyiszk/csdr) - A simple DSP library and command-line tool for Software Defined Radio.
* [simpl/ngx_devel_kit](https://github.com/simpl/ngx_devel_kit) - Nginx Development Kit - an Nginx module that adds additional generic tools that module developers can use in their own modules
* [simple2d/simple2d](https://github.com/simple2d/simple2d) - :video_game: Simple, open-source 2D graphics for everyone
* [simplegeo/libgeohash](https://github.com/simplegeo/libgeohash) - A pure C implementation of the Geohash algorithm.
* [simtr/The-Powder-Toy](https://github.com/simtr/The-Powder-Toy) - Written in C++ and using SDL, The Powder Toy is a desktop version of the classic 'falling sand' physics sandbox, it simulates air pressure and velocity as well as heat.
* [sipcapture/hepipe](https://github.com/sipcapture/hepipe) - HEP-PIPE: Pipe arbitrary data (logs, events, cdrs, etc) to HEP server (HOMER)
* [sisong/HDiffPatch](https://github.com/sisong/HDiffPatch) - a C\C++ library and command-line tools for binary data Diff & Patch; fast and create small delta/differential; support large files and limit memory requires when diff&patch.
* [siu/minunit](https://github.com/siu/minunit) - Minimal unit testing framework for C
* [sixstars/CTF](https://github.com/sixstars/CTF) - A writeup summary for CTF competitions, problems.
* [sixstars/ctf](https://github.com/sixstars/ctf) - A writeup summary for CTF competitions, problems.
* [skarnet/s6](https://github.com/skarnet/s6) - The s6 supervision suite.
* [skeeto/interactive-c-demo](https://github.com/skeeto/interactive-c-demo) - Demonstration of interactive C programming
* [skopjehacklab/MeteoKutija](https://github.com/skopjehacklab/MeteoKutija) - The MeteoBox (MeteoKutija) is a cheap device that collects a set of meteorological data and publishes it to a central database.
* [skvadrik/re2c](https://github.com/skvadrik/re2c) - lexer generator for C/C++
* [skx/simple.vm](https://github.com/skx/simple.vm) - Simple virtual machine which inteprets bytecode.
* [slact/nginx_http_push_module](https://github.com/slact/nginx_http_push_module) - Turn NGiNX into an adept HTTP push server.
* [slash-lang/slash](https://github.com/slash-lang/slash) - A new language for the web
* [slembcke/Chipmunk2D](https://github.com/slembcke/Chipmunk2D) - A fast and lightweight 2D game physics library.
* [sleuthkit/sleuthkit](https://github.com/sleuthkit/sleuthkit) - The Sleuth Kit® (TSK) is a library and collection of command line digital forensics tools that allow you to investigate volume and file system data. The library can be incorporated into larger digital forensics tools and the command line tools can be directly used to find evidence.
* [slim-curve/slim-curve](https://github.com/slim-curve/slim-curve) - SLIM Curve: a package for exponential curve fitting of combined spectral lifetime image data
* [smealum/ctrulib](https://github.com/smealum/ctrulib) - C library for writing user mode arm11 code for the 3DS (CTR)
* [smira/memcached_functions_mysql](https://github.com/smira/memcached_functions_mysql) - Memcached functions for MySQL as UDF, tailored for usage in replication and pushing data to MemcacheQ
* [smistad/GPU-Marching-Cubes](https://github.com/smistad/GPU-Marching-Cubes) - A GPU implementation of the Marching Cubes algorithm for extracting surfaces from volumes using OpenCL and OpenGL
* [smithlabcode/methpipe](https://github.com/smithlabcode/methpipe) - A pipeline for analyzing DNA methylation data from bisulfite sequencing.
* [smtlaissezfaire/c_type_sizes](https://github.com/smtlaissezfaire/c_type_sizes) - show the sizes of C data types
* [snaga/monetdb_fdw](https://github.com/snaga/monetdb_fdw) - monetdb_fdw - PostgreSQL Foreign Data Wrapper for MonetDB
* [snaga/xlogdump](https://github.com/snaga/xlogdump) - A tool for extracting data from the PostgreSQL's write ahead logs.
* [snavely/bundler_sfm](https://github.com/snavely/bundler_sfm) - Bundler Structure from Motion Toolkit
* [snielsen/DeathToDSStore](https://github.com/snielsen/DeathToDSStore) - .DS_Store is an abomination and must be stopped.
* [snooda/net-speeder](https://github.com/snooda/net-speeder) - net-speeder 在高延迟不稳定链路上优化单线程下载速度
* [solusipse/ureq](https://github.com/solusipse/ureq) - Micro C library for handling HTTP requests on low resource systems.
* [sonsongithub/CoreAR](https://github.com/sonsongithub/CoreAR) - AR(Augmented reality) framework for iOS, based on a visual code like ARToolKit
* [sonyxperiadev/kernel-copyleft](https://github.com/sonyxperiadev/kernel-copyleft) - Copyleft archives for Xperia kernels
* [sounos/hidbase](https://github.com/sounos/hidbase) - Distributed Data Storage System
* [soveran/clac](https://github.com/soveran/clac) - Command-line, stack-based calculator with postfix notation
* [sp4cerat/RLE-based-Voxel-Raycasting](https://github.com/sp4cerat/RLE-based-Voxel-Raycasting) - CUDA based Voxel Raycasting - Paper: Efficient, High-Quality, GPU-Based Visualization of Voxelized Surface Data
* [spark/core-common-lib](https://github.com/spark/core-common-lib) - Common library for projects that use the Spark Core with the CC3000
* [spark/firmware](https://github.com/spark/firmware) - Firmware for Particle Devices
* [sphde/sphde](https://github.com/sphde/sphde) - Shared Persistent Heap Data Environment
* [spotify/sparkey](https://github.com/spotify/sparkey) - Simple constant key/value storage library, for read-heavy systems with infrequent large bulk inserts.
* [sptim/mp3hash](https://github.com/sptim/mp3hash) - Command line tool to calculate the hash of the music data in mp3 files (without id3v1 & id3v2 metadata). Useful to find dupes with e.g. different genre names.
* [sqlcipher/sqlcipher](https://github.com/sqlcipher/sqlcipher) - SQLCipher is an SQLite extension that provides 256 bit AES encryption of database files.
* [squix78/esp8266-weather-station-color](https://github.com/squix78/esp8266-weather-station-color) - ESP8266 Weather Station in Color using ILI9341 TFT 240x320 display
* [srdja/Collections-C](https://github.com/srdja/Collections-C) - A library of generic data structures.
* [srijs/udp-stats-redis-adapter](https://github.com/srijs/udp-stats-redis-adapter) - Small performant frontend to redis, receiving minimal statistics data via udp messaging.
* [ssfrr/HearThereOSC](https://github.com/ssfrr/HearThereOSC) - A small program to receive some IMU orientation data from the HearThere Head Tracker
* [sshirokov/csgtool](https://github.com/sshirokov/csgtool) - 3D CSG Tool
* [st3fan/ios-openssl](https://github.com/st3fan/ios-openssl) - Port of OpenSSL for iOS
* [starnight/simple-data-structure](https://github.com/starnight/simple-data-structure) - Simple Data Structure library
* [statsite/statsite](https://github.com/statsite/statsite) - C implementation of statsd
* [stawel/cheali-charger](https://github.com/stawel/cheali-charger) - cheap lipo charger
* [steakknife/unsign](https://github.com/steakknife/unsign) - Remove code signatures from OSX Mach-O binaries (note: unsigned binaries cannot currently be re-codesign'ed. Patches welcome!)
* [stec-inc/EnhanceIO](https://github.com/stec-inc/EnhanceIO) - EnhanceIO Open Source for Linux
* [stedolan/jq](https://github.com/stedolan/jq) - Command-line JSON processor
* [stefanesser/dumpdecrypted](https://github.com/stefanesser/dumpdecrypted) - Dumps decrypted mach-o files from encrypted iPhone applications from memory to disk. This tool is necessary for security researchers to be able to look under the hood of encryption.
* [stefanesser/suhosin](https://github.com/stefanesser/suhosin) - Suhosin Extension
* [stefanhafeneger/PushMeBaby](https://github.com/stefanhafeneger/PushMeBaby) - iOS Push Notification Debug App
* [stellar/stellar-core](https://github.com/stellar/stellar-core) - stellar-core is the backbone of the Stellar network. It maintains a local copy of the ledger, communicating and staying in sync with other instances of stellar-core on the network. Optionally, stellar-core can store historical records of the ledger and participate in consensus.
* [stellarscience/xdm](https://github.com/stellarscience/xdm) - An Extensible Data Model
* [stephane/libmodbus](https://github.com/stephane/libmodbus) - A Modbus library for Linux, Mac OS X, FreeBSD, QNX and Windows
* [stephenmathieson/describe.h](https://github.com/stephenmathieson/describe.h) - Simple BDD describe test thingy for C
* [stephenrkell/liballocs](https://github.com/stephenrkell/liballocs) - Runtime and toolchain for whole-program monitoring of allocations and their data types
* [stepmania/stepmania](https://github.com/stepmania/stepmania) - Advanced rhythm game for Windows, Linux and OS X. Designed for both home and arcade use.
* [stevedekorte/basekit](https://github.com/stevedekorte/basekit) - C based OO portable data structure library
* [stevedekorte/coroutine](https://github.com/stevedekorte/coroutine) - C multiplatform coroutine implementation via ucontext, fibers or setjmp.
* [stevedekorte/garbagecollector](https://github.com/stevedekorte/garbagecollector) - Incrementall garbage collector library in C for use by high level language implementions.
* [stevedekorte/io](https://github.com/stevedekorte/io) - Io programming language
* [stevedekorte/skipdb](https://github.com/stevedekorte/skipdb) - C based ordered key-value ACID DB using skiplist datastructure.
* [stevedekorte/vertexdb](https://github.com/stevedekorte/vertexdb) - C graph db server using tokyocabinet & libevent
* [steven-schronk/C-Data-Structures](https://github.com/steven-schronk/C-Data-Structures) - Collection of basic data structures in C.
* [stevestreza/CrashReporter](https://github.com/stevestreza/CrashReporter) - Send iOS crash reports by email
* [stm32duino/Arduino_Core_STM32](https://github.com/stm32duino/Arduino_Core_STM32) - STM32 core support for Arduino
* [strands-project/data_compression](https://github.com/strands-project/data_compression) - Video encoding for 8 bit RGB images, 16 bit grayscale depth images and possibly more.
* [strazzere/android-unpacker](https://github.com/strazzere/android-unpacker) - Android Unpacker presented at Defcon 22: Android Hacker Protection Level 0
* [stripydog/kplex](https://github.com/stripydog/kplex) - kplex marine data multiplexer
* [stubma/WiEngine](https://github.com/stubma/WiEngine) - C++ implemented, cocos2d like cross-platform game engine
* [studio-ousia/mprpc](https://github.com/studio-ousia/mprpc) - A fast MessagePack RPC library
* [styxyang/dnsmasq-chinadns](https://github.com/styxyang/dnsmasq-chinadns) - A patched version of dnsmasq which filters out some spurious IP
* [sufficientlysecure/ad-away](https://github.com/sufficientlysecure/ad-away) - AdAway is an open source ad blocker for Android using the hosts file.
* [suhetao/stm32f4_mpu9250](https://github.com/suhetao/stm32f4_mpu9250) - Access the data of 3-axis magnetometer and DMP from MPU9250 with SPI interface, All data fusion via EKF/UKF/CKF/SRCKF algorithm
* [sumatrapdfreader/sumatrapdf](https://github.com/sumatrapdfreader/sumatrapdf) - SumatraPDF reader
* [supertunaman/cdl](https://github.com/supertunaman/cdl) - Chicken Dance License! The official IANAL license.
* [suprgyabhushan/Data-Structures-And-Algorithms](https://github.com/suprgyabhushan/Data-Structures-And-Algorithms) - All my codes done in the Course DSA during the second semester at IIIT Bangalore
* [sustrik/libdill](https://github.com/sustrik/libdill) - Structured concurrency in C
* [sustrik/libmill](https://github.com/sustrik/libmill) - Go-style concurrency in C
* [sustrik/msg_control](https://github.com/sustrik/msg_control) - Helper functions for dealing with socket ancillary data
* [suzukiplan/Touhou-VGS-MML-data](https://github.com/suzukiplan/Touhou-VGS-MML-data) - 東方BGM on VGSのMMLデータ公開＆サポート用のレポジトリです
* [svanderburg/libamivideo](https://github.com/svanderburg/libamivideo) - Conversion library for Amiga planar graphics data and EHB, HAM screen modes
* [swatkat/twitcurl](https://github.com/swatkat/twitcurl) - twitcurl is a pure C++ library for twitter APIs.
* [swenson/sort](https://github.com/swenson/sort) - Sorting routine implementations in "template" C
* [swetland/dcpu16](https://github.com/swetland/dcpu16) - Virtual Machine and Assembler for Notch's DCPU-16 Architecture
* [switchbrew/libnx](https://github.com/switchbrew/libnx) - Library for Switch Homebrew
* [swoole/php-cp](https://github.com/swoole/php-cp) - pdo and redis tcp connect proxy
* [swoole/swoole-src](https://github.com/swoole/swoole-src) - Asynchronous & concurrent & distributed networking framework for PHP.
* [symisc/PH7](https://github.com/symisc/PH7) - An Embedded Implementation of PHP (C Library)
* [symisc/sod](https://github.com/symisc/sod) - An Embedded Computer Vision & Machine Learning Library (CPU Optimized & IoT Capable)
* [symisc/unqlite](https://github.com/symisc/unqlite) - An Embedded NoSQL, Transactional Database Engine
* [symisc/vedis](https://github.com/symisc/vedis) - An Embedded Implementation of Redis
* [synergy/synergy](https://github.com/synergy/synergy) - Share one mouse and keyboard between multiple computers on your desk.
* [synthetos/TinyG](https://github.com/synthetos/TinyG) - Affordable Industrial Grade Motion Control
* [syoyo/tinygltfloader](https://github.com/syoyo/tinygltfloader) - Header only C++ Tiny glTF loader.
* [sysstat/sysstat](https://github.com/sysstat/sysstat) - Performance monitoring tools for Linux
* [systemd/casync](https://github.com/systemd/casync) - Content-Addressable Data Synchronization Tool
* [systemd/systemd](https://github.com/systemd/systemd) - The systemd System and Service Manager
* [syuhari/cocos2dx_recipe](https://github.com/syuhari/cocos2dx_recipe) - Cocos2d-x 開発のレシピのサンプルコード
* [sztupy/luadec51](https://github.com/sztupy/luadec51) - Lua Decompiler for Lua version 5.1
* [tadasv/csv_parser](https://github.com/tadasv/csv_parser) - Callback based (SAX like) CSV Parser for C
* [taf2/curb](https://github.com/taf2/curb) - Ruby bindings for libcurl
* [taf2/libebb](https://github.com/taf2/libebb) - a lightweight high-performance HTTP server library for C
* [tai/ruby-p-for-c](https://github.com/tai/ruby-p-for-c) - Data dumper macro for C, which dumps content of any data/structure/expression without prior knowledge of actual format. Works just like "p" or "pp" in Ruby.
* [tailhook/objpath](https://github.com/tailhook/objpath) - A library that allows to traverse data structures by path
* [tailhook/zerogw](https://github.com/tailhook/zerogw) - A fast HTTP/WebSocket to zeromq gateway
* [takev/mod_okioki](https://github.com/takev/mod_okioki) - An apache module that offers a RESTful data service with a PostgresQL server.
* [tallsam/DAFWAWeatherWatch](https://github.com/tallsam/DAFWAWeatherWatch) - Pebble watch face using dafwa weather api data.
* [tanakh/cmdline](https://github.com/tanakh/cmdline) - A Command Line Parser
* [tang3w/CocoaSugar](https://github.com/tang3w/CocoaSugar) - Some Cocoa Touch improvements can make developing apps easier
* [taogogo/geohash-php-extention](https://github.com/taogogo/geohash-php-extention) - a php extension for geohash,geohash is writen in c,very fast to convert geohash and coord.(一个转换经纬度和geohash的PHP扩展)
* [tarantool/tarantool](https://github.com/tarantool/tarantool) - Get your data in RAM. Get compute close to data. Enjoy the performance.
* [tarcieri/cool.io](https://github.com/tarcieri/cool.io) - Simple evented I/O for Ruby (but please check out Celluloid::IO instead)
* [tarequeh/DES](https://github.com/tarequeh/DES) - Implementation of Data Encryption Standard (DES) in C
* [tass-belgium/picotcp](https://github.com/tass-belgium/picotcp) - PicoTCP is a free TCP/IP stack implementation
* [tatsuhiro-t/nghttp2](https://github.com/tatsuhiro-t/nghttp2) - nghttp2 - HTTP/2 C Library
* [tatsuhiro-t/spdylay](https://github.com/tatsuhiro-t/spdylay) - The experimental SPDY protocol version 2, 3 and 3.1 implementation in C
* [tatsuhiro-t/wslay](https://github.com/tatsuhiro-t/wslay) - The WebSocket library in C
* [taviso/ctypes.sh](https://github.com/taviso/ctypes.sh) - A foreign function interface for bash.
* [taylor001/crown](https://github.com/taylor001/crown) - The flexible game engine.
* [tbeu/ExternData](https://github.com/tbeu/ExternData) - :page_facing_up: Modelica library for reading data from INI, JSON, XML and Excel XLS files
* [tboox/tbox](https://github.com/tboox/tbox) - 🎁 A glib-like multi-platform c library
* [tbuktu/libntru](https://github.com/tbuktu/libntru) - C Implementation of NTRUEncrypt
* [tcbrindle/raytracer.hpp](https://github.com/tcbrindle/raytracer.hpp) - Simple compile-time raytracer using C++17
* [tcurdt/iProxy](https://github.com/tcurdt/iProxy) - Let's you connect your laptop to the iPhone to surf the web.
* [teachop/FlexCAN_Library](https://github.com/teachop/FlexCAN_Library) - Arduino library for CAN on Teensy 3.1
* [teamBICYCLE/libdatac](https://github.com/teamBICYCLE/libdatac) - a collection of data library
* [tedluo/rs485](https://github.com/tedluo/rs485) - This is a simple drive for rs485 to translate data between two arm 6410 openboard
* [tekknolagi/carp](https://github.com/tekknolagi/carp) - "interesting" VM in C. Let's see how this goes.
* [telehash/telehash-c](https://github.com/telehash/telehash-c) - telehash tools library in c
* [teletautala/fullypwnd](https://github.com/teletautala/fullypwnd) - This program is designed to identify operating system and running services and find exploits for those services and attempt to connect.  I wanted that when the program finishes it's scan there was a way to report, annotate and clarify data.
* [tenderlove/psych](https://github.com/tenderlove/psych) - A libyaml wrapper for Ruby
* [texane/stlink](https://github.com/texane/stlink) - stm32 discovery line linux programmer
* [tfoldi/fuse-tableaufs](https://github.com/tfoldi/fuse-tableaufs) - User-space filesystem for Tableau Server for accessing workbooks and data sources as files.
* [tglman/orientdb-c](https://github.com/tglman/orientdb-c) - The C client of  OrientDB
* [the-tcpdump-group/libpcap](https://github.com/the-tcpdump-group/libpcap) - the LIBpcap interface to various kernel packet capture mechanism
* [the-tcpdump-group/tcpdump](https://github.com/the-tcpdump-group/tcpdump) - the TCPdump network dissector
* [theKeithD/thmj3g-tools](https://github.com/theKeithD/thmj3g-tools) - Collection of tools to unpack and repack data used by the D.N.A.Softwares doujin game, Touhou Unreal Mahjong 3rd Generation.
* [theck01/offbrand_lib](https://github.com/theck01/offbrand_lib) - A collecton of generic reference counted data structures, tools to create compatible C style classes, and demo applications
* [thegenemyers/DAZZ_DB](https://github.com/thegenemyers/DAZZ_DB) - The Dazzler Data Base
* [thegenemyers/DEXTRACTOR](https://github.com/thegenemyers/DEXTRACTOR) - Bax File Decoder and Data Compressor
* [theunamedguy/market-sim](https://github.com/theunamedguy/market-sim) - A retro stock-trading game utilizing live market data
* [thlorenz/learnuv](https://github.com/thlorenz/learnuv) - Learn uv for fun and profit, a self guided workshop to the library that powers Node.js.
* [thomasbhatia/nwEPC---EPC-SAE-Gateway](https://github.com/thomasbhatia/nwEPC---EPC-SAE-Gateway) - nwEPC is a free and open source framework software implementation of SAE/EPC Serving Gateway or SGW and Packet Data Network Gateway or PGW, which is sometimes referred as SAE-Gateway as well.
* [thomasdenney/ObjectiveGumbo](https://github.com/thomasdenney/ObjectiveGumbo) - An Objective-C wrapper with utility functions around Gumbo for easy HTML5 parsing in Cocoa and Cocoa Touch
* [thoughtbot/pick](https://github.com/thoughtbot/pick) - fuzzy select anything.
* [thunisoft/unispim](https://github.com/thunisoft/unispim) - 华宇拼音输入法核心源码(source code of unispim)
* [thvdburgt/KnR-The-C-Programming-Language-Solutions](https://github.com/thvdburgt/KnR-The-C-Programming-Language-Solutions) - My solutions to the exercises in the book "The C Programming Language" (2nd edition) by Brian W. Kernighan and Dennis M. Ritchie, also referred to as K&R.
* [tiancaiamao/datastruct](https://github.com/tiancaiamao/datastruct) - some useful data struct piece of code
* [tiancaiamao/go-internals](https://github.com/tiancaiamao/go-internals) - dig into implemention of the go programming language
* [tianocore/edk2](https://github.com/tianocore/edk2) - EDK II
* [tianyaqu/mongodb-in-financial-market](https://github.com/tianyaqu/mongodb-in-financial-market) - mongodb solution for financial market data
* [tiehuis/2048-cli](https://github.com/tiehuis/2048-cli) - The game 2048 for your Linux terminal (https://github.com/gabrielecirulli/2048)
* [tiglabs/containerdns](https://github.com/tiglabs/containerdns) - a full cache DNS for kubernetes
* [tilgovi/couchdb-lounge](https://github.com/tilgovi/couchdb-lounge) - The Lounge is a proxy-based partitioning/clustering framework for CouchDB
* [timburks/NuMongoDB](https://github.com/timburks/NuMongoDB) - An Objective-C interface to MongoDB for use with Nu
* [timperrett/Mac-SoapClient](https://github.com/timperrett/Mac-SoapClient) - 10.7 Compatible version of this: http://code.google.com/p/mac-soapclient/
* [timwr/CVE-2014-3153](https://github.com/timwr/CVE-2014-3153) - CVE-2014-3153 aka towelroot
* [timwr/CVE-2016-5195](https://github.com/timwr/CVE-2016-5195) - CVE-2016-5195 (dirtycow/dirtyc0w) proof of concept for Android
* [tinyalsa/tinyalsa](https://github.com/tinyalsa/tinyalsa) - Tiny library to interface with ALSA in the Linux kernel
* [tizian/Cendric2](https://github.com/tizian/Cendric2) - 2D Game
* [tj/histo](https://github.com/tj/histo) - beautiful charts in the terminal for static or streaming data
* [tj/luna](https://github.com/tj/luna) - luna programming language - a small, elegant VM implemented in C
* [tj/mon](https://github.com/tj/mon) - mon(1) - Simple single-process process monitoring program written in C
* [tj/watch](https://github.com/tj/watch) - watch(1) periodically executes the given command - useful for auto-testing, auto-building, auto-anything
* [tj90241/cen64](https://github.com/tj90241/cen64) - Cycle-Accurate Nintendo 64 Emulator
* [tjko/jpegoptim](https://github.com/tjko/jpegoptim) - jpegoptim - utility to optimize/compress JPEG files
* [tmk/tmk_keyboard](https://github.com/tmk/tmk_keyboard) - keyboard controller firmware for Atmel AVR USB family
* [tmm1/gctools](https://github.com/tmm1/gctools) - profiler/logger/oobgc for rgengc in ruby 2.1
* [tmm1/pygments.rb](https://github.com/tmm1/pygments.rb) - pygments syntax highlighting in ruby
* [tmm1/rblineprof](https://github.com/tmm1/rblineprof) - line-profiler for ruby
* [tmux/tmux](https://github.com/tmux/tmux) - tmux source code
* [tnightingale/DTE](https://github.com/tnightingale/DTE) - Dumb Terminal Emulator - Data Comm, COMP 3980
* [tnm/vulcan](https://github.com/tnm/vulcan) - Generate test data for Redis
* [todace/G-CVSNT](https://github.com/todace/G-CVSNT) - G-CVSNT Gaijin (and Gamedev) CVSNT version - modified for large amounts of binary data (typically for gamedev)
* [todbot/arduino-serial](https://github.com/todbot/arduino-serial) - Example C and Java host code to talking to an arduino or other "serial" device
* [toddtreece/lib_mysqludf_mongodb](https://github.com/toddtreece/lib_mysqludf_mongodb) - MySQL UDF for inserting data into MongoDB
* [tokuhirom/shirokaned](https://github.com/tokuhirom/shirokaned) - simple cache server for small binary data, feed contents with http protocol, master-master support.
* [toland/patron](https://github.com/toland/patron) - Ruby HTTP client based on libcurl
* [toland/qlmarkdown](https://github.com/toland/qlmarkdown) - QuickLook generator for Markdown files.
* [tomxue/spi](https://github.com/tomxue/spi) - to show to make SPI data transfer under Linux
* [tonyrog/cl](https://github.com/tonyrog/cl) - OpenCL binding for Erlang
* [topameng/CsToLua](https://github.com/topameng/CsToLua) - The fastest unity lua binding solution
* [torbensko/Kinect-to-Maya-motion-capture](https://github.com/torbensko/Kinect-to-Maya-motion-capture) - A set of scripts to help you capture the Kinect's motion capture data in Maya
* [torch/DEPRECEATED-torch7-distro](https://github.com/torch/DEPRECEATED-torch7-distro) - Torch7: state-of-the-art machine learning algorithms
* [torch/tds](https://github.com/torch/tds) - Torch C data structures
* [torvalds/linux](https://github.com/torvalds/linux) - Linux kernel source tree
* [toymachine/libredis](https://github.com/toymachine/libredis) - A C based general low-level PHP extension and client library for Redis, focusing on performance, generality and efficient parallel communication with multiple Redis servers. As a bonus, a  Ketama Consistent Hashing implementation is provided as well.
* [tpoechtrager/cctools-port](https://github.com/tpoechtrager/cctools-port) - Apple cctools port for Linux, *BSD and Windows (Cygwin)
* [tpoindex/crobots](https://github.com/tpoindex/crobots) - CROBOTS is a programming game, for programmers (or aspiring programmers.)
* [traildb/traildb](https://github.com/traildb/traildb) - TrailDB is an efficient tool for storing and querying series of events
* [trailofbits/cb-multios](https://github.com/trailofbits/cb-multios) - DARPA Challenges Sets for Linux, Windows, and macOS
* [trailofbits/ctf](https://github.com/trailofbits/ctf) - CTF Field Guide
* [traviscross/mtr](https://github.com/traviscross/mtr) - Official repository for mtr, a network diagnostic tool
* [traviskaufman/MaxCurl](https://github.com/traviskaufman/MaxCurl) - Data retrieval client for MaxMSP
* [trezor/trezor-core](https://github.com/trezor/trezor-core) - :lock: TREZOR Core
* [trezor/trezor-crypto](https://github.com/trezor/trezor-crypto) - :orange_book: Heavily optimized cryptography algorithms for embedded devices.
* [triSYCL/triSYCL](https://github.com/triSYCL/triSYCL) - Modern C++ for accelerators based on SYCL from Khronos Group
* [triaquae/CrazyEye](https://github.com/triaquae/CrazyEye) - OpenSource IT Automation Software
* [trink/hindsight](https://github.com/trink/hindsight) - Hindsight - light weight data processing skeleton
* [tristanheaven/asteroids](https://github.com/tristanheaven/asteroids) - Asteroid taxonomic classification using light curve data
* [troglobit/finit](https://github.com/troglobit/finit) - Fast init for Linux systems. Cookies included
* [troglobit/inadyn](https://github.com/troglobit/inadyn) - Dynamic DNS client with SSL/TLS support
* [tronkko/dirent](https://github.com/tronkko/dirent) - C/C++ library for retrieving information on files and directories
* [troydhanson/kvspool](https://github.com/troydhanson/kvspool) - A library to support streaming data applications
* [troydhanson/tpl](https://github.com/troydhanson/tpl) - tpl - a small binary serialization library for C
* [troydhanson/uthash](https://github.com/troydhanson/uthash) - C macros for hash tables and more
* [tsgates/mbox](https://github.com/tsgates/mbox) - A lightweight sandbox tool for non-root users
* [tsuna/contextswitch](https://github.com/tsuna/contextswitch) - Little micro-benchmark for Linux to test the cost of context switching and system calls
* [tsuraan/Jerasure](https://github.com/tsuraan/Jerasure) - Github repo for Jerasure Library - C Implementation of Reed-Solomon coding
* [tsznxx/wLib](https://github.com/tsznxx/wLib) - Python Modules for High-throughput Sequencing Data Analysis
* [tuanpmt/esp_mqtt](https://github.com/tuanpmt/esp_mqtt) -  MQTT client library for ESP8266 Soc
* [tvheadend/tvheadend](https://github.com/tvheadend/tvheadend) - Tvheadend is a TV streaming server for Linux supporting DVB-S, DVB-S2, DVB-C, DVB-T, ATSC, IPTV,SAT>IP and other formats through the unix pipe as input sources.
* [tvondra/pg_check](https://github.com/tvondra/pg_check) - a tool to verify integrity of PostgreSQL data files
* [twitter/fatcache](https://github.com/twitter/fatcache) - Memcache on SSD
* [twitter/jvmgcprof](https://github.com/twitter/jvmgcprof) - A simple utility for profile allocation and garbage collection activity in the JVM
* [twitter/twemcache](https://github.com/twitter/twemcache) - Twemcache is the Twitter Memcached
* [twitter/twemproxy](https://github.com/twitter/twemproxy) - A fast, light-weight proxy for memcached and redis
* [twogood/dynamite](https://github.com/twogood/dynamite) - PKWARE Data Compression decompressor tool and library
* [tyler/Bogart](https://github.com/tyler/Bogart) - It's like Sinatra... in C.
* [u0u0/Quick-Cocos2dx-Community](https://github.com/u0u0/Quick-Cocos2dx-Community) - Cocos2d-Lua 社区版
* [uTox/uTox](https://github.com/uTox/uTox) - µTox the lightest and fluffiest Tox client
* [ubixum/UXN1212_firmware](https://github.com/ubixum/UXN1212_firmware) - Firmware for the Ubixum UXN1212 USB data acquisition board
* [uci-cbcl/EXTREME](https://github.com/uci-cbcl/EXTREME) - An online EM implementation of the MEME model for fast motif discovery in large ChIP-Seq and DNase-Seq Footprinting data
* [uclouvain/openjpeg](https://github.com/uclouvain/openjpeg) - Official repository of the OpenJPEG project
* [udp/json-parser](https://github.com/udp/json-parser) - Very low footprint JSON parser written in portable ANSI C
* [udp/lacewing](https://github.com/udp/lacewing) - Cross-platform network I/O library for C/C++
* [ufjf-dcc/dsgraph](https://github.com/ufjf-dcc/dsgraph) - DSGraph is an C/C++ library for visualizing data structures.
* [ufo-kit/ufo-core](https://github.com/ufo-kit/ufo-core) - GLib-based framework for GPU-based data processing
* [ufoym/RecursiveBF](https://github.com/ufoym/RecursiveBF) - A lightweight C++ library for recursive bilateral filtering [Yang, Qingxiong. "Recursive bilateral filtering". European Conference on Computer Vision, 2012].
* [ufoym/recursive-bf](https://github.com/ufoym/recursive-bf) - A lightweight C++ library for recursive bilateral filtering [Yang, Qingxiong. "Recursive bilateral filtering". European Conference on Computer Vision, 2012].
* [ultralight-ux/ultralight](https://github.com/ultralight-ux/ultralight) - Ultralight— a lightweight, pure-GPU, HTML UI renderer for C++
* [umitanuki/s3_fdw](https://github.com/umitanuki/s3_fdw) - foreign-data wrapper for Amazon S3
* [umitanuki/tinyint-postgresql](https://github.com/umitanuki/tinyint-postgresql) - A tiny int implementation as a data type of PostgreSQL
* [unbit/spockfs](https://github.com/unbit/spockfs) - SpockFS is an HTTP based network filesystem
* [unbit/uwsgi](https://github.com/unbit/uwsgi) - uWSGI application server container
* [universal-ctags/ctags](https://github.com/universal-ctags/ctags) - A maintained ctags implementation
* [unrealircd/unrealircd](https://github.com/unrealircd/unrealircd) - Official UnrealIRCd repository. Downloads are available from our site
* [uranushiko/Yeelink](https://github.com/uranushiko/Yeelink) - My project used to send data to Yeelink.
* [urbit/archaeology](https://github.com/urbit/archaeology) - An Operating Function
* [urbit/urbit](https://github.com/urbit/urbit) - An operating function
* [urcu/userspace-rcu](https://github.com/urcu/userspace-rcu) - This repo is a mirror of the official lttng-tools git found at git://git.lttng.org/userspace-rcu.git. liburcu is a LGPLv2.1 userspace RCU (read-copy-update) library. This data synchronization library provides read-side access which scales linearly with the number of cores.
* [usrbinnc/netcat-cpi-kernel-module](https://github.com/usrbinnc/netcat-cpi-kernel-module) - Kernel module edition of the Cycles Per Instruction (2014) album.
* [uzbl/uzbl](https://github.com/uzbl/uzbl) - A web browser that adheres to the unix philosophy.
* [v92/libiorouter](https://github.com/v92/libiorouter) - libiorouter is LD_PRELOAD library for caching data and metadata requests from backend directory to local directory transparently to application.
* [valotrading/tick](https://github.com/valotrading/tick) - Tick, a market data tool.
* [valr/cbatticon](https://github.com/valr/cbatticon) - A lightweight and fast battery icon that sits in your system tray
* [vanhauser-thc/thc-hydra](https://github.com/vanhauser-thc/thc-hydra) - hydra
* [varnish/Varnish-Cache](https://github.com/varnish/Varnish-Cache) - Moved. New address: https://github.com/varnishcache/varnish-cache/
* [varnish/hitch](https://github.com/varnish/hitch) - A scalable TLS proxy.
* [varnish/libvmod-cookie](https://github.com/varnish/libvmod-cookie) - A Varnish module for simpler use of the cookie header.
* [varnish/libvmod-curl](https://github.com/varnish/libvmod-curl) - cURL bindings for Varnish through the Varnish Module interface
* [varnishcache/varnish-cache](https://github.com/varnishcache/varnish-cache) - Varnish Cache source code repository
* [vdloo/Beacontalk](https://github.com/vdloo/Beacontalk) - Peer to peer chat-program that sends data over Wi-Fi without associations.
* [vdrolia/speed_hash](https://github.com/vdrolia/speed_hash) - Hash a lot of data as fast as you can
* [veracrypt/VeraCrypt](https://github.com/veracrypt/VeraCrypt) - Disk encryption with strong security based on TrueCrypt
* [verement/cellminer](https://github.com/verement/cellminer) - Bitcoin miner for the Cell Broadband Engine Architecture
* [versatica/OverSIP](https://github.com/versatica/OverSIP) - OverSIP: the SIP framework you dreamed about
* [verse/verse](https://github.com/verse/verse) - Network protocol for real-time sharing between graphical applications
* [verzhak/sfire](https://github.com/verzhak/sfire) - Quantum GIS plugin for mapping of burnt forest areas using Landsat 5 data sets
* [vhmth/Lego-Box](https://github.com/vhmth/Lego-Box) - Write up all the data structures!
* [vi/chaoticfs](https://github.com/vi/chaoticfs) - Encrypting FUSE filesystem with "false bottom" allowing exposing the data only partially
* [vi/fdlinecombine](https://github.com/vi/fdlinecombine) - Read multiple fds and print data to stdout linewise.
* [videolan/vlc](https://github.com/videolan/vlc) - VLC media player - All pull requests are ignored, please follow https://wiki.videolan.org/Sending_Patches_VLC/
* [vifm/vifm](https://github.com/vifm/vifm) - Vifm is a file manager with curses interface, which provides Vi[m]-like environment for managing objects within file systems, extended with some useful ideas from mutt.
* [vijay03/optfs](https://github.com/vijay03/optfs) - The Optimistic File System (OptFS) is a Linux ext4 variant that implements Optimistic Crash Consistency, a new approach to crash consistency in journaling file systems. OptFS improves performance for many workloads, sometimes by an order of magnitude. OptFS provides strong consistency, equivalent to data journaling mode of ext4.
* [vim/vim](https://github.com/vim/vim) - The official Vim repository
* [vimfung/LuaScriptCore](https://github.com/vimfung/LuaScriptCore) - 一款简单易用的多平台Lua桥接器，目前支持在iOS、Mac OS X、Android以及Unity3D中使用，让原生环境与Lua无障碍沟通。
* [vincentbernat/bootstrap.c](https://github.com/vincentbernat/bootstrap.c) - Boilerplate for small C projects (autotools)
* [vincenthz/libjson](https://github.com/vincenthz/libjson) - a JSON parser and printer library in C. easy to integrate with any model.
* [vinniefalco/LuaBridge](https://github.com/vinniefalco/LuaBridge) - A lightweight, dependency-free library for binding Lua to C++
* [virtio-win/kvm-guest-drivers-windows](https://github.com/virtio-win/kvm-guest-drivers-windows) - Windows paravirtualized
* [visit1985/mdp](https://github.com/visit1985/mdp) - A command-line based markdown presentation tool.
* [vivekannan/calc](https://github.com/vivekannan/calc) - Simple command-line based calculator.
* [vivien/i3blocks](https://github.com/vivien/i3blocks) - A flexible scheduler for i3bar
* [vjeux/jspp](https://github.com/vjeux/jspp) - C++ shaped into Javascript
* [vk-com/kphp-kdb](https://github.com/vk-com/kphp-kdb) - VK-KittenPHP/DB/Engine suite
* [vkholodkov/nginx-upload-module](https://github.com/vkholodkov/nginx-upload-module) - A module for nginx web server for handling file uploads using multipart/form-data encoding (RFC 1867).
* [vladimirvivien/go-cshared-examples](https://github.com/vladimirvivien/go-cshared-examples) - Calling Go Functions from Other Languages using C Shared Libraries
* [vlfeat/vlfeat](https://github.com/vlfeat/vlfeat) - An open library of computer vision algorithms
* [vlm/asn1c](https://github.com/vlm/asn1c) - The ASN.1 Compiler
* [vmayoral/bb_mpu9150](https://github.com/vmayoral/bb_mpu9150) - BeagleBone ROS package that publishes the Invensense MPU-9150 data into a Topic.
* [vmayoral/freeDDS](https://github.com/vmayoral/freeDDS) - An open source Data Distribution Service (DDS) for embedded devices implemented for ROS
* [vmg/clar](https://github.com/vmg/clar) - What tests are made of.
* [vmg/crustache](https://github.com/vmg/crustache) - The templating engine which may explode right under your nose
* [vmg/houdini](https://github.com/vmg/houdini) - The Escapist
* [vmg/redcarpet](https://github.com/vmg/redcarpet) - The safe Markdown parser, reloaded.
* [vmg/rinku](https://github.com/vmg/rinku) - Autolinking. Ruby. Yes, that's pretty much it.
* [vmg/sundown](https://github.com/vmg/sundown) - Standards compliant, fast, secure markdown processing library in C
* [vmprof/vmprof-python](https://github.com/vmprof/vmprof-python) - vmprof - a statistical program profiler
* [vmt/udis86](https://github.com/vmt/udis86) - Disassembler Library for x86 and x86-64
* [vndmtrx/libadt](https://github.com/vndmtrx/libadt) - :vertical_traffic_light:libadt - an abstract data types library
* [vonzhou/CSAPP](https://github.com/vonzhou/CSAPP) - CSAPP,《深入理解计算机系统结构》2nd ，阅读与实践！
* [vozlt/nginx-module-sysguard](https://github.com/vozlt/nginx-module-sysguard) - Nginx sysguard module
* [vozlt/nginx-module-vts](https://github.com/vozlt/nginx-module-vts) - Nginx virtual host traffic status module
* [vpereira/pcapreader](https://github.com/vpereira/pcapreader) - saving pcap data on mongodb//tests with and without capped collections
* [vrogier/ocilib](https://github.com/vrogier/ocilib) - OCILIB (C and C++ Drivers for Oracle) - Open source C and C++ library for accessing Oracle databases
* [vsbuffalo/seqqs](https://github.com/vsbuffalo/seqqs) - seqqs is a C program/library for gathering quality statistics from sequencing data
* [vstakhov/libucl](https://github.com/vstakhov/libucl) - Universal configuration library parser
* [vstakhov/rspamd](https://github.com/vstakhov/rspamd) - Rapid spam filtering system.
* [vtudose/Let-s-build-a-compiler](https://github.com/vtudose/Let-s-build-a-compiler) - A C version of the Let's Build a Compiler, by Jack Crenshaw
* [vurtun/gui](https://github.com/vurtun/gui) - A lightweight ANSI C imgui toolkit
* [vurtun/mmx](https://github.com/vurtun/mmx) - single header libraries for C/C++
* [vurtun/zahnrad](https://github.com/vurtun/zahnrad) - A small ANSI C gui toolkit
* [vvv/under.c](https://github.com/vvv/under.c) - DER data decoder/encoder
* [vysheng/tg](https://github.com/vysheng/tg) - telegram-cli
* [wahern/cqueues](https://github.com/wahern/cqueues) - Continuation Queues: Embeddable asynchronous networking, threading, and notification framework for Lua on Unix.
* [wahern/dns](https://github.com/wahern/dns) - dns.c: Single file non-blocking DNS C library without callbacks or external dependencies.
* [wandenberg/nginx-push-stream-module](https://github.com/wandenberg/nginx-push-stream-module) - A pure stream http push technology for your Nginx setup. Comet made easy and really scalable.
* [wangkuiwu/datastructs_and_algorithm](https://github.com/wangkuiwu/datastructs_and_algorithm) - Data struct and algorithm introduction and implementation in C/C++/Java.
* [wankdanker/node-unixodbc-isql-json](https://github.com/wankdanker/node-unixodbc-isql-json) - A hacky solution for querying ODBC data sources (including MS SQL) with nodejs.
* [wargio/r2dec-js](https://github.com/wargio/r2dec-js) - radare2 plugin - converts asm to pseudo-C code.
* [warmcat/libwebsockets](https://github.com/warmcat/libwebsockets) - canonical libwebsockets.org websocket library
* [waruqi/tbox](https://github.com/waruqi/tbox) - A glib-like multi-platform c library
* [wasabiz/xrope](https://github.com/wasabiz/xrope) - rope data structure
* [watmough/jwHash](https://github.com/watmough/jwHash) - Simple hash table implementation for C.
* [wbhart/Cesium3](https://github.com/wbhart/Cesium3) - Fast interpreter with macros, local type inference, LLVM backend.
* [wbhart/comb](https://github.com/wbhart/comb) - Combinators in C
* [wc-duck/dbgtools](https://github.com/wc-duck/dbgtools) - Small collection of debug-related drop-in c/c++-utils
* [wdas/partio](https://github.com/wdas/partio) - C++ (with python bindings) library for easily reading/writing/manipulating common animation particle formats such as PDB, BGEO, PTC.   See the discussion group @ http://groups.google.com/group/partio-discuss
* [wdas/ptex](https://github.com/wdas/ptex) - Per-Face Texture Mapping for Production Rendering
* [wdlindmeier/Interferometer-Watch](https://github.com/wdlindmeier/Interferometer-Watch) - A data visualization to observe the state of LIGO machines
* [webcpp/hi-nginx](https://github.com/webcpp/hi-nginx) - A fast and robust web server and application server for C++,Python,Lua ,Java, PHP7,Javascript and multiple jsr-223 JVM language
* [webglearth/gdaldem_web](https://github.com/webglearth/gdaldem_web) - Utility for encoding elevation data (DEM) for use on the web (with WebGL Earth). Elevation value is encoded into RGB.
* [weechat/weechat](https://github.com/weechat/weechat) - The extensible chat client.
* [welefen/SetCard](https://github.com/welefen/SetCard) - a brain & puzzle game by cocos2d-html5
* [wellsie1116/Darxen](https://github.com/wellsie1116/Darxen) - Downloader, parser, and renderer for NEXRAD data
* [wengkai/ACLLib](https://github.com/wengkai/ACLLib) - ACLLib is a bunch of C functions covers Win32API and provides simpler API to beginners for programming Windows GUI applications. It compiles with MinGW and MS Visual Studio Express
* [wenjun1055/c](https://github.com/wenjun1055/c) - C语言学习代码
* [wernerd/ZRTPCPP](https://github.com/wernerd/ZRTPCPP) - C++ Implementation of ZRTP protocol - GNU ZRTP C++
* [wertarbyte/tiny-gps](https://github.com/wertarbyte/tiny-gps) - read NMEA data from serial GPS receiver (and sonar and optical sensor)  and offer it as I2C slave using ATTiny
* [wesleyd/charade](https://github.com/wesleyd/charade) - Ssh-agent clone for cygwin that proxies to pageant
* [wesleykendall/mpitutorial](https://github.com/wesleykendall/mpitutorial) - MPI programming lessons in C and executable code examples
* [westes/flex](https://github.com/westes/flex) - The Fast Lexical Analyzer - scanner generator for lexing in C and C++
* [wez/lemon-php](https://github.com/wez/lemon-php) - A PHP parser generator, based on the lemon parser generator tool. lemon-php requires a C compiler to build, and this will generate pure-PHP parsers.
* [wezm/open2300](https://github.com/wezm/open2300) - Open2300 is a package of software tools that reads (and writes) data from a Lacrosse WS23xx Weather Stations. This repo is an import of the official SVN repo with some additions.
* [wg/wrk](https://github.com/wg/wrk) - Modern HTTP benchmarking tool
* [wiire/pixiewps](https://github.com/wiire/pixiewps) - An offline WPS bruteforce utility
* [wiiudev/libwiiu](https://github.com/wiiudev/libwiiu) - Build system and examples for running C code on the Wii U
* [wikrsh/hello_fdw](https://github.com/wikrsh/hello_fdw) - Hello world program for PostgreSQL's foreign data wrapper(FDW)
* [willemt/cbuffer](https://github.com/willemt/cbuffer) - A circular buffer written in C using Posix calls to create a contiguously mapped memory space. BSD Licensed.
* [willemt/pearldb](https://github.com/willemt/pearldb) - A Lightweight Durable HTTP Key-Value Pair Database in C
* [willemt/raft](https://github.com/willemt/raft) - C implementation of the Raft Consensus protocol, BSD licensed
* [williame/hellepoll](https://github.com/williame/hellepoll) - A blazingly-fast async HTTP server written in C++
* [wilseypa/odroidNetworking](https://github.com/wilseypa/odroidNetworking) - Data/code/notes relating to our studies with low latency networking and big.LITTLE task assignment on the odroid platform
* [winnukem/racehound](https://github.com/winnukem/racehound) - Data race detector for Linux kernel modules
* [winton/redis_parse](https://github.com/winton/redis_parse) - Reads huge amounts of pipe-delimited data from Redis, filters it, and returns counts by occurence
* [wiredtiger/wiredtiger](https://github.com/wiredtiger/wiredtiger) - WiredTiger's source tree
* [wishstudio/flinux](https://github.com/wishstudio/flinux) - Foreign LINUX - Run unmodified Linux applications inside Windows.
* [wizzard/libtprint](https://github.com/wizzard/libtprint) - TPrint is a simple C library to print ASCII tabular data.
* [wkoszek/cpu60](https://github.com/wkoszek/cpu60) - Example of CPU simulation in software
* [wmutils/core](https://github.com/wmutils/core) - Set of window manipulation tools
* [wolkykim/libasyncd](https://github.com/wolkykim/libasyncd) - Embeddable Event-based Asynchronous Message/HTTP Server library for C/C++
* [wolkykim/qlibc](https://github.com/wolkykim/qlibc) - qLibc is a simple and powerful C library
* [woodrow/cidr-report_analysis](https://github.com/woodrow/cidr-report_analysis) - Data processing & analysis tools to replicate the CIDR Report and study Internet route aggregation.
* [wouterverweirder/AIR-Sudden-Motion-Sensor-Extension](https://github.com/wouterverweirder/AIR-Sudden-Motion-Sensor-Extension) - Native Extension for Adobe AIR, exposing the sudden motion sensor data of mac portables in your AIR application
* [wren-lang/wren](https://github.com/wren-lang/wren) - The Wren Programming Language
* [wtangiit/awesim](https://github.com/wtangiit/awesim) - event-driven simulator for data aware distributed workflow system
* [wujunze/nginx-http-echo-module](https://github.com/wujunze/nginx-http-echo-module) - A simple Nginx echo module
* [wukezhan/air](https://github.com/wukezhan/air) - a high performance, lightweight framework for php5 & php7 written in c
* [x2on/libssh2-for-iOS](https://github.com/x2on/libssh2-for-iOS) - A script for compiling libssh2 for iOS Devices (iPhone, iPad, iPod Touch). The example app can connect to an server with SSH and execute commands.
* [x86-64/frozen](https://github.com/x86-64/frozen) - Data management and processing library
* [x893/CMSIS-DAP](https://github.com/x893/CMSIS-DAP) - STM32 port for CMSIS-DAP with additional serial (CDC) support
* [xaberus/nih](https://github.com/xaberus/nih) - libnih, the library interactive data dumper will be based upon
* [xaionaro/clsync](https://github.com/xaionaro/clsync) - file live sync daemon based on inotify/kqueue/bsm (Linux, FreeBSD), written in GNU C
* [xant/XML-TinyXML](https://github.com/xant/XML-TinyXML) - minimal perl-xs module to handle XML data
* [xant/libhl](https://github.com/xant/libhl) - Simple and fast C library implementing a thread-safe API to manage hash-tables, linked lists, lock-free ring buffers and queues
* [xavier-chen/simplep2p](https://github.com/xavier-chen/simplep2p) - Test NAT Traversal after using pjnath to see if we can send data to peer
* [xbmc/android](https://github.com/xbmc/android) - OBSOLETE Android port. Now merged into mainline!
* [xcir/libvmod-parsereq](https://github.com/xcir/libvmod-parsereq) - parsing post,get,cookie data
* [xelatihy/yocto-gl](https://github.com/xelatihy/yocto-gl) - A collection of C/C++ single-file libraries for building physically-based graphics applications
* [xelerance/Openswan](https://github.com/xelerance/Openswan) - Openswan
* [xemul/criu](https://github.com/xemul/criu) - Checkpoint/Restore tool
* [xeniaqian94/Reliable-Data-Transfer-3.0-Protocol-Networking](https://github.com/xeniaqian94/Reliable-Data-Transfer-3.0-Protocol-Networking) - Project of COMP 3234, Computer and Communication Networks
* [xerpi/libsicksaxis](https://github.com/xerpi/libsicksaxis) - SickSaxis is a C library that lets you connect a Sixaxis or a DualShock3 to the Wii and read its data. It also lets you turn on and off the controller LEDs, enable or disable the rumble and get and set the controllers' bluetooth MAC address.
* [xiao70/X70FSD](https://github.com/xiao70/X70FSD) - Windows file system filter drivers(minifilter) to encrypt, compress, or otherwise modify file-based data require some of the most complex kernel software developed for Windows.
* [xiehuc/pidgin-lwqq](https://github.com/xiehuc/pidgin-lwqq) - a pidgin plugin based on lwqq, a excellent safe useful library for webqq protocol
* [xiph/flac](https://github.com/xiph/flac) - Free Lossless Audio Codec
* [xiph/opus](https://github.com/xiph/opus) - Modern audio compression for the internet.
* [xiph/rnnoise](https://github.com/xiph/rnnoise) - Recurrent neural network for audio noise reduction
* [xjdrew/lua-zset](https://github.com/xjdrew/lua-zset) - lua data structure same as redis sorted set
* [xlar54/Commodore-Pi](https://github.com/xlar54/Commodore-Pi) - A native Commodore 64 emulator and operating system for the Raspberry Pi
* [xnko/libapi](https://github.com/xnko/libapi) - libapi is a cross platform high performance io library written in c. It provides ability to write event driven servers and applications with continous code
* [xobs/ax2xx-code](https://github.com/xobs/ax2xx-code) - Some code for the AX211 or AX215 8051-based CPU
* [xoreaxeaxeax/movfuscator](https://github.com/xoreaxeaxeax/movfuscator) - The single instruction C compiler
* [xorg62/tty-clock](https://github.com/xorg62/tty-clock) - Clock using lib ncurses
* [xroche/coffeecatch](https://github.com/xroche/coffeecatch) - CoffeeCatch, a tiny native POSIX signal catcher (especially useful for JNI code on Android/Dalvik)
* [xsawyerx/xs-fun](https://github.com/xsawyerx/xs-fun) - XS is fun: a simple and easy tutorial on writing Perl XS
* [xstevens/decoderbufs](https://github.com/xstevens/decoderbufs) - A PostgreSQL logical decoder output plugin to deliver data as Protocol Buffers
* [xtaci/libkcp](https://github.com/xtaci/libkcp) - FEC enhanced KCP session library for iOS/Android in C++
* [xtacocorex/CHIP_IO](https://github.com/xtacocorex/CHIP_IO) - A CHIP IO library for Python: IO+PWM+SPWM+ADC+Utilities
* [xurenlu/ngx_mem_backend_module](https://github.com/xurenlu/ngx_mem_backend_module) - simple nginx module to fetch data from memcached and echo data;
* [xwang149/Dsim](https://github.com/xwang149/Dsim) - Data transfer simulator
* [xxorde/librekinect](https://github.com/xxorde/librekinect) - Depth data from a kinect sensor! Small and fast kernel driver. Also for embedded devices like the raspberry pi!
* [xyjax/sdd2json](https://github.com/xyjax/sdd2json) - EVE static data dump to JSON exporter
* [y123456yz/Reading-and-comprehense-linux-Kernel-network-protocol-stack](https://github.com/y123456yz/Reading-and-comprehense-linux-Kernel-network-protocol-stack) - linux内核网络协议栈源码阅读分析注释--带详尽中文分析注释以及相关流程分析调用注释，对理解分析内核协议栈源码很有帮助
* [y123456yz/reading-code-of-nginx-1.9.2](https://github.com/y123456yz/reading-code-of-nginx-1.9.2) - nginx-1.9.2源码通读分析注释，带详尽函数中文分析注释以及相关函数流程调用注释，最全面的nginx源码阅读分析中文注释，更新完毕
* [yaderbh/dstruct](https://github.com/yaderbh/dstruct) - An object oriented implementation of data structures for PHP
* [yaml/libyaml](https://github.com/yaml/libyaml) - Canonical source repository for LibYAML
* [yaouser/C](https://github.com/yaouser/C) - linux下的C语言及关于kernel的介绍
* [yaoweibin/nginx_tcp_proxy_module](https://github.com/yaoweibin/nginx_tcp_proxy_module) - add the feature of tcp proxy with nginx, with health check and status monitor
* [yarikoptic/NiPy-OLD](https://github.com/yarikoptic/NiPy-OLD) - Analysis of structural and functional neuroimaging data in Python (yet not stabilized -- fork on your risk)
* [yarrick/iodine](https://github.com/yarrick/iodine) - Official git repo for iodine dns tunnel
* [yarrick/pingfs](https://github.com/yarrick/pingfs) - Stores your data in ICMP ping packets
* [yasm/yasm](https://github.com/yasm/yasm) - Yasm Assembler mainline development tree
* [yellows8/ctr-httpwn](https://github.com/yellows8/ctr-httpwn) - 3DS HTTP-sysmodule exploit for bypassing required sysupdates.
* [yixuan/fdaplus](https://github.com/yixuan/fdaplus) - Enhancement of the 'fda' package for functional data analysis
* [yl790/algorithms-and-data-structures](https://github.com/yl790/algorithms-and-data-structures) - for future reference
* [yomoncada/C-Language](https://github.com/yomoncada/C-Language) - First steps of my C Language programing.
* [yongboy/c_socket.io_server](https://github.com/yongboy/c_socket.io_server) - The socket.io Linux C server
* [yosefk/checkedthreads](https://github.com/yosefk/checkedthreads) - checkedthreads: no race condition goes unnoticed! Simple API, automatic load balancing, Valgrind-based checking
* [yotamr/traces](https://github.com/yotamr/traces) - API tracing framework for Linux C/C++ applications
* [youngsterxyf/Data-Structures-and-Algorithms](https://github.com/youngsterxyf/Data-Structures-and-Algorithms) - simple implementation of some data structures and algorithms
* [yourtion/30dayMakeOS](https://github.com/yourtion/30dayMakeOS) - 《30天自制操作系统》源码中文版。自己制作一个操作系统（OSASK）的过程
* [yourtion/LearningMasteringAlgorithms-C](https://github.com/yourtion/LearningMasteringAlgorithms-C) - Mastering Algorithms with C 《算法精解：C语言描述》源码及Xcode工程、Linux工程
* [youzan/zan](https://github.com/youzan/zan) - 高效稳定、安全易用、线上实时验证的全异步高性能网络库，通过PHP扩展方式使用。
* [yrutschle/sslh](https://github.com/yrutschle/sslh) - Applicative Protocol Multiplexer (e.g. share SSH and HTTPS on the same port)
* [yunnian/php-nsq](https://github.com/yunnian/php-nsq) - a php nsq client write by c extension,the fastest  nsq client
* [yurial/tread](https://github.com/yurial/tread) - read file, exit at no data when timed out
* [yuriks/SHView](https://github.com/yuriks/SHView) - Spherical Harmonics data viewer
* [yusugomori/DeepLearning](https://github.com/yusugomori/DeepLearning) - Deep Learning (Python, C/C++, Java, Scala, Go)
* [yuya-takeyama/hashtable_dump](https://github.com/yuya-takeyama/hashtable_dump) - A Zend Extension to dump HashTable data structure on Zend Engine.
* [yuyuyu101/C-Buffered-tree](https://github.com/yuyuyu101/C-Buffered-tree) - A buffered-tree implemented in dictionary type and more
* [yyuu/pyenv](https://github.com/yyuu/pyenv) - Simple Python version management
* [z3APA3A/3proxy](https://github.com/z3APA3A/3proxy) - 3proxy - tiny free proxy server
* [zammitjames/dataparksearch](https://github.com/zammitjames/dataparksearch) - Full featured web search engine
* [zaphire/Monocle-Engine](https://github.com/zaphire/Monocle-Engine) - Open source game engine for lush 2D. Inspired by Aquaria, FlashPunk and Unity.
* [zardus/preeny](https://github.com/zardus/preeny) - Some helpful preload libraries for pwning stuff.
* [zarya/esp8266_i2c_driver](https://github.com/zarya/esp8266_i2c_driver) - ESP8266 I2C Driver
* [zdevito/ATen](https://github.com/zdevito/ATen) - ATen: A TENsor library for C++11
* [zebrafishlabs/nginx-statsd](https://github.com/zebrafishlabs/nginx-statsd) - An nginx module for sending stats to statsd.
* [zedshaw/learn-c-the-hard-way-lectures](https://github.com/zedshaw/learn-c-the-hard-way-lectures) - All of the code from Learn C The Hard Way, each project, plus the presentation slides used in the videos.
* [zedshaw/liblcthw](https://github.com/zedshaw/liblcthw) - The library you create when you are done with Learn C The Hard Way
* [zeevt/csnappy](https://github.com/zeevt/csnappy) - Google snappy in C for Linux Kernel
* [zenovich/runkit](https://github.com/zenovich/runkit) - Runkit that works!
* [zeromq/czmq](https://github.com/zeromq/czmq) - High-level C binding for ØMQ
* [zeromq/rbzmq](https://github.com/zeromq/rbzmq) - Ruby binding for 0MQ
* [zeromq/zyre](https://github.com/zeromq/zyre) - Zyre - an open-source framework for proximity-based peer-to-peer applications
* [zfogg/ascii-chat](https://github.com/zfogg/ascii-chat) - ASCII video chat.
* [zfsonlinux/spl](https://github.com/zfsonlinux/spl) - Solaris Porting Layer
* [zfsonlinux/zfs](https://github.com/zfsonlinux/zfs) - Native ZFS for Linux
* [zfsrogue/zfs-crypto](https://github.com/zfsrogue/zfs-crypto) - ZFS On Linux with crypto patches
* [zhaojh329/libumqtt](https://github.com/zhaojh329/libumqtt) - A Lightweight and fully asynchronous MQTT 3.1.1 client C library based on libubox for Embedded Linux. Support QoS 0, 1 and 2. Support ssl.
* [zhaojh329/libuwsc](https://github.com/zhaojh329/libuwsc) - A Lightweight and fully asynchronous WebSocket client C library based on libubox for Embedded Linux.
* [zhemao/libds](https://github.com/zhemao/libds) - Simple, memory-safe data-structures in C.
* [zhengshuxin/acl](https://github.com/zhengshuxin/acl) - One advanced C/C++ library for Linux/Mac/FreeBSD/Solaris(x86)/Windows/Android/IOS
* [zhicheng/db](https://github.com/zhicheng/db) - A New DBM in Pure C
* [zlib-ng/zlib-ng](https://github.com/zlib-ng/zlib-ng) - zlib replacement with optimizations for "next generation" systems.
* [zmap/zmap](https://github.com/zmap/zmap) - ZMap Internet Scanner
* [zmartzone/mod_auth_openidc](https://github.com/zmartzone/mod_auth_openidc) -  OpenID Connect Relying Party and OAuth 2.0 Resource Server for Apache HTTP Server 2.x
* [znort987/blockparser](https://github.com/znort987/blockparser) - Simple C++ bitcoin blockchain parser
* [zpl-c/zpl](https://github.com/zpl-c/zpl) - 📐 Your C99 Powerkit
* [zsaleeba/picoc](https://github.com/zsaleeba/picoc) - A very small C interpreter
* [zserge/partcl](https://github.com/zserge/partcl) - ParTcl - a micro Tcl implementation
* [zserge/webview](https://github.com/zserge/webview) - Tiny cross-platform webview library for C/C++/Golang. Uses WebKit (Gtk/Cocoa) and MSHTML (Windows)
* [zsh-users/zsh](https://github.com/zsh-users/zsh) - Mirror of the Z shell source code repository.
* [zsummer/breeze](https://github.com/zsummer/breeze) - 一个C++的轻量级的分布式服务器引擎, 架构思想为一切皆service.
* [zsummer/zsummerX](https://github.com/zsummer/zsummerX) - zsummerX is a cross-platform C++ high performance lightweight network library. via IOCP/EPOLL/SELECT.
* [zupet/LuaTinker](https://github.com/zupet/LuaTinker) - LUA to C++ Binding Library
* [zwdzwd/biscuit](https://github.com/zwdzwd/biscuit) - a little tool for bisulfite data
* [zyearn/zaver](https://github.com/zyearn/zaver) - Yet another fast and efficient HTTP server




[484]: https://www.codeproject.com/Articles/6154/Writing-Efficient-C-and-C-Code-Optimization
[483]: https://docs.google.com/presentation/d/1h49gY3TSiayLMXYmRMaAEMl05FaJ-Z6jDOWOz3EsqqQ/edit?pli=1#slide=id.p
[482]: https://www.chiark.greenend.org.uk/~sgtatham/mp/
[481]: http://www.greenend.org.uk/rjk/tech/inline.html
[480]: http://snaipe.me/c/c-smart-pointers/
[479]: https://graphics.stanford.edu/~seander/bithacks.html
[478]: http://danluu.com/malloc-tutorial/
[477]: http://250bpm.com/blog:56
[476]: http://blog.llvm.org/2011/05/what-every-c-programmer-should-know.html
[475]: https://proprogramming.org/some-unknown-features-or-tricks-in-c-language/
[474]: https://hintjens.gitbooks.io/scalable-c/content/index.html
[473]: https://computing.llnl.gov/tutorials/mpi/
[472]: https://computing.llnl.gov/tutorials/openMP/
[471]: https://www.youtube.com/playlist?list=PLLX-Q6B8xqZ8n8bwjGdzBJ25X2utwnoEG
[470]: https://nullprogram.com/blog/2017/03/30
[469]: https://nullprogram.com/blog/2015/02/17
[468]: https://jvns.ca/blog/2014/12/14/fun-with-threads/
[467]: http://mpitutorial.com/
[466]: http://blog.noctua-software.com/c-tricks.html
[465]: https://blogs.oracle.com/linux/8-gdb-tricks-you-should-know-v2
[464]: http://blog.pkh.me/p/20-templating-in-c.html
[462]: https://computing.llnl.gov/tutorials/pthreads/
[461]: https://web.archive.org/web/20170620131430/https://www.tedunangst.com/flak/post/memcpy-vs-memmove
[460]: https://www.recurse.com/blog/5-learning-c-with-gdb
[459]: https://gist.github.com/eatonphil/21b3d6569f24ad164365

[457]: http://nethack4.org/blog/building-c.html
[456]: http://nullprogram.com/blog/2017/08/20/
[455]: https://pdos.csail.mit.edu/6.828/2017/readings/pointers.pdf
[454]: http://nullprogram.com/blog/2017/09/21/
[453]: http://www.etalabs.net/compare_libcs.html
[452]: http://c-faq.com/
[451]: https://locklessinc.com/benchmarks_allocator.shtml

[440]: https://github.com/alanxz/rabbitmq-c
[439]: https://github.com/dertuxmalwieder/libvldmail
[438]: https://github.com/nfc-tools/libnfc
[437]: https://github.com/cloudwu/pbc
[436]: http://sourceware.org/binutils/docs/bfd/
[435]: https://gnu.org/software/gss/
[434]: https://github.com/swenson/sort
[433]: https://github.com/antirez/linenoise
[432]: https://github.com/recp/tm
[431]: http://kitsune-dsu.com/
[430]: http://www.colm.net/open-source/ragel/
[429]: http://libcello.org/
[428]: https://github.com/jeremyevans/ape_tag_libs/tree/master/c
[427]: https://criu.org/Main_Page
[426]: https://github.com/sinemetu1/twitc
[425]: https://www.gnu.org/software/gnulib/
[423]: https://github.com/obgm/libcoap
[422]: https://gnu.org/software/freeipmi/index.html
[421]: https://github.com/commonmark/cmark/blob/master/COPYING
[420]: https://github.com/commonmark/cmark
[419]: https://en.wikipedia.org/wiki/Knuth's_Algorithm_X
[418]: https://github.com/blynn/dlx
[417]: https://github.com/simplegeo/libgeohash
[416]: https://github.com/google/gumbo-parser
[415]: https://glade.gnome.org/
[414]: https://www.gnu.org/software/gperf/
[413]: https://brechtsanders.github.io/xlsxio/

[412]: https://github.com/docopt/docopt.c
[411]: https://github.com/cofyc/argparse
[410]: https://github.com/jibsen/parg

[409]: https://github.com/google/cpu_features
[408]: https://github.com/libimobiledevice/libimobiledevice
[407]: https://libusb.info/

[406]: http://www.dyncall.org/
[405]: https://gnu.org/software/libffcall/
[404]: https://github.com/atgreen/libffi

[403]: http://libcox.symisc.net/
[402]: https://github.com/dmw/caffeine
[401]: http://savannah.nongnu.org/projects/attr/

[400]: http://libevent.org/
[399]: http://software.schmorp.de/pkg/libev.html
[398]: http://facebook.github.io/libphenom/index.html
[397]: http://libuv.org

[396]: https://github.com/openvenues/libpostal
[395]: http://libtrading.org/
[394]: https://tulipindicators.org/

[393]: http://www.throwtheswitch.org/cexception
[392]: https://github.com/esneider/debug
[391]: http://hardysimpson.github.io/zlog/
[390]: https://github.com/gpakosz/whereami

[389]: https://lodev.org/lodepng/
[388]: https://github.com/mozilla/mozjpeg
[387]: http://www.vips.ecs.soton.ac.uk/index.php?title=VIPS
[386]: https://wiki.gnome.org/action/show/Projects/LibRsvg?action=show&redirect=LibRsvg
[385]: http://www.libpng.org/
[384]: https://libjpeg-turbo.virtualgl.org/
[383]: https://pngquant.org/lib/
[382]: https://github.com/prideout/heman
[381]: https://sourceforge.net/projects/giflib/
[380]: https://github.com/libgd/libgd

[379]: https://github.com/codeplea/tinyexpr
[378]: https://github.com/riolet/WAFer
[377]: http://www.pell.portland.or.us/~orc/Code/discount/
[376]: https://github.com/jgm/cmark
[375]: https://github.com/hoedown/hoedown
[374]: https://github.com/nsf/termbox
[373]: https://gnu.org/software/ncurses/
[372]: https://github.com/sabotage-linux/netbsd-curses
[371]: https://github.com/doches/progressbar
[370]: https://github.com/zeromq/zproto


[364]: https://kore.io/
[363]: http://www.koanlogic.com/klone/
[362]: http://facil.io/
[361]: https://dasoftver.bitbucket.io/cloudgizer

[360]: http://re2c.org/index.html
[359]: https://github.com/orangeduck/mpc
[358]: https://github.com/abiggerhammer/hammer
[357]: https://www.gnu.org/software/bison/
[356]: https://github.com/westes/flex

[355]: https://github.com/evolutional/utest
[354]: http://www.throwtheswitch.org/unity
[353]: https://wiki.haskell.org/Introduction_to_QuickCheck2
[352]: https://github.com/silentbicycle/theft
[351]: https://nemequ.github.io/munit
[350]: https://github.com/codeplea/minctest
[349]: https://github.com/silentbicycle/greatest
[348]: http://cunit.sourceforge.net/
[347]: https://github.com/bvdberg/ctest
[346]: https://criterion.readthedocs.io/en/master
[345]: https://cmocka.org/
[344]: http://www.throwtheswitch.org/cmock
[343]: https://github.com/vmg/clar
[342]: https://github.com/yhfudev/cpp-ci-unit-test.git
[341]: https://libcheck.github.io/check
[340]: http://users.jyu.fi/~sapekiis/cheat

[339]: https://github.com/Juniper/libxo
[338]: https://github.com/vstakhov/libucl
[337]: https://github.com/0intro/libelf
[336]: https://github.com/martinh/libconfuse
[335]: https://github.com/mongodb/libbson
[334]: https://www.pyyaml.org/wiki/LibYAML
[333]: http://xmlsoft.org/
[332]: http://expat.sourceforge.net/
[331]: https://madmurphy.github.io/libconfini/html/index.html
[330]: https://github.com/ndevilla/iniparser
[329]: https://github.com/benhoyt/inih
[328]: https://lloyd.github.io/yajl/
[327]: https://github.com/netmail-open/wjelement/
[326]: https://github.com/sheredom/json.h
[325]: https://zserge.com/jsmn.html
[324]: https://github.com/NeonMercury/jfes
[323]: http://www.digip.org/jansson/
[322]: https://github.com/rgamble/libcsv

[321]: https://github.com/JuliaLang/utf8proc
[320]: https://github.com/sheredom/utf8.h
[319]: http://tartarus.org/martin/PorterStemmer/
[318]: https://github.com/wooorm/stmr.c
[317]: https://github.com/antirez/sds
[316]: https://boyerjohn.github.io/rapidstring/index.html
[315]: https://github.com/josephg/librope
[314]: https://gnu.org/software/libiconv/
[313]: https://gnu.org/software/libunistring/
[312]: https://en.wikipedia.org/wiki/Levenshtein_distance
[311]: https://github.com/wooorm/levenshtein.c
[310]: http://site.icu-project.org/
[309]: http://mike.steinert.ca/bstring/

[308]: https://uclibc-ng.org/
[307]: http://pdclib.e43.eu/
[306]: https://www.musl-libc.org/
[305]: https://www.gnu.org/software/libc/
[304]: https://www.fefe.de/dietlibc/
[303]: https://en.wikipedia.org/wiki/Capability-based_security
[302]: https://github.com/NuxiNL/cloudlibc
[301]: https://github.com/aosp-mirror/platform_bionic

[300]: https://github.com/RandyGaul/tinyheaders
[299]: https://github.com/nothings/stb
[298]: https://github.com/DanielGibson/Snippets/
[297]: https://github.com/prideout/par
[296]: https://github.com/vurtun/mmx
[295]: http://www.fefe.de/djb/
[294]: https://github.com/clibs/clib/wiki/Packages
[293]: https://github.com/clibs/clib
[292]: http://ccodearchive.net/

[291]: https://en.wikipedia.org/wiki/External_Data_Representation
[290]: https://github.com/troydhanson/tpl
[289]: https://github.com/protobuf-c/protobuf-c
[288]: http://opic.rocks/
[287]: https://github.com/ludocode/mpack
[286]: http://avro.apache.org/docs/current/api/c/index.html#_introduction_to_avro_c
[285]: https://google.github.io/flatbuffers/
[284]: https://github.com/dvidelabs/flatcc
[283]: https://msgpack.org/
[282]: https://github.com/camgunz/cmp
[281]: https://github.com/jmckaskill/c-capnproto
[280]: https://github.com/liteserver/binn

[279]: https://github.com/laurikari/tre/
[278]: https://github.com/cesanta/slre
[277]: http://www.pcre.org/
[276]: https://github.com/kkos/oniguruma
[275]: https://github.com/k-takata/Onigmo

[274]: https://bitbucket.org/MDukhan/yeppp
[273]: http://www.libtom.net/TomsFastMath/
[272]: http://slepc.upv.es/
[271]: https://github.com/cvxgrp/scs
[270]: http://www.mcs.anl.gov/petsc/
[269]: http://pari.math.u-bordeaux.fr/
[268]: http://www.libtom.net/LibTomPoly/
[267]: http://www.libtom.net/LibTomMath/
[266]: http://www.netlib.org/lapack/lapacke.html
[265]: https://sourceforge.net/projects/kissfft/
[264]: https://www.gnu.org/software/gsl/
[263]: https://gnu.org/software/mpria/
[262]: http://mpfr.loria.fr/index.html
[261]: http://www.multiprecision.org/index.php?prog=mpc&page=home
[260]: https://gmplib.org/
[259]: https://gnu.org/software/glpk/
[258]: http://flintlib.org/
[257]: http://www.fftw.org/
[256]: https://github.com/adis300/fft-c
[255]: http://www.feynarts.de/cuba/
[254]: https://scientificc.github.io/cmathl/
[253]: https://github.com/clMathLibraries/clBLAS
[252]: http://math-atlas.sourceforge.net/
[251]: https://github.com/fredrik-johansson/arb
[250]: http://apophenia.info

[249]: https://github.com/zeromq/zyre
[248]: https://tatsuhiro-t.github.io/wslay/
[247]: https://github.com/silentbicycle/socket99
[246]: https://gnu.org/software/osip/
[245]: https://nanomsg.github.io/nng/
[244]: https://github.com/nanomsg/nanomsg
[243]: https://cesanta.com
[242]: https://lwan.ws
[241]: https://github.com/JonnyWhatshisface/libwebsock
[240]: https://github.com/LibVNC/libvncserver
[239]: https://risoflora.github.io/libsagui/
[238]: http://sourceforge.net/projects/libquickmail/
[237]: https://www.coralbits.com/libonion/
[236]: https://gnu.org/software/libmicrohttpd/
[235]: https://gnu.org/software/libidn/
[234]: http://www.hughes.com.au/products/libhttpd/
[233]: http://www.etpan.org
[232]: https://curl.haxx.se/libcurl/
[231]: http://www.nlnetlabs.nl/projects/ldns/index.html
[230]: https://github.com/joyent/http-parser
[229]: https://www.gnu.org/software/adns/
[228]: https://github.com/it4e/CHL
[227]: http://lionet.info/asn1c/compiler.html

[226]: http://paulbatchelor.github.io/proj/soundpipe.html
[225]: https://github.com/lieff/minimp3
[224]: http://libsound.io
[223]: http://www.mega-nerd.com/libsndfile/
[222]: https://mpv.io
[221]: https://gstreamer.freedesktop.org/
[220]: https://www.ffmpeg.org/
[219]: https://github.com/aubio/aubio

[218]: https://github.com/minad/tlsf
[217]: http://www.gii.upv.es/tlsf/
[216]: https://talloc.samba.org/talloc/doc/html/index.html
[215]: https://github.com/rampantpixels/rpmalloc
[214]: https://locklessinc.com/
[213]: http://jemalloc.net
[212]: https://www.hboehm.info/gc/

[211]: http://xforms-toolkit.org/
[210]: http://www.tcl.tk/
[209]: https://sourceforge.net/projects/tinyfiledialogs/
[208]: https://github.com/vurtun/nuklear
[207]: http://webserver2.tecgraf.puc-rio.br/iup/
[206]: https://www.gtk.org/

[205]: https://spdx.org/licenses/MPL-1.1.html
[204]: http://www.sgi.com/tech/opengl/?/license.html
[203]: https://www.opengl.org/
[202]: https://github.com/memononen/nanovg
[201]: https://github.com/ands/lightmapper
[200]: https://gnu.org/software/libxmi/
[199]: https://github.com/saitoha/libsixel
[198]: https://github.com/cacalabs/libcaca
[197]: http://ebassi.github.io/graphene/
[196]: http://cairographics.org/

[195]: https://github.com/ferreiradaselva/uastar
[194]: https://clover.moe/spearmint
[193]: http://www.libsigil.com/
[192]: https://github.com/grimfang4/sdl-gpu
[191]: https://www.libsdl.org/
[190]: https://www.libretro.com/
[189]: https://github.com/libretro/RetroArch
[188]: https://www.raylib.com
[187]: https://github.com/id-Software/Quake-2
[186]: https://github.com/id-Software/Quake
[185]: http://orx-project.org
[184]: https://github.com/ferreiradaselva/mathc
[183]: https://xiph.org/ao/
[182]: https://github.com/Kazade/kazmath
[181]: https://ioquake3.org
[180]: https://www.glfw.org/
[179]: http://freeglut.sourceforge.net
[178]: https://github.com/shlomif/fc-solve
[177]: https://github.com/anholt/libepoxy
[176]: https://icculus.org/twilight/darkplaces/
[175]: https://www.sfml-dev.org/index.php
[174]: https://www.sfml-dev.org/download/csfml/
[173]: https://github.com/orangeduck/Corange
[172]: http://chipmunk-physics.net
[171]: https://github.com/recp/cglm
[170]: https://liballeg.org

[169]: http://cyan4973.github.io/xxHash
[168]: https://github.com/leo-yuriev/t1ha
[167]: https://github.com/centaurean/spookyhash
[166]: https://github.com/google/highwayhash
[165]: https://github.com/lemire/clhash

[164]: https://github.com/waruqi/tbox
[163]: http://wolkykim.github.io/qlibc
[162]: http://www.mission-base.com/peter/source/
[161]: http://www.koanlogic.com/libu/
[160]: https://github.com/keybuk/libnih
[159]: http://libcork.readthedocs.io/en/0.14.0/
[158]: http://attractivechaos.github.io/klib/#About
[157]: https://www.enlightenment.org
[156]: http://www.eso.org/sci/software/cpl/
[155]: https://fragglet.github.io/c-algorithms
[154]: http://apr.apache.org/
[65]: https://github.com/parallella/pal

[120]: http://www.doxygen.nl/
[119]: https://hplgit.github.io/doconce/doc/web/index.html
[118]: http://www.gedanken.org.uk/software/cxref/

[107]: https://github.com/swenson/vector.h
[106]: http://troydhanson.github.io/uthash/
[105]: https://github.com/gpakosz/PackedArray
[104]: https://github.com/nbulischeck/list.h
[103]: https://faragon.github.io/libsrt.html
[102]: https://github.com/theck01/offbrand_lib
[101]: https://github.com/P-p-H-d/mlib
[100]: http://liblfds.org/
[99]: https://igraph.org/
[98]: https://github.com/recp/ds
[97]: http://adtinfo.org/libavl.html/index.html
[96]: https://github.com/jtsiomb/kdtree
[95]: https://github.com/srdja/Collections-C
[58]: https://github.com/xant/libhl

[94]: http://whitedb.org/
[93]: https://unqlite.org/
[92]: https://www.sqlite.org/
[91]: https://github.com/spotify/sparkey
[90]: http://sophia.systems
[89]: https://redis.io/
[88]: https://www.postgresql.org/
[87]: https://symas.com/lightning-memory-mapped-database/
[86]: http://mongoc.org/
[85]: https://github.com/redis/hiredis
[84]: https://github.com/groonga/groonga
[83]: http://www.oracle.com/us/products/database/berkeley-db

[82]: https://github.com/trezor/trezor-crypto
[81]: http://www.saphir2.com/sphlib/
[80]: https://github.com/awslabs/s2n
[79]: http://maciejczyzewski.me/retter/
[78]: https://github.com/miracl/MIRACL
[77]: https://tls.mbed.org/
[76]: https://www.libtom.net
[75]: https://download.libsodium.org/doc
[74]: https://openquantumsafe.org/
[73]: https://www.openssl.org/source/license.html
[72]: https://www.openssl.org/
[71]: https://gnupg.org/related_software/libgcrypt
[70]: http://www.gnutls.org/
[69]: https://gnu.org/software/gsasl/

[68]: https://tinycthread.github.io/
[67]: https://en.wikipedia.org/wiki/POSIX_Threads
[66]: https://gnu.org/software/pth/
[64]: https://www.open-mpi.org/
[63]: https://www.openmp.org/
[62]: http://tuxfan.github.io/ocl-mla/
[61]: https://github.com/matze/oclkit
[60]: http://libmill.org/
[59]: http://liburcu.org/
[57]: http://libdill.org/
[56]: https://github.com/sharow/libconcurrent
[55]: http://www.shlomifish.org/rwlock/
[54]: http://concurrencykit.org
[53]: https://github.com/yosefk/checkedthreads
[52]: http://repo.hu/projects/cchan/

[51]: http://facebook.github.io/zstd/
[50]: https://github.com/Dead2/zlib-ng
[49]: https://github.com/libarchive/libarchive
[48]: http://zlib.net
[47]: https://github.com/kuba--/zip
[46]: https://github.com/powturbo/TurboRLE
[45]: https://github.com/powturbo/TurboPFor
[44]: https://github.com/quixdb/squash
[43]: https://github.com/antirez/smaz
[42]: https://github.com/lemire/simdcomp
[41]: http://ed-von-schleck.github.io/shoco
[40]: https://github.com/vasi/pixz
[39]: http://www.oberhumer.com/opensource/lzo/
[38]: http://lz4.github.io/lz4/
[37]: https://github.com/inikep/lizard
[36]: http://www.bzip.org/
[35]: https://github.com/adamierymenko/huffandpuff
[34]: https://github.com/gildor2/fast_zlib
[33]: https://github.com/atomicobject/heatshrink
[32]: https://github.com/centaurean/density
[31]: https://github.com/Cyan4973/FiniteStateEntropy
[30]: http://roaringbitmap.org/
[29]: https://github.com/RoaringBitmap/CRoaring
[28]: http://lzip.nongnu.org/lzip.html
[27]: http://lzip.nongnu.org/clzip.html
[26]: https://github.com/google/brotli
[25]: http://blosc.org/pages/blosc-in-depth


[10]: https://github.com/jppbsi/LibDEEP/wiki
[9]: https://github.com/attractivechaos/kann
[8]: https://codeplea.com/genann
[7]: http://leenissen.dk/fann/wp/
[6]: https://github.com/100/Cranium
[5]: http://libccv.org

[AFL-2.1]: https://spdx.org/licenses/AFL-2.1.html
[AGPL-3.0-only]: https://spdx.org/licenses/AGPL-3.0-only.html
[AGPL-3.0-or-later]: https://spdx.org/licenses/AGPL-3.0-or-later.html
[Apache-2.0]: https://spdx.org/licenses/Apache-2.0.html
[BSD-1-Clause]: https://spdx.org/licenses/BSD-1-Clause.html
[BSD-2-Clause]: https://spdx.org/licenses/BSD-2-Clause.html
[BSD-3-Clause]: https://spdx.org/licenses/BSD-3-Clause.html
[BSD-4-Clause]: https://spdx.org/licenses/BSD-4-Clause.html
[CC0-1.0]: https://spdx.org/licenses/CC0-1.0.html
[curl]: https://spdx.org/licenses/curl.html
[GPL-2.0-only]: https://spdx.org/licenses/GPL-2.0-only.html
[GPL-2.0-or-later]: https://spdx.org/licenses/GPL-2.0-or-later.html
[GPL-3.0-only]: https://spdx.org/licenses/GPL-3.0-only.html
[GPL-3.0-or-later]: https://spdx.org/licenses/GPL-3.0-or-later.html
[ICU]: https://spdx.org/licenses/ICU.html
[ISC]: https://spdx.org/licenses/ISC.html
[LGPL-2.0-or-later]: https://spdx.org/licenses/LGPL-2.0-or-later.html
[LGPL-2.1-only]: https://spdx.org/licenses/LGPL-2.1-only.html
[LGPL-2.1-or-later]: https://spdx.org/licenses/LGPL-2.1-or-later.html
[LGPL-3.0-only]: https://spdx.org/licenses/LGPL-3.0-only.html
[LGPL-3.0-or-later]: https://spdx.org/licenses/LGPL-3.0-or-later.html
[Libpng]: https://spdx.org/licenses/Libpng.html
[MIT]: https://spdx.org/licenses/MIT.html
[MPL-2.0]: https://spdx.org/licenses/MPL-2.0.html
[NCSA]: https://spdx.org/licenses/NCSA.html
[OLDAP-2.8]: https://spdx.org/licenses/OLDAP-2.8.html
[PostgreSQL]: https://spdx.org/licenses/PostgreSQL.html
[TCL]: https://spdx.org/licenses/TCL.html
[Unlicense]: https://spdx.org/licenses/Unlicense.html
[WTFPL]: https://spdx.org/licenses/WTFPL.html
[X11]: https://spdx.org/licenses/X11.html
[Zlib]: https://spdx.org/licenses/Zlib.html
