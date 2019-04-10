# Awesome C #

A curated list of C good stuff.

**An important note:** this list is WIP in a sense of validating entries and
creating uniform look. I'm trying to finish it ASAP, but it takes time, so keep
it in mind.

**An important note:** first and foremost linked resources are for C, therefore
C++ is an afterthought.

**Note:** there are several awesome-c lists already, but they are having
somewhat different sets of libraries in them. This list tries to incorporate
them all, and many more other resources. Consider it my personal cheat sheet and
index for easier search instead of github stars. Also, original list categories
are a mess.

**Note:** all licenses after project descriptions are leading to actual license
text or declaration, if any provided. Source code with no license attached is
considered as automatically copyrighted by law or it is falling under the case
of terms of service of provided source code publication and hosting service, so
keep this in mind. Also, probably sometimes license can be provided or
mentioned, but I've failed to find it.

I am not an attorney btw.

Incorporated lists:

* https://github.com/aleksandar-todorovic/awesome-c (rare updates, too vague and
  sometimes mismatched categories, not very wide selection of content)
* https://github.com/kozross/awesome-c (updated regularly, but has even less
  content than one above)
* https://github.com/uhub/awesome-c (regular updated, much more content, but
  much more of it doesn't even belong to C list. Also, no structure at all)

--------------------------------------------------------------------------------

<a id="-"/></a>
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
		* [Articles and Other Resources](#articles-and-other-resources)
			* [Benchmarks](#benchmarks)
			* [Beginner Level](#beginner-level)
			* [Intermediate Level](#intermediate-level)
			* [Advanced Level](#advanced-level)
		* [Code Examples](#code-examples)
			* [Operating Systems](#operating-systems)
			* [Emulators and VMs](#emulators-vms)
			* [UI, Windowing and Graphics](#windowing-graphics)
			* [Language Implementations](#language-implementations)
			* [Challenges](#challenges)
			* [Other Examples](#other-examples)

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
* [Filetype Targets](#filetype-targets)
	* [Binaries](#binaries)
	* [CSV](#csv)
	* [JSON](#json)
	* [INI](#ini)
	* [XML](#xml)
	* [Other Filetypes](#other-filetypes)
* [Flow Control and Language Extension](#flow-control)
* [Game Development](#gamedev)
	* [Engines](#gamedev-engines)
	* [Graphics Rendering](#gamedev-rendering)
	* [Helping Libraries](#gamedev-helping-libraries)
* [Geography](#geography)
* [GUI](#gui)
* [Hardware Oriented](#hardware-oriented)
* [Hashing](#hashing)
* [Image Processing and Computer Vision](#image-processing)
* [Integrated Debugging](#integrated-debugging)
* [I/O](#io)
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
* [OpenCL](#opencl)
* [OS Specifics](#os-specifics)
* [Procedural Generation](#procedural-generation)
* [Regex](#regex)
* [Serialization](#serialization)
* [Source Code Collections](#source-code-collections)
* [Standard Libraries](#standart-libraries)
* [String Manipulation](#string-manipulation)
* [Testing](#testing)
* [TUI](#tui)
* [Web Frameworks](#web-frameworks)
* [Web Service APIs](#web-service-apis)

--------------------------------------------------------------------------------

* [Uncategorized](#uncategorized)

--------------------------------------------------------------------------------

<a id="meta"/></a>
## Meta ##
<a id="standarts"/></a>
<details>
  <summary>Standarts</summary>

  ### <a href="#-">`^`</a> Standarts ###
  * [Draft C89 standard][1-1]
  * [Draft C99 standard][1-2]
  * [Draft C11 standard][1-3]
  * [Draft C18 standard][1-4]

  [1-4]: https://web.archive.org/web/20181230041359if_/http://www.open-std.org/jtc1/sc22/wg14/www/abq/c17_updated_proposed_fdis.pdf
  [1-3]: https://port70.net/~nsz/c/c11/n1570.html
  [1-2]: https://port70.net/~nsz/c/c99/n1256.html
  [1-1]: https://port70.net/~nsz/c/c89/c89-draft.html
</details>

-------------------------------------------------------------------------------

<a id="tooling"></a>
### Tooling ###
<a id="build-systems"></a>
<details>
  <summary>Build Systems</summary>

  #### <a href="#-">`^`</a> Build Systems ####
  * [aimake][2-1] - Build tool designed to avoid complex configurations. [`GPL 3`][2-21]
  * [Autoconf][2-2] - Extensible package of M4 macros that produce shell scripts
  to automatically configure software source code packages. Part of the
  Autotools. [`GPL 2`][2-22]
  * [Automake][2-3] - Tool for automatically generating `Makefile.in` files
  compliant with the GNU Coding Standards. Requires the use of Autoconf. Part of
  the Autotools. [`GPL 2`][2-23]
  * [Bazel][2-4] - Build system for various operating systems and targets. [`Apache 2`][2-24]
  * [Buck][2-5] - Build system created and used by Facebook. [`Apache 2`][2-25]
  * [CMake][2-6] - Cross-platform family of tools designed to build, package and
  test software. Written in C++11. [`BSD 3-Clause`][2-26]
  * [GNU Make][2-7] - Tool which controls the generation of executables and
  other non-source files of a program. [`GPL 3`][2-27]
  * [jamplus/jamplus][2-29] - Jamplus is a generic code and data build system
  derived from the original Perforce version of Jam. [`License`][2-28]
  * [Libtool][2-11] - Generic library support script. Part of the Autotools. [`GPL 2`][2-30]
  * [Meson][2-12] - Build system based on Ninja and Python. [`Apache 2`][2-31]
  * [Ninja][2-13] - Small, simple build system with a focus on speed. [`Apache 2`][2-32]
  * [Premake][2-14] - Generates project files for Visual Studio, Xcode and GNU
  Make. Targets suppport can be extended via modules. [`BSD 3-Clause`][2-33]
  * [Qbs][2-15] - Modern build tool for software projects. [`Licenses`][2-34]
  * [qmake][2-16] - Build system included with the Qt Framework. [`Licenses`][2-35]
  * [SCons][2-18] - Software construction tool based on Python. [`License`][2-36]
  * [gittup/tup][2-37] - Tup is a file-based build system. [`GPL 2`][2-38]
  * [xmake][2-19] - Cross-platform build utility based on Lua. [`Apache 2`][2-39]
  * [zproject][2-20] - Project generator and build system support tool for
  ZeroMQ project. [`MPL 2`][2-40]

  [2-40]: https://github.com/zeromq/zproject/blob/master/LICENSE
  [2-39]: https://github.com/xmake-io/xmake/blob/master/LICENSE.md
  [2-38]: https://github.com/gittup/tup/blob/master/COPYING
  [2-37]: https://github.com/gittup/tup
  [2-36]: https://github.com/SCons/scons/blob/master/LICENSE
  [2-35]: https://code.qt.io/cgit/qt/qtbase.git/tree/
  [2-34]: https://doc.qt.io/qbs/attributions.html
  [2-33]: https://github.com/premake/premake-core/blob/master/LICENSE.txt
  [2-32]: https://github.com/ninja-build/ninja/blob/master/COPYING
  [2-31]: http://mesonbuild.com/legal.html
  [2-30]: http://git.savannah.gnu.org/cgit/libtool.git/tree/AUTHORS
  [2-29]: https://github.com/jamplus/jamplus
  [2-28]: https://github.com/jamplus/jamplus/blob/master/LICENSE
  [2-27]: http://git.savannah.gnu.org/cgit/make.git/tree/COPYING
  [2-26]: https://cmake.org/licensing/
  [2-25]: https://github.com/facebook/buck/blob/master/LICENSE
  [2-24]: https://github.com/bazelbuild/bazel/blob/master/LICENSE
  [2-23]: http://git.savannah.gnu.org/cgit/automake.git/tree/COPYING
  [2-22]: http://git.savannah.gnu.org/gitweb/?p=autoconf.git;a=blob_plain;f=COPYING;hb=HEAD
  [2-21]: http://nethack4.org/projects/aimake/documentation.html#COPYRIGHT
  [2-20]: https://github.com/zeromq/zproject
  [2-19]: https://xmake.io/
  [2-18]: https://www.scons.org/
  [2-17]: N/A
  [2-16]: https://doc.qt.io/qt-5/qmake-manual.html
  [2-15]: http://doc.qt.io/qbs/
  [2-14]: https://github.com/premake/premake-core
  [2-13]: https://github.com/ninja-build/ninja
  [2-12]: http://mesonbuild.com/
  [2-11]: https://www.gnu.org/software/libtool/
  [2-10]: N/A
  [2-9]: N/A
  [2-8]: N/A
  [2-7]: https://www.gnu.org/software/make/
  [2-6]: https://cmake.org/
  [2-5]: https://buckbuild.com/
  [2-4]: https://bazel.build/
  [2-3]: https://www.gnu.org/software/automake/automake.html
  [2-2]: https://www.gnu.org/software/autoconf/autoconf.html
  [2-1]: http://nethack4.org/projects/aimake/
</details>

<a id="compilers"></a>
<details>
  <summary>Compilers</summary>

  #### <a href="#-">`^`</a> Compilers ####
  * [rui314/8cc][3-10] - A Small C Compiler. [`MIT`][3-9]
  * [rui314/9cc][3-12] - A Small C Compiler. [`MIT`][3-11]
  * [jserv/amacc][3-14] - Small C Compiler generating ELF executable for Arm
  architecture. [`GPL 2`][3-13]
  * [andrewchambers/c][3-16] - small self hosting C compiler. [`BSD 2-Clause`][3-15]
  * [cc65/cc65][3-18] - cc65 - a freeware C compiler for 6502 based systems. [`Zlib`][3-17]
  * [Clang][3-2] - Compiler for LLVM. Supports C11. [`NCSA`][3-19]
  * [CompCert][3-5] - Fully-verified C compiler. Supports almost all of C89. [`License`][3-20]
  * [GCC][3-1] a C compiler as part of its compiler set. Supports C11. [`License`][3-21]
  * [Intel SPMD][3-7] - Compiler for a variant of the C language, for single
  program, multiple data programming. [`License`][3-22]
  * [PCC][3-3] - Venerable compiler. Supports C99. [`Licenses`][3-4]
  * [larmel/lacc][3-24] - A simple, self-hosting C compiler. [`MIT`][3-23]
  * [drh/lcc][3-26] - The lcc retargetable ANSI C compiler. [`License`][3-25]
  * [TCC][3-6] - Tiny C Compiler; a small, fast C compiler. Supports C99 (except
  complex types). [`LGPL 2.1`][3-27]
  * [alexfru/SmallerC][3-29] - Simple C compiler. [`License`][3-28]

  [3-29]: https://github.com/alexfru/SmallerC
  [3-28]: https://github.com/alexfru/SmallerC/blob/master/license.txt
  [3-27]: https://repo.or.cz/tinycc.git/blob/HEAD:/COPYING
  [3-26]: https://github.com/drh/lcc
  [3-25]: https://github.com/drh/lcc/blob/master/CPYRIGHT
  [3-24]: https://github.com/larmel/lacc
  [3-23]: https://github.com/larmel/lacc/blob/master/LICENSE.md
  [3-22]: https://github.com/ispc/ispc/blob/master/LICENSE.txt
  [3-21]: https://www.gnu.org/licenses/gcc-exception.html
  [3-20]: https://github.com/AbsInt/CompCert/blob/master/LICENSE
  [3-19]: https://opensource.org/licenses/UoI-NCSA.php
  [3-18]: https://github.com/cc65/cc65
  [3-17]: https://github.com/cc65/cc65/blob/master/LICENSE
  [3-16]: https://github.com/andrewchambers/c
  [3-15]: https://github.com/andrewchambers/c/blob/master/LICENSE
  [3-14]: https://github.com/jserv/amacc
  [3-13]: https://github.com/jserv/amacc/blob/master/LICENSE
  [3-12]: https://github.com/rui314/9cc
  [3-11]: https://github.com/rui314/9cc/blob/master/LICENSE
  [3-10]: https://github.com/rui314/8cc
  [3-9]: https://github.com/rui314/8cc/blob/master/LICENSE
  [3-8]: https://github.com/ispc/ispc/blob/master/LICENSE.txt
  [3-7]: http://ispc.github.io/
  [3-6]: https://bellard.org/tcc/
  [3-5]: http://compcert.inria.fr/
  [3-4]: http://pcc.ludd.ltu.se/licenses/
  [3-3]: http://pcc.ludd.ltu.se/
  [3-2]: https://clang.llvm.org/
  [3-1]: https://gcc.gnu.org/
</details>

<a id="debugging-and-analysis"></a>
<details>
  <summary>Debugging and Analysis</summary>

  #### <a href="#-">`^`</a> Debugging and Analysis ####
  * [C-Reduce][4-1] - Tool that takes a large C file with a property of interest
  and automatically produces a much smaller C file that has the same property.
  Intended to help create minimal bug-demonstrating cases in complex code. [`License`][4-14]
  * [CBMC][4-2] - C Bounded Model Checker; a tool for verification of array
  bounds, pointer safety and user-specified assertions. [`License`][4-15]
  * [cgdb/cgdb][4-17] - Console front-end to the GNU debugger. [`GPL 2`][4-16]
  * [GNU cflow][4-6] - Analyzes a collection of source files and prints a graph
  charting control flow in the program. [`GPL 3`][4-18]
  * [ClangCheck][4-4] - Static analysis tool, designed to work with Clang. [`NCSA`][4-19]
  * [GNU Complexity][4-7] - Tool for measuring the complexity of source code. [`GPL 3`][4-20]
  * [Cppcheck][4-5] - Static analysis tool. Despite the name, works well with C. [`GPL 3`][4-21]
  * [CScout][4-8] - Source code analyzer and refactoring browser for C programs. [`GPL 3`][4-22]
  * [agl/ctgrind][4-23] - Checking that functions are constant time with
  Valgrind. `No license`
  * [GNU DDD][4-9] - Graphical front-end for a range of command-line debuggers. [`Licenses`][4-24]
  * [GDB][4-10] - GNU Project debugger. [`Licenses`][4-25]
  * [lldb][4-11] - LLVM debugger. [`NCSA`][4-19]
  * [rr][4-12] - Debugger that records non-deterministic executions to allow for
  deterministic debugging. [`License`][4-26]
  * [SVF-tools/SVF][4-27] - Pointer Analysis and Program Dependence Analysis for
  C and C++ Programs. [`License`][4-28]
  * [Valgrind][4-13] - Range of dynamic analysis tools, including a leak
  checker. [`GPL 2`][4-29]

  [4-29]: http://www.valgrind.org/
  [4-28]: https://github.com/SVF-tools/SVF/blob/master/LICENSE.TXT
  [4-27]: https://github.com/SVF-tools/SVF
  [4-26]: https://github.com/mozilla/rr/blob/master/LICENSE
  [4-25]: https://sourceware.org/git/gitweb.cgi?p=binutils-gdb.git;a=tree
  [4-24]: http://svn.savannah.gnu.org/viewvc/ddd/trunk/
  [4-23]: https://github.com/agl/ctgrind
  [4-22]: https://github.com/dspinellis/cscout/blob/master/LICENSE.txt
  [4-21]: https://github.com/danmar/cppcheck/blob/master/COPYING
  [4-20]: https://ftp.gnu.org/gnu/complexity/
  [4-19]: https://opensource.org/licenses/UoI-NCSA.php
  [4-18]: http://git.savannah.gnu.org/cgit/cflow.git/tree/COPYING
  [4-17]: https://github.com/cgdb/cgdb
  [4-16]: https://github.com/cgdb/cgdb/blob/master/COPYING
  [4-15]: https://www.cprover.org/cbmc/LICENSE
  [4-14]: https://github.com/csmith-project/creduce/blob/master/COPYING
  [4-13]: http://www.valgrind.org/
  [4-12]: https://rr-project.org/
  [4-11]: https://lldb.llvm.org/
  [4-10]: https://www.gnu.org/software/gdb/
  [4-9]: https://www.gnu.org/software/ddd/ddd.html
  [4-8]: https://www.spinellis.gr/cscout/
  [4-7]: https://www.gnu.org/software/complexity/
  [4-6]: http://www.gnu.org/software/cflow/
  [4-5]: http://cppcheck.sourceforge.net/
  [4-4]: https://clang.llvm.org/docs/ClangCheck.html
  [4-3]: N/A
  [4-2]: https://www.cprover.org/cbmc/
  [4-1]: https://embed.cs.utah.edu/creduce/
</details>

<a id="documentation-generation"></a>
<details>
  <summary>Documentation Generation</summary>

  #### <a href="#-">`^`</a> Documentation Generation ####
  * [Cxref][5-1] - Generates documentation in either LaTeX, HTML, RTF or SGML. [`GPL 2`][5-5]
  * [DocOnce][5-2] - Modestly tagged markup language that can be used to
  generate a range of formats. [`BSD 3-Clause`][5-6]
  * [Doxygen][5-3] - De-facto standard tool for generating documentation from
  annotated sources. Can generate a large range of formats. [`GPL 2`][5-7]
  * [GTK-Doc][5-4] - Tool for generating C documentation from annotated sources.
  Has support for the Autotools. [`GPL 2`][5-8]

  [5-8]: https://gitlab.gnome.org/GNOME/gtk-doc/blob/master/COPYING
  [5-7]: http://www.doxygen.nl/
  [5-6]: https://github.com/hplgit/doconce/blob/master/LICENSE
  [5-5]: http://www.gedanken.org.uk/viewvc/cxref/trunk/doc/COPYING?view=markup
  [5-4]: https://www.gtk.org/gtk-doc/
  [5-3]: http://www.doxygen.nl/
  [5-2]: https://hplgit.github.io/doconce/doc/web/index.html
  [5-1]: http://www.gedanken.org.uk/software/cxref/
</details>

<a id="editors"></a>
<details>
  <summary>Editors</summary>

  #### <a href="#-">`^`</a> Editors ####
  * [Anjuta DevStudio][6-1] - GNOME IDE. [`GPL 2`][6-12]
  * [Atom][6-3] - Hackable text editor for the 21st century. [`MIT`][6-13]
  * [Code::Blocks][6-2] - Extendable, configurable IDE supporting C. [`GPL 3`][6-14]
  * [CodeLite][6-4] - Cross-platform IDE. [`GPL 2`][6-15]
  * [Eclipse][6-6] - IDE written in Java. [`EPL 2`][6-16]
  * [Geany][6-5] - Small and fast IDE. [`GPL 2`][6-17]
  * [KDevelop][6-8] - KDE IDE. [`GPL 2`][6-18]
  * [Qt Creator][6-9] - Cross-platform IDE written with C++ and Qt, part of the
  Qt SDK. Supports Clang Code Model. [`GPL 3 w/ exceptions`][6-19]
  * [Visual Studio Code][6-11] - Code editing, redefined. Visual Studio Code. [`MIT`][6-20]

  [6-20]: https://github.com/Microsoft/vscode/blob/master/LICENSE.txt
  [6-19]: https://code.qt.io/cgit/qt-creator/qt-creator.git/tree/LICENSE.GPL3-EXCEPT
  [6-18]: https://phabricator.kde.org/source/kdevelop/browse/master/COPYING
  [6-17]: https://github.com/geany/geany/blob/master/COPYING
  [6-16]: https://www.eclipse.org/legal/epl-2.0/
  [6-15]: https://github.com/eranif/codelite/blob/master/LICENSE
  [6-14]: http://svn.code.sf.net/p/codeblocks/code/trunk/COPYING
  [6-13]: https://github.com/atom/atom/blob/master/LICENSE.md
  [6-12]: https://gitlab.gnome.org/GNOME/anjuta/blob/master/COPYING
  [6-11]: https://github.com/Microsoft/vscode
  [6-10]: N/A
  [6-9]: https://www.qt.io/qt-features-libraries-apis-tools-and-ide/#ide
  [6-8]: https://www.kdevelop.org/
  [6-7]: https://directory.fsf.org/wiki/License:EPL-1.0
  [6-6]: http://www.eclipse.org/ide/
  [6-5]: https://www.geany.org/
  [6-4]: https://codelite.org/
  [6-3]: https://atom.io/
  [6-2]: http://www.codeblocks.org/
  [6-1]: http://anjuta.org/
</details>

<a id="microsoft-windows-environment"></a>
<details>
  <summary>Microsoft Windows Environment</summary>

  #### <a href="#-">`^`</a> Microsoft Windows Environment ####
  * [Cygwin][7-1] - Designed to emulate a POSIX-compatible environment
  extensively under Windows. [`Licenses`][7-2]
  * [MinGW-w64][7-3] - Minimalist environment for C development on Windows with
  64 bit support. [`Licenses`][7-4]
  * [MSYS2][7-5] - Minimal SYStem 2; aims to provide support for a POSIX
  environment on Windows, with a package manager based on Arch Linux's
  pacman. Packages have individual licenses, otherwise, as MinGW and Cygwin. [`BSD 3-Clause`][7-6]
  * [reactos][7-7] - A free Windows-compatible Operating System. [`GPL 2`][7-8]

  [7-8]: https://github.com/reactos/reactos/blob/master/COPYING
  [7-7]: https://github.com/reactos/reactos
  [7-6]: https://github.com/msys2/MINGW-packages/blob/master/LICENSE
  [7-5]: http://msys2.github.io/
  [7-4]: http://mingw.org/license
  [7-3]: http://mingw-w64.yaxm.org/doku.php/start
  [7-2]: https://cygwin.com/licensing.html
  [7-1]: https://cygwin.com/
</details>

<a id="profiling"></a>
<details>
  <summary>Profiling</summary>

  #### <a href="#-">`^`</a> Profiling ####
  * [gperftools][8-1] - Collection of utilities for measuring and improving
  performance. [`BSD 3-Clause`][8-5]
  * [gprof][8-2] - Performance analysis tool. Part of GNU binutils. [`Licenses`][8-6]
  * [OProfile][8-3] - Statistical profiler for Linux. Can profile any code
  (including the kernel!) with low overhead and without recompilation. [`GPL 2`][8-7]
  * [perf][8-4] - Linux kernel-based profiler with a lot of functionality. [`GPL 2`][8-8]

  [8-8]: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/tree/COPYING
  [8-7]: https://sourceforge.net/p/oprofile/oprofile/ci/master/tree/COPYING
  [8-6]: https://sourceware.org/git/gitweb.cgi?p=binutils-gdb.git;a=tree
  [8-5]: https://github.com/gperftools/gperftools/blob/master/COPYING
  [8-4]: https://perf.wiki.kernel.org/index.php/Main_Page
  [8-3]: http://oprofile.sourceforge.net/news/
  [8-2]: https://www.gnu.org/software/binutils/
  [8-1]: https://github.com/gperftools/gperftools
</details>

<a id="text-editor-extensions"></a>
<details>
  <summary>Text Editor Extensions</summary>

  #### <a href="#-">`^`</a> Text Editor Extensions ####
  * [CCompletion][9-1] - Notepad++ autocompletion plugin. Works with all
  identifiers recognized by Ctags. This is a download link. [`GPL 2`]
  * [CEDET][9-2] - Collection of Emacs Development Environment Tools; designed
  to provide IDE-like features to Emacs. Built-in. [`GPL 2`][9-10]
  * [lvzixun/Clang-Complete][9-13] - an autocomplete plugin for sublimetext3. `No license`
  * [editorconfig-core-c][9-14] - EditorConfig core library written in C (for
  use by plugins supporting EditorConfig parsing). [`License`][9-15]
  * [Flycheck][9-3] - Modern syntax checking for Emacs. For C, it can use either
  GCC or Clang as a back-end. [`GPL 3`][9-11]
  * [AtomLinter/linter-clang][9-4] - Lint C code in Atom, using Clang. `No license`
  * [hebaishi/linter-gcc][9-5] - Lint C code in Atom, using GCC. [`MIT`][9-12]
  * [Neomake][9-6] - make and linting framework for Neovim/Vim. [`MIT`][9-16]
  * [Syntastic][9-7] - Syntax checking and linting for Vim. [`WTFPL`][9-17]
  * [YASnippet][9-8] - Emacs code template system, with C templates for common
  snippets. [`EPLA`][9-18]
  * [YouCompleteMe][9-9] - Code completion engine for Vim. [`GPL 3`][9-19]

  [9-19]: https://github.com/Valloric/YouCompleteMe/blob/master/COPYING.txt
  [9-18]: https://github.com/joaotavora/yasnippet/blob/master/CONTRIBUTING.md
  [9-17]: https://github.com/vim-syntastic/syntastic/blob/master/LICENCE
  [9-16]: https://github.com/neomake/neomake/blob/master/LICENSE
  [9-15]: https://github.com/editorconfig/editorconfig-core-c/blob/master/LICENSE
  [9-14]: https://github.com/editorconfig/editorconfig-core-c
  [9-13]: https://github.com/lvzixun/Clang-Complete
  [9-12]: https://github.com/hebaishi/linter-gcc/blob/master/LICENSE.md
  [9-11]: https://github.com/flycheck/flycheck/blob/master/COPYING
  [9-10]: https://sourceforge.net/projects/cedet/
  [9-9]: http://valloric.github.io/YouCompleteMe/
  [9-8]: http://joaotavora.github.io/yasnippet/
  [9-7]: https://github.com/vim-syntastic/syntastic
  [9-6]: https://github.com/neomake/neomake
  [9-5]: https://github.com/hebaishi/linter-gcc
  [9-4]: https://github.com/AtomLinter/linter-clang
  [9-3]: https://github.com/flycheck/flycheck
  [9-2]: http://cedet.sourceforge.net/
  [9-1]: http://freeweb.siol.net/rmihor/NppCCompletionPlugin.zip
</details>

<a id="utilities"></a>
<details>
  <summary>Utilities</summary>

  #### <a href="#-">`^`</a> Utilities ####
  * [Artistic Style][10-4] - Fast and small automatic source code formatter that
  supports C. [`MIT`][10-17]
  * [biicode][10-5] - Dependency manager. [`MIT`][10-18]
  * [ryanmjacobs/c][10-6] - Compile and execute C "scripts" in one go on the
  command line. Also has shebang support. [`MIT`][10-19]
  * [libav/c99-to-c89][10-20] - Tool to convert C99 code to MSVC-compatible C89. [`Apache 2`][10-21]
  * [RhysU/c99sh][10-7] - Run C files using hash-bang. [`BSD 2-Clause`][10-22]
  * [aquynh/capstone][10-23] - Dissasembly/disassembler framework. [`BSD 3-clause`][10-24]
  * [ccache][10-1] - Compiler cache designed to speed up recompilation. [`GPL 3`][10-25]
  * [cdecl][10-8] - Online service to translate C declarations into English and
  vice versa. [`Public domain`]
  * [cinclude2dot][10-9] - Graphs include dependencies in a project using
  Graphviz. [`GPL`][10-26]
  * [jbremer/darm][10-27] - A light-weight and efficient disassembler written in
  C for the ARMv7 instruction set. [`BSD 3-Clause`][10-28]
  * [jacob-carlborg/dstep][10-29] - A tool for converting C and Objective-C
  headers to D modules. [`Boost`][10-30]
  * [anael-seghezzi/CToy][10-31] - Interactive C coding environment. [`License`][10-32]
  * [distcc][10-2] - Program that allows builds to be distributed among several
  machines. [`GPL 3`][10-33]
  * [GNU Global][10-10] - Source code tagging tool. [`GPL 3`][10-34]
  * [GPP][10-11] - General-purpose preprocessor. More versatile than the C
  preprocessor, but more flexible than m4. [`LGPL 3`][10-35]
  * [Highlight][10-12] - Converts source code to formatted text with
  highlighting. [`GPL 3`][10-36]
  * [include-what-you-use][10-13] - Helps find unecessary inclusions and make
  suggestions for fixing them. Based on LLVM/Clang (and only works with it). [`License`][10-37]
  * [GNU indent][10-14] - Formats C source code automatically to make it easier
  to read. Also converts from one style of source to another. [`GPL 3`][10-38]
  * [m-schmoock/lcpp][10-39] - A Lua C PreProcessor. [`MIT`][10-40]
  * [mcpp][10-41] - Portable C preprocessor. [`2-clause BSD`][10-42]
  * [jimenezrick/patch-AuthenticAMD][10-43] - Utility for patching binaries
  generated by the Intel Compiler to get the maximum performance on AMD CPUs. [`GPL 3`][10-44]
  * [radare2][10-45] - unix-like reverse engineering framework and commandline
  tools security. [`LGPL 3`][10-46]
  * [buserror/simavr][10-47] - simavr is a lean, mean and hackable AVR simulator
  for linux & OSX. [`GPL 3`][10-48]
  * [SMACK][10-15] - Modular software verification toolchain and a
  self-contained software verifier. Currently only works with programs compiled
  using Clang. [`License`][10-49]
  * [sickill/stderred][10-50] - stderr in red. [`License`][10-51]
  * [ggreer/the_silver_searcher][10-52] - A code-searching tool similar to ack,
  but faster. [`Apache 2`][10-53]
  * [unifdef][10-16] - Removes #ifdef and #if directives with their delimited
  text without touching any other part of the file. [`Licenses`][10-54]

  [10-54]: http://dotat.at/cgi/git/unifdef.git/blob/HEAD:/COPYING
  [10-53]: https://github.com/ggreer/the_silver_searcher/blob/master/LICENSE
  [10-52]: https://github.com/ggreer/the_silver_searcher
  [10-51]: https://github.com/sickill/stderred/blob/master/LICENSE
  [10-50]: https://github.com/sickill/stderred
  [10-49]: https://github.com/smackers/smack/blob/master/LICENSE
  [10-48]: https://github.com/buserror/simavr/blob/master/COPYING
  [10-47]: https://github.com/buserror/simavr
  [10-46]: https://github.com/radare/radare2/blob/master/COPYING
  [10-45]: https://github.com/radare/radare2
  [10-44]: https://github.com/jimenezrick/patch-AuthenticAMD/blob/master/COPYING
  [10-43]: https://github.com/jimenezrick/patch-AuthenticAMD
  [10-42]: https://sourceforge.net/projects/mcpp/
  [10-41]: http://mcpp.sourceforge.net/
  [10-40]: https://github.com/m-schmoock/lcpp/blob/master/lcpp.lua
  [10-39]: https://github.com/m-schmoock/lcpp
  [10-38]: http://git.savannah.gnu.org/cgit/indent.git/tree/COPYING
  [10-37]: https://github.com/include-what-you-use/include-what-you-use/blob/master/LICENSE.TXT
  [10-36]: https://github.com/tajmone/highlight/blob/master/COPYING
  [10-35]: https://logological.org/gpp
  [10-34]: https://www.gnu.org/software/global/license.html
  [10-33]: https://github.com/distcc/distcc/blob/master/COPYING
  [10-32]: https://github.com/anael-seghezzi/CToy/blob/master/src/ctoy.c
  [10-31]: https://github.com/anael-seghezzi/CToy
  [10-30]: https://github.com/jacob-carlborg/dstep
  [10-29]: https://github.com/jacob-carlborg/dstep
  [10-28]: https://github.com/jbremer/darm/blob/master/LICENSE.txt
  [10-27]: https://github.com/jbremer/darm
  [10-26]: https://www.flourish.org/cinclude2dot/cinclude2dot
  [10-25]: https://ccache.samba.org/license.html
  [10-24]: https://github.com/aquynh/capstone/blob/master/LICENSE.TXT
  [10-23]: https://github.com/aquynh/capstone
  [10-22]: https://github.com/RhysU/c99sh/blob/master/LICENSE.txt
  [10-21]: https://github.com/libav/c99-to-c89/blob/master/LICENSE
  [10-20]: https://github.com/libav/c99-to-c89
  [10-19]: https://github.com/ryanmjacobs/c/blob/master/LICENSE
  [10-18]: https://github.com/biicode/biicode/blob/master/LICENSE
  [10-17]: https://sourceforge.net/projects/astyle/
  [10-16]: http://dotat.at/prog/unifdef/
  [10-15]: https://github.com/smackers/smack
  [10-14]: https://www.gnu.org/software/indent/
  [10-13]: https://github.com/include-what-you-use/include-what-you-use
  [10-12]: http://www.andre-simon.de/doku/highlight/en/highlight.php
  [10-11]: https://logological.org/gpp
  [10-10]: https://www.gnu.org/software/global/
  [10-9]: https://www.flourish.org/cinclude2dot/
  [10-8]: https://cdecl.org/
  [10-7]: https://github.com/RhysU/c99sh
  [10-6]: https://github.com/ryanmjacobs/c
  [10-5]: https://biicode.github.io/biicode/
  [10-4]: http://astyle.sourceforge.net/
  [10-3]: N/A
  [10-2]: https://github.com/distcc/distcc
  [10-1]: https://ccache.samba.org/
</details>

--------------------------------------------------------------------------------

<a id="reading-material"></a>
### Reading Material ###
<a id="books"></a>
<details>
  <summary>Books</summary>

  #### <a href="#-">`^`</a> Books ####
  ##### Reference Books #####
  * [C in a Nushell 2E][11-1] - Concise reference book for C11.
  * [C Pocket Reference][11-2] - Concise reference book for C99.
  * [C: A Reference Manual 5E][11-3] - Full reference book for C99.
  * [SEI CERT C Coding Standard][11-4] - Coding  recommendations from CERT.
  * [The C Programming Language 2E][11-5] - Original book on C, by its creators.

  [11-5]: https://en.wikipedia.org/wiki/The_C_Programming_Language
  [11-4]: https://wiki.sei.cmu.edu/confluence/display/c/SEI+CERT+C+Coding+Standard
  [11-3]: http://careferencemanual.com/
  [11-2]: http://shop.oreilly.com/product/9780596004361.do
  [11-1]: http://shop.oreilly.com/product/0636920033844.do

  ##### Beginner Books #####
  * [C Primer Plus 6E][12-1] - Complete tutorial on programming in C11.
  * [C Programming: A Modern Approach][12-2] - Book to learn the basics of C.
  * [Head First C][12-3] - 'Head-first' style book for learning C.
  * [The GNU C Programming Tutorial][12-4] - Beware, GNU C is not standart C. (PDF)

  [12-4]: http://www.crasseux.com/books/ctut.pdf
  [12-3]: http://shop.oreilly.com/product/0636920015482.do
  [12-2]: http://knking.com/books/c2/index.html
  [12-1]: https://www.pearson.com/us/higher-education/program/Prata-C-Primer-Plus-6th-Edition/PGM4399.html

  ##### Intermediate Books #####
  * [21st Century C][13-1] - Programming book on C that touches tooling subject.
  * [Understanding and Using C Pointers][13-2] - In-depth book on pointers in C.
  * [Algorithms in C, Parts 1-4: Fundamentals, Data Structures, Sorting, Searching][13-3]
  * [C Interfaces and Implementations: Techniques for Creating Reusable Software][13-4]
  * [The Standard C Library][13-5]
  * [Let Us C][13-6]
  * [C Programming FAQs: Frequently Asked Questions][13-7]
  * [OpenGL SuperBible][13-8]
  * [OpenGL Insights][13-9]

  [13-9]: http://openglinsights.com/
  [13-8]: http://www.openglsuperbible.com
  [13-7]: https://www.goodreads.com/book/show/528549.C_Programming_FAQs
  [13-6]: https://www.goodreads.com/book/show/2522685.Let_Us_C
  [13-5]: https://www.goodreads.com/book/show/522100.The_Standard_C_Library
  [13-4]: https://www.goodreads.com/book/show/475432.C_Interfaces_and_Implementations
  [13-3]: https://www.goodreads.com/book/show/27862.Algorithms_in_C_Parts_1_4
  [13-2]: http://shop.oreilly.com/product/0636920028000.do
  [13-1]: http://shop.oreilly.com/product/0636920033677.do

  ##### Advanced Books #####
  * [Expert C Programming: Deep C Secrets][14-1] - Interesting, in-depth and
  entertaining look at the innards of C.
  * [Pointers on C][14-3]
  * [The C Puzzle Book][14-4]

  [14-4]: https://www.goodreads.com/book/show/811303.The_C_Puzzle_Book
  [14-3]: https://www.goodreads.com/book/show/526293.Pointers_on_C
  [14-2]: N/A
  [14-1]: https://dl.acm.org/citation.cfm?id=179241
</details>

#### Articles and Other Resources ####

<a id="benchmarks"></a>
<details>
  <summary>Benchmarks</summary>

  ##### <a href="#-">`^`</a> Benchmarks #####
  * [Benchmarks of the Lockless Memory Allocator][15-1]
  * [Comparison of C/POSIX standard library implementations for Linux][15-2] - A
  bit outdated, but shows overall tendencies
  * [Finding the best 64-bit simulation PRNG][15-3]
  * [rxin/db-benchmarks][15-4] - Collection of some database benchmarks, along
  with tools to parallelize the data generation.

  [15-4]: https://github.com/rxin/db-benchmarks
  [15-3]: http://nullprogram.com/blog/2017/09/21/
  [15-2]: http://www.etalabs.net/compare_libcs.html
  [15-1]: https://locklessinc.com/benchmarks_allocator.shtml
</details>

<a id="beginner-level"></a>
<details>
  <summary>Beginner Level</summary>

  ##### <a href="#-">`^`</a> Beginner Level #####
  * [A tutorial on pointers][16-1]
  * [A tutorial on portable Makefiles][16-2]
  * [Building C Projects][16-3]
  * [Introduction to \`fun' C][16-4]
  * [Learning C with GDB][16-5]
  * [Tutorial on pointers][16-6]
  * [C Programming Wikibook][16-7]
  * [POSIX Threads Programming tutorial][16-8]
  * [Templating in C][16-9]

  [16-9]: http://blog.pkh.me/p/20-templating-in-c.html
  [16-8]: https://computing.llnl.gov/tutorials/pthreads/
  [16-7]: https://en.wikibooks.org/wiki/C_Programming
  [16-6]: http://home.netcom.com/~tjensen/ptr/pointers.htm
  [16-5]: https://www.recurse.com/blog/5-learning-c-with-gdb
  [16-4]: https://gist.github.com/eatonphil/21b3d6569f24ad164365
  [16-3]: http://nethack4.org/blog/building-c.html
  [16-2]: http://nullprogram.com/blog/2017/08/20/
  [16-1]: https://pdos.csail.mit.edu/6.828/2017/readings/pointers.pdf
</details>

<a id="intermediate-level"></a>
<details>
  <summary>Intermediate Level</summary>

  ##### <a href="#-">`^`</a> Intermediate Level #####
  * [A comprehensive MPI tutorial resource][17-1]
  * [Diving into concurrency: trying out mutexes and atomics][17-2]
  * [Generic C reference counting][17-3]
  * [How to write portable C without complicating your build][17-4]
  * [Scalable C - Writing Large-Scale Distributed C][17-5]
  * [8 gdb tricks you should know][17-6]
  * [10 C99 tricks][17-7]
  * [Introduction to OpenMP][17-8] (video)
  * [OpenMP tutorial][17-9]
  * [memcpy vs memmove][17-10]
  * [MPI tutorial][17-11]
  * [Some unknown features or tricks in C language][17-12]
  * [The lost art of C structure packing][17-13]
  * [What a C programmer should know about memory][17-14]
  * [What every C programmer should know about undefined behaviour][17-15]
  * [arjun024/hide-data-in-ptr][17-16] - how to hide data inside pointers
  * [OpenGL Book][17-17]
  * [Autotools Tutorial][17-18] (PDF)
  * [C FAQ - comp.lang.c Frequently Asked Questions][17-19]
  * [Akagi201/learning-cmake][17-20] - CMake examples
  * [Let's build a database][17-21]
  * [nikhilm/uvbook][17-22] - An Introduction to libuv

  [17-22]: https://github.com/nikhilm/uvbook
  [17-21]: https://cstack.github.io/db_tutorial/
  [17-20]: https://github.com/Akagi201/learning-cmake
  [17-19]: http://c-faq.com/
  [17-18]: https://www.lrde.epita.fr/~adl/dl/autotools.pdf
  [17-17]: http://openglbook.com/
  [17-16]: https://github.com/arjun024/hide-data-in-ptr
  [17-15]: http://blog.llvm.org/2011/05/what-every-c-programmer-should-know.html
  [17-14]: http://marek.vavrusa.com/memory/
  [17-13]: http://www.catb.org/esr/structure-packing/
  [17-12]: https://proprogramming.org/some-unknown-features-or-tricks-in-c-language/
  [17-11]: https://computing.llnl.gov/tutorials/mpi/
  [17-10]: https://web.archive.org/web/20170620131430/https://www.tedunangst.com/flak/post/memcpy-vs-memmove
  [17-9]: https://computing.llnl.gov/tutorials/openMP/
  [17-8]: https://www.youtube.com/playlist?list=PLLX-Q6B8xqZ8n8bwjGdzBJ25X2utwnoEG
  [17-7]: https://blog.noctua-software.com/c-tricks.html
  [17-6]: https://blogs.oracle.com/linux/8-gdb-tricks-you-should-know-v2
  [17-5]: https://hintjens.gitbooks.io/scalable-c/content/index.html
  [17-4]: https://nullprogram.com/blog/2017/03/30
  [17-3]: https://nullprogram.com/blog/2015/02/17
  [17-2]: https://jvns.ca/blog/2014/12/14/fun-with-threads/
  [17-1]: http://mpitutorial.com/
</details>

<a id="advanced-level"></a>
<details>
  <summary>Advanced Level</summary>

  ##### <a href="#-">`^`</a> Advanced Level #####
  * [Advanced metaprogramming in C][18-1]
  * [Quick tutorial on implementing and debugging malloc, free, calloc, and realloc][18-2]
  * [Bit twiddling hacks][18-3]
  * [I do not know C][18-4]
  * [Implementing smart pointers for the C programming language][18-5]
  * [Inline functions in C][18-6]
  * [Metaprogramming custom control structures in C][18-7]
  * [Some dark corners of C][18-8] (Presentation)
  * [Writing efficient C and C code optimization][18-9]
  * [What every programmer should know about memory][18-10] (PDF)
  * [Learn libuv][18-11]
  * [Let's build a compiler][18-12]
  * [Write a compiler][18-13]

  [18-13]: https://norasandler.com/2017/11/29/Write-a-Compiler.html
  [18-12]: https://compilers.iecc.com/crenshaw/
  [18-11]: http://thlorenz.com/learnuv/book/
  [18-10]: https://www.akkadia.org/drepper/cpumemory.pdf
  [18-9]: https://www.codeproject.com/articles/6154/writing-efficient-c-and-c-code-optimization
  [18-8]: https://docs.google.com/presentation/d/1h49gY3TSiayLMXYmRMaAEMl05FaJ-Z6jDOWOz3EsqqQ/edit?pli=1#slide=id.gaf50702c_0153
  [18-7]: https://www.chiark.greenend.org.uk/~sgtatham/mp/
  [18-6]: http://www.greenend.org.uk/rjk/tech/inline.html
  [18-5]: https://snai.pe/c/c-smart-pointers/
  [18-4]: https://kukuruku.co/post/i-do-not-know-c/
  [18-3]: https://graphics.stanford.edu/~seander/bithacks.html
  [18-2]: http://danluu.com/malloc-tutorial/
  [18-1]: http://250bpm.com/blog:56
</details>

<a id="code-examples"></a>
#### Code Examples ####

<a id="operating-systems"></a>
<details>
  <summary>Operating Systems</summary>

  ##### <a href="#-">`^`</a> Operating Systems #####
  * [Plan 9][19-1] - OS from Bell Labs.
  * [ChibiOS][19-2] - RTOS with development environment.
  * [EtchedPixels/FUZIX][19-3] - Superior rehaul of UZI.
  * [Harvey-OS/harvey][19-4] - An OS based on Plan 9.
  * [SilverRainZ/OS67][19-5] - An Unix-like toy kernel.
  * [RIOT-OS/RIOT][19-6] - OS for IoT.
  * [arjun024/mkernel][19-7] - Very basic kernel.
  * [Stichting-MINIX-Research-Foundation/minix][19-8] - MINIX3.
  * [guilleiguaran/xv6][19-9] - Mirror for Xv6 operating system.
  * [raphydaphy/Q-Operating-System][19-10] - Ambitious and abandoned OS designed
  for 64-bit CPUs.
  * [seL4/seL4][19-11] - Microkernel aimed to be secure and correct.
  * [klange/toaruos][19-12] - Desktop OS with userspace, written from scratch.
  * [nickbjohnson4224/rhombus][19-13] - OS with libc and some drivers ready.
  * [rswier/swieros][19-14] - Kernel, compiler and userland.
  * [jbangert/trapcc][19-15] - Example of using Intel instruction execution
  gimick.
  * [mbedmicro/mbed][19-16] - OS for ARM Cortex-M.

  [19-16]: https://github.com/ARMmbed/mbed-os
  [19-15]: https://github.com/jbangert/trapcc
  [19-14]: https://github.com/rswier/swieros
  [19-13]: https://github.com/nickbjohnson4224/rhombus
  [19-12]: https://github.com/klange/toaruos
  [19-11]: https://github.com/seL4/seL4
  [19-10]: https://github.com/raphydaphy/Q-Operating-System
  [19-9]: https://github.com/guilleiguaran/xv6
  [19-8]: https://github.com/Stichting-MINIX-Research-Foundation/minix
  [19-7]: https://github.com/arjun024/mkernel
  [19-6]: https://github.com/RIOT-OS/RIOT
  [19-5]: https://github.com/SilverRainZ/OS67
  [19-4]: https://github.com/Harvey-OS/harvey
  [19-3]: https://github.com/EtchedPixels/FUZIX
  [19-2]: https://github.com/ChibiOS/ChibiOS
  [19-1]: https://9p.io/plan9/index.html
</details>

<a id="emulators-vms"></a>
<details>
  <summary>Emulators, VMs</summary>

  ##### <a href="#-">`^`</a> Emulators, VMs #####
  * [CTurt/Cinoop][20-1] - Multiplatform Game Boy emulator.
  * [LIJI32/SameBoy][20-2] - Game Boy and Game Boy Color emulator written in C.
  * [MoarVM][20-3] - A VM with adaptive optimization and JIT compilation, built
  for Rakudo Perl 6.
  * [felixangell/mac][20-4] - Virtual machine in c.
  * [jakogut/tinyvm][20-5] - TinyVM is a small, fast, lightweight virtual
  machine written in pure ANSI C.
  * [rsms/sol][20-6] - A sunny little virtual machine.
  * [mgba][20-7] - mGBA Game Boy Advance Emulator.
  * [tekknolagi/carp][20-8] - Well documented VM written from scratch.
  * [reicast/reicast-emulator][20-9] - Multiplatform Sega Dreamcast emulator.
  * [haldean/x6502][20-10] - 6502 emulator that one day dreams of being an
  Atari 2600.
  * [n64dev/cen64][20-11] - Cycle-Accurate Nintendo 64 Emulator.
  * [wkoszek/cpu60][20-12] - Example of CPU simulation in software.
  * [swetland/dcpu16][20-13] - Virtual Machine and Assembler for Notch's DCPU-16
  Architecture.
  * [AlexAltea/orbital][20-14] - PS4 emulator.

  [20-14]: https://github.com/AlexAltea/orbital
  [20-13]: https://github.com/swetland/dcpu16
  [20-12]: https://github.com/wkoszek/cpu60
  [20-11]: https://github.com/n64dev/cen64
  [20-10]: https://github.com/haldean/x6502
  [20-9]: https://github.com/reicast/reicast-emulator
  [20-8]: https://github.com/tekknolagi/carp
  [20-7]: https://github.com/mgba-emu/mgba
  [20-6]: https://github.com/rsms/sol
  [20-5]: https://github.com/jakogut/tinyvm
  [20-4]: https://github.com/felixangell/mac
  [20-3]: https://github.com/MoarVM/MoarVM
  [20-2]: https://github.com/LIJI32/SameBoy
  [20-1]: https://github.com/CTurt/Cinoop
</details>

<a id="windowing-graphics"></a>
<details>
  <summary>UI, Windowing, Graphics</summary>

  ##### <a href="#-">`^`</a> UI, Windowing, Graphics #####
  * [LemonBoy/bar][21-1] - A featherweight bar based on xcb.
  * [HarveyHunt/howm][21-2] - A lightweight, X11 tiling window manager that
  behaves like vim.
  * [chneukirchen/cwm][21-3] - portable version of OpenBSD's cwm(1) window
  manager.
  * [mil/foo-wm][21-4] - A minimal window manager that organizes windows in a
  tree data structure, provides a socket to send commands to, and nothing more.
  * [pyknite/catwm][21-5] - catwm is a very simple tiling window manager.
  * [jordansissel/xdotool][21-6] - fake keyboard/mouse input, window management,
  and more.
  * [muennich/sxiv][21-7] - Simple X Image Viewer.
  * [island-org/island][21-8] - Lightweight and low-level creative coding
  toolkits in C.
  * [robm/dzen][21-9] - Dzen is a general purpose messaging, notification and
  menuing program for X11.
  * [McNopper/OpenGL][21-10] - OpenGL 3 and 4 with GLSL.

  [21-10]: https://github.com/McNopper/OpenGL
  [21-9]: https://github.com/robm/dzen
  [21-8]: https://github.com/island-org/island
  [21-7]: https://github.com/muennich/sxiv
  [21-6]: https://github.com/jordansissel/xdotool
  [21-5]: https://github.com/pyknite/catwm
  [21-4]: https://github.com/mil/foo-wm
  [21-3]: https://github.com/chneukirchen/cwm
  [21-2]: https://github.com/HarveyHunt/howm
  [21-1]: https://github.com/LemonBoy/bar
</details>

<a id="language-implementations"></a>
<details>
  <summary>Language Implementations</summary>

  ##### <a href="#-">`^`</a> Language Implementations #####
  * [Fedjmike/mini-c][22-1] - Dr Strangehack, or: how to write a self-hosting C
  compiler in 10 hours.
  * [HuoLanguage/huo][22-2] - Interpreted language written in C.
  * [Wilfred/babyc][22-3] - A toy C compiler.
  * [dimkr/szl][22-4] - A lightweight, embeddable scripting language.
  * [espruino/Espruino][22-5] - The Espruino JavaScript interpreter.
  * [fabianishere/brainfuck][22-6] - Brainfuck interpreter written in C.
  * [feeley/gambit][22-7] - Gambit is an efficient implementation of the Scheme
  programming language.
  * [wren-lang/wren][22-8] - The Wren Programming Language.
  * [cksystemsteaching/selfie][22-9] - An educational software system of a tiny
  self-compiling C compiler, a tiny self-executing RISC-V emulator, and a tiny
  self-hosting RISC-V hypervisor.
  * [darius/ichbins][22-10] - A tiny self-hosting Lisp-to-C compiler.
  * [fragglet/yoctolisp][22-11] - Tiny Scheme-like Lisp interpreter written in
  a weekend.
  * [marcobambini/gravity][22-12] - Gravity Programming Language.
  * [justinmeza/lci][22-13] - A LOLCODE interpreter written in C.
  * [mruby/mruby][22-14] - Lightweight Ruby.
  * [stevedekorte/io][22-15] - Io programming language.
  * [philburk/pforth][22-16] - Portable Forth in C.
  * [carld/micro-lisp][22-17] - A very small Lisp programming language that used
  to be under 200 lines of C.
  * [kevinlawler/kona][22-18] - Open-source implementation of the K programming
  language.
  * [ndreynolds/flathead][22-19] - A toy JavaScript interpreter written in C.
  * [bl0ckeduser/new-bpf-tools][22-20] - Subset-of-C compiler targeting 32-bit
  x86.
  * [intellectualheaven/ceed][22-21] - A tiny x86 compiler with ELF and PE
  target.
  * [janet-lang/janet][22-22] - A dynamic language and bytecode vm.
  * [jnz/q3vm][22-23] - Q3VM - Embeddable bytecode virtual machine/interpreter
  for C-language input.
  * [tj/luna][22-24] - luna programming language - a small, elegant VM
  implemented in C.
  * [rui314/minilisp][22-25] - A readable lisp in less than 1k lines of C.
  * [rebol/rebol][22-26] - Source code for the Rebol interpreter.
  * [mortdeus/legacy-cc][22-27] - The earliest versions of the very first c
  compiler known to exist in the wild written by the late legend himself dmr.
  * [paladin-t/my_basic][22-28] - Lightweight BASIC interpreter written in
  standard C in dual files. Aimed to be embeddable, extendable and portable.
  * [pikelang/Pike][22-29] - Pike is a dynamic programming language with a
  syntax similar to Java and C. It is simple to learn, does not require long
  compilation passes and has powerful built-in data types allowing simple and
  really fast data manipulation.
  * [riolet/rix][22-30] - Rix language combines the power of C language and the
  convenience of a high level language.
  * [lotabout/write-a-C-interpreter][22-31] - Write a simple interpreter of C.
  Inspired by c4 and largely based on it.
  * [nickdesaulniers/bf_interpreter_jit_compiler][22-32] - Teach myself about
  interpreters, JITs, and compilers using the Brainfuck language as the toy
  language.
  * [skx/simple.vm][22-33] - Simple virtual machine which inteprets bytecode.

  [22-33]: https://github.com/skx/simple.vm
  [22-32]: https://github.com/nickdesaulniers/bf_interpreter_jit_compiler
  [22-31]: https://github.com/lotabout/write-a-C-interpreter
  [22-30]: https://github.com/riolet/rix
  [22-29]: https://github.com/pikelang/Pike
  [22-28]: https://github.com/paladin-t/my_basic
  [22-27]: https://github.com/mortdeus/legacy-cc
  [22-26]: https://github.com/rebol/rebol
  [22-25]: https://github.com/rui314/minilisp
  [22-24]: https://github.com/tj/luna
  [22-23]: https://github.com/jnz/q3vm
  [22-22]: https://github.com/janet-lang/janet
  [22-21]: https://github.com/intellectualheaven/ceed
  [22-20]: https://github.com/bl0ckeduser/new-bpf-tools
  [22-19]: https://github.com/ndreynolds/flathead
  [22-18]: https://github.com/kevinlawler/kona
  [22-17]: https://github.com/carld/micro-lisp
  [22-16]: https://github.com/philburk/pforth
  [22-15]: https://github.com/stevedekorte/io
  [22-14]: https://github.com/mruby/mruby
  [22-13]: https://github.com/justinmeza/lci
  [22-12]: https://github.com/marcobambini/gravity
  [22-11]: https://github.com/fragglet/yoctolisp
  [22-10]: https://github.com/darius/ichbins
  [22-9]: https://github.com/cksystemsteaching/selfie
  [22-8]: https://github.com/wren-lang/wren
  [22-7]: https://github.com/feeley/gambit
  [22-6]: https://github.com/fabianishere/brainfuck
  [22-5]: https://github.com/espruino/Espruino
  [22-4]: https://github.com/dimkr/szl
  [22-3]: https://github.com/Wilfred/babyc
  [22-2]: https://github.com/HuoLanguage/huo
  [22-1]: https://github.com/Fedjmike/mini-c
</details>

<a id="challenges"></a>
<details>
  <summary>Challenges</summary>

  ##### <a href="#-">`^`</a> Challenges #####
  * [trailofbits/cb-multios][23-1] - DARPA Challenges Sets for Linux, Windows,
  and macOS.
  * [FreddieV4/DailyProgrammerChallenges][23-2] - External Repo of Challenges
  from r/dailyprogrammer.
  * [Coderbyte challenges][23-3]
  * [Project Euler][23-4]
  * [HackerRank][23-5]
  * [CodeChef][23-6]
  * [CodeWars][23-7]
  * [Codingame][23-8]
  * [/r/DailyProgrammer][23-9]
  * [leetcode][23-10]
  * [eatnumber1/goal][23-11] - g()()()()('al') → "gooooal"

  [23-11]: https://github.com/eatnumber1/goal
  [23-10]: https://leetcode.com/problemset/algorithms/
  [23-9]: https://old.reddit.com/r/dailyprogrammer/
  [23-8]: https://www.codingame.com
  [23-7]: https://www.codewars.com
  [23-6]: https://www.codechef.com/
  [23-5]: https://www.hackerrank.com
  [23-4]: https://projecteuler.net/
  [23-3]: https://www.coderbyte.com/challenges
  [23-2]: https://github.com/FreddieV4/DailyProgrammerChallenges
  [23-1]: https://github.com/trailofbits/cb-multios
</details>

<a id="other-examples"></a>
<details>
  <summary>Other Examples</summary>

  ##### <a href="#-">`^`</a> Other Examples #####
  * [MinhasKamal/CreepyCodeCollection][24-1] - A Nonsense Collection of
  Disgusting Codes.
  * [Visgean/Zeus][24-2] - Zeus trojan horse - leaked in 2011.
  * [andreafabrizi/prism][24-3] - PRISM is an user space stealth reverse shell
  backdoor, written in pure C.
  * [brenns10/lsh][24-4] - Simple shell implementation.
  * [jeff-1amstudios/restful-doom][24-5] - HTTP+JSON API hosted inside the 1993
  DOOM engine!
  * [chelyaev/ffmpeg-tutorial][24-6] - A set of tutorials that demonstrates how
  to write a video player based on FFmpeg.
  * [rcr/rirc][24-7] - A terminal IRC client in C.
  * [xoreaxeaxeax/movfuscator][24-8] - The single instruction C compiler.
  * [deadbits/InsecureProgramming][24-9] - Mirror of insecure programming
  examples.
  * [irssi/irssi][24-10] - The client of the future.
  * [xorg62/tty-clock][24-11] - Clock using lib ncurses.
  * [vanhauser-thc/thc-hydra][24-12] - Hydra.
  * [posva/catimg][24-13] - Fast image printing in your terminal.
  * [pkieltyka/stash][24-14] - Steganography application that hides data within
  a bitmap image.
  * [regehr/ub-canaries][24-15] - Collection of C/C++ programs that try to get
  compilers to exploit undefined behavior.
  * [tnightingale/DTE][24-16] - Dumb Terminal Emulator - Data Comm, COMP 3980.

  [24-16]: https://github.com/tnightingale/DTE
  [24-15]: https://github.com/regehr/ub-canaries
  [24-14]: https://github.com/pkieltyka/stash
  [24-13]: https://github.com/posva/catimg
  [24-12]: https://github.com/vanhauser-thc/thc-hydra
  [24-11]: https://github.com/xorg62/tty-clock
  [24-10]: https://github.com/irssi/irssi
  [24-9]: https://github.com/deadbits/InsecureProgramming
  [24-8]: https://github.com/xoreaxeaxeax/movfuscator
  [24-7]: https://github.com/rcr/rirc
  [24-6]: https://github.com/chelyaev/ffmpeg-tutorial
  [24-5]: https://github.com/jeff-1amstudios/restful-doom
  [24-4]: https://github.com/brenns10/lsh
  [24-3]: https://github.com/andreafabrizi/prism
  [24-2]: https://github.com/Visgean/Zeus
  [24-1]: https://github.com/MinhasKamal/CreepyCodeCollection
</details>

--------------------------------------------------------------------------------

<a id="ai"></a>
<details>
  <summary>AI</summary>

  ## <a href="#-">`^`</a> AI ##
  Neural nets, machine learning, pattern recognition etc.
  * [cjac/cmusphinx][25-20] - CMU Sphinx - Speech Recognition Toolkit. [`Licenses`][25-21]
  * [100/Cranium][25-4] - A portable, header-only, artificial neural network
  library written in C99. [`MIT`][25-5]
  * [pjreddie/darknet][25-42] - Convolutional Neural Networks. [`License`][25-43]
  * [TheWeatherChannel/dClass][25-16] - Device Classification Engine. [`Apache 2`][25-17]
  * [2hanson/DecisionTree][25-6] - Decision Tree. [`MIT`][25-7]
  * [yusugomori/DeepLearning][25-40] - Deep Learning (several languages, C
  included). [`MIT`][25-41]
  * [encog/encog-c][25-27] - C implementation of Encog - machine learning
  framework for Java/C#. `No license`
  * [codeplea/genann][25-24] - simple neural network library in ANSI C. [`Zlib`][25-25]
  * [attractivechaos/kann][25-1] - Two-file ANN library. [`MIT`][25-2]
  * [Blei-Lab/lda-c][25-8] - This is a C implementation of variational EM for
  latent Dirichlet allocation (LDA), a topic model for text or other discrete
  data. [`LGPL 2.1`][25-9]
  * [jppbsi/LibDEEP][25-3] - Deep learning library. `No license`
  * [H2CO3/libsprec][25-12] - C library for speech recognition using the Google
  Speech API. [`License`][25-13]
  * [robwhess/opensift][25-32] - Open-Source SIFT Library. [`License`][25-33]
  * [dake/openVP][25-26] - Voice Print Recognition in C language. `No license`
  * [cmusphinx/pocketsphinx][25-22] - Lightweight speech recognition engine,
  specifically tuned for handheld and mobile devices, though it works equally
  well on the desktop. [`BSD 2-Clause`][25-23]
  * [HIPS/Probabilistic-Backpropagation][25-14] - Implementation in C and Theano
  of the method Probabilistic Backpropagation for scalable Bayesian inference in
  deep neural networks. [`BSD 3-Clause`][25-15]
  * [GHamrouni/Recommender][25-10] - A C library for product
  recommendations/suggestions using collaborative filtering (CF). [`BSD 2-Clause`][25-11]
  * [ufoym/recursive-bf][25-34] - A lightweight library for recursive bilateral
  filtering. [`MIT`][25-35]
  * [xiph/rnnoise][25-38] - Recurrent neural network for audio noise reduction. [`License`][25-39]
  * [antirez/shapeme][25-18] - Evolve images using simulated annealing. [`BSD 2-Clause`][25-19]
  * [symisc/sod][25-36] - An Embedded Computer Vision & Machine Learning Library
  (CPU Optimized & IoT Capable). [`GPL 3`][25-37]
  * [iunderstand/SWE][25-30] - Learning Semantic Word Embeddings based on
  Ordinal Knowledge Constraints. [`Apache 2`][25-31]
  * [glouw/tinn][25-28] - The tiny neural network library. [`MIT`][25-29]

  [25-43]: https://github.com/pjreddie/darknet/blob/master/LICENSE
  [25-42]: https://github.com/pjreddie/darknet
  [25-41]: https://github.com/yusugomori/DeepLearning/blob/master/LICENSE.txt
  [25-40]: https://github.com/yusugomori/DeepLearning
  [25-39]: https://github.com/xiph/rnnoise/blob/master/COPYING
  [25-38]: https://github.com/xiph/rnnoise
  [25-37]: https://github.com/symisc/sod/blob/master/LICENSE
  [25-36]: https://github.com/symisc/sod
  [25-35]: https://github.com/ufoym/recursive-bf/blob/master/LICENSE
  [25-34]: https://github.com/ufoym/recursive-bf
  [25-33]: https://github.com/robwhess/opensift/blob/master/LICENSE
  [25-32]: https://github.com/robwhess/opensift
  [25-31]: https://github.com/iunderstand/SWE/blob/master/LICENSE
  [25-30]: https://github.com/iunderstand/SWE
  [25-29]: https://github.com/glouw/tinn/blob/master/LICENSE
  [25-28]: https://github.com/glouw/tinn
  [25-27]: https://github.com/encog/encog-c
  [25-26]: https://github.com/dake/openVP
  [25-25]: https://github.com/codeplea/genann/blob/master/LICENSE
  [25-24]: https://github.com/codeplea/genann
  [25-23]: https://github.com/cmusphinx/pocketsphinx/blob/master/LICENSE
  [25-22]: https://github.com/cmusphinx/pocketsphinx
  [25-21]: https://github.com/cjac/cmusphinx
  [25-20]: https://github.com/cjac/cmusphinx
  [25-19]: https://github.com/antirez/shapeme/blob/master/LICENSE
  [25-18]: https://github.com/antirez/shapeme
  [25-17]: https://github.com/TheWeatherChannel/dClass/blob/master/LICENSE
  [25-16]: https://github.com/TheWeatherChannel/dClass
  [25-15]: https://github.com/HIPS/Probabilistic-Backpropagation/blob/master/LICENSE
  [25-14]: https://github.com/HIPS/Probabilistic-Backpropagation
  [25-13]: https://github.com/H2CO3/libsprec/blob/master/LICENSE
  [25-12]: https://github.com/H2CO3/libsprec
  [25-11]: https://github.com/GHamrouni/Recommender/blob/master/LICENSE
  [25-10]: https://github.com/GHamrouni/Recommender
  [25-9]: https://github.com/blei-lab/lda-c/blob/master/license.txt
  [25-8]: https://github.com/Blei-Lab/lda-c
  [25-7]: https://github.com/2hanson/DecisionTree
  [25-6]: https://github.com/2hanson/DecisionTree
  [25-5]: https://github.com/100/Cranium/blob/master/LICENSE
  [25-4]: https://github.com/100/Cranium
  [25-3]: https://github.com/jppbsi/LibDEEP/wiki
  [25-2]: https://github.com/attractivechaos/kann/blob/master/LICENSE.txt
  [25-1]: https://github.com/attractivechaos/kann
</details>

<a id="algoritm-implementations"></a>
<details>
  <summary>Algoritm Implementations</summary>

  ## <a href="#-">`^`</a> Algoritm Implementations ##
  Some generic agoritms or ones with no specific attachments.
  * [dhuertas/AES][26-28] - AES algorithm implementation in C. `No license`
  * [mischasan/aho-corasick][26-40] - A-C implementation in "C". Tight-packed
  (interleaved) state-transition matrix. [`LGPL 3`][26-41]
  * [davidreynolds/algorithms][26-27] - A repository of assorted algorithms and
  data structures. `No license`
  * [BigZaphod/AStar][26-5] - C Implementation of the A\* Pathfinding Algorithm. [`License`][26-6]
  * [citiususc/BigBWA][26-25] - Approaching the Burrows-Wheeler Aligner to Big
  Data Technologies. [`GPL 3`][26-26]
  * [TheAlgorithms/C][26-17] - All Algorithms implemented in C `No license`
  * [chaoslawful/ccard-lib][26-24] - C library for estimating cardinality in
  streams for which it is infeasible to store all events in memory. `No license`
  * [agl/curve25519-donna][26-18] - Implementations of a fast Elliptic-curve
  Diffie-Hellman primitive. [`License`][26-19]
  * [aimxhaisse/des][26-22] - C implementation of DES. [`License`][26-23]
  * [tarequeh/DES][26-49] - Implementation of Data Encryption Standard in C. [`MIT`][26-50]
  * [blynn/dlx][26-3] - Implementation of Knuth's Algorithm X, with example
  solvers. [`GPL 3`][26-4]
  * [oap/ekf-angles][26-44] - Extended Kalman Filter for Accelerometer and Gyro
  data. `No license`
  * [Cyan4973/FiniteStateEntropy][26-13] - Finite State Entropy and Huff0. [`BSD 2-Clause`][26-14]
  * [BlackLight/fkmeans][26-9] - A tiny library in C for managing kmeans
  clusterization algorithm over arbitrary data sets, both by manually specifying
  the number k of clusters and computing it automatically using Schwarz
  criterion. [`GPL 3`][26-10]
  * [kljensen/Gemoda][26-32] - A generic motif discovery algorithm for
  sequential data. [`GPL 2`][26-33]
  * [lacker/ikalman][26-38] - An iPhone-friendly Kalman filter written in C. [`MIT`][26-39]
  * [tsuraan/Jerasure][26-51] - C Implementation of Reed-Solomon coding. [`License`][26-52]
  * [jmcejuela/Levenshtein-MySQL-UDF][26-30] - General Levenshtein algorithm and
  k-bounded levenshtein distance in linear time and constant space. [`LGPL 3`][26-31]
  * [CVLearner/Mixture-of-Gaussians][26-11] - Fit a Gaussian mixture model given
  a set of data. [`MIT`][26-12]
  * [richarddurbin/pbwt][26-47] - Implementation of Positional Burrows-Wheeler
  Transform for genetic data. [`License`][26-48]
  * [ntamas/plfit][26-45] - Fitting power-law distributions to empirical data,
  according to the method of Clauset, Shalizi and Newman. [`License`][26-46]
  * [Kevincav/Radix-Sort][26-15] - Radix Sort with different data types. [`MIT`][26-16]
  * [duckythescientist/obfuscatedLife][26-29] - Conway's Game of Life in 9 lines
  of C. `No license`
  * [kokke/tiny-AES-c][26-34] - Small portable AES128/192/256 in C. [`Unlicense`][26-35]
  * [kroitor/gjk.c][26-36] - Gilbert-Johnson-Keerthi (GJK) collision detection
  algorithm in 200 lines of clean plain C. [`WTFPL`][26-37]
  * [ai-ku/scode][26-20] - Sphere embedding (s-code) is a variation of Euclidean
  embedding of co-occurence data (code). [`MIT`][26-21]
  * [swenson/sort][26-1] - Collection of sorting routines, which type-specialize
  at compile-time with a user-defined type. [`MIT`][26-2]
  * [msteinbeck/tinyspline][26-42] - ANSI C library for NURBS, B-Splines, and
  Bézier curves with interfaces for C++, C#, D, Java, Lua, Octave, PHP, Python,
  R, and Ruby. [`MIT`][26-43]
  * [ferreiradaselva/uastar][26-7] - Minimal A\* implementation. [`Zlib`][26-8]

  [26-52]: https://github.com/tsuraan/Jerasure/blob/master/License.txt
  [26-51]: https://github.com/tsuraan/Jerasure
  [26-50]: https://github.com/tarequeh/DES/blob/master/LICENSE
  [26-49]: https://github.com/tarequeh/DES
  [26-48]: https://github.com/richarddurbin/pbwt/blob/master/utils.c
  [26-47]: https://github.com/richarddurbin
  [26-46]: https://github.com/ntamas/plfit/blob/master/src/main.c
  [26-45]: https://github.com/ntamas/plfit
  [26-44]: https://github.com/oap/ekf-angles
  [26-43]: https://github.com/msteinbeck/tinyspline/blob/master/LICENSE
  [26-42]: https://github.com/msteinbeck/tinyspline
  [26-41]: https://github.com/mischasan/aho-corasick/blob/master/LICENSE
  [26-40]: https://github.com/mischasan/aho-corasick
  [26-39]: https://github.com/lacker/ikalman/blob/master/LICENSE
  [26-38]: https://github.com/lacker/ikalman
  [26-37]: https://github.com/kroitor/gjk.c/blob/master/LICENSE.txt
  [26-36]: https://github.com/kroitor/gjk.c
  [26-35]: https://github.com/kokke/tiny-AES-c/blob/master/unlicense.txt
  [26-34]: https://github.com/kokke/tiny-AES-c
  [26-33]: https://github.com/kljensen/Gemoda/blob/master/COPYING
  [26-32]: https://github.com/kljensen/Gemoda
  [26-31]: https://github.com/juanmirocks/Levenshtein-MySQL-UDF/blob/master/LICENSE
  [26-30]: https://github.com/jmcejuela/Levenshtein-MySQL-UDF
  [26-29]: https://github.com/duckythescientist/obfuscatedLife
  [26-28]: https://github.com/dhuertas/AES
  [26-27]: https://github.com/davidreynolds/algorithms
  [26-26]: https://github.com/citiususc/BigBWA/blob/master/LICENSE
  [26-25]: https://github.com/citiususc/BigBWA
  [26-24]: https://github.com/chaoslawful/ccard-lib
  [26-23]: https://github.com/aimxhaisse/des#license
  [26-22]: https://github.com/aimxhaisse/des
  [26-21]: https://github.com/ai-ku/scode/blob/master/LICENSE
  [26-20]: https://github.com/ai-ku/scode
  [26-19]: https://github.com/agl/curve25519-donna/blob/master/LICENSE.md
  [26-18]: https://github.com/agl/curve25519-donna
  [26-17]: https://github.com/TheAlgorithms/C
  [26-16]: https://github.com/Kevincav/Radix-Sort/blob/master/LICENSE.txt
  [26-15]: https://github.com/Kevincav/Radix-Sort
  [26-14]: https://github.com/Cyan4973/FiniteStateEntropy/blob/dev/LICENSE
  [26-13]: https://github.com/Cyan4973/FiniteStateEntropy
  [26-12]: https://github.com/CVLearner/Mixture-of-Gaussians/blob/master/LICENSE
  [26-11]: https://github.com/CVLearner/Mixture-of-Gaussians
  [26-10]: https://github.com/BlackLight/fkmeans/blob/master/kmeans.h
  [26-9]: https://github.com/BlackLight/fkmeans
  [26-8]: https://github.com/felselva/uastar#license
  [26-7]: https://github.com/felselva/uastar
  [26-6]: https://github.com/BigZaphod/AStar/blob/master/AStar.h
  [26-5]: https://github.com/BigZaphod/AStar
  [26-4]: https://github.com/blynn/dlx/blob/master/COPYING
  [26-3]: https://github.com/blynn/dlx
  [26-2]: https://github.com/swenson/sort/blob/master/LICENSE.md
  [26-1]: https://github.com/swenson/sort
</details>

<a id="argument-parsing"></a>
<details>
  <summary>Argument Parsing</summary>

  ## <a href="#-">`^`</a> Argument Parsing ##
  * [cofyc/argparse][27-9] - Command-line arguments parsing library. [`MIT`][27-10]
  * [clibs/commander][27-7] - Commander option parser ported to C - simple API,
  auto-generated --help. [`MIT`][27-8]
  * [docopt/docopt.c][27-3] - Implementation of a command-line option parser. [`MIT`][27-4]
  * [clibs/flag][27-5] - Go-style flag parsing for C. [`MIT`][27-6]
  * [jibsen/parg][27-1] - A single-file reimplementation of getopt with better
  defaults. [`License`][27-2]

  [27-10]: https://github.com/cofyc/argparse/blob/master/LICENSE
  [27-9]: https://github.com/cofyc/argparse
  [27-8]: https://github.com/clibs/commander#license
  [27-7]: https://github.com/clibs/commander
  [27-6]: https://github.com/clibs/flag/blob/master/LICENSE
  [27-5]: https://github.com/clibs/flag
  [27-4]: https://github.com/docopt/docopt.c/blob/master/LICENSE-MIT
  [27-3]: https://github.com/docopt/docopt.c
  [27-2]: https://github.com/jibsen/parg/blob/master/COPYING
  [27-1]: https://github.com/jibsen/parg
</details>

<a id="calculations"></a>
<details>
  <summary>Calculations and Math</summary>

  ## <a href="#-">`^`</a> Calculations and Math ##
  * [b-k/apophenia][28-3] - Library for statistical and scientific computing. [`GPL 2`][28-4]
  * [fredrik-johansson/arb][28-1] - Library for arbitrary-precision interval
  arithmetic. [`LGPL 2.1`][28-2]
  * [ATLAS][28-5] - Automatically Tuned Linear Algebra Software. [`License`][28-6]
  * [BLAS][28-7] - Basic Linear Algebra Subprograms; a set of routines that
  provide vector and matrix operations. [`License`][28-8]
  * [Lichtso/CCWT][28-54] - Complex Continuous Wavelet Transformation. [`MIT`][28-55]
  * [CDFLIB][28-11] - Library with routines to evaluate cumulative density
  functions for a variety of standard probability distributions.
  Also can compute one parameter of the CDF given the others. `No license`
  * [ScientificC/cmathl][28-12] - Pure-C Math library with a great variety of
  mathematical functions and CMake build support. Seeks to be close to C89/C90
  compliant for portability. [`MIT`][28-13]
  * [Cuba][28-14] - Library for multidimensional numerical integration. [`LGPL`][28-15]
  * [adis300/fft-c][28-16] - A high-performance Fourier Transform from netlib's
  fftpack; wrapped in a user-friendly format. [`MIT`][28-17]
  * [FFTW][28-18] - The Fastest Fourier Transform in the West; a
  highly-optimized fast Fourier transform routine. [`GPL 2`][28-19]
  * [FLINT][28-20] - Fast Library for Number Theory; a library supporting
  arithmetic with numbers, polynomials, power series and matrices, among others. [`LGPL 2.1`][28-21]
  * [gjrand][28-48] - Library of random-number generation routines. [`GPL 2`][28-49]
  * [GLPK][28-22] - GNU Linear Programming Kit; a package designed for solving
  large-scale linear programming, mixed integer programming and other related
  problems. [`GPL 3`][28-23]
  * [GMP][28-24] - GNU Multple Precision Arithmetic Library; a library for
  arbitrary-precision arithmetic. [`Licenses`][28-25]
  * [GNU MPC][28-26] - Library for complex number arithmetic. [`LGPL 3`][28-27]
  * [GNU MPFR][28-28] - Library for arbitrary-precision floating-point
  arithmetic. [`LGPL 3`][28-29]
  * [GNU MPRIA][28-30] - Portable mathematics library for multi-precision
  rational interval arithmetic. [`GPL 3`][28-31]
  * [GSL][28-32] - The GNU Scientific Library; a sophisticated numerical
  library. [`GPL3`][28-33]
  * [HdrHistogram/HdrHistogram_c][28-50] - C port of the HdrHistogram. [`License`][28-51]
  * [igraph][28-34]- Library for creating and manipulating large graphs. [`GPL2`][28-35]
  * [KISS FFT][28-36] - Very simple fast Fourier transform library. [`BSD`][28-37]
  * [LAPACKE][28-38] - C interface to LAPACK. [`License`][28-39]
  * [PARI/GP][28-40] - Computer algebra system for number theory; includes a
  compiler to C. [`GLP`][28-41]
  * [PETSc][28-42] - Suite of data structures and routines for scalable parallel
  solution of scientific applications modelled by partial differential
  equations. [`License`][28-43]
  * [PROB][28-44] - Library that handles various discrete and continuous
  probability density functions. [`LGPL 3`][28-45]
  * [PetteriAimonen/libfixmatrix][28-69] - C library for fixed point matrix,
  quaternion and vector calculations. [`MIT`][28-70]
  * [canonizer/libgpuvm][28-56] - library which simplifies host-GPU data
  transfer using userspace pagefault handling. `No license`
  * [libtom/libtommath][28-65] - LibTomMath is a free open source portable
  number theoretic multiple-precision integer library written entirely in C. [`Unlicense`][28-66]
  * [JuliaMath/openlibm][28-52] - High quality system independent, portable,
  open source libm implementation. [`License`][28-53]
  * [imneme/pcg-c][28-63] - PCG — C Implementation. [`Apache 2`][28-64]
  * [imneme/pcg-c-basic][28-61] - PCG — Minimal C Implementation. [`Apache 2`][28-62]
  * [libtom/tomsfastmath][28-67] - TomsFastMath is a fast public domain, open
  source, large integer arithmetic library written in portable ISO C. [`Licenses`][28-68]
  * [cvxgrp/scs][28-71] - C package that solves convex cone problems via
  operator splitting. [`MIT`][28-72]
  * [SLEPc][28-9] - Library for the solution of large, sparse eigenvalue
  problems on parallel computers. [`BSD 2-Clause`][28-10]
  * [slim-curve/slim-curve][28-73] - SLIM Curve: a package for exponential curve
  fitting of combined spectral lifetime image data. [`GPL 3`][28-73]
  * [tinyexpr][28-75] - Tiny recursive-descent parser, compiler and evaluation
  engine for simple mathematical expressions. [`Zlib`][28-76]
  * [Yeppp!][28-46] - Very fast, SIMD-optimized mathematical library. [`License`][28-47]

  [28-76]: https://github.com/codeplea/tinyexpr/blob/master/LICENSE
  [28-75]: https://github.com/codeplea/tinyexpr
  [28-74]: https://github.com/slim-curve/slim-curve/blob/master/LICENSE.txt
  [28-73]: https://github.com/slim-curve/slim-curve
  [28-72]: https://github.com/cvxgrp/scs/blob/master/LICENSE.txt
  [28-71]: https://github.com/cvxgrp/scs
  [28-70]: https://github.com/PetteriAimonen/libfixmatrix/blob/master/LICENSE
  [28-69]: https://github.com/PetteriAimonen/libfixmatrix
  [28-68]: https://github.com/libtom/tomsfastmath/blob/develop/LICENSE
  [28-67]: https://github.com/libtom/tomsfastmath
  [28-66]: https://github.com/libtom/libtommath/blob/develop/LICENSE
  [28-65]: https://github.com/libtom/libtommath
  [28-64]: https://github.com/imneme/pcg-c/blob/master/LICENSE.txt
  [28-63]: https://github.com/imneme/pcg-c
  [28-62]: https://github.com/imneme/pcg-c-basic/blob/master/LICENSE.txt
  [28-61]: https://github.com/imneme/pcg-c-basic
  [28-60]: N/A
  [28-59]: N/A
  [28-58]: N/A
  [28-57]: N/A
  [28-56]: https://github.com/canonizer/libgpuvm
  [28-55]: https://github.com/Lichtso/CCWT/blob/master/LICENSE
  [28-54]: https://github.com/Lichtso/CCWT
  [28-53]: https://github.com/JuliaMath/openlibm/blob/master/LICENSE.md
  [28-52]: https://github.com/JuliaMath/openlibm
  [28-51]: https://github.com/HdrHistogram/HdrHistogram_c/blob/master/LICENSE.txt
  [28-50]: https://github.com/HdrHistogram/HdrHistogram_c
  [28-49]: https://sourceforge.net/projects/gjrand/
  [28-48]: https://sourceforge.net/projects/gjrand/
  [28-47]: https://bitbucket.org/MDukhan/yeppp/src/7830144789416f9fbed3998a4c711147533cb546/LICENSE.txt?at=default&fileviewer=file-view-default
  [28-46]: https://bitbucket.org/MDukhan/yeppp
  [28-45]: https://people.sc.fsu.edu/~jburkardt/c_src/prob/prob.html
  [28-44]: https://people.sc.fsu.edu/~jburkardt/c_src/prob/prob.html
  [28-43]: https://www.mcs.anl.gov/petsc/documentation/license.html
  [28-42]: https://www.mcs.anl.gov/petsc/
  [28-41]: http://pari.math.u-bordeaux.fr/
  [28-40]: http://pari.math.u-bordeaux.fr/
  [28-39]: http://www.netlib.org/lapack/LICENSE.txt
  [28-38]: http://www.netlib.org/lapack/lapacke.html
  [28-37]: https://sourceforge.net/projects/kissfft/
  [28-36]: https://sourceforge.net/projects/kissfft/
  [28-35]: https://github.com/igraph/igraph/blob/master/COPYING
  [28-34]: https://github.com/igraph/igraph
  [28-33]: http://git.savannah.gnu.org/cgit/gsl.git/tree/COPYING
  [28-32]: http://www.gnu.org/software/gsl/
  [28-31]: https://www.gnu.org/software/mpria/
  [28-30]: https://www.gnu.org/software/mpria/
  [28-29]: https://www.mpfr.org/index.html#intro
  [28-28]: https://www.mpfr.org/index.html
  [28-27]: http://www.multiprecision.org/mpc/
  [28-26]: http://www.multiprecision.org/mpc/
  [28-25]: https://gmplib.org/repo/gmp/file/tip
  [28-24]: https://gmplib.org/
  [28-23]: https://ftp.gnu.org/gnu/glpk/
  [28-22]: https://www.gnu.org/software/glpk/
  [28-21]: https://github.com/wbhart/flint2/blob/trunk/LICENSE
  [28-20]: http://flintlib.org/
  [28-19]: https://github.com/FFTW/fftw3/blob/master/COPYING
  [28-18]: http://www.fftw.org/
  [28-17]: https://github.com/adis300/fft-c/blob/master/LICENSE
  [28-16]: https://github.com/adis300/fft-c
  [28-15]: http://www.feynarts.de/cuba/
  [28-14]: http://www.feynarts.de/cuba/
  [28-13]: https://github.com/ScientificC/cmathl/blob/master/LICENSE
  [28-12]: https://github.com/ScientificC/cmathl
  [28-11]: https://people.sc.fsu.edu/~jburkardt/c_src/cdflib/cdflib.html
  [28-10]: https://bitbucket.org/slepc/slepc/src/d7223e0d001456999ded7111aa33c2b4cd3dcbfa/LICENSE?at=master&fileviewer=file-view-default
  [28-9]: http://slepc.upv.es/
  [28-8]: http://www.netlib.org/blas/#_licensing
  [28-7]: http://www.netlib.org/blas/
  [28-6]: https://sourceforge.net/projects/math-atlas/
  [28-5]: http://math-atlas.sourceforge.net/
  [28-4]: https://github.com/b-k/apophenia/blob/master/install/COPYING
  [28-3]: https://github.com/b-k/apophenia
  [28-2]: https://github.com/fredrik-johansson/arb/blob/master/LICENSE
  [28-1]: https://github.com/fredrik-johansson/arb
</details>

<a id="compression"></a>
<details>
  <summary>Compression</summary>

  ## <a href="#-">`^`</a> Compression ##
  * [Blosc/bcolz][29-1] - Fast, multi-threaded, meta-compressor library. [`Licenses`][29-2]
  * [kiyo-masui/bitshuffle][29-51] - Filter for improving compression of typed
  binary data. [`License`][29-52]
  * [google/brotli][29-33] - Generic lossless compression algorithm based on
  LZ77, Huffman coding and 2nd order context modelling. [`MIT`][29-34]
  * [bzip2][29-11] - Patent-free, high-quality data compression library. [`BSD 4-Clause`][29-12]
  * [Blosc/c-blosc][29-37] - A blocking, shuffling and loss-less compression
  library that can be faster than memcpy(). [`Licenses`][29-38]
  * [clzip][29-3] - C lzip implementation. [`GPL 2`][29-4]
  * [richox/comprox][29-65] - An experimental lossless data compression program
  with high compression ratio. [`BSD 3-Clause`][29-66]
  * [RoaringBitmap/CRoaring][29-39] - Roaring bitmaps in C (and C++). [`Apache 2`][29-40]
  * [adnanozsoy/CUDA_Compression][29-41] - A GPU-based LZSS compression
  algorithm, highly tuned for NVIDIA GPGPUs and for streaming data, leveraging
  the respective strengths of CPUs and GPUs together. [`Apache 2`][29-42]
  * [centaurean/density][29-49] - Superfast compression library. [`BSD 3-Clause`][29-50]
  * [gildor2/fast_zlib][29-7] - Improved zlib, which runs 2 to 10 times faster. [`BSD 3-Clause`][29-8]
  * [Cyan4973/FiniteStateEntropy][29-5] - Two efficient compression codecs
  optimized for modern CPUs. [`BSD 2-Clause`][29-6]
  * [rjsikarwar/gpu_compression][29-67] - Nine Light weight Schemes to Compress
  and Decompress the data of Database Using GPU and also a planer. `No license`
  * [atomicobject/heatshrink][29-47] - data compression library for
  embedded/real-time systems. [`ISC`][29-48]
  * [adamierymenko/huffandpuff][29-9] - Minimal Huffman encoder and decoder. [`Public domain`][29-10]
  * [libarchive/libarchive][29-55] - Multi-format archive and compression
  library. [`Licenses`][29-56]
  * [nih-at/libzip][29-25] - A C library for reading, creating, and modifying
  zip archives. [`BSD 3-Clause`][29-26]
  * [inikep/lizard][29-13] - Formerly LZ5. Achieves compression ratios
  comparable with zip and zlib at decompression speeds of 1000MB/s and faster. [`Licenses`][29-14]
  * [lz4/lz4][29-57] - Extremely Fast Compression algorithm. [`Licenses`][29-58]
  * [lzo][29-27] - Very fast data compression library. [`GPL 2`][29-28]
  * [richgel999/miniz][29-63] - Single C source file zlib-replacement library. [`License`][29-64]
  * [moinakg/pcompress][29-61] - A Parallelized Data Deduplication
  and Compression utility. [`LGPL 3`][29-62]
  * [vasi/pixz][29-15] - Parallel, indexed xz compressor. [`BSD 2-Clause`][29-16]
  * [mist64/pucrunch][29-59] - pucrunch, an Optimizing Hybrid LZ77 RLE Data
  Compression Program for C64/C128/VIC-20/Plus4. [`LGPL 2.1`][29-60]
  * [quicklz][29-35] - Fast compression library. [`Licenses`][29-36]
  * [Ed-von-Schleck/shoco][29-17] - Compressor for small text strings. [`MIT`][29-18]
  * [lemire/simdcomp][29-19] - Simple library for compressing lists of integers
  using binary packing. Makes use of SIMD instructions on x86. [`BSD 3-Clause`][29-20]
  * [antirez/smaz][29-45] - Small strings compression library. [`BSD 3-Clause`][29-46]
  * [andikleen/snappy-c][29-43] - C port of the snappy compressor. [`License`][29-44]
  * [quixdb/squash][29-21] - Compression abstraction library, complete with
  utilities. [`MIT`][29-22]
  * [powturbo/TurboPFor][29-23] - Fast integer compression. [`GPL 2`][29-24]
  * [powturbo/TurboRLE][29-70] - Fastest Run Length Encoding. [`GPL 2`][29-71]
  * [kuba--/zip][29-53] - A portable, simple zip library written in C. [`Unlicense`][29-54]
  * [madler/zlib][29-29] - Massively-spiffy yet delicately-unobtrusive
  compression library. [`Zlib`][29-30]
  * [zlib-ng/zlib-ng][29-68] - zlib replacement with optimizations for
  "next generation" systems. [`Zlib`][29-69]
  * [facebook/zstd][29-31] - Fast real-time compression algorithm. [`BSD 3-Clause`][29-32]
  * [jsvennevid/filearchive][29-72] - File archive library allowing for easy
  creation and access to data stored inside a container through a simple API. [`MIT`][29-73]

  [29-73]: https://github.com/jsvennevid/filearchive/blob/master/LICENSE
  [29-72]: https://github.com/jsvennevid/filearchive
  [29-71]: https://github.com/powturbo/TurboRLE/blob/master/trle.h
  [29-70]: https://github.com/powturbo/TurboRLE
  [29-69]: https://github.com/zlib-ng/zlib-ng/blob/develop/LICENSE.md
  [29-68]: https://github.com/zlib-ng/zlib-ng
  [29-67]: https://github.com/rjsikarwar/gpu_compression
  [29-66]: https://github.com/richox/comprox/blob/master/LICENSE
  [29-65]: https://github.com/richox/comprox
  [29-64]: https://github.com/richgel999/miniz/blob/master/LICENSE
  [29-63]: https://github.com/richgel999/miniz
  [29-62]: https://github.com/moinakg/pcompress/blob/master/COPYING
  [29-61]: https://github.com/moinakg/pcompress
  [29-60]: https://github.com/mist64/pucrunch/blob/master/pucrunch.c
  [29-59]: https://github.com/mist64/pucrunch
  [29-58]: https://github.com/lz4/lz4/blob/dev/LICENSE
  [29-57]: https://github.com/lz4/lz4
  [29-56]: https://github.com/libarchive/libarchive/blob/master/COPYING
  [29-55]: https://github.com/libarchive/libarchive
  [29-54]: https://github.com/kuba--/zip/blob/master/UNLICENSE
  [29-53]: https://github.com/kuba--/zip
  [29-52]: https://github.com/kiyo-masui/bitshuffle/blob/master/LICENSE
  [29-51]: https://github.com/kiyo-masui/bitshuffle
  [29-50]: https://github.com/centaurean/density/blob/master/LICENSE.md
  [29-49]: https://github.com/centaurean/density
  [29-48]: https://github.com/atomicobject/heatshrink/blob/master/LICENSE
  [29-47]: https://github.com/atomicobject/heatshrink
  [29-46]: https://github.com/antirez/smaz/blob/master/COPYING
  [29-45]: https://github.com/antirez/smaz
  [29-44]: https://github.com/andikleen/snappy-c/blob/master/LICENSE
  [29-43]: https://github.com/andikleen/snappy-c
  [29-42]: https://github.com/adnanozsoy/CUDA_Compression/blob/master/culzss.c
  [29-41]: https://github.com/adnanozsoy/CUDA_Compression
  [29-40]: https://github.com/RoaringBitmap/CRoaring/blob/master/LICENSE
  [29-39]: https://github.com/RoaringBitmap/CRoaring
  [29-38]: https://github.com/Blosc/c-blosc/tree/master/LICENSES
  [29-37]: https://github.com/Blosc/c-blosc
  [29-36]: http://www.quicklz.com/quicklz.c
  [29-35]: http://www.quicklz.com/index.php
  [29-34]: https://github.com/google/brotli/blob/master/LICENSE
  [29-33]: https://github.com/google/brotli
  [29-32]: https://github.com/facebook/zstd/blob/dev/LICENSE
  [29-31]: https://github.com/facebook/zstd
  [29-30]: http://zlib.net/zlib_license.html
  [29-29]: https://github.com/madler/zlib
  [29-28]: http://www.oberhumer.com/opensource/lzo/#abstract
  [29-27]: http://www.oberhumer.com/opensource/lzo/
  [29-26]: https://github.com/nih-at/libzip/blob/master/LICENSE
  [29-25]: https://github.com/nih-at/libzip
  [29-24]: https://github.com/powturbo/TurboPFor/blob/master/fp.c
  [29-23]: https://github.com/powturbo/TurboPFor
  [29-22]: https://github.com/quixdb/squash/blob/master/COPYING
  [29-21]: https://github.com/quixdb/squash
  [29-20]: https://github.com/lemire/simdcomp/blob/master/LICENSE
  [29-19]: https://github.com/lemire/simdcomp
  [29-18]: https://github.com/Ed-von-Schleck/shoco/blob/master/LICENSE
  [29-17]: http://ed-von-schleck.github.io/shoco
  [29-16]: https://github.com/vasi/pixz/blob/master/LICENSE
  [29-15]: https://github.com/vasi/pixz
  [29-14]: https://github.com/inikep/lizard/blob/lizard/LICENSE
  [29-13]: https://github.com/inikep/lizard
  [29-12]: https://sourceforge.net/projects/bzip2/files/
  [29-11]: http://www.bzip.org/
  [29-10]: https://github.com/adamierymenko/huffandpuff/blob/master/huffman.h
  [29-9]: https://github.com/adamierymenko/huffandpuff
  [29-8]: https://github.com/gildor2/fast_zlib/blob/master/LICENSE.txt
  [29-7]: https://github.com/gildor2/fast_zlib
  [29-6]: https://github.com/Cyan4973/FiniteStateEntropy/blob/dev/LICENSE
  [29-5]: https://github.com/Cyan4973/FiniteStateEntropy
  [29-4]: http://lzip.nongnu.org/clzip.html
  [29-3]: http://lzip.nongnu.org/clzip.html
  [29-2]: https://github.com/Blosc/bcolz/tree/master/LICENSES
  [29-1]: https://github.com/Blosc/bcolz
</details>

<a id="concurrency-and-parallelism"></a>
<details>
  <summary>Concurrency and Parallelism</summary>

  ## <a href="#-">`^`</a> Concurrency and Parallelism ##
  * [yosefk/checkedthreads][30-1] - A simple library for parallelism, with
  built-in checking for race conditions. [`BSD 2-Clause`][30-2]
  * [FCFS RWLock][30-3] - First-come first-served Readers/Writers lock for POSIX
  threads. [`Licenses`][30-4]
  * [sharow/libconcurrent][30-5] - Concurrent programming library, using
  coroutines, for C11. [`Zlib`][30-6]
  * [liburcu][30-7] - Data synchronization library, which scales linearly with
  the number of cores. [`LGPL 2.1`][30-8]
  * [cchan][30-9] - Small library for channel constructs for inter-thread
  communication. [`Public Domain`][30-10]
  * [pmodels/mpich][30-11] - Another implementation of MPI. [`License`][30-12]
  * [open-mpi/ompi][30-13] - Message passing interface implementation. [`License`][30-14]
  * [GNU pth][30-15] - Portable implementation for non-preemptive priority-based
  scheduling for multiple threads of execution. [`LGPL 2.1`][30-16]
  * [POSIX threads][30-17] - The POSIX thread library. `No license`
  * [tinycthread/tinycthread][30-18] - Portable, small implementation of the C11
  threads API. [`License`][30-19]
  * [Pithikos/C-Thread-Pool][30-20] - A minimal but powerful thread pool in
  ANSI C. [`MIT`][30-21]
  * [baruch/libwire][30-22] - User space threading (aka coroutines) library for
  C resembling GoLang and goroutines. [`MIT`][30-23]
  * [bjoernknafla/amp][30-24] - C portable low-level assemblies for parallelism
  and threading. [`BSD 3-Clause`][30-25]
  * [bjoernknafla/peak][30-26] - Parallelism exploration assembly kit. C toolkit
  to experiment with task- and data-parallelism. [`BSD 3-Clause`][30-27]
  * [cloudwu/coroutine][30-28] - A asymmetric coroutine library for C. [`MIT`][30-29]
  * [concurrencykit/ck][30-30] - Concurrency primitives, safe memory reclamation
  mechanisms and non-blocking (including lock-free) data structures designed to
  aid in the research, design and implementation of high performance concurrent
  systems developed in C99+. [`Licenses`][30-31]
  * [etmc/lemon][30-32] - Lemon is an MPI parallel I/O library that is intended
  to allow for efficient parallel I/O of both binary and metadata on massively
  parallel architectures. Data is stored in the SciDAC Lattice QCD Interchange
  Message Encapsulation format, that allows for storing large blocks of binary
  data and corresponding metadata in the same file. [`GPL 3`][30-33]
  * [geertj/cgreenlet][30-34] - Coroutines for C/C++. [`MIT`][30-35]
  * [halayli/lthread][30-36] - lthread, a multicore enabled coroutine library
  written in C. [`BSD 2-Clause`][30-37]
  * [hnes/libaco][30-38] - A blazing fast and lightweight C asymmetric coroutine
  library. [`Apache 2`][30-39]
  * [jtsiomb/c11threads][30-40] - Trivial C11 threads.h implementation over
  POSIX threads. [`Public domain`][30-41]
  * [matianfu/FUNK][30-42] - a c continuation library inspired by Adam Dunkel's
  ProtoThread. [`Apache 2`][30-43]
  * [mbrossard/threadpool][30-44] - A simple C Thread pool implementation. [`BSD 2-Clause`][30-45]
  * [oneoo/alilua-coevent-module][30-46] - epoll base coroutine module. [`MIT`][30-47]
  * [ramonza/libcoro][30-48] - Lightweight C coroutines. [`BSD 2-Clause`][30-49]
  * [sustrik/libdill][30-50] - Structured concurrency in C. [`MIT`][30-51]
  * [sustrik/libmill][30-52] - Go-style concurrency in C. [`MIT`][30-53]
  * [stevedekorte/coroutine][30-54] - C multiplatform coroutine implementation
  via ucontext, fibers or setjmp. `No license`
  * [parallella/pal][30-55] - An optimized C library for math, parallel
  processing and data movement. [`Apache 2`][30-56]

  [30-56]: https://github.com/parallella/pal/blob/master/LICENSE
  [30-55]: https://github.com/parallella/pal
  [30-54]: https://github.com/stevedekorte/coroutine
  [30-53]: https://github.com/sustrik/libmill/blob/master/COPYING
  [30-52]: https://github.com/sustrik/libmill
  [30-51]: https://github.com/sustrik/libdill/blob/master/COPYING
  [30-50]: https://github.com/sustrik/libdill
  [30-49]: https://github.com/ramonza/libcoro/blob/master/LICENSE
  [30-48]: https://github.com/ramonza/libcoro
  [30-47]: https://github.com/oneoo/alilua-coevent-module/blob/master/LICENSE
  [30-46]: https://github.com/oneoo/alilua-coevent-module
  [30-45]: https://github.com/mbrossard/threadpool/blob/master/LICENSE
  [30-44]: https://github.com/mbrossard/threadpool
  [30-43]: https://github.com/matianfu/FUNK/blob/master/LICENSE
  [30-42]: https://github.com/matianfu/FUNK
  [30-41]: https://github.com/jtsiomb/c11threads
  [30-40]: https://github.com/jtsiomb/c11threads
  [30-39]: https://github.com/hnes/libaco/blob/master/LICENSE
  [30-38]: https://github.com/hnes/libaco
  [30-37]: https://github.com/halayli/lthread/blob/master/LICENSE
  [30-36]: https://github.com/halayli/lthread
  [30-35]: https://github.com/geertj/cgreenlet/blob/master/LICENSE
  [30-34]: https://github.com/geertj/cgreenlet
  [30-33]: https://github.com/etmc/lemon/blob/master/COPYING
  [30-32]: https://github.com/etmc/lemon
  [30-31]: https://github.com/concurrencykit/ck/blob/master/LICENSE
  [30-30]: https://github.com/concurrencykit/ck
  [30-29]: https://github.com/cloudwu/coroutine/blob/master/LICENSE
  [30-28]: https://github.com/cloudwu/coroutine
  [30-27]: https://github.com/bjoernknafla/peak/blob/master/COPYRIGHT.txt
  [30-26]: https://github.com/bjoernknafla/peak
  [30-25]: https://github.com/bjoernknafla/amp/blob/master/COPYRIGHT.txt
  [30-24]: https://github.com/bjoernknafla/amp
  [30-23]: https://github.com/baruch/libwire/blob/master/LICENSE
  [30-22]: https://github.com/baruch/libwire
  [30-21]: https://github.com/Pithikos/C-Thread-Pool/blob/master/LICENSE
  [30-20]: https://github.com/Pithikos/C-Thread-Pool
  [30-19]: https://github.com/tinycthread/tinycthread
  [30-18]: https://github.com/tinycthread/tinycthread
  [30-17]: https://en.wikipedia.org/wiki/POSIX_Threads
  [30-16]: ftp://ftp.gnu.org/gnu/pth/
  [30-15]: https://www.gnu.org/software/pth/
  [30-14]: https://github.com/open-mpi/ompi/blob/master/LICENSE
  [30-13]: https://github.com/open-mpi
  [30-12]: https://github.com/pmodels/mpich/blob/master/COPYRIGHT
  [30-11]: https://github.com/pmodels/mpich
  [30-10]: http://repo.hu/projects/cchan/
  [30-9]: http://repo.hu/projects/cchan/
  [30-8]: http://liburcu.org/
  [30-7]: http://liburcu.org/
  [30-6]: https://github.com/sharow/libconcurrent/blob/master/LICENSE
  [30-5]: https://github.com/sharow/libconcurrent
  [30-4]: https://bitbucket.org/shlomif/fcfs-rwlock/src/65dd5211852781b82ef0fd732a0b0d542e9c726c/LICENSE?at=default&fileviewer=file-view-default
  [30-3]: http://www.shlomifish.org/rwlock/
  [30-2]: https://github.com/yosefk/checkedthreads/blob/master/LICENSE.txt
  [30-1]: https://github.com/yosefk/checkedthreads
</details>

<a id="opencl"></a>
<details>
  <summary>OpenCL</summary>

  ## <a href="#-">`^`</a> OpenCL ##

  OpenCL, CUDA, OpenMP and other similar APIs.
  * [cf4ocl][31-1] - The C Framework for OpenCL. [`LGPL 3`][31-2]
  * [clMathLibraries/clRNG][31-3] - an OpenCL based software library containing
  random number generation functions. [`License`][31-4]
  * [tuxfan/ocl-mla][31-5] - OpenCL Mid-Level Abstractions. [`License`][31-6]
  * [matze/oclkit][31-7] - Two-file OpenCL wrapper. [`GPL 3`][31-8]
  * [emrainey/OpenCL-Environment][31-9] - A series of utilities aimed at making
  OpenCL easier to use. [`Apache 2`][31-10]

  [31-10]: https://github.com/emrainey/OpenCL-Environment/blob/master/LICENSE-2.0.txt
  [31-9]: https://github.com/emrainey/OpenCL-Environment
  [31-8]: https://github.com/matze/oclkit/blob/master/COPYING
  [31-7]: https://github.com/matze/oclkit
  [31-6]: https://github.com/tuxfan/ocl-mla/blob/master/LICENSE
  [31-5]: https://github.com/tuxfan/ocl-mla
  [31-4]: https://github.com/clMathLibraries/clRNG/blob/master/LICENSE
  [31-3]: https://github.com/clMathLibraries/clRNG
  [31-2]: https://github.com/fakenmc/cf4ocl/blob/master/COPYING
  [31-1]: https://github.com/fakenmc/cf4ocl
</details>

<a id="crypto"></a>
<details>
  <summary>Cryptography</summary>

  ## <a href="#-">`^`</a> Cryptography ##
  * [GNU SASL][32-1] - Implementation of the Simple Authentication and Security
  Layer and few common SASL mechanisms. [`Licenses`][32-2]
  * [aidansteele/sphlib][32-3] - Set of implementations of various hash
  functions, including several cryptographic ones. [`MIT`][32-4]
  * [GnuTLS][32-5] - Secure communication library, implementing SSL, TLS and
  DTLS. [`LGPL 2.1`][32-6]
  * [libgcrypt][32-7] - General-purpose cryptography library, with a range of
  available ciphers. [`Licenses`][32-8]
  * [OpenSSL][32-9] - Implementation of the SSL and TLS protocols, and also
  includes a cryptography library. [`Licenses`][32-10]
  * [jedisct1/libsodium][32-11] - A modern, portable and easy to use crypto
  library. [`ISC`][32-12]
  * [ARMmbed/mbedtls][32-13] - An open source, portable, easy to use, readable
  and flexible SSL library. [`License`][32-14]
  * [B-Con/crypto-algorithms][32-15] - Basic implementations of standard
  cryptography algorithms, like AES and SHA-1. `No license`
  * [WickrInc/wickr-crypto-c][32-16] - An implementation of the Wickr Secure
  Messaging Protocol in C. [`License`][32-17]
  * [ashwinraghav/Parallel_Open_SSL][32-18] - Use your idle GPU to encrypt your
  data. Give your CPU some breathing time! [`Licenses`][32-19]
  * [awslabs/s2n][32-20] - s2n : an implementation of the TLS/SSL protocols. [`Apache 2`][32-21]
  * [bitcoin-core/secp256k1][32-22] - Optimized C library for EC operations on
  curve secp256k1. [`MIT`][32-23]
  * [cloudflare/keyless][32-24] - CloudFlare's Keyless SSL Server Reference
  Implementation. [`Agreement`][32-25]
  * [ctz/cifra][32-26] - A collection of cryptographic primitives targeted at
  embedded use. [`License`][32-27]
  * [cyassl/cyassl][32-28] - Small, fast, portable implementation of TLS/SSL for
  embedded devices to the cloud. [`GPL 2`][32-29]
  * [eduardsui/tlse][32-30] - Single C file TLS 1.2/1.3 implementation, using
  tomcrypt as crypto library. [`BSD 2-Clause`][32-31]
  * [h2o/picotls][32-32] - TLS 1.3 implementation in C (master supports RFC8446
  as well as draft-26, -27, -28). [`License`][32-33]
  * [jedisct1/libhydrogen][32-34] - A lightweight, secure, easy-to-use crypto
  library suitable for constrained environments. [`ISC`][32-35]
  * [libressl-portable/openbsd][32-36] - LibreSSL source code. [`Licenses`][32-37]
  * [libtom/libtomcrypt][32-38] - LibTomCrypt is a fairly comprehensive, modular
  and portable cryptographic toolkit that provides developers with a vast array
  of well known published block ciphers, one-way hash functions, chaining modes,
  pseudo-random number generators, public key cryptography and a plethora of
  other routines. [`Licenses`][32-39]
  * [maciejczyzewski/retter][32-40] - A collection of hash functions, ciphers,
  tools, libraries, and materials related to cryptography. `No license`
  * [mikeryan/crackle][32-41] - Crack and decrypt BLE encryption. [`BSD 2-Clause`][32-42]
  * [open-quantum-safe/liboqs][32-43] - C library for quantum-resistant
  cryptographic algorithms. [`MIT`][32-44]
  * [tbuktu/libntru][32-45] - C Implementation of NTRUEncrypt. [`Licenses`][32-46]
  * [trezor/trezor-crypto][32-47] - Heavily optimized cryptography
  algorithms for embedded devices. [`MIT`][32-48]
  * [droe/sslsplit][32-49] - Transparent SSL/TLS interception. [`BSD 2-Clause`][32-50]
  * [orlp/ed25519][32-51] - Portable C implementation of Ed25519, a high-speed
  high-security public-key signature system. [`Zlib`][32-52]
  * [wolfSSL/wolfssl][32-53] - wolfSSL (formerly CyaSSL) is a small, fast,
  portable implementation of TLS/SSL for embedded devices to the cloud. [`GPL 2`][32-54]
  * [rg3/bcrypt][32-55] - bcrypt password hash C library. [`License`][32-56]

  [32-56]: https://github.com/rg3/libbcrypt/blob/master/COPYING
  [32-55]: https://github.com/rg3/bcrypt
  [32-54]: https://github.com/wolfSSL/wolfssl/blob/master/COPYING
  [32-53]: https://github.com/wolfSSL/wolfssl
  [32-52]: https://github.com/orlp/ed25519/blob/master/license.txt
  [32-51]: https://github.com/orlp/ed25519
  [32-50]: https://github.com/droe/sslsplit/blob/develop/LICENSE
  [32-49]: https://github.com/droe/sslsplit
  [32-48]: https://github.com/trezor/trezor-crypto/blob/master/LICENSE
  [32-47]: https://github.com/trezor/trezor-crypto
  [32-46]: https://github.com/tbuktu/libntru/blob/master/LICENSE
  [32-45]: https://github.com/tbuktu/libntru
  [32-44]: https://github.com/open-quantum-safe/liboqs/blob/master/LICENSE.txt
  [32-43]: https://github.com/open-quantum-safe/liboqs
  [32-42]: https://github.com/mikeryan/crackle/blob/master/LICENSE
  [32-41]: https://github.com/mikeryan/crackle
  [32-40]: https://github.com/maciejczyzewski/retter
  [32-39]: https://github.com/libtom/libtomcrypt/blob/develop/LICENSE
  [32-38]: https://github.com/libtom/libtomcrypt
  [32-37]: https://en.wikipedia.org/wiki/LibreSSL
  [32-36]: https://github.com/libressl-portable/openbsd
  [32-35]: https://github.com/jedisct1/libhydrogen/blob/master/LICENSE
  [32-34]: https://github.com/jedisct1/libhydrogen
  [32-33]: https://github.com/h2o/picotls/blob/master/lib/picotls.c
  [32-32]: https://github.com/h2o/picotls
  [32-31]: https://github.com/eduardsui/tlse/blob/master/LICENSE
  [32-30]: https://github.com/eduardsui/tlse
  [32-29]: https://github.com/cyassl/cyassl/blob/master/COPYING
  [32-28]: https://github.com/cyassl/cyassl
  [32-27]: https://github.com/ctz/cifra/blob/master/COPYING
  [32-26]: https://github.com/ctz/cifra
  [32-25]: https://github.com/cloudflare/keyless/blob/master/LICENSE
  [32-24]: https://github.com/cloudflare/keyless
  [32-23]: https://github.com/bitcoin-core/secp256k1/blob/master/COPYING
  [32-22]: https://github.com/bitcoin-core/secp256k1
  [32-21]: https://github.com/awslabs/s2n/blob/master/LICENSE
  [32-20]: https://github.com/awslabs/s2n
  [32-19]: https://github.com/ashwinraghav/Parallel_Open_SSL/blob/master/LICENSE
  [32-18]: https://github.com/ashwinraghav/Parallel_Open_SSL
  [32-17]: https://github.com/WickrInc/wickr-crypto-c/blob/master/LICENSE
  [32-16]: https://github.com/WickrInc/wickr-crypto-c
  [32-15]: https://github.com/B-Con/crypto-algorithms
  [32-14]: https://github.com/ARMmbed/mbedtls/blob/development/LICENSE
  [32-13]: https://github.com/ARMmbed/mbedtls
  [32-12]: https://github.com/jedisct1/libsodium/blob/master/LICENSE
  [32-11]: https://github.com/jedisct1/libsodium
  [32-10]: https://www.openssl.org/source/license.txt
  [32-9]: https://www.openssl.org
  [32-8]: https://gnupg.org/related_software/libgcrypt/
  [32-7]: https://gnupg.org/related_software/libgcrypt/
  [32-6]: https://www.gnutls.org/
  [32-5]: https://www.gnutls.org/
  [32-4]: https://github.com/aidansteele/sphlib/blob/master/LICENSE.txt
  [32-3]: https://github.com/aidansteele/sphlib
  [32-2]: https://www.gnu.org/software/gsasl/#TOCnews
  [32-1]: https://www.gnu.org/software/gsasl
</details>

<a id="databases"></a>
<details>
  <summary>Databases</summary>

  ## <a href="#-">`^`</a> Databases ##
  * [priitj/whitedb][33-1] - Lightweight database library, operating entirely in
  main memory. [`GPL 3`][33-2]
  * [mongodb/mongo-c-driver][33-3] - High-performance client library for
  MongoDB. [`Apache 2`][33-4]
  * [SQLite][33-5] - Self-contained, serverless, zero-configuration,
  transactional SQL database engine with a C interface. [`Public domain`][33-6]
  * [symisc/unqlite][33-7] - Self-contained, serverless, zero-configuration,
  transactional NoSQL engine with a C interface. [`License`][33-8]
  * [Akash91/CoSQL][33-9] - A Co-Relational Key-Value Data Store. `No license`
  * [GNOME/libgda][33-10] - Libgda is a (relatively small) database access
  library. [`GPL 2`][33-11]
  * [Softmotions/ejdb][33-12] - EJDB — Embeddable JSON Database engine. [`MIT`][33-13]
  * [aerospike/aerospike-client-c][33-14] - Aerospike C Client. [`License`][33-15]
  * [bcmpinc/dagdb][33-16] - small database for storing semi-structured data. [`GPL 3`][33-17]
  * [maciejczyzewski/hashbase][33-18] - A fast, efficient on-disk/in-memory
  database with many different kind of data structures. [`MIT`][33-19]
  * [maxmind/libmaxminddb][33-20] - C library for the MaxMind DB file format. [`Apache 2`][33-21]
  * [pmwkaa/sophia][33-22] - modern emeddable key-value database. [`License`][33-23]
  * [redis/hiredis][33-24] - Minimalistic C client for Redis. [`BSD 3-Clause`][33-25]
  * [seppo0010/rlite][33-26] - self-contained, serverless, zero-configuration,
  transactional redis-compatible database engine. rlite is to Redis what SQLite
  is to SQL. [`BSD 2-Clause`][33-27]
  * [sqlcipher/sqlcipher][33-28] - SQLCipher is an SQLite extension that
  provides 256 bit AES encryption of database files. [`License`][33-29]
  * [tglman/orientdb-c][33-30] - The C client of  OrientDB. `No license`
  * [spotify/sparkey][33-31] - Simple constant key/value storage library, for
  read-heavy systems with infrequent large bulk inserts. [`Apache 2`][33-32]
  * [vrogier/ocilib][33-33] - Open source C and C++ library for accessing
  Oracle databases. [`Apache 2`][33-34]
  * [symisc/vedis][33-35] - An Embedded Implementation of Redis. [`License`][33-36]

  [33-36]: https://github.com/symisc/vedis/blob/master/license.txt
  [33-35]: https://github.com/symisc/vedis
  [33-34]: https://github.com/vrogier/ocilib/blob/master/LICENSE
  [33-33]: https://github.com/vrogier/ocilib
  [33-32]: https://github.com/spotify/sparkey/blob/master/LICENSE
  [33-31]: https://github.com/spotify/sparkey
  [33-30]: https://github.com/tglman/orientdb-c
  [33-29]: https://github.com/sqlcipher/sqlcipher/blob/master/LICENSE
  [33-28]: https://github.com/sqlcipher/sqlcipher
  [33-27]: https://github.com/seppo0010/rlite/blob/master/LICENSE
  [33-26]: https://github.com/seppo0010/rlite
  [33-25]: https://github.com/redis/hiredis/blob/master/COPYING
  [33-24]: https://github.com/redis/hiredis
  [33-23]: https://github.com/pmwkaa/sophia/blob/master/LICENSE
  [33-22]: https://github.com/pmwkaa/sophia
  [33-21]: https://github.com/maxmind/libmaxminddb/blob/master/LICENSE
  [33-20]: https://github.com/maxmind/libmaxminddb
  [33-19]: https://github.com/maciejczyzewski/hashbase/blob/master/LICENSE
  [33-18]: https://github.com/maciejczyzewski/hashbase
  [33-17]: https://github.com/bcmpinc/dagdb/blob/master/LICENSE
  [33-16]: https://github.com/bcmpinc/dagdb
  [33-15]: https://github.com/aerospike/aerospike-client-c/blob/master/LICENSE.md
  [33-14]: https://github.com/aerospike/aerospike-client-c
  [33-13]: https://github.com/Softmotions/ejdb/blob/master/LICENSE
  [33-12]: https://github.com/Softmotions/ejdb
  [33-11]: https://github.com/GNOME/libgda/blob/master/COPYING
  [33-10]: https://github.com/GNOME/libgda
  [33-9]: https://github.com/Akash91/CoSQL
  [33-8]: https://github.com/symisc/unqlite/blob/master/LICENSE
  [33-7]: https://github.com/symisc/unqlite
  [33-6]: https://www.sqlite.org/copyright.html
  [33-5]: https://www.sqlite.org/about.html
  [33-4]: https://github.com/mongodb/mongo-c-driver/blob/master/COPYING
  [33-3]: https://github.com/mongodb/mongo-c-driver
  [33-2]: https://github.com/priitj/whitedb/blob/master/COPYING
  [33-1]: https://github.com/priitj/whitedb
</details>

<a id="data-structures"></a>
<details>
  <summary>Data Structures and Types</summary>

  ## <a href="#-">`^`</a> Data Structures and Types ##
  * [recp/ds][34-1] - Common Data Structures and Algorithms. [`MIT`][34-2]
  * [P-p-H-d/mlib][34-3] - Library for generic, but typesafe C containers.
  Implemented as header-only. [`BSD 2-Clause`][34-4]
  * [libsrt][34-5] - Soft and hard real-time data structures. [`BSD 3-Clause`][34-6]
  * [nbulischeck/list.h][34-7] - Implementations for single- and double-linked
  list functions. [`GPL 3`][34-8]
  * [gpakosz/PackedArray][34-9] - Random-access array of tightly packed unsigned
  integers of any desired width. Has a SIMD-optimized implementation. [`WTFPL`][34-10]
  * [swenson/vector.h][34-11] - Header library for typed lists. [`MIT`][34-12]
  * [20centaurifux/datatypes][34-13] - A collection of various datatypes in C
  (linked lists, stack, queue, red-black tree and hash table). [`GPL 3`][34-14]
  * [ClickerMonkey/CDSL][34-15] - A data structure library written in C. [`License`][34-16]
  * [Incarnation-p-lee/libds][34-17] - Unified data structure implementation
  library of C. [`GPL 2`][34-18]
  * [LPD-EPFL/ASCYLIB][34-19] - Concurrent-search data-structure library with
  over 30 implementantions of linked lists, hash tables, skip lists, and binary
  search trees. [`GPL 2`][34-20]
  * [MichaelJWelsh/cdsa][34-21] - A library of generic intrusive data structures
  and algorithms in ANSI C. [`ISC`][34-22]
  * [ZSShen/C-Common-Data-Structures][34-23] - Uniform C APIs for data structure
  manipulation. `No license`
  * [agl/critbit][34-24] - Critbit trees in C. `No license`
  * [antirez/rax][34-25] - A radix tree implementation in ANSI C. [`BSD 2-Clause`][34-26]
  * [armon/libart][34-27] - Adaptive Radix Trees implemented in C. [`BSD 3-Clause`][34-28]
  * [ashinkarov/trie][34-29] - Simple implementation of trie data structure. [`License`][34-30]
  * [bcopeland/em_misc][34-31] - External memory data structure playground. `No license`
  * [begeekmyfriend/bplustree][34-32] - A minimal but extreme fast B+ tree
  indexing structure demo for billions of key-value storage. [`MIT`][34-33]
  * [chrismoos/hash-ring][34-34] - C hash ring library. [`Apache 2`][34-35]
  * [chriso/bitset][34-36] - A compressed bitset with supporting data structures
  and algorithms. [`LGPL`][34-37]
  * [codeprepper/data-structures][34-38] - Arrays, linked lists, stacks and
  queues. [`MIT`][34-39]
  * [dminor/skip-quadtree][34-40] - Implementation of the skip quadtree and
  compressed quadtree data structures. [`License`][34-41]
  * [douglascrockford/DEC64][34-42] - Decimal floating point. `No license`
  * [fmela/libdict][34-43] - C library of key-value data structures with an
  object-oriented interface. [`BSD 2-Clause`][34-44]
  * [fragglet/c-algorithms][34-45] - A library of common data structures and
  algorithms written in C. [`ISC`][34-46]
  * [gnudennis/ds_c][34-47] - Data Structure In C. `No license`
  * [graphitemaster/libintrusive][34-48] - Intrusive data structures for C. [`Unlicense`][34-49]
  * [grundprinzip/bitcompressedvector][34-50] - Provide a container for integral
  data types that applies light-weight bit compression. [`License`][34-51]
  * [hacatu/haclib][34-52] - A utility library providing data types C should
  have been made with such as vectors and sequences, mostly as macros. [`MPL 2`][34-53]
  * [hyPiRion/c-rrb][34-54] - RRB-tree implemented as a library in C. [`MIT`][34-55]
  * [hyPiRion/roulette-tree][34-56] - Data structure for efficient
  fitness-proportionate selection. [`MIT`][34-57]
  * [jarun/dslib][34-58] - A library of handy data structures. [`GPL 3`][34-58]
  * [johnj/llds][34-60] - Low-Level Data Structure - efficient data structures,
  and fast data access in the 2.6/3.0 kernel. [`License`][34-61]
  * [jtsiomb/kdtree][34-62] - A simple C library for working with KD-Trees. [`License`][34-63]
  * [jvirkki/libbloom][34-64] - A simple and small bloom filter implementation
  in plain C. [`BSD 2-Clause`][34-65]
  * [ksheedlo/kmdata][34-66] - Data structures for C programmers, by
  C programmers. `No license`
  * [louiswins/RB-Tree][34-67] - An implementation of the Red-Black Tree data
  structure. `No license`
  * [livioso/datastructures-in-C][34-68] - Implementation of a some data
  structures in C for educational purposes. `No license`
  * [malbrain/Btree-source-code][34-69] - A working project for High-concurrency
  B-tree source code in C. [`License`][34-70]
  * [michaeltyson/TPCircularBuffer][34-71] - A simple, fast circular buffer
  implementation. [`License`][34-72]
  * [mikedlowis/data-structures][34-73] - A collection of data structures
  implemented in C to be included in multiple projects. [`BSD 2-Clause`][34-74]
  * [naraing/dsLib][34-75] - An algorithm library with core data-sttructures and
  common algortihm implementations on those data structures. [`GPL 3`][34-76]
  * [noporpoise/BitArray][34-77] - C bit array structs and methods. [`License`][34-78]
  * [orangejulius/cs_fundamentals][34-79] - simple implementations of common
  data structures/algorithms. [`GPL 3`][34-80]
  * [paulasmuth/libsmatrix][34-81] - thread-safe sparse matrix data structure. [`MIT`][34-82]
  * [pcdavid/data-structures][34-83] - Sample implementations of classical data
  structures in C. [`WTFPL`][34-84]
  * [petewarden/c_hashmap][34-85] - A simple string hashmap in C. [`Public domain`][34-86]
  * [rxi/map][34-87] - A type-safe hash map implementation for C. [`MIT`][34-88]
  * [rxi/vec][34-89] - A type-safe dynamic array implementation for C. [`MIT`][34-90]
  * [siganakis/tny][34-91] - Tiny data structures that pack a punch! [`License`][34-92]
  * [srdja/Collections-C][34-93] - A library of generic data structures. [`LGPL 3`][34-94]
  * [steven-schronk/C-Data-Structures][34-95] - Collection of basic data
  structures in C. [`GPL 3`][34-96]
  * [wasabiz/xrope][34-97] - rope data structure. `No license`
  * [torch/tds][34-98] - Torch C data structures. [`License`][34-99]
  * [watmough/jwHash][34-100] - Simple hash table implementation for C. [`Apache 2`][34-101]
  * [zhemao/libds][34-102] - Simple, memory-safe data-structures in C. [`MIT`][34-103]
  * [willemt/cbuffer][34-104] - A circular buffer written in C using Posix calls
  to create a contiguously mapped memory space. BSD Licensed. [`License`][34-105]
  * [xant/libhl][34-106] - Simple and fast C library implementing a thread-safe
  API to manage hash-tables, linked lists, lock-free ring buffers and queues. [`LGPL 3`][34-107]
  * [yuyuyu101/C-Buffered-tree][34-108] - A buffered-tree implemented in
  dictionary type and more. [`MIT`][34-109]
  * [MagerValp/AsmHeap][34-110] - Heap data structure in 6502 assembler. `No license`
  * [Snaipe/libcsptr][34-111] - Smart pointers in C. [`MIT`][34-112]
  * [C-Macro-Collections][34-113] - Generate simple and generic data structures
  using macros. [`MIT`][34-114]
  * [troydhanson/uthash][34-115] - C macros for hash tables and more. [`License`][34-116]
  * [begeekmyfriend/CuckooFilter][34-117] - Substitute for bloom filter. [`License`][34-118]
  * [bitly/dablooms][34-119] - scaling, counting, bloom filter library. [`MIT`][34-120]

  [34-120]: https://github.com/bitly/dablooms/blob/master/LICENSE
  [34-119]: https://github.com/bitly/dablooms
  [34-118]: https://github.com/begeekmyfriend/CuckooFilter/blob/master/LICENSE
  [34-117]: https://github.com/begeekmyfriend/CuckooFilter
  [34-116]: https://github.com/troydhanson/uthash/blob/master/LICENSE
  [34-115]: https://github.com/troydhanson/uthash
  [34-114]: https://github.com/LeoVen/C-Macro-Collections/blob/master/LICENSE
  [34-113]: https://github.com/LeoVen/C-Macro-Collections
  [34-112]: https://github.com/Snaipe/libcsptr/blob/master/LICENSE
  [34-111]: https://github.com/Snaipe/libcsptr
  [34-110]: https://github.com/MagerValp/AsmHeap
  [34-109]: https://github.com/yuyuyu101/C-Buffered-tree/blob/master/LICENSE
  [34-108]: https://github.com/yuyuyu101/C-Buffered-tree
  [34-107]: https://github.com/xant/libhl/blob/master/LICENSE
  [34-106]: https://github.com/xant/libhl
  [34-105]: https://github.com/willemt/cbuffer/blob/master/LICENSE
  [34-104]: https://github.com/willemt/cbuffer
  [34-103]: https://github.com/zhemao/libds/blob/master/LICENSE
  [34-102]: https://github.com/zhemao/libds
  [34-101]: https://github.com/watmough/jwHash/blob/master/LICENSE
  [34-100]: https://github.com/watmough/jwHash
  [34-99]: https://github.com/torch/tds/blob/master/LICENSE
  [34-98]: https://github.com/torch/tds/
  [34-97]: https://github.com/wasabiz/xrope
  [34-96]: https://github.com/steven-schronk/C-Data-Structures/blob/master/COPYING
  [34-95]: https://github.com/steven-schronk/C-Data-Structures
  [34-94]: https://github.com/srdja/Collections-C/blob/master/COPYING
  [34-93]: https://github.com/srdja/Collections-C
  [34-92]: https://github.com/siganakis/tny/blob/master/src/main.c
  [34-91]: https://github.com/siganakis/tny
  [34-90]: https://github.com/rxi/vec/blob/master/LICENSE
  [34-89]: https://github.com/rxi/vec
  [34-88]: https://github.com/rxi/map/blob/master/LICENSE
  [34-87]: https://github.com/rxi/map
  [34-86]: https://github.com/petewarden/c_hashmap/blob/master/License.md
  [34-85]: https://github.com/petewarden/c_hashmap
  [34-84]: https://github.com/pcdavid/data-structures/blob/master/COPYING
  [34-83]: https://github.com/pcdavid/data-structures
  [34-82]: https://github.com/asmuth-archive/libsmatrix/blob/master/src/smatrix.c
  [34-81]: https://github.com/asmuth-archive/libsmatrix
  [34-80]: https://github.com/orangejulius/cs_fundamentals/blob/master/COPYING
  [34-79]: https://github.com/orangejulius/cs_fundamentals
  [34-78]: https://github.com/noporpoise/BitArray/blob/master/LICENSE
  [34-77]: https://github.com/noporpoise/BitArray
  [34-76]: https://github.com/naraing/dsLib/blob/master/COPYING
  [34-75]: https://github.com/naraing/dsLib
  [34-74]: https://github.com/mikedlowis/libcds/blob/master/LICENSE.md
  [34-73]: https://github.com/mikedlowis/libcds
  [34-72]: https://github.com/michaeltyson/TPCircularBuffer/blob/master/TPCircularBuffer.c
  [34-71]: https://github.com/michaeltyson/TPCircularBuffer
  [34-70]: https://github.com/malbrain/Btree-source-code/blob/master/btree2/btree2v.c
  [34-69]: https://github.com/malbrain/Btree-source-code
  [34-68]: https://github.com/livioso/datastructures-in-C
  [34-67]: https://github.com/louiswins/RB-Tree
  [34-66]: https://github.com/ksheedlo/kmdata
  [34-65]: https://github.com/jvirkki/libbloom/blob/master/LICENSE
  [34-64]: https://github.com/jvirkki/libbloom
  [34-63]: https://github.com/jtsiomb/kdtree/blob/master/COPYING
  [34-62]: https://github.com/jtsiomb/kdtree
  [34-61]: https://github.com/johnj/llds/blob/master/LICENSE
  [34-60]: https://github.com/johnj/llds
  [34-59]: https://github.com/jarun/dslib/blob/master/LICENSE
  [34-58]: https://github.com/jarun/dslib
  [34-57]: https://github.com/hypirion/roulette-tree/blob/master/COPYING
  [34-56]: https://github.com/hypirion/roulette-tree
  [34-55]: https://github.com/hypirion/c-rrb/blob/development/COPYING
  [34-54]: https://github.com/hypirion/c-rrb
  [34-53]: https://github.com/hacatu/haclib/blob/master/LICENSE.txt
  [34-52]: https://github.com/hacatu/haclib
  [34-51]: https://github.com/grundprinzip/bitcompressedvector#licence
  [34-50]: https://github.com/grundprinzip/bitcompressedvector
  [34-49]: https://github.com/graphitemaster/libintrusive/blob/master/LICENSE
  [34-48]: https://github.com/graphitemaster/libintrusive
  [34-47]: https://github.com/gnudennis/ds_c
  [34-46]: https://github.com/fragglet/c-algorithms/blob/master/COPYING
  [34-45]: https://github.com/fragglet/c-algorithms
  [34-44]: https://github.com/fmela/libdict/blob/master/LICENSE
  [34-43]: https://github.com/fmela/libdict
  [34-42]: https://github.com/douglascrockford/DEC64
  [34-41]: https://github.com/dminor/skip-quadtree/blob/master/include/quadtree.h
  [34-40]: https://github.com/dminor/skip-quadtree
  [34-39]: https://github.com/codeprepper/data-structures/blob/master/LICENSE
  [34-38]: https://github.com/codeprepper/data-structures
  [34-37]: https://github.com/chriso/bitset#license
  [34-36]: https://github.com/chriso/bitset
  [34-35]: https://github.com/chrismoos/hash-ring/blob/master/LICENSE
  [34-34]: https://github.com/chrismoos/hash-ring
  [34-33]: https://github.com/begeekmyfriend/bplustree/blob/disk-io/LICENSE
  [34-32]: https://github.com/begeekmyfriend/bplustree
  [34-31]: https://github.com/bcopeland/em_misc
  [34-30]: https://github.com/ashinkarov/trie/blob/master/trie.h
  [34-29]: https://github.com/ashinkarov/trie
  [34-28]: https://github.com/armon/libart/blob/master/LICENSE
  [34-27]: https://github.com/armon/libart
  [34-26]: https://github.com/antirez/rax/blob/master/COPYING
  [34-25]: https://github.com/antirez/rax
  [34-24]: https://github.com/agl/critbit
  [34-23]: https://github.com/ZSShen/C-Common-Data-Structures
  [34-22]: https://github.com/MichaelJWelsh/cdsa/blob/master/LICENSE
  [34-21]: https://github.com/MichaelJWelsh/cdsa
  [34-20]: https://github.com/LPD-EPFL/ASCYLIB/blob/master/LICENSE
  [34-19]: https://github.com/LPD-EPFL/ASCYLIB
  [34-18]: https://github.com/Incarnation-p-lee/libds/blob/master/LICENSE
  [34-17]: https://github.com/Incarnation-p-lee/libds
  [34-16]: https://github.com/ClickerMonkey/CDSL/blob/master/lib/vector.c
  [34-15]: https://github.com/ClickerMonkey/CDSL
  [34-14]: https://github.com/20centaurifux/datatypes/blob/master/COPYING
  [34-13]: https://github.com/20centaurifux/datatypes
  [34-12]: https://github.com/swenson/vector.h/blob/master/LICENSE
  [34-11]: https://github.com/swenson/vector.h
  [34-10]: https://github.com/gpakosz/PackedArray/blob/master/LICENSE
  [34-9]: https://github.com/gpakosz/PackedArray
  [34-8]: https://github.com/nbulischeck/list.h/blob/master/LICENSE
  [34-7]: https://github.com/nbulischeck/list.h
  [34-6]: https://github.com/faragon/libsrt/blob/master/LICENSE
  [34-5]: https://github.com/faragon/libsrt
  [34-4]: https://github.com/P-p-H-d/mlib/blob/master/LICENSE
  [34-3]: https://github.com/P-p-H-d/mlib
  [34-2]: https://github.com/recp/ds/blob/master/LICENSE
  [34-1]: https://github.com/recp/ds
</details>

<a id="events"></a>
<details>
  <summary>Events</summary>

  ## <a href="#-">`^`</a> Events ##
  * [libev][35-1] - Yet another event loop. [`BSD 2-Clause`][35-2]
  * [libevent][35-3] - Event loop replacement for network servers. [`BSD 3-Clause`][35-4]
  * [Lupus/libevfibers][35-5] - Small C fiber library that uses libev based event loop and libcoro based coroutine context switching. [`Apache 2`][35-6]
  * [facebook/libphenom][35-7] - An eventing framework for building high performance and high scalability systems in C. [`Apache 2`][35-8]
  * [libuv/libuv][35-9] - Cross-platform asychronous I/O. [`Licenses`][35-10]

  [35-10]: https://github.com/libuv/libuv/blob/v1.x/LICENSE
  [35-9]: https://github.com/libuv/libuv
  [35-8]: https://github.com/facebookarchive/libphenom/blob/master/LICENSE
  [35-7]: https://github.com/facebookarchive/libphenom/
  [35-6]: https://github.com/Lupus/libevfibers/blob/master/LICENSE
  [35-5]: https://github.com/Lupus/libevfibers
  [35-4]: http://libevent.org/LICENSE.txt
  [35-3]: http://libevent.org/
  [35-2]: http://cvs.schmorp.de/libev/LICENSE?view=markup
  [35-1]: http://software.schmorp.de/pkg/libev.html
</details>

<a id="ffi"></a>
<details>
  <summary>Foreign Function Interfaces</summary>

  ## <a href="#-">`^`</a> Foreign Function Interfaces ##
  * [GNU Libffcall][36-1] - Collection of libraries for building foreign
  function interfaces. [`GPL 3`][36-2]
  * [dyncall][36-3] - Another foreign function interface library. [`License`][36-4]
  * [atgreen/libffi][36-5] - A portable foreign-function interface library. [`License`][36-6]
  * [dyu/ffi-overhead][36-7] - comparing the c ffi overhead on various
  programming languages. [`Apache 2`][36-8]
  * [jmckaskill/luaffi][36-9] - Standalone FFI library for calling C functions
  from lua. Compatible with the luajit FFI interface. [`License`][36-10]
  * [taviso/ctypes.sh][36-11] - A foreign function interface for bash. [`MIT`][36-12]

  [36-12]: https://github.com/taviso/ctypes.sh/blob/master/COPYING
  [36-11]: https://github.com/taviso/ctypes.sh
  [36-10]: https://github.com/jmckaskill/luaffi/blob/master/ffi.h
  [36-9]: https://github.com/jmckaskill/luaffi
  [36-8]: https://github.com/dyu/ffi-overhead/blob/master/LICENSE
  [36-7]: https://github.com/dyu/ffi-overhead
  [36-6]: https://github.com/atgreen/libffi/blob/master/LICENSE
  [36-5]: https://github.com/atgreen/libffi
  [36-4]: http://hg.dyncall.org/pub/dyncall/dyncall/file/b104c5beec8b/LICENSE
  [36-3]: http://www.dyncall.org/
  [36-2]: https://www.gnu.org/software/libffcall/
  [36-1]: https://gnu.org/software/libffcall/
</details>

--------------------------------------------------------------------------------

<a id="filetype-targets"></a>
## Filetype Targets ##
Libraries for working with specific filetypes or classes of filetypes.

<a id="binaries"></a>
<details>
  <summary>╠════ Binaries</summary>

  ### <a href="#-">`^`</a> Binaries ###
  * [bfd][37-1] - Library for manipulating binary object files. Part of GNU
  binutils. [`Licenses`][37-2]
  * [0intro/libelf][37-3] - Simple library for parsing ELF files. [`MIT`][37-4]
  * [fuzxxl/memf][37-5] - Portable scanf/printf-like functions to marshal
  binary data. [`BSD 2-Clause`][37-6]
  * [nicklockwood/FastCoding][37-7] - A faster and more flexible binary file
  format replacement for NSCoding, Property Lists and JSON. [`License`][37-8]
  * [abiggerhammer/hammer][37-9] - Parser combinators for binary formats. [`GPL 2`][37-10]

  [37-10]: https://github.com/abiggerhammer/hammer/blob/master/LICENSE
  [37-9]: https://github.com/abiggerhammer/hammer
  [37-8]: https://github.com/nicklockwood/FastCoding/blob/master/LICENCE.md
  [37-7]: https://github.com/nicklockwood/FastCoding
  [37-6]: https://github.com/fuzxxl/memf/blob/master/COPYING
  [37-5]: https://github.com/fuzxxl/memf
  [37-4]: https://github.com/0intro/libelf/blob/master/LICENSE
  [37-3]: https://github.com/0intro/libelf
  [37-2]: https://sourceware.org/git/gitweb.cgi?p=binutils-gdb.git;a=tree
  [37-1]: https://www.gnu.org/software/binutils/
</details>

<a id="csv"></a>
<details>
  <summary>╠════ CSV</summary>

  ### <a href="#-">`^`</a> CSV ###
  * [rgamble/libcsv][38-1] - Simple, streaming CSV parser. [`LGPL 2.1`][38-2]
  * [tadasv/csv_parser][38-3] - Callback based (SAX like) CSV Parser for C. [`MIT`][38-4]

  [38-4]: https://github.com/tadasv/csv_parser/blob/master/LICENSE
  [38-3]: https://github.com/tadasv/csv_parser
  [38-2]: https://github.com/rgamble/libcsv/blob/master/LICENSE
  [38-1]: https://github.com/rgamble/libcsv
</details>

<a id="json"></a>
<details>
  <summary>╠════ JSON</summary>

  ### <a href="#-">`^`</a> JSON ###
  * [NeonMercury/jfes][39-1] - JSON For Embedded Systems; simple JSON engine
  without any dependencies. [`MIT`][39-2]
  * [zserge/jsmn][39-3] - Minimalistic JSON parser. [`MIT`][39-4]
  * [netmail-open/wjelement][39-5] - Advanced JSON manipulation library, with
  support for JSON Schema. [`Licenses`][39-6]
  * [DaveGamble/cJSON][39-7] - Ultralightweight JSON parser in ANSI C. [`MIT`][39-8]
  * [akheron/jansson][39-9] - C library for encoding, decoding and manipulating
  JSON data. [`MIT`][39-10]
  * [armink/struct2json][39-11] - A fast convert library between the JSON and C
  structure. Implement structure serialization and deserialization for C. [`MIT`][39-12]
  * [cesanta/frozen][39-13] - JSON parser and generator for C/C++ with
  scanf/printf like interface. Targeting embedded systems. [`Apache 2`][39-14]
  * [cloudflare/lua-resty-json][39-15] - json lib for lua and C. [`BSD 2-Clause`][39-16]
  * [json-c/json-c][39-17] - Official code repository for json-c. [`License`][39-18]
  * [keenerd/jshon][39-19] - JSON parser designed for maximum convenience within
  the shell. [`MIT`][39-20]
  * [kgabis/parson][39-21] - Lightweight JSON library written in C. [`MIT`][39-22]
  * [kevinbirch/kanabo][39-23] - query JSON/YAML data with JSONPath. [`License`][39-24]
  * [lloyd/yajl][39-25] - A fast streaming JSON parsing library in C. [`ISC`][39-26]
  * [orangeduck/json2c][39-27] - Convert JSON to C data literals. [`BSD 3-Clause`][39-28]
  * [quartzjer/js0n][39-29] - Flexible Zero-Footprint JSON Parser in C. [`Unlicense`][39-30]
  * [sheredom/json.h][39-31] - json parser for C and C++. [`Unlicense`][39-32]
  * [vincenthz/libjson][39-33] - a JSON parser and printer library in C. Easy to
  integrate with any model. [`License`][39-34]
  * [udp/json-parser][39-35] - Very low footprint JSON parser written in
  portable ANSI. [`License`][39-36]

  [39-36]: https://github.com/udp/json-parser/blob/master/LICENSE
  [39-35]: https://github.com/udp/json-parser
  [39-34]: https://github.com/vincenthz/libjson/blob/master/json.h
  [39-33]: https://github.com/vincenthz/libjson
  [39-32]: https://github.com/sheredom/json.h/blob/master/LICENSE
  [39-31]: https://github.com/sheredom/json.h/
  [39-30]: https://github.com/quartzjer/js0n/blob/master/UNLICENSE
  [39-29]: https://github.com/quartzjer/js0n
  [39-28]: https://github.com/orangeduck/json2c/blob/master/LICENSE
  [39-27]: https://github.com/orangeduck/json2c
  [39-26]: https://github.com/lloyd/yajl/blob/master/COPYING
  [39-25]: https://github.com/lloyd/yajl
  [39-24]: https://github.com/kevinbirch/kanabo/blob/master/LICENSE.md
  [39-23]: https://github.com/kevinbirch/kanabo
  [39-22]: https://github.com/kgabis/parson/blob/master/LICENSE
  [39-21]: https://github.com/kgabis/parson
  [39-20]: https://github.com/keenerd/jshon/blob/master/LICENSE
  [39-19]: https://github.com/keenerd/jshon
  [39-18]: https://github.com/json-c/json-c/blob/master/COPYING
  [39-17]: https://github.com/json-c/json-c
  [39-16]: https://github.com/cloudflare/lua-resty-json/blob/master/LICENSE
  [39-15]: https://github.com/cloudflare/lua-resty-json
  [39-14]: https://github.com/cesanta/frozen/blob/master/LICENSE
  [39-13]: https://github.com/cesanta/frozen
  [39-12]: https://github.com/armink/struct2json/blob/master/LICENSE
  [39-11]: https://github.com/armink/struct2json
  [39-10]: https://github.com/akheron/jansson/blob/master/LICENSE
  [39-9]: https://github.com/akheron/jansson
  [39-8]: https://github.com/DaveGamble/cJSON/blob/master/LICENSE
  [39-7]: https://github.com/DaveGamble/cJSON
  [39-6]: https://github.com/netmail-open/wjelement
  [39-5]: https://github.com/netmail-open/wjelement
  [39-4]: https://github.com/zserge/jsmn/blob/master/LICENSE
  [39-3]: https://github.com/zserge/jsmn
  [39-2]: https://github.com/NeonMercury/jfes/blob/master/LICENSE
  [39-1]: https://github.com/NeonMercury/jfes
</details>

<a id="ini"></a>
<details>
  <summary>╠════ INI</summary>

  ### <a href="#-">`^`</a> INI ###
  * [ndevilla/iniparser][40-1] - Parser for .ini files. [`MIT`][40-2]
  * [madmurphy/libconfini][40-3] - Yet another INI parser. [`GPL 3`][40-4]
  * [benhoyt/inih][40-5] - Simple .INI file parser in C, good for embedded
  systems. [`License`][40-6]

  [40-6]: https://github.com/benhoyt/inih/blob/master/LICENSE.txt
  [40-5]: https://github.com/benhoyt/inih
  [40-4]: https://github.com/madmurphy/libconfini/blob/master/COPYING
  [40-3]: https://github.com/madmurphy/libconfini
  [40-2]: https://github.com/ndevilla/iniparser/blob/master/LICENSE
  [40-1]: https://github.com/ndevilla/iniparser
</details>

<a id="markdown"></a>
<details>
  <summary>╠════ Markdown</summary>

  ### <a href="#-">`^`</a> Markdown ###
  * [hoedown/hoedown][41-1] - Fully standards-compliant, extension-supporting,
  UTF-8 aware, fast Markdown parser. [`ISC`][41-2]
  * [commonmark/cmark][41-3] - Library for parsing the CommonMark dialect of
  Markdown. [`License`][41-4]
  * [Orc/discount][41-5]- My C implementation of John Gruber's Markdown markup
  language. [`License`][41-6]
  * [commonsguy/cwac-anddown][41-7] - CWAC AndDown: Markdown Utility Library. [`Apache 2`][41-8]
  * [fletcher/MultiMarkdown-6][41-9] - Lightweight markup processor to produce
  HTML, LaTeX, and more. [`License`][41-10]
  * [jgm/peg-markdown][41-11] - An implementation of markdown in C, using a
  PEG grammar. [`Licenses`][41-12]
  * [vmg/sundown][41-13] - Standards compliant, fast, secure markdown processing
  library in C. [`License`][41-14]

  [41-14]: https://github.com/vmg/sundown#license
  [41-13]: https://github.com/vmg/sundown
  [41-12]: https://github.com/jgm/peg-markdown/blob/master/LICENSE
  [41-11]: https://github.com/jgm/peg-markdown
  [41-10]: https://github.com/fletcher/MultiMarkdown-6/blob/develop/LICENSE.txt
  [41-9]: https://github.com/fletcher/MultiMarkdown-6
  [41-8]: https://github.com/commonsguy/cwac-anddown/blob/master/LICENSE
  [41-7]: https://github.com/commonsguy/cwac-anddown
  [41-6]: https://github.com/Orc/discount/blob/master/COPYRIGHT
  [41-5]: https://github.com/Orc/discount
  [41-4]: https://github.com/commonmark/cmark/blob/master/COPYING
  [41-3]: https://github.com/commonmark/cmark
  [41-2]: https://github.com/hoedown/hoedown/blob/master/LICENSE
  [41-1]: https://github.com/hoedown/hoedown
</details>

<a id="xml"></a>
<details>
  <summary>╠════ XML</summary>

  ### <a href="#-">`^`</a> XML ###
  * [libexpat/libexpat][42-1] - Stream-oriented XML parser. [`License`][42-2]
  * [libxml2][42-3] - Standards-compliant, portable XML parser. [`MIT`][42-4]
  * [michaelrsweet/mxml][42-5] - Small XML reading and writing library.
  No dependencies aside from C standard library. [`Apache 2`][42-6]

  [42-6]: https://github.com/michaelrsweet/mxml/blob/master/LICENSE
  [42-5]: https://github.com/michaelrsweet/mxml
  [42-4]: https://gitlab.gnome.org/GNOME/libxml2/blob/master/Copyright
  [42-3]: http://xmlsoft.org/
  [42-2]: https://github.com/libexpat/libexpat/blob/master/expat/COPYING
  [42-1]: https://github.com/libexpat/libexpat
</details>

<a id="other-filetypes"></a>
<details>
  <summary>╚════ Other Filetypes</summary>

  ### <a href="#-">`^`</a> Other Filetypes ###
  * [yaml/libyaml][43-1] - Canonical source repository for LibYAML. [`MIT`][43-2]
  * [mongodb/libbson][43-3] - BSON utility library. [`Apache 2`][43-4]
  * [martinh/libconfuse][43-5] - Small configuration file parser library. [`ISC`][43-6]
  * [vstakhov/libucl][43-7] - Universal configuration library parser. [`BSD 2-Clause`][43-8]
  * [Juniper/libxo][43-9] - Allows an application to generate plain text, XML,
  JSON and HTML output using a common set of function calls. The application
  decides at runtime what output style should be produced. [`BSD 2-Clause`][43-10]
  * [brechtsanders/xlsxio][43-11] - Cross-platform library for reading and
  writing .xlsx files. [`MIT`][43-12]
  * [arrbee/diff-match-patch-c][43-13] - C language port of
  google-diff-match-patch library. [`License`][43-14]
  * [hyperrealm/libconfig][43-15] - C/C++ library for processing configuration
  files. [`LGPL 2.1`][43-16]
  * [jedwing/CHMLib][43-17] - Library for reading Microsoft ITSS/CHM format
  files. [`LGPL 2.1`][43-18]
  * [jmcnamara/libxlsxwriter][43-19] - A C library for creating
  Excel XLSX files. [`License`][43-20]
  * [libharu/libharu][43-21] - Free PDF library. [`Zlib`][43-22]
  * [samtools/htslib][43-23] - C library for high-throughput sequencing data
  formats. [`License`][43-24]

  [43-24]: https://github.com/samtools/htslib/blob/develop/LICENSE
  [43-23]: https://github.com/samtools/htslib
  [43-22]: https://github.com/libharu/libharu/blob/master/LICENCE
  [43-21]: https://github.com/libharu/libharu
  [43-20]: https://github.com/jmcnamara/libxlsxwriter/blob/master/License.txt
  [43-19]: https://github.com/jmcnamara/libxlsxwriter
  [43-18]: https://github.com/jedwing/CHMLib/blob/master/COPYING
  [43-17]: https://github.com/jedwing/CHMLib
  [43-16]: https://github.com/hyperrealm/libconfig/blob/master/LICENSE
  [43-15]: https://github.com/hyperrealm/libconfig
  [43-14]: https://github.com/arrbee/diff-match-patch-c/blob/master/LICENSE
  [43-13]: https://github.com/arrbee/diff-match-patch-c
  [43-12]: https://github.com/brechtsanders/xlsxio/blob/master/LICENSE.txt
  [43-11]: https://github.com/brechtsanders/xlsxio
  [43-10]: https://github.com/Juniper/libxo/blob/master/LICENSE
  [43-9]: https://github.com/Juniper/libxo
  [43-8]: https://github.com/vstakhov/libucl/blob/master/COPYING
  [43-7]: https://github.com/vstakhov/libucl
  [43-6]: https://github.com/martinh/libconfuse/blob/master/LICENSE
  [43-5]: https://github.com/martinh/libconfuse
  [43-4]: https://github.com/mongodb/libbson/blob/master/COPYING
  [43-3]: https://github.com/mongodb/libbson
  [43-2]: https://github.com/yaml/libyaml/blob/master/LICENSE
  [43-1]: https://github.com/yaml/libyaml
</details>

--------------------------------------------------------------------------------

<a id="flow-control"></a>
<details>
  <summary>Flow Control and Language Extension</summary>

  ## <a href="#-">`^`</a> Flow Control and Language Extension ##
  * [orangeduck/Cello][44-1] - Library introducing higher-level
  programming to C. [`BSD 2-Clause`][44-2]
  * [Ragel][44-3] - DSL for state machines that compiles to C. [`License`][44-4]
  * [kitsune-dsu/kitsune-core][44-5] - Efficient, general-purpose framework for
  dynamic software updating. [`License`][44-6]
  * [P99][44-7] - Suite of macros to implement advanced features like default
  function arguments, scope-bound resources, etc. [`License`][44-8]
  * [CObjectSystem/COS][44-9] - C Object System. [`Apache 2`][44-10]
  * [H2CO3/Sparkling][44-11] - Lightweight extension language. [`BSD 2-Clause`][44-12]
  * [lua/lua][44-13] - Embeddable scripting programming language. [`License`][44-14]
  * [Zeex/subhook][44-15] - Simple hooking library for C/C++
  (x86 only, 32/64-bit, no dependencies). [`BSD 2-Clause`][44-16]
  * [arnaudbrejeon/cspec][44-17] - Behavior driven development in C. [`GPL 3`][44-18]
  * [comex/substitute][44-19] - A free runtime modification library. [`License`][44-20]
  * [elua/elua][44-21] - Highly portable version of Lua. [`License`][44-22]
  * [eudoxia0/magma][44-23] - Extending C with cmacro. [`License`][44-24]
  * [graphitemaster/lambdapp][44-25] - Anonymous functions in C. [`Unlicense`][44-26]
  * [guillermocalvo/exceptions4c][44-27] - Exception handling framework for C. [`LGPL 3`][44-28]
  * [orangeduck/LuaAutoC][44-29] - Automagically use C Functions and Structs
  with the Lua API. [`License`][44-30]
  * [pfultz2/Cloak][44-31] - A mini-preprocessor library to demostrate the
  recursive capabilites of the preprocessor. [`Boost`][44-32]
  * [skeeto/interactive-c-demo][44-33] - Demonstration of interactive
  C programming. [`Unlicense`][44-34]
  * [symisc/PH7][44-35] - An Embedded Implementation of PHP (C Library). [`License`][44-36]
  * [yasm/yasm][44-37] - Provides libyasm - embeddable YASM engine. [`License`][44-38]
  * [zserge/partcl][44-39] - Micro Tcl implementation. [`MIT`][44-40]
  * [cesanta/mjs][44-41] - Embedded JavaScript engine for C/C++. [`License`][44-42]
  * [graphitemaster/incbin][44-43] - Include binary files in C/C++. [`Unlicense`][44-44]
  * [pkrumins/bithacks.h][44-45] - bithacks.h is a C header file containing
  useful bit manipulation macros. [`MIT`][44-46]
  * [breckinloggins/ngtemplate][44-47] - A template engine written in C designed
  to be syntax-compatible with Google CTemplate. [`MIT`][44-48]

  [44-48]: https://github.com/breckinloggins/ngtemplate/blob/master/LICENSE
  [44-47]: https://github.com/breckinloggins/ngtemplate
  [44-46]: https://github.com/pkrumins/bithacks.h/blob/master/bithacks.h
  [44-45]: https://github.com/pkrumins/bithacks.h
  [44-44]: https://github.com/graphitemaster/incbin/blob/master/UNLICENSE
  [44-43]: https://github.com/graphitemaster/incbin
  [44-42]: https://github.com/cesanta/mjs/blob/master/LICENSE
  [44-41]: https://github.com/cesanta/mjs
  [44-40]: https://github.com/zserge/partcl/blob/master/LICENSE
  [44-39]: https://github.com/zserge/partcl
  [44-38]: https://github.com/yasm/yasm/blob/master/COPYING
  [44-37]: https://github.com/yasm/yasm
  [44-36]: https://github.com/symisc/PH7/blob/master/license.txt
  [44-35]: https://github.com/symisc/PH7
  [44-34]: https://github.com/skeeto/interactive-c-demo/blob/master/UNLICENSE
  [44-33]: https://github.com/skeeto/interactive-c-demo
  [44-32]: https://github.com/pfultz2/Cloak/blob/master/cloak.h
  [44-31]: https://github.com/pfultz2/Cloak
  [44-30]: https://github.com/orangeduck/LuaAutoC/blob/master/LICENSE.md
  [44-29]: https://github.com/orangeduck/LuaAutoC
  [44-28]: https://github.com/guillermocalvo/exceptions4c/blob/master/COPYING
  [44-27]: https://github.com/guillermocalvo/exceptions4c
  [44-26]: https://github.com/graphitemaster/lambdapp/blob/master/LICENSE
  [44-25]: https://github.com/graphitemaster/lambdapp
  [44-24]: https://github.com/eudoxia0/magma#id40
  [44-23]: https://github.com/eudoxia0/magma
  [44-22]: https://github.com/elua/elua/blob/master/LICENSE
  [44-21]: https://github.com/elua/elua
  [44-20]: https://github.com/comex/substitute/blob/master/LICENSE.txt
  [44-19]: https://github.com/comex/substitute
  [44-18]: https://github.com/arnaudbrejeon/cspec/blob/master/COPYING
  [44-17]: https://github.com/arnaudbrejeon/cspec
  [44-16]: https://github.com/Zeex/subhook/blob/master/LICENSE.txt
  [44-15]: https://github.com/Zeex/subhook
  [44-14]: https://www.lua.org/license.html
  [44-13]: https://github.com/lua/lua
  [44-12]: https://github.com/H2CO3/Sparkling/blob/master/LICENSE.txt
  [44-11]: https://github.com/H2CO3/Sparkling
  [44-10]: https://github.com/CObjectSystem/COS/blob/master/LICENSE
  [44-9]: https://github.com/CObjectSystem/COS
  [44-8]: http://p99.gforge.inria.fr/p99-html/
  [44-7]: http://p99.gforge.inria.fr/
  [44-6]: https://github.com/kitsune-dsu/kitsune-core/blob/master/LICENSE
  [44-5]: http://kitsune-dsu.com/
  [44-4]: https://www.colm.net/open-source/ragel/
  [44-3]: https://www.colm.net/open-source/ragel/
  [44-2]: https://github.com/orangeduck/Cello/blob/master/LICENSE.md
  [44-1]: https://github.com/orangeduck/Cello
</details>

--------------------------------------------------------------------------------

<a id="gamedev"></a>
## Game Development ##
Engines, libraries and other helpful things specifically for making games.

<a id="gamedev-engines"></a>
<details>
  <summary>╠════ Game Engines</summary>

  ### <a href="#-">`^`</a> Game Engines ###
  * [xonotic/darkplaces][45-1] - Modified version of the Quake2 engine. [`GPL 2`][45-2]
  * [ioquake/ioq3][45-3] - The Quake3 engine, freed at last. [`GPL 2`][45-4]
  * [orx/orx][45-5] - Portable, lightweight, plugin-based, data-driven,
  2D-oriented game engine. [`License`][45-6]
  * [zturtleman/spearmint][45-7] - Engine designed for FPS games. [`GPL 3`][45-8]
  * [Gigoteur/UnicornConsole][45-9] - Unicorn Console: create quick game! [`MIT`][45-10]
  * [MarilynDafa/Bulllord-Engine][45-11] - lightspeed lightweight elegant game
  engine in pure c. [`MIT`][45-12]
  * [HerculesWS/Hercules][45-13] - Creation of a robust massively multiplayer
  online role playing game (MMORPG) server package. [`GPL 3`][45-14]
  * [Olde-Skuul/doom3do][45-15] - The complete archive for DOOM for the 3DO. [`MIT`][45-16]
  * [RandyGaul/AsciiEngine][45-17] - Game engine written in C to create Ascii
  art games within the Windows console. [`MIT`][45-18]
  * [littlewolf][45-19] - The tiny software graphics and game engine. [`MIT`][45-20]
  * [eduard-permyakov/permafrost-engine][45-21] - An OpenGL 3.3 RTS game engine
  written in C. [`GPL 3`][45-22]
  * [ejoy/ejoy2d][45-23] - A 2D Graphics Engine for Mobile Game. [`MIT`][45-24]
  * [etlegacy/etlegacy][45-25] - ET: Legacy is based on the source code of the
  Wolfenstein: Enemy Territory which was released under the GPLv3 license. [`GPL 3`][45-26]
  * [fabiensanglard/chocolate_duke3D][45-27] - chocolate Duke Nukem 3D. [`License`][45-28]
  * [a-nikolaev/curseofwar][45-29] - A Real Time Strategy game for Linux. [`GPL 3`][45-30]
  * [chocolate-doom/chocolate-doom][45-31] - Chocolate Doom is a Doom source
  port that is minimalist and historically accurate. [`GPL 2`][45-32]
  * [cxong/cdogs-sdl][45-33] - Classic overhead run-and-gun game. [`GPL 2`][45-34]
  * [fogleman/Craft][45-35] - A simple Minecraft clone written in C using modern
  OpenGL (shaders). [`MIT`][45-36]
  * [id-Software/DOOM][45-37] - DOOM Open Source Release. [`License`][45-38]
  * [id-Software/Quake-2][45-39] - Quake 2 GPL Source Release. [`GPL 2`][45-40]
  * [id-Software/Quake-III-Arena][45-41] - Quake III Arena GPL Source Release. [`GPL 2`][45-42]
  * [id-Software/Quake][45-43] - Quake GPL Source Release. [`GPL 2`][45-44]
  * [keendreams/keen][45-45] - Keen Dreams on Greenlight! [`GPL 2`][45-46]
  * [linleyh/liberation-circuit][45-47] - Trapped in a hostile computer system,
  you must make a way out - RTS/coding game. [`GPL 3`][45-48]
  * [martincohen/Punity][45-49] - A tiny game engine in C. [`MIT`][45-50]
  * [orangeduck/Corange][45-51] - Pure C Game Engine. [`License`][45-52]
  * [naev/naev][45-53] - Naev is a 2d action/rpg space game that combines
  elements from the action, rpg and simulation genres. [`GPL 3`][45-54]
  * [nikki93/cgame][45-55] - some ideas involving games and C. `No license`
  * [scottcgi/Mojoc][45-56] - A cross-platform, open-source, pure C  game engine
  for mobile game. [`MIT`][45-57]
  * [septag/darkhammer][45-58] - darkHAMMER is a lightweight, open-source,
  multiplatform game engine. written in C (C99) language, supports python
  and C# bindings and lua scripts. [`License`][45-59]
  * [taylor001/crown][45-60] - The flexible game engine. [`MIT`][45-61]
  * [theunamedguy/market-sim][45-62] - A retro stock-trading game utilizing
  live market data. [`GPL 2`][45-63]
  * [tpoindex/crobots][45-64] - CROBOTS is a programming game, for programmers
  (or aspiring programmers). [`GPL 2`][45-65]
  * [andwn/cave-story-md][45-66] - A fan port of Cave Story for the
  Sega Mega Drive. [`License`][45-67]
  * [angband/angband][45-68] - A free, single-player roguelike dungeon exploration game. [`License`][45-69]
  * [nesbox/tic.computer][45-70] - Public TIC-80 issues tracker. [`MIT`][45-71]
  * [q2vkpt][45-72] - Real-time path tracer VKPT integrated into q2pro Quake 2 client. [`GPL 2`][45-73]

  [45-73]: https://github.com/cschied/q2vkpt/blob/master/LICENSE
  [45-72]: https://github.com/cschied/q2vkpt
  [45-71]: https://github.com/nesbox/TIC-80/blob/master/LICENSE
  [45-70]: https://github.com/nesbox/TIC-80
  [45-69]: https://github.com/angband/angband/blob/master/copying.txt
  [45-68]: https://github.com/angband/angband
  [45-67]: https://github.com/andwn/cave-story-md/blob/master/doc/LICENSE.md
  [45-66]: https://github.com/andwn/cave-story-md
  [45-65]: https://github.com/tpoindex/crobots/blob/master/LICENSE
  [45-64]: https://github.com/tpoindex/crobots
  [45-63]: https://github.com/built1n/market-sim/blob/master/LICENSE
  [45-62]: https://github.com/built1n/market-sim
  [45-61]: https://github.com/dbartolini/crown/blob/master/LICENSE
  [45-60]: https://github.com/dbartolini/crown
  [45-59]: https://github.com/septag/darkhammer/blob/master/LICENSE
  [45-58]: https://github.com/septag/darkhammer
  [45-57]: https://github.com/scottcgi/Mojoc/blob/master/LICENSE
  [45-56]: https://github.com/scottcgi/Mojoc
  [45-55]: https://github.com/nikki93/cgame
  [45-54]: https://github.com/naev/naev/blob/master/LICENSE
  [45-53]: https://github.com/naev/naev
  [45-52]: https://github.com/orangeduck/Corange/blob/master/LICENCE.md
  [45-51]: https://github.com/orangeduck/Corange
  [45-50]: https://github.com/martincohen/Punity/blob/master/LICENSE.md
  [45-49]: https://github.com/martincohen/Punity
  [45-48]: https://github.com/linleyh/liberation-circuit/blob/master/LICENSE.md
  [45-47]: https://github.com/linleyh/liberation-circuit
  [45-46]: https://github.com/keendreams/keen/blob/master/LICENSE
  [45-45]: https://github.com/keendreams/keen
  [45-44]: https://github.com/id-Software/Quake/blob/master/gnu.txt
  [45-43]: https://github.com/id-Software/Quake
  [45-42]: https://github.com/id-Software/Quake-III-Arena/blob/master/COPYING.txt
  [45-41]: https://github.com/id-Software/Quake-III-Arena
  [45-40]: https://github.com/id-Software/Quake-2/blob/master/gnu.txt
  [45-39]: https://github.com/id-Software/Quake-2
  [45-38]: https://github.com/id-Software/DOOM/blob/master/linuxdoom-1.10/DOOMLIC.TXT
  [45-37]: https://github.com/id-Software/DOOM
  [45-36]: https://github.com/fogleman/Craft/blob/master/LICENSE.md
  [45-35]: https://github.com/fogleman/Craft
  [45-34]: https://github.com/cxong/cdogs-sdl/blob/master/COPYING
  [45-33]: https://github.com/cxong/cdogs-sdl
  [45-32]: https://github.com/chocolate-doom/chocolate-doom/blob/master/COPYING.md
  [45-31]: https://github.com/chocolate-doom/chocolate-doom
  [45-30]: https://github.com/a-nikolaev/curseofwar/blob/master/LICENSE
  [45-29]: https://github.com/a-nikolaev/curseofwar
  [45-28]: https://github.com/fabiensanglard/chocolate_duke3D/blob/master/Game/src/duke3d.h
  [45-27]: https://github.com/fabiensanglard/chocolate_duke3D
  [45-26]: https://github.com/etlegacy/etlegacy/blob/master/COPYING.txt
  [45-25]: https://github.com/etlegacy/etlegacy
  [45-24]: https://github.com/ejoy/ejoy2d/blob/master/LICENSE
  [45-23]: https://github.com/ejoy/ejoy2d
  [45-22]: https://github.com/eduard-permyakov/permafrost-engine/blob/master/LICENSE.txt
  [45-21]: https://github.com/eduard-permyakov/permafrost-engine
  [45-20]: https://github.com/glouw/littlewolf/blob/master/LICENSE
  [45-19]: https://github.com/glouw/littlewolf
  [45-18]: https://github.com/RandyGaul/AsciiEngine/blob/master/LICENSE.txt
  [45-17]: https://github.com/RandyGaul/AsciiEngine
  [45-16]: https://github.com/Olde-Skuul/doom3do/blob/master/LICENSE
  [45-15]: https://github.com/Olde-Skuul/doom3do
  [45-14]: https://github.com/HerculesWS/Hercules/blob/stable/LICENSE
  [45-13]: https://github.com/HerculesWS/Hercules
  [45-12]: https://github.com/MarilynDafa/Bulllord-Engine/blob/master/LICENSE
  [45-11]: https://github.com/MarilynDafa/Bulllord-Engine
  [45-10]: https://github.com/Gigoteur/UnicornConsole/blob/master/LICENSE.md
  [45-9]: https://github.com/Gigoteur/UnicornConsole
  [45-8]: https://github.com/zturtleman/spearmint/blob/master/COPYING.txt
  [45-7]: https://github.com/zturtleman/spearmint
  [45-6]: https://github.com/orx/orx/blob/master/LICENSE
  [45-5]: https://github.com/orx/orx
  [45-4]: https://github.com/ioquake/ioq3/blob/master/COPYING.txt
  [45-3]: https://github.com/ioquake/ioq3
  [45-2]: https://github.com/xonotic/darkplaces/blob/master/COPYING
  [45-1]: https://github.com/xonotic/darkplaces
</details>

<a id="gamedev-rendering"></a>
<details>
  <summary>╠════ Graphics Rendering</summary>

  ### <a href="#-">`^`</a> Graphics Rendering ###
  Everything related to video rendering only. Also visit
  [awesome-opengl](https://github.com/eug/awesome-opengl) and
  [awesome-vulkan](https://github.com/vinjn/awesome-vulkan).
  * [grimfang4/sdl-gpu][46-1] - Library for high-performance, modern 2D
  graphics. Based on SDL. [`MIT`][46-2]
  * [dcnieho/FreeGLUT][46-3] - Alternative to the OpenGL Utility Toolkit. Allows
  the creation and management of windows with OpenGL contexts. [`License`][46-4]
  * [MauriceGit/Cloth_Simulation][46-5] - Cloth-Visualization via
  particle-simulation. [`ISC`][46-6]
  * [MauriceGit/Partikel_accelleration_on_GPU][46-7] - Particle accelleration
  with OpenGL 4.3, using the compute shader to calculate particle movement on
  graphics hardware. [`ISC`][46-8]
  * [ands/lightmapper][46-9] - A C/C++ single-file library for drop-in lightmap
  baking. Just use your existing OpenGL renderer to bounce light! [`Public domain`][46-10]
  * [ands/seamoptimizer][46-11] - A C/C++ single-file library that minimizes the
  hard transition errors of disjoint edges in lightmaps. [`Public domain`][46-12]
  * [ebassi/graphene][46-13] - A thin layer of graphic data types. [`MIT`][46-14]
  * [cacalabs/libcaca][46-15] - ASCII renderer for terminal-based interfaces. [`WTFPL`][46-16]
  * [OpenGL][46-17] - Industry adopted 2D and 3D graphics API. `Graphics API`
  * [OpenGL ES][46-18] - Industry adopted 2D and 3D graphics API for mobile and
  embedded devices. `Graphics API`
  * [OpenGL SC][46-19] - Graphic and compute standard for industry requiring
  system safety certification. `Graphics API`
  * [Vulkan][46-20] - Explicit graphic and compute API for modern cross-platform
  development. `Graphics API`
  * [Cairo][46-21] -2D graphics library. [`Licenses`][46-22]
  * [Cogl][46-23] - GPU graphics and utilities API. [`License`][46-24]
  * [glfw/glfw][46-25] - A multi-platform library for OpenGL, OpenGL ES, Vulkan,
  window and input. [`Zlib`][46-26]
  * [nigels-com/glew][46-27] - The OpenGL Extension Wrangler Library. [`License`][46-28]
  * [anoek/ex-sdl-cairo-freetype-harfbuzz][46-29] - Example code which uses SDL,
  cairo, freetype, and harfbuzz to do ttf/otf text layout and rendering. `No license`
  * [ashima/webgl-noise][46-30] - Procedural Noise Shader Routines compatible
  with WebGL. [`MIT`][46-31]
  * [grz0zrg/fbg][46-32] - Lightweight C 2D graphics API agnostic library with
  parallelism support. [`BSD 3-Clause`][46-33]
  * [ileben/ShivaVG][46-34] - OpenGL based ANSI C implementation of the OpenVG
  standard. [`LGPL 2.1`][46-35]
  * [jpbruyere/vkvg][46-36] - Vulkan vector drawing, try to stay close to
  cairo api. [`MIT`][46-37]
  * [memononen/nanovg][46-38] - Antialiased 2D vector drawing library on top of
  OpenGL for UI and visualizations. [`Zlib`][46-39]
  * [micahpearlman/MonkVG][46-40] - OpenVG 1.1 like vector graphics API
  implementation optimized for game use currently using an OpenGL ES backend
  that should be compatible with any HW that supports OpenGL ES 2.0 which
  includes most iOS and Android devices. [`License`][46-41]
  * [minusinf/opengl_dataviewer][46-42] - A simple OpenGL xyzw dataviewer. [`GPL 3`][46-43]
  * [rougier/freetype-gl][46-44] - OpenGL text using one vertex buffer, one
  texture and FreeType. [`License`][46-45]
  * [simple2d/simple2d][46-46] - Simple, open-source 2D graphics for everyone. [`MIT`][46-47]
  * [jakogut/tinyflock][46-48] - A simple, high-performance, threaded, and
  interactive flocking demo written in C with GLFW. `No license`
  * [anholt/libepoxy][46-49] - Library for handling OpenGL function pointer
  management. [`License`][46-50]

  [46-50]: https://github.com/anholt/libepoxy/blob/master/COPYING
  [46-49]: https://github.com/anholt/libepoxy
  [46-48]: https://github.com/jakogut/tinyflock
  [46-47]: https://github.com/simple2d/simple2d/blob/master/LICENSE.md
  [46-46]: https://github.com/simple2d/simple2d
  [46-45]: https://github.com/rougier/freetype-gl/blob/master/LICENSE
  [46-44]: https://github.com/rougier/freetype-gl
  [46-43]: https://github.com/pspoerri/opengl_dataviewer/blob/master/src/main.h
  [46-42]: https://github.com/pspoerri/opengl_dataviewer
  [46-41]: https://github.com/micahpearlman/MonkVG/blob/master/LICENSE
  [46-40]: https://github.com/micahpearlman/MonkVG
  [46-39]: https://github.com/memononen/nanovg/blob/master/LICENSE.txt
  [46-38]: https://github.com/memononen/nanovg
  [46-37]: https://github.com/jpbruyere/vkvg/blob/master/LICENSE.md
  [46-36]: https://github.com/jpbruyere/vkvg
  [46-35]: https://github.com/ileben/ShivaVG/blob/master/COPYING
  [46-34]: https://github.com/ileben/ShivaVG
  [46-33]: https://github.com/grz0zrg/fbg/blob/master/LICENSE
  [46-32]: https://github.com/grz0zrg/fbg
  [46-31]: https://github.com/ashima/webgl-noise/blob/master/LICENSE
  [46-30]: https://github.com/ashima/webgl-noise
  [46-29]: https://github.com/anoek/ex-sdl-cairo-freetype-harfbuzz
  [46-28]: https://github.com/nigels-com/glew/blob/master/LICENSE.txt
  [46-27]: https://github.com/nigels-com/glew
  [46-26]: https://github.com/glfw/glfw/blob/master/LICENSE.md
  [46-25]: https://github.com/glfw/glfw
  [46-24]: https://gitlab.gnome.org/GNOME/cogl/blob/master/COPYING
  [46-23]: https://gitlab.gnome.org/GNOME/cogl
  [46-22]: https://www.cairographics.org/
  [46-21]: https://www.cairographics.org/
  [46-20]: https://www.khronos.org/vulkan/
  [46-19]: https://www.khronos.org/openglsc/
  [46-18]: https://www.khronos.org/opengles/
  [46-17]: https://www.opengl.org/
  [46-16]: https://github.com/cacalabs/libcaca/blob/master/COPYING
  [46-15]: https://github.com/cacalabs/libcaca
  [46-14]: https://github.com/ebassi/graphene/blob/master/LICENSE
  [46-13]: https://github.com/ebassi/graphene
  [46-12]: https://github.com/ands/seamoptimizer/blob/master/seamoptimizer.h
  [46-11]: https://github.com/ands/seamoptimizer
  [46-10]: https://github.com/ands/lightmapper/blob/master/lightmapper.h
  [46-9]: https://github.com/ands/lightmapper
  [46-8]: https://github.com/MauriceGit/Partikel_accelleration_on_GPU/blob/master/LICENSE
  [46-7]: https://github.com/MauriceGit/Partikel_accelleration_on_GPU
  [46-6]: https://github.com/MauriceGit/Cloth_Simulation/blob/master/LICENSE
  [46-5]: https://github.com/MauriceGit/Cloth_Simulation
  [46-4]: https://github.com/dcnieho/FreeGLUT/blob/git_master/freeglut/freeglut/COPYING
  [46-3]: https://github.com/dcnieho/FreeGLUT
  [46-2]: https://github.com/grimfang4/sdl-gpu/blob/master/LICENSE.txt
  [46-1]: https://github.com/grimfang4/sdl-gpu
</details>

<a id="gamedev-helping-libraries"></a>
<details>
  <summary>╚════ Gamedev Helping Libraries</summary>

  ### <a href="#-">`^`</a> Gamedev Helping Libraries ###
  * [sigil][47-1] - Sound, Input and Graphics Integration Library; a simple
  alternative to other libraries for doing all those things. Various licenses,
  all open source. [`Licenses`][47-2]
  * [SFML/CSFML][47-3] - Binding for SFML in C. [`License`][47-4]
  * [SDL][47-5] - Cross-platform development library designed to provide
  low-level access to audio, keyboard, mouse, joystick and graphics hardware via
  OpenGL. SDL2 is the most current version. [`Zlib`][47-6]
  * [HBehrens/obj2opengl][47-7] - script to convert 3D models of OBJ files to
  C/C++ float arrays (vertices, faces, texture) compatible with OpenGL ES
  glDrawArrays compatible with iPhone/iPad. [`GPL 3`][47-8]
  * [Kazade/kazmath][47-9] - A C math library targeted at games. [`BSD 2-Clause`][47-10]
  * [R4stl1n/cAudio][47-11] - 3D Audio Engine Based on Openal. [`Zlib`][47-12]
  * [Tangent128/luasdl2][47-13] - A pure C binding of SDL 2.0 for Lua 5.1,
  Lua 5.2, and LuaJIT. [`ISC`][47-14]
  * [ccore/ccore_rewrite][47-15] - A cross platform low level game development
  library. [`BSD 3-Clause`][47-16]
  * [cloudwu/skynet][47-17] - A lightweight online game framework. [`MIT`][47-18]
  * [felselva/mathc][47-19] - Pure C math library for 2D and 3D programming. [`Zlib`][47-20]
  * [gabomdq/SDL_GameControllerDB][47-21] - A community sourced database of game
  controller mappings to be used with SDL2 Game Controller functionality. [`License`][47-22]
  * [geon/gloss][47-23] - A bidirectional path tracer written in C. [`MIT`][47-24]
  * [jarikomppa/soloud][47-25] - Free, easy, portable audio engine for games. [`License`][47-26]
  * [liballeg/allegro5][47-27] - The official Allegro 5 git repository. [`License`][47-28]
  * [recp/cglm][47-29] - Highly Optimized Graphics Math (glm) for C. [`MIT`][47-30]
  * [raysan5/raylib][47-31] - A simple and easy-to-use library to enjoy
  videogames programming. [`Zlib`][47-32]
  * [rxi/lovedos][47-33] - A framework for making 2D DOS games in Lua. [`MIT`][47-34]
  * [slembcke/Chipmunk2D][47-35] - A fast and lightweight 2D game physics
  library. [`MIT`][47-36]
  * [shaunlebron/blinky][47-37] - Exploring peripheral vision in games
  (using Quake). [`MIT`][47-38]
  * [nem0/OpenFBX][47-39] - Lightweight open source FBX importer. [`MIT`][47-40]

  [47-40]: https://github.com/nem0/OpenFBX/blob/master/LICENSE
  [47-39]: https://github.com/nem0/OpenFBX
  [47-38]: https://github.com/shaunlebron/blinky/blob/master/LICENSE
  [47-37]: https://github.com/shaunlebron/blinky
  [47-36]: https://github.com/slembcke/Chipmunk2D/blob/master/LICENSE.txt
  [47-35]: https://github.com/slembcke/Chipmunk2D
  [47-34]: https://github.com/rxi/lovedos/blob/master/LICENSE
  [47-33]: https://github.com/rxi/lovedos
  [47-32]: https://github.com/raysan5/raylib/blob/master/LICENSE.md
  [47-31]: https://github.com/raysan5/raylib
  [47-30]: https://github.com/recp/cglm/blob/master/LICENSE
  [47-29]: https://github.com/recp/cglm
  [47-28]: https://github.com/liballeg/allegro5/blob/master/LICENSE.txt
  [47-27]: https://github.com/liballeg/allegro5
  [47-26]: https://github.com/jarikomppa/soloud/blob/master/LICENSE
  [47-25]: https://github.com/jarikomppa/soloud
  [47-24]: https://github.com/geon/gloss/blob/master/LICENSE.md
  [47-23]: https://github.com/geon/gloss
  [47-22]: https://github.com/gabomdq/SDL_GameControllerDB/blob/master/LICENSE
  [47-21]: https://github.com/gabomdq/SDL_GameControllerDB
  [47-20]: https://github.com/felselva/mathc/blob/master/LICENSE
  [47-19]: https://github.com/felselva/mathc
  [47-18]: https://github.com/cloudwu/skynet/blob/master/LICENSE
  [47-17]: https://github.com/cloudwu/skynet
  [47-16]: https://github.com/ccore/ccore_rewrite/blob/master/LICENSE
  [47-15]: https://github.com/ccore/ccore_rewrite
  [47-14]: https://github.com/Tangent128/luasdl2/blob/master/LICENSE
  [47-13]: https://github.com/Tangent128/luasdl2
  [47-12]: https://github.com/R4stl1n/cAudio/blob/master/License.txt
  [47-11]: https://github.com/R4stl1n/cAudio
  [47-10]: https://github.com/Kazade/kazmath/blob/master/LICENSE.md
  [47-9]: https://github.com/Kazade/kazmath
  [47-8]: https://github.com/HBehrens/obj2opengl/blob/master/LICENSE.txt
  [47-7]: https://github.com/HBehrens/obj2opengl
  [47-6]: https://www.libsdl.org/license.php
  [47-5]: https://www.libsdl.org
  [47-4]: https://github.com/SFML/CSFML/blob/master/license.txt
  [47-3]: https://github.com/SFML/CSFML
  [47-2]: https://gitlab.com/geoff-nagy/sigil/blob/master/LICENSES.txt
  [47-1]: http://www.libsigil.com/
</details>

--------------------------------------------------------------------------------

<a id="geography"></a>
<details>
  <summary>Geography</summary>

  ## <a href="#-">`^`</a> Geography ##
  Geodata, street maps, navigation and so on
  * [Unidata/gempak][48-1] - Analysis, display, and product generation package
  for meteorological data. [`BSD 3-Clause`][48-2]
  * [evanmiller/ProjCL][48-3] - Crazy-fast map projections and geodesic
  calculations. [`License`][48-4]
  * [olofsj/GLMap][48-5] - An OpenGL ES 2.0 renderer for Openstreetmap data. [`LGPL 3`][48-6]
  * [olofsj/Whichway][48-7] - C library for flexible (bike, foot, car) routing
  in road networks from Openstreetmap data. `No license`
  * [maxmind/geoip-api-c][48-8] - GeoIP Legacy C API. [`License`][48-9]
  * [navit-gps/navit][48-10] - The open source (GPL v2) turn-by-turn navigation
  software for many OS. [`License`][48-11]
  * [lionsoul2014/ip2region][48-12] - Offline IP location library with accuracy
  rate of 99.9% and 0.0x millseconds searching performance. DB file is less then
  5Mb with all ip address stored. binding for Java, PHP, C, Python, Nodejs,
  Golang, C#, lua. Binary, B-tree, Memory searching algorithm. [`Apache 2`][48-13]
  * [openvenues/libpostal][48-14] - A C library for parsing/normalizing street
  addresses around the world. Powered by statistical NLP and open geo data. [`MIT`][48-15]
  * [propublica/simple-tiles][48-16] - Simple tile generation for maps. [`MIT`][48-17]
  * [simplegeo/libgeohash][48-18] - A pure C implementation of the Geohash
  algorithm. [`BSD 3-Clause`][48-19]
  * [kosma/minmea][48-20] - Lightweight GPS NMEA 0183 parser library in pure C. [`WTFPL`][48-21]
  * [geocommons/geocoder][48-22] - Modular Street Address Geocoder. [`LGPL 3`][48-23]
  * [bauerca/gridfloat][48-24] - Slice and dice USGS elevation data from the
  command line. [`MIT`][48-25]

  [48-25]: https://github.com/bauerca/gridfloat/blob/master/LICENSE
  [48-24]: https://github.com/bauerca/gridfloat
  [48-23]: https://github.com/geocommons/geocoder/blob/master/LICENSE.txt
  [48-22]: https://github.com/geocommons/geocoder
  [48-21]: https://github.com/kosma/minmea/blob/master/COPYING
  [48-20]: https://github.com/kosma/minmea
  [48-19]: https://github.com/simplegeo/libgeohash/blob/master/LICENSE
  [48-18]: https://github.com/simplegeo/libgeohash
  [48-17]: https://github.com/propublica/simple-tiles/blob/master/LICENSE
  [48-16]: https://github.com/propublica/simple-tiles
  [48-15]: https://github.com/openvenues/libpostal/blob/master/LICENSE
  [48-14]: https://github.com/openvenues/libpostal
  [48-13]: https://github.com/lionsoul2014/ip2region/blob/master/LICENSE.md
  [48-12]: https://github.com/lionsoul2014/ip2region
  [48-11]: https://github.com/navit-gps/navit/blob/trunk/COPYING
  [48-10]: https://github.com/navit-gps/navit
  [48-9]: https://github.com/maxmind/geoip-api-c/blob/master/LICENSE
  [48-8]: https://github.com/maxmind/geoip-api-c
  [48-7]: https://github.com/olofsj/Whichway
  [48-6]: https://github.com/olofsj/GLMap/blob/master/COPYING
  [48-5]: https://github.com/olofsj/GLMap
  [48-4]: https://github.com/evanmiller/ProjCL/blob/master/LICENSE
  [48-3]: https://github.com/evanmiller/ProjCL
  [48-2]: https://github.com/Unidata/gempak/blob/master/LICENSE
  [48-1]: https://github.com/Unidata/gempak
</details>

<a id="gui"></a>
<details>
  <summary>GUI</summary>

  ## <a href="#-">`^`</a> GUI ##
  * [tinyfiledialogs][49-1] - Single-file library for simple dialogs. Compatible
  with many other toolkits and OSes. [`Zlib`][49-2]
  * [vurtun/nuklear][49-3] - A single-header ANSI C gui library. [`Licenses`][49-4]
  * [andlabs/libui][49-5] - Simple and portable (but not inflexible) GUI library
  in C that uses the native GUI technologies of each platform it supports. [`License`][49-6]
  * [lc-soft/LCUI][49-7] - A small C library for building user interfaces with
  C, XML and CSS. [`MIT`][49-8]
  * [littlevgl/lvgl][49-9] - Graphics library to create an embedded GUI with
  easy-to-use graphical elements, beautiful visual effects and low memory
  footprint. It offers anti-aliasing, opacity, and animations using only one
  frame buffer. [`MIT`][49-10]
  * [ocornut/imgui_club][49-11] - Nice things to use along dear imgui. `No license`
  * [GTK+][49-12] - Cross-platform widget toolkit. [`License`][49-13]
  * [IUP][49-14] - Another cross-platform widget toolkit. [`License`][49-15]
  * [Tk][49-16] - Basic widget toolkit. Part of Tcl/Tk. [`License`][49-17]
  * [XForms Toolkit][49-18] - Widget toolkit designed for the XWindow system. [`LGPL 2.1`][49-19]
  * [Clutter][49-20] - UI library based on OpenGL. [`LGPL 2.1`][49-21]
  * [randrew/layout][49-22] - Single-file library for calculating 2D UI layouts
  using stacking boxes. Compiles as C99 or C++. [`License`][49-23]
  * [cimgui/cimgui][49-24] - c-api for imgui. [`MIT`][49-25]

  [49-25]: https://github.com/cimgui/cimgui/blob/master/LICENSE
  [49-24]: https://github.com/cimgui/cimgui
  [49-23]: https://github.com/randrew/layout/blob/master/license.md
  [49-22]: https://github.com/randrew/layout
  [49-21]: https://gitlab.gnome.org/GNOME/clutter/blob/master/COPYING
  [49-20]: https://gitlab.gnome.org/GNOME/clutter
  [49-19]: http://git.savannah.nongnu.org/cgit/xforms.git/tree/COPYING.LIB
  [49-18]: http://xforms-toolkit.org/
  [49-17]: https://github.com/tcltk/tk/blob/master/license.terms
  [49-16]: http://www.tcl.tk/
  [49-15]: http://webserver2.tecgraf.puc-rio.br/iup/en/copyright.html
  [49-14]: http://webserver2.tecgraf.puc-rio.br/iup/
  [49-13]: https://gitlab.gnome.org/GNOME/gtk/blob/master/COPYING
  [49-12]: https://www.gtk.org
  [49-11]: https://github.com/ocornut/imgui_club
  [49-10]: https://github.com/littlevgl/lvgl/blob/master/LICENCE.txt
  [49-9]: https://github.com/littlevgl/lvgl
  [49-8]: https://github.com/lc-soft/LCUI/blob/develop/LICENSE.TXT
  [49-7]: https://github.com/lc-soft/LCUI
  [49-6]: https://github.com/andlabs/libui/blob/master/LICENSE
  [49-5]: https://github.com/andlabs/libui
  [49-4]: https://github.com/vurtun/nuklear#license
  [49-3]: https://github.com/vurtun/nuklear
  [49-2]: https://sourceforge.net/projects/tinyfiledialogs/
  [49-1]: https://sourceforge.net/projects/tinyfiledialogs/
</details>

<a id="hardware-oriented"></a>
<details>
  <summary>Hardware Oriented</summary>

  ## <a href="#-">`^`</a> Hardware Oriented ##
  * [obgm/libcoap][50-1] - Implementation of the Constrained Application
  Protocol. [`License`][50-2]
  * [Genymobile/scrcpy][50-3] - Display and control your Android device. [`Apache 2`][50-4]
  * [Azure/azure-iot-sdk-c][50-5] - A C99 SDK for connecting devices to
  Microsoft Azure IoT services. [`MIT`][50-6]
  * [FoxelSA/libfastcal][50-7] - Fast calibration data access. [`AGPL 3`][50-8]
  * [Stephane-D/SGDK][50-9] - SGDK: A small, open and free development kit for
  the Sega Megadrive. [`MIT`][50-10]
  * [andygock/avr-uart][50-11] - AVR UART C Library. [`License`][50-12]
  * [anrieff/libcpuid][50-13] - a small C library for x86 CPU detection and
  feature extraction. [`BSD 2-Clause`][50-14]
  * [coocox/cox][50-15] - CoX is an peripherals library with a unified standard
  interface specially for ARM Cortex M. [`BSD 3-Clause`][50-16]
  * [edorfaus/TEMPered][50-17] - C library and program for reading the TEMPer
  family of thermometer and hygrometer devices. [`BSD 2-Clause`][50-18]
  * [google/cpu_features][50-19] - A cross platform C99 library to get cpu
  features at runtime. [`Apache 2`][50-20]
  * [jackmitch/libsoc][50-21] - C library for interfacing with common SoC
  peripherals through generic kernel interfaces. [`LGPL 2.1`][50-22]
  * [joan2937/pigpio][50-23] - C library for the Raspberry which allows control
  of the General Purpose Input Outputs (GPIO). [`Unlicense`][50-24]
  * [libimobiledevice/libimobiledevice][50-25] - A cross-platform protocol
  library to communicate with iOS devices. [`LGPL 2.1`][50-26]
  * [libopencm3/libopencm3][50-27] - Open Source ARM cortex m microcontroller
  library. [`GPL 3`][50-28]
  * [libusb/libusb][50-29] - A cross-platform library to access USB devices. [`LGPL 2.1`][50-30]
  * [micronucleus/micronucleus][50-31] - ATTiny usb bootloader with a strong
  emphasis on bootloader compactness. [`License`][50-32]
  * [nfc-tools/libnfc][50-33] - Platform independent Near Field Communication
  library. [`LGPL 3`][50-34]
  * [signal11/hidapi][50-35] - A Simple library for communicating with USB and
  Bluetooth HID devices on Linux, Mac, and Windows. [`Licenses`][50-36]
  * [wiiudev/libwiiu][50-37] - Build system and examples for running C code
  on the Wii U. `No license`
  * [floooh/chips][50-38] - 8-bit chip and system emulators in standalone
  C headers. [`Zlib`][50-39]

  [50-39]: https://github.com/floooh/chips/blob/master/LICENSE
  [50-38]: https://github.com/floooh/chips
  [50-37]: https://github.com/wiiudev/libwiiu
  [50-36]: https://github.com/signal11/hidapi/blob/master/LICENSE.txt
  [50-35]: https://github.com/signal11/hidapi
  [50-34]: https://github.com/nfc-tools/libnfc/blob/master/COPYING
  [50-33]: https://github.com/nfc-tools/libnfc
  [50-32]: https://github.com/micronucleus/micronucleus/blob/master/License.txt
  [50-31]: https://github.com/micronucleus/micronucleus
  [50-30]: https://github.com/libusb/libusb/blob/master/COPYING
  [50-29]: https://github.com/libusb/libusb
  [50-28]: https://github.com/libopencm3/libopencm3/blob/master/COPYING.GPL3
  [50-27]: https://github.com/libopencm3/libopencm3
  [50-26]: https://github.com/libimobiledevice/libimobiledevice/blob/master/COPYING
  [50-25]: https://github.com/libimobiledevice/libimobiledevice
  [50-24]: https://github.com/joan2937/pigpio/blob/master/UNLICENCE
  [50-23]: https://github.com/joan2937/pigpio
  [50-22]: https://github.com/jackmitch/libsoc/blob/master/LICENCE
  [50-21]: https://github.com/jackmitch/libsoc
  [50-20]: https://github.com/google/cpu_features/blob/master/LICENSE
  [50-19]: https://github.com/google/cpu_features
  [50-18]: https://github.com/edorfaus/TEMPered/blob/master/LICENSE
  [50-17]: https://github.com/edorfaus/TEMPered
  [50-16]: https://github.com/coocox/cox/blob/master/LICENSE
  [50-15]: https://github.com/coocox/cox
  [50-14]: https://github.com/anrieff/libcpuid/blob/master/COPYING
  [50-13]: https://github.com/anrieff/libcpuid
  [50-12]: https://github.com/andygock/avr-uart/blob/master/LICENSE.txt
  [50-11]: https://github.com/andygock/avr-uart
  [50-10]: https://github.com/Stephane-D/SGDK/blob/master/license.txt
  [50-9]: https://github.com/Stephane-D/SGDK
  [50-8]: https://github.com/FoxelSA/libfastcal/blob/master/LICENSE
  [50-7]: https://github.com/FoxelSA/libfastcal
  [50-6]: https://github.com/Azure/azure-iot-sdk-c/blob/master/LICENSE
  [50-5]: https://github.com/Azure/azure-iot-sdk-c
  [50-4]: https://github.com/Genymobile/scrcpy/blob/master/LICENSE
  [50-3]: https://github.com/Genymobile/scrcpy
  [50-2]: https://github.com/obgm/libcoap/blob/develop/LICENSE
  [50-1]: https://github.com/obgm/libcoap
</details>

<a id="hashing"></a>
<details>
  <summary>Hashing</summary>

  ## <a href="#-">`^`</a> Hashing ##
  Hash function implementations for non-cryptographic purposes.
  * [centaurean/spookyhash][51-1] - Fast hash function. [`BSD 3-Clause`][51-2]
  * [leo-yuriev/t1ha][51-3] - Fast Positive Hash - a portable, fast hash
  function. [`BSD 3-Clause`][51-4]
  * [Cyan4973/xxHash][51-5] - Extremely fast non-cryptographic hash algorithm. [`BSD 2-Clause`][51-6]
  * [PeterScott/murmur3][51-7] - Murmur3 hash in C. [`Public domain`][51-8]
  * [RJ/ketama][51-9] - C library for consistent hashing, and langauge bindings. [`BSD 2-Clause`][51-10]
  * [cr-marcstevens/sha1collisiondetection][51-11] - Library and command line
  tool to detect SHA-1 collision in a file. [`MIT`][51-12]
  * [clibs/hash][51-13] - C hash implementation based on khash. [`MIT`][51-14]
  * [lemire/clhash][51-15] - C library implementing fast CLHash function. [`Apache 2`][51-16]
  * [mattsta/crcspeed][51-17] - This make CRC be fast. Included implementations:
  CRC-64-Jones and CRC-16-CCITT. [`BSD 3-Clause`][51-18]
  * [plashchynski/str2hex][51-19] - Data formats convertion utility. [`Apache 2`][51-20]

  [51-20]: https://github.com/plashchynski/str2hex/blob/master/LICENSE
  [51-19]: https://github.com/plashchynski/str2hex
  [51-18]: https://github.com/mattsta/crcspeed/blob/master/crcspeed.h
  [51-17]: https://github.com/mattsta/crcspeed
  [51-16]: https://github.com/lemire/clhash/blob/master/LICENSE
  [51-15]: https://github.com/lemire/clhash
  [51-14]: https://github.com/clibs/hash/blob/master/khash.h
  [51-13]: https://github.com/clibs/hash
  [51-12]: https://github.com/cr-marcstevens/sha1collisiondetection/blob/master/LICENSE.txt
  [51-11]: https://github.com/cr-marcstevens/sha1collisiondetection
  [51-10]: https://github.com/RJ/ketama/blob/master/LICENSE.txt
  [51-9]: https://github.com/RJ/ketama
  [51-8]: https://github.com/PeterScott/murmur3/blob/master/murmur3.h
  [51-7]: https://github.com/PeterScott/murmur3
  [51-6]: https://github.com/Cyan4973/xxHash/blob/dev/LICENSE
  [51-5]: https://github.com/Cyan4973/xxHash
  [51-4]: https://github.com/leo-yuriev/t1ha/blob/master/LICENSE
  [51-3]: https://github.com/leo-yuriev/t1ha
  [51-2]: https://github.com/centaurean/spookyhash/blob/master/LICENSE.md
  [51-1]: https://github.com/centaurean/spookyhash
</details>

<a id="image-processing"></a>
<details>
  <summary>Image Processing and Computer Vision</summary>

  ## <a href="#-">`^`</a> Image Processing and Computer Vision ##
  * [libgd/libgd][52-1] - Library for the dynamic creation of images by
  programmers. [`License`][52-2]
  * [giflib][52-3] - Library for reading and writing gif images. [`License`][52-4]
  * [libjpeg-turbo/libjpeg-turbo][52-5] - Faster library for reading and
  writing JPEG files. [`Licenses`][52-6]
  * [libpng][52-7] - The official PNG reference library. [`License`][52-8]
  * [liuliu/ccv][52-9] - C-based/Cached/Core Computer Vision Library, A Modern
  Computer Vision Library. [`License`][52-10]
  * [Phildo/pixQL][52-11] - SQL for image processing. `No license`
  * [XadillaX/byakuren][52-12] -  A theme color extracting library. [`MIT`][52-13]
  * [ansilove/ansilove][52-14] - ANSi / ASCII art to PNG converter. [`BSD 2-Clause`][52-15]
  * [bluesmoon/pngtocss][52-16] - Read in a gradient from a png file and spit
  out CSS for it. [`BSD`][52-17]
  * [brendangregg/Dump2PNG][52-18] - Visualize file data as a PNG. [`License`][52-19]
  * [buaazp/zimg][52-20] - A lightweight and high performance image storage and
  processing system. [`BSD 3-Clause`][52-21]
  * [dbohdan/s2png][52-22] - Store data of any kind inside PNG images. [`GPL 2`][52-23]
  * [ginsweater/gif-h][52-24] - Simple C++ one-header library for the creation
  of animated GIFs from image data. [`Unlicense`][52-25]
  * [libvips/libvips][52-26] - A fast image processing library with low memory
  needs. [`LGPL 2.1`][52-27]
  * [mozilla/mozjpeg][52-28] - Improved JPEG encoder. [`Licenses`][52-29]
  * [openslide/openslide][52-30] - C library for reading virtual slide images. [`License`][52-31]
  * [pornel/giflossy][52-32] - Lossy GIF compressor. [`GPL 2`][52-33]
  * [pornel/pngquant][52-34] - Lossy PNG compressor. [`License`][52-35]
  * [rflynn/imgmin][52-36] - Lossy image optimization. [`MIT`][52-37]
  * [uclouvain/openjpeg][52-38] - Official repository of the OpenJPEG project. [`BSD 2-Clause`][52-39]
  * [vlfeat/vlfeat][52-40] - An open library of computer vision algorithms. [`BSD 2-Clause`][52-41]
  * [libspng][52-42] - Secure PNG reading/writing. [`BSD 2-Clause`][52-43]
  * [ImageMagick/ImageMagick][52-44] - Image processing suite with C interface. [`License`][52-45]
  * [saitoha/libsixel][52-46] - Library implementing the SIXEL protocol, allowing beautiful graphics in your terminal. [`License`][52-47]

  [52-47]: https://github.com/saitoha/libsixel/blob/master/LICENSE
  [52-46]: https://github.com/saitoha/libsixel
  [52-45]: https://github.com/ImageMagick/ImageMagick/blob/master/LICENSE
  [52-44]: https://github.com/ImageMagick/ImageMagick
  [52-43]: https://gitlab.com/randy408/libspng/blob/master/LICENSE
  [52-42]: https://libspng.org/
  [52-41]: https://github.com/vlfeat/vlfeat/blob/master/COPYING
  [52-40]: https://github.com/vlfeat/vlfeat
  [52-39]: https://github.com/uclouvain/openjpeg/blob/master/LICENSE
  [52-38]: https://github.com/uclouvain/openjpeg
  [52-37]: https://github.com/rflynn/imgmin/blob/master/LICENSE-MIT.txt
  [52-36]: https://github.com/rflynn/imgmin
  [52-35]: https://github.com/kornelski/pngquant/blob/master/COPYRIGHT
  [52-34]: https://github.com/kornelski/pngquant
  [52-33]: https://github.com/kornelski/giflossy/blob/master/COPYING
  [52-32]: https://github.com/kornelski/giflossy
  [52-31]: https://github.com/openslide/openslide/blob/master/LICENSE.txt
  [52-30]: https://github.com/openslide/openslide
  [52-29]: https://github.com/mozilla/mozjpeg/blob/master/LICENSE.md
  [52-28]: https://github.com/mozilla/mozjpeg
  [52-27]: https://github.com/libvips/libvips/blob/master/COPYING
  [52-26]: https://github.com/libvips/libvips
  [52-25]: https://github.com/ginsweater/gif-h/blob/master/LICENSE
  [52-24]: https://github.com/ginsweater/gif-h
  [52-23]: https://github.com/dbohdan/s2png/blob/master/LICENSE
  [52-22]: https://github.com/dbohdan/s2png
  [52-21]: https://github.com/buaazp/zimg/blob/master/LICENSE
  [52-20]: https://github.com/buaazp/zimg
  [52-19]: https://github.com/brendangregg/Dump2PNG/blob/master/dump2png.c
  [52-18]: https://github.com/brendangregg/Dump2PNG
  [52-17]: https://github.com/bluesmoon/pngtocss#license
  [52-16]: https://github.com/bluesmoon/pngtocss
  [52-15]: https://github.com/ansilove/ansilove/blob/master/LICENSE
  [52-14]: https://github.com/ansilove/ansilove
  [52-13]: https://github.com/XadillaX/byakuren/blob/master/LICENSE
  [52-12]: https://github.com/XadillaX/byakuren
  [52-11]: https://github.com/Phildo/pixQL
  [52-10]: https://github.com/liuliu/ccv/blob/unstable/COPYING
  [52-9]: https://github.com/liuliu/ccv
  [52-8]: https://sourceforge.net/p/libpng/code/ci/master/tree/LICENSE
  [52-7]: http://www.libpng.org
  [52-6]: https://github.com/libjpeg-turbo/libjpeg-turbo/blob/master/LICENSE.md
  [52-5]: https://github.com/libjpeg-turbo/libjpeg-turbo
  [52-4]: https://sourceforge.net/p/giflib/code/ci/master/tree/COPYING
  [52-3]: https://sourceforge.net/projects/giflib/
  [52-2]: https://github.com/libgd/libgd/blob/master/COPYING
  [52-1]: https://github.com/libgd/libgd
</details>

<a id="integrated-debugging"></a>
<details>
  <summary>Integrated Debugging and Logging</summary>

  ## <a href="#-">`^`</a> Integrated Debugging and Logging ##
  * [gpakosz/whereami][53-1] - One-file library for locating the current
  executable on the file system. [`MIT`][53-2]
  * [HardySimpson/zlog][53-3] - Reliable, pure C logging library. [`LGPL 2.1`][53-4]
  * [esneider/debug][53-5] - One-header library for easier 'printf debugging'. [`MIT`][53-6]
  * [ThrowTheSwitch/CException][53-7] - Implementation of exceptions. [`License`][53-8]
  * [google/pblog][53-9] - Small, low overhead, structured logging library
  intended for logging formware events. [`Apache 2`][53-10]
  * [0xmalloc/c-log][53-11] - a fast ,stable and thread-safe log lib(logger)
  for C/C++ language. [`Apache 2`][53-12]
  * [Celtoys/Remotery][53-13] - Single C file, Realtime CPU/GPU Profiler with
  Remote Web Viewer. [`Apache 2`][53-14]
  * [armink/EasyLogger][53-15] - A ultra-lightweight(ROM<1.6K, RAM<0.3k),
  high-performance C/C++ log library. [`MIT`][53-16]
  * [cyrus-and/prof][53-17] - Self-contained C/C++ profiler library for Linux. [`License`][53-18]
  * [facebook/liblogfaf][53-19] - A library that logs messages using
  non-blocking UDP datagrams. [`BSD 3-Clause`][53-20]
  * [kmcallister/embedded-breakpoints][53-21] - Embed GDB breakpoints in C
  source code. [`BSD 3-Clause`][53-22]
  * [ntpeters/SimpleLogger][53-23] - Basic logger for C and C++ projects. [`MIT`][53-24]
  * [openjudge/sandbox][53-25] - Open-source suite of software components for
  C/C++ and Python developers to create automated profiling tools and watchdog
  programs. [`BSD 3-Clause`][53-26]
  * [rxi/log.c][53-27] - A simple logging library implemented in C99. [`MIT`][53-28]
  * [yosefk/checkedthreads][53-29] - checkedthreads: no race condition goes
  unnoticed! Simple API, automatic load balancing, Valgrind-based checking. [`BSD 2-Clause`][53-30]
  * [libFirm][53-31] - Library that provides a graph-based intermediate
  representation, optimizations and assembly code generation suitable for use in
  compilers. Comes with an example C front-end under the same license. [`GPL 2`][53-32]

  [53-32]: https://pp.ipd.kit.edu/git/cparser/tree/COPYING
  [53-31]: https://pp.ipd.kit.edu/firm/
  [53-30]: https://github.com/yosefk/checkedthreads/blob/master/LICENSE.txt
  [53-29]: https://github.com/yosefk/checkedthreads
  [53-28]: https://github.com/rxi/log.c/blob/master/LICENSE
  [53-27]: https://github.com/rxi/log.c
  [53-26]: https://github.com/openjudge/sandbox/blob/V_0_3_x/sample2.c
  [53-25]: https://github.com/openjudge/sandbox
  [53-24]: https://github.com/ntpeters/SimpleLogger/blob/master/LICENSE
  [53-23]: https://github.com/ntpeters/SimpleLogger
  [53-22]: https://github.com/kmcallister/embedded-breakpoints/blob/master/LICENSE
  [53-21]: https://github.com/kmcallister/embedded-breakpoints
  [53-20]: https://github.com/facebook/liblogfaf/blob/master/LICENSE
  [53-19]: https://github.com/facebook/liblogfaf
  [53-18]: https://github.com/cyrus-and/prof#license
  [53-17]: https://github.com/cyrus-and/prof
  [53-16]: https://github.com/armink/EasyLogger/blob/master/LICENSE
  [53-15]: https://github.com/armink/EasyLogger
  [53-14]: https://github.com/Celtoys/Remotery/blob/master/LICENSE
  [53-13]: https://github.com/Celtoys/Remotery
  [53-12]: https://github.com/0xmalloc/c-log/blob/master/LICENSE
  [53-11]: https://github.com/0xmalloc/c-log
  [53-10]: https://github.com/google/pblog/blob/master/LICENSE
  [53-9]: https://github.com/google/pblog
  [53-8]: https://github.com/ThrowTheSwitch/CException/blob/master/LICENSE.txt
  [53-7]: https://github.com/ThrowTheSwitch/CException
  [53-6]: https://github.com/esneider/debug/blob/master/debug.h
  [53-5]: https://github.com/esneider/debug
  [53-4]: https://github.com/HardySimpson/zlog/blob/master/COPYING
  [53-3]: https://github.com/HardySimpson/zlog
  [53-2]: https://github.com/gpakosz/whereami/blob/master/LICENSE.MIT
  [53-1]: https://github.com/gpakosz/whereami
</details>

<a id="io"></a>
<details>
  <summary>I/O</summary>

  ## <a href="#-">`^`</a> I/O ##
  * [Lajnold/falloc][54-1] - falloc creates files of a user-specified size. It
  uses the posix_fallocate syscall for allocating the right size directly,
  instead of copying data like the commonly used dd tool does. [`GPL 3`][54-2]
  * [cgaebel/pipe][54-3] - A simple thread-safe FIFO in C. [`MIT`][54-4]
  * [cxong/tinydir][54-5] - Lightweight, portable and easy to integrate C
  directory and file reader. [`License`][54-6]
  * [reverbrain/eblob][54-7] - Eblob is an append-only low-level IO library,
  which saves data in blob files. Created as low-level backend for elliptics. [`LGPL 3`][54-8]
  * [tronkko/dirent][54-9] - C/C++ library for retrieving information on files
  and directories. [`MIT`][54-10]
  * [jwerle/fs.c][54-11] - File system API much like Node's fs module. [`MIT`][54-12]

  [54-12]: https://github.com/jwerle/fs.c/blob/master/LICENSE
  [54-11]: https://github.com/jwerle/fs.c
  [54-10]: https://github.com/tronkko/dirent/blob/master/LICENSE
  [54-9]: https://github.com/tronkko/dirent
  [54-8]: https://github.com/reverbrain/eblob/blob/master/LICENSE
  [54-7]: https://github.com/reverbrain/eblob
  [54-6]: https://github.com/cxong/tinydir/blob/master/COPYING
  [54-5]: https://github.com/cxong/tinydir
  [54-4]: https://github.com/cgaebel/pipe
  [54-3]: https://github.com/cgaebel/pipe
  [54-2]: https://github.com/Lajnold/falloc/blob/master/COPYING
  [54-1]: https://github.com/Lajnold/falloc
</details>

<a id="lexing-and-parsing"></a>
<details>
  <summary>Lexing and Parsing</summary>

  ## <a href="#-">`^`</a> Lexing and Parsing ##
  * [GNU Bison][55-1] - General-purpose parser generator that converts an
  annotated context-free grammar into a range of parsers. [`GPL 3`][55-2]
  * [bbu/simple-interpreter][55-3] - A hackable and extensible lexer, parser
  and interpreter for a minimalistic, imperative, C-like language. `No license`
  * [dcreager/libpush][55-4] - An arrow-based parser combinator library for C. [`BSD 3-Clause`][55-5]
  * [kmussel/Moment][55-6] - Natural Language Date Parser Using Lex/Yacc/C. [`MIT`][55-7]
  * [skvadrik/re2c][55-8] - lexer generator for C/C++. [`License`][55-9]
  * [westes/flex][55-10] - The Fast Lexical Analyzer - scanner generator for
  lexing in C and C++. [`License`][55-11]
  * [orangeduck/mpc][55-12] - Parser combinator library. [`BSD 2-Clause`][55-13]

  [55-13]: https://github.com/orangeduck/mpc/blob/master/LICENSE.md
  [55-12]: https://github.com/orangeduck/mpc
  [55-11]: https://github.com/westes/flex/blob/master/COPYING
  [55-10]: https://github.com/westes/flex
  [55-9]: https://github.com/skvadrik/re2c/blob/master/LICENSE
  [55-8]: https://github.com/skvadrik/re2c
  [55-7]: https://github.com/kmussel/Moment/blob/master/LICENSE
  [55-6]: https://github.com/kmussel/Moment
  [55-5]: https://github.com/dcreager/libpush/blob/master/LICENSE.txt
  [55-4]: https://github.com/dcreager/libpush
  [55-3]: https://github.com/bbu/simple-interpreter
  [55-2]: https://www.gnu.org/software/bison/
  [55-1]: https://www.gnu.org/software/bison/
</details>

<a id="memory-management"></a>
<details>
  <summary>Memory Management</summary>

  ## <a href="#-">`^`</a> Memory Management ##
  * [Boehm GC][56-1] - Garbage collection for C. Various licenses, all open
  source. [`License`][56-2]
  * [Lockless Memory Allocator][56-3] - Efficient memory allocator. [`GPL 3`][56-4]
  * [talloc][56-5] - Hierarchical, reference-counted memory pool system with
  destructors. [`LGPL 3`][56-6]
  * [mattconte/tlsf][56-7] - Two-Level Segregated Fit allocator; a
  general-purpose, dynamic memory allocator designed to meet real-time
  requirements. [`BSD 3-Clause`][56-8]
  * [jemalloc/jemalloc][56-9] - General purpose malloc(3) implementation that
  emphasizes fragmentation avoidance and scalable concurrency support, commonly
  used in production systems. [`License`][56-10]
  * [dlmalloc][56-11] - Doug Lea's malloc(3) implementation, useful for academic
  and research purposes. [`Public domain`][56-12]
  * [CCareaga/heap_allocator][56-13] - A simple heap memory allocator in
  ~200 lines. [`MIT`][56-14]
  * [ivmai/bdwgc][56-15] - The Boehm-Demers-Weiser conservative C/C++ Garbage
  Collector (libgc, bdwgc, boehm-gc). [`License`][56-16]
  * [mulle-nat/mulle-allocator][56-17] - Flexible C memory allocation scheme
  with leak checking. [`BSD 3-Clause`][56-18]
  * [munificent/mark-sweep][56-19] - A simple mark-sweep garbage collector in C. [`MIT`][56-20]
  * [ned14/nedmalloc][56-22] - Fast portable thread caching malloc
  implementation written in C for multiple threads without lock contention based
  on dlmalloc. Optimised for x86 and x64. Compatible with C++. Can patch itself
  into existing binaries on Windows. [`Boost`][56-22]
  * [orangeduck/tgc][56-23] - A Tiny Garbage Collector for C. [`BSD 2-Clause`][56-24]
  * [rampantpixels/rpmalloc][56-25] - Public domain cross platform lock free
  thread caching 32-byte aligned memory allocator implemented in C. [`License`][56-26]
  * [stevedekorte/garbagecollector][56-27] - Incrementall garbage collector
  library in C for use by high level language implementions. [`BSD 3-Clause`][56-28]

  [56-28]: https://github.com/stevedekorte/garbagecollector/blob/master/source/Collector.h
  [56-27]: https://github.com/stevedekorte/garbagecollector
  [56-26]: https://github.com/rampantpixels/rpmalloc/blob/develop/LICENSE
  [56-25]: https://github.com/rampantpixels/rpmalloc
  [56-24]: https://github.com/orangeduck/tgc/blob/master/LICENSE.md
  [56-23]: https://github.com/orangeduck/tgc
  [56-22]: https://github.com/ned14/nedmalloc/blob/master/License.txt
  [56-21]: https://github.com/ned14/nedmalloc
  [56-20]: https://github.com/munificent/mark-sweep/blob/master/COPYRIGHT
  [56-19]: https://github.com/munificent/mark-sweep
  [56-18]: https://github.com/mulle-c/mulle-allocator/blob/release/LICENSE
  [56-17]: https://github.com/mulle-c/mulle-allocator
  [56-16]: https://github.com/ivmai/bdwgc#copyright--warranty
  [56-15]: https://github.com/ivmai/bdwgc
  [56-14]: https://github.com/CCareaga/heap_allocator/blob/master/LICENSE
  [56-13]: https://github.com/CCareaga/heap_allocator
  [56-12]: http://g.oswego.edu/pub/misc/malloc.c
  [56-11]: http://g.oswego.edu/pub/misc/malloc.c
  [56-10]: https://github.com/jemalloc/jemalloc/blob/dev/COPYING
  [56-9]: https://github.com/jemalloc/jemalloc
  [56-8]: https://github.com/mattconte/tlsf/blob/master/tlsf.h
  [56-7]: https://github.com/mattconte/tlsf
  [56-6]: https://www.samba.org/ftp/talloc/
  [56-5]: https://talloc.samba.org/talloc/doc/html/index.html
  [56-4]: https://locklessinc.com/gpl3.shtml
  [56-3]: https://locklessinc.com/
  [56-2]: https://www.hboehm.info/gc/license.txt
  [56-1]: https://www.hboehm.info/gc/
</details>

<a id="multimedia"></a>
<details>
  <summary>Multimedia</summary>

  ## <a href="#-">`^`</a> Multimedia ##
  Audio and video processing
  * [jeremyevans/ape_tag_libs][57-1] - Library for working with APEv2 tags. [`MIT`][57-2]
  * [lieff/minimp3][57-3] - Lightweight MP3 decoder single header library. [`License`][57-4]
  * [FFMPEG][57-5] - Complete, cross-platform solution to record, convert and
  stream audio and video. [`LGPL 2.1`][57-6]
  * [GStreamer][57-7] - Framework for audio and visual media. [`LGPL 2`][57-8]
  * [mpv-player/mpv][57-9] - Media player MPV with provided library libmpv.
  Compile with ``./waf configure --disable-cplayer --enable-libmpv-shared`` to
  not have the music player. [`License`][57-10]
  * [andrewrk/libsoundio][57-11] - Library for cross-platform, real-time audio input and
  output. Has a range of back-ends. [`MIT`][57-12]
  * [AVbin/AVbin](https://github.com/AVbin/AVbin) - AVbin is a C library that provides a thin, cross-platform wrapper around Libav’s video- and audio-decoding functionality, providing long-term binary compatibility for applications and languages that need it.  See also: Pyglet, a python media framework that makes extensive use of AVbin.
  * [LnxPrgr3/crossfeed](https://github.com/LnxPrgr3/crossfeed) - Headphone crossfeed filter
  * [PaulBatchelor/Soundpipe](https://github.com/PaulBatchelor/Soundpipe) - A lightweight music DSP library.
  * [Themaister/libfmsynth](https://github.com/Themaister/libfmsynth) - A C library which implements an FM synthesizer
  * [UniversalPrimer/flv-analyzer](https://github.com/UniversalPrimer/flv-analyzer) - Loads an FLV file into sane C data structures and outputs fields as human readable
  * [Vidvox/hap-qt-codec](https://github.com/Vidvox/hap-qt-codec) - A QuickTime codec for Hap video
  * [acrisci/playerctl](https://github.com/acrisci/playerctl) - mpris command-line controller and library for spotify, vlc, audacious, bmp, cmus, and others.
  * [aubio/aubio](https://github.com/aubio/aubio) - a library for audio and music analysis
  * [cmatsuoka/libxmp](https://github.com/cmatsuoka/libxmp) - Libxmp is a library that renders module files to PCM data.
  * [cnlohr/colorchord](https://github.com/cnlohr/colorchord) - Chromatic Sound to Light Conversion System
  * [csound/csound](https://github.com/csound/csound) - Main repository for Csound
  * [dxjia/ffmpeg-commands-executor-library](https://github.com/dxjia/ffmpeg-commands-executor-library) - execute ffmpeg commands through a jni shared library.
  * [erikd/libsndfile](https://github.com/erikd/libsndfile) - A C library for reading and writing sound files containing sampled audio data..
  * [imankulov/wav2rtp](https://github.com/imankulov/wav2rtp) - wav2rtp is a simple tool intended to convert speech data from wav files to RTP data stream
  * [kfish/libfishsound](https://github.com/kfish/libfishsound) - A simple programming interface for decoding and encoding audio data using Xiph.org codecs (FLAC, Speex and Vorbis)
  * [libass/libass](https://github.com/libass/libass) - libass is a portable subtitle renderer for the ASS/SSA (Advanced Substation Alpha/Substation Alpha) subtitle format.
  * [libav/libav](https://github.com/libav/libav) - Libav github mirror, clone of git://git.libav.org/libav
  * [libpd/libpd](https://github.com/libpd/libpd) - Pure Data embeddable audio synthesis library
  * [mltframework/mlt](https://github.com/mltframework/mlt) - MLT Multimedia Framework
  * [sahib/glyr](https://github.com/sahib/glyr) - Glyr is a music related metadata searchengine, both with commandline interface and C API
  * [simonyiszk/csdr](https://github.com/simonyiszk/csdr) - A simple DSP library and command-line tool for Software Defined Radio.
  * [strands-project/data_compression](https://github.com/strands-project/data_compression) - Video encoding for 8 bit RGB images, 16 bit grayscale depth images and possibly more.
  * [sptim/mp3hash](https://github.com/sptim/mp3hash) - Command line tool to calculate the hash of the music data in mp3 files (without id3v1 & id3v2 metadata). Useful to find dupes with e.g. different genre names.
  * [xiph/flac](https://github.com/xiph/flac) - Free Lossless Audio Codec
  * [xiph/opus](https://github.com/xiph/opus) - Modern audio compression for the internet.
  * [mhroth/tinyosc](https://github.com/mhroth/tinyosc) - A minimal Open Sound Control (OSC) library written in vanilla C.
  * [libao](https://xiph.org/ao/) - Cross-platform audio library with a wide variety of outputs. [`GNU GPL2.1 or later`](http://www.gnu.org/licenses/old-licenses/gpl-2.0.html)

  [57-12]: https://github.com/andrewrk/libsoundio/blob/master/LICENSE
  [57-11]: http://libsound.io/
  [57-10]: https://github.com/mpv-player/mpv/blob/master/Copyright
  [57-9]: https://github.com/mpv-player/mpv
  [57-8]: https://gitlab.freedesktop.org/gstreamer/gstreamer/blob/master/COPYING
  [57-7]: https://gstreamer.freedesktop.org/
  [57-6]: https://www.ffmpeg.org/legal.html
  [57-5]: https://www.ffmpeg.org/
  [57-4]: https://github.com/lieff/minimp3/blob/master/LICENSE
  [57-3]: https://github.com/lieff/minimp3
  [57-2]: https://github.com/jeremyevans/ape_tag_libs/tree/master/c
  [57-1]: https://github.com/jeremyevans/ape_tag_libs/tree/master/c
</details>

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
* [chutsu/cog](https://github.com/chutsu/cog) - C common library containing common data structures, sorting algorithms and utility functions
* [cs50/libcs50](https://github.com/cs50/libcs50) - CS50 Library for C
* [dcreager/libcork](https://github.com/dcreager/libcork) - A simple, easily embeddable cross-platform C library
* [faragon/libsrt](https://github.com/faragon/libsrt) - libsrt is a C library for writing fast and safe C code, faster. It provides string, vector, bit set, set, map, hash set, and hash map handling. Suitable for soft and hard real-time. Allows both heap and stack allocation.  *BETA* (API still can change: suggestions are welcome)
* [gregvirgin/libcork](https://github.com/gregvirgin/libcork) - A simple, easily embeddable cross-platform C library
* [happyfish100/libfastcommon](https://github.com/happyfish100/libfastcommon) - c common functions library extracted from my open source project FastDFS. this library is very simple and stable.  functions including: string, logger, chain, hash, socket, ini file reader, base64 encode / decode, url encode / decode, fast timer, skiplist, object pool etc. detail info please see the c header files.
* [koanlogic/libu](https://github.com/koanlogic/libu) - LibU is a multiplatform utility library written in C, with APIs for handling memory allocation, networking and URI parsing, string manipulation, debugging, and logging in a very compact way, plus many other miscellaneous tasks
* [letoram/arcan](https://github.com/letoram/arcan) - Arcan - [Display Server, Multimedia Framework, Game Engine] -> "Desktop Engine"
* [saprykin/plibsys](https://github.com/saprykin/plibsys) - Highly portable C system library: threads and synchronization primitives, sockets (TCP, UDP, SCTP), IPv4 and IPv6, IPC, hash functions (MD5, SHA-1, SHA-2, SHA-3, GOST), binary trees (RB, AVL) and more. Native code performance.
* [tboox/tbox](https://github.com/tboox/tbox) - 🎁 A glib-like multi-platform c library
* [waruqi/tbox](https://github.com/waruqi/tbox) - A glib-like multi-platform c library
* [zpl-c/zpl](https://github.com/zpl-c/zpl) - 📐 Your C99 Powerkit
* [dmw/caffeine](https://github.com/dmw/caffeine) - C Application Framework

## Networking ##
### DNS ###
* [GNU adns][229] - Advanced, easy-to-use, asynch-capable DNS client library
  and utilities. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [ldns][231] - Library to simplify DNS programming. [``BSD-3-Clause``][BSD-3-Clause]
* [bagder/c-ares](https://github.com/bagder/c-ares) - c-ares is a C library for asynchronous DNS requests
* [farsightsec/dnstable](https://github.com/farsightsec/dnstable) - encoding format, library, and utilities for passive DNS data
* [res0nat0r/tsunami-udp](https://github.com/res0nat0r/tsunami-udp) -  A fast user-space file transfer protocol that uses TCP control and UDP data for transfer over very high speed long distance networks (≥ 1 Gbps and even 10 GE), designed to provide more throughput than possible with TCP over the same networks.
* [wahern/dns](https://github.com/wahern/dns) - dns.c: Single file non-blocking DNS C library without callbacks or external dependencies.

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
* [civetweb/civetweb](https://github.com/civetweb/civetweb) - Embedded C/C++ web server
* [h2o/h2o](https://github.com/h2o/h2o) - H2O - the optimized HTTP/1, HTTP/2 server
* [h2o/picohttpparser](https://github.com/h2o/picohttpparser) - tiny HTTP parser written in C (used in HTTP::Parser::XS et al.)
* [iafonov/multipart-parser-c](https://github.com/iafonov/multipart-parser-c) - Http multipart parser implemented in C
* [joyent/http-parser](https://github.com/joyent/http-parser) - http request/response parser for c
* [zyearn/zaver](https://github.com/zyearn/zaver) - Yet another fast and efficient HTTP server
* [monkey/monkey](https://github.com/monkey/monkey) - Monkey HTTP Server
* [reagent/http](https://github.com/reagent/http) - Simple HTTP client in C
* [solusipse/ureq](https://github.com/solusipse/ureq) - Micro C library for handling HTTP requests on low resource systems.
* [tatsuhiro-t/nghttp2](https://github.com/tatsuhiro-t/nghttp2) - nghttp2 - HTTP/2 C Library
* [taf2/libebb](https://github.com/taf2/libebb) - a lightweight high-performance HTTP server library for C
* [wg/wrk](https://github.com/wg/wrk) - Modern HTTP benchmarking tool

### Mail ###
* [LibEtPan][233] - Mail library providing an efficient network for IMAP, SMTP,
  POP and NNTP. [``BSD-3-Clause``][BSD-3-Clause]
* [libvldmail][439] - Email validation library. No external dependencies
  (not even regexps). [``WTFPL``][WTFPL]
* [libquickmail][238] - Library intended to give developers a way to send email
  from their applications. Supports multiple To/Cc/Bcc recipients and
  attachments without size limits. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [dinhviethoa/libetpan](https://github.com/dinhviethoa/libetpan) - Mail Framework for C Language

### Messaging ###
* [NNG][245] - nanomsg-next-generation - lightweight brokerless messaging. [``MIT``][MIT]
* [rabbitmq-c][440] - Client library for [RabbitMQ][229]. [``MIT``][MIT]
* [zproto][370] - Protocol framework for ZeroMQ. [``MIT``][MIT]
* [nanomsg][244] - C-based implementation of ZeroMQ. [``MIT``][MIT]
* [antirez/disque](https://github.com/antirez/disque) - Disque is a distributed message broker
* [circonus-labs/fq](https://github.com/circonus-labs/fq) - F@#$*&%Q (Message queue that is fast, brokered, in C and gets out of your way)
* [paulasmuth/fyrehose](https://github.com/paulasmuth/fyrehose) - message broker for JSON data streams
* [zeromq/czmq](https://github.com/zeromq/czmq) - High-level C binding for ØMQ

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
* [GROX13/BitTorrent](https://github.com/GROX13/BitTorrent) - BitTorrent protocol.
* [JFreegman/toxic](https://github.com/JFreegman/toxic) - An ncurses-based Tox client
* [LibVNC/libvncserver](https://github.com/LibVNC/libvncserver) - LibVNCServer/LibVNCClient are cross-platform C libraries that allow you to easily implement VNC server or client functionality in your program.
* [Librevault/librevault](https://github.com/Librevault/librevault) - Librevault - Peer-to-peer, decentralized and open source file sync.
* [Netsukuku/netsukuku](https://github.com/Netsukuku/netsukuku) - Revived C-code
* [Tox/toxic](https://github.com/Tox/toxic) - CLI Tox client
* [armon/bloomd](https://github.com/armon/bloomd) - C network daemon for bloom filters
* [armon/hlld](https://github.com/armon/hlld) - C network daemon for HyperLogLogs
* [bagder/spindly](https://github.com/bagder/spindly) - a portable C library for SPDY transport (DEAD project!)
* [boazsegev/c-server-tools](https://github.com/boazsegev/c-server-tools) - Write network services in C using dynamic protocols such as HTTP and Websockets
* [c9s/r3](https://github.com/c9s/r3) - libr3 is a high-performance path dispatching library. It compiles your route paths into a prefix tree (trie). By using the constructed prefix trie in the start-up time, you may dispatch your routes with efficiency
* [cesanta/fossa](https://github.com/cesanta/fossa) - Async non-blocking multi-protocol networking library for C/C++
* [chmduquesne/xmppipe](https://github.com/chmduquesne/xmppipe) - This program allows to pipe data through an xmpp tunnel
* [chokepoint/CryptHook](https://github.com/chokepoint/CryptHook) - TCP/UDP symmetric encryption tunnel wrapper
* [clibs/dumpasn1](https://github.com/clibs/dumpasn1) - Display the contents of ASN.1 encoded data
* [deltachat/deltachat-core](https://github.com/deltachat/deltachat-core) - Delta.Chat C-Library with e2e chat-over-email functionality & Python bindings
* [fastos/fastsocket](https://github.com/fastos/fastsocket) - Fastsocket is a highly scalable socket and its underlying networking implementation of Linux kernel. With the straight linear scalability, Fastsocket can provide extremely good performance in multicore machines. In addition, it is very easy to use and maintain. As a result, it has been deployed in the production environment of SINA.
* [felipec/msn-pecan](https://github.com/felipec/msn-pecan) - MSN Messenger library in C
* [iem-projects/pd-iemrtp](https://github.com/iem-projects/pd-iemrtp) - RTP support for Pure Data
* [irungentoo/toxcore](https://github.com/irungentoo/toxcore) - The future of online communications.
* [japeq/bencode-tools](https://github.com/japeq/bencode-tools) - bencode-tools is a collection of tools for manipulating bencoded data.
* [libssh2/libssh2](https://github.com/libssh2/libssh2) - the SSH library
* [lsalzman/enet](https://github.com/lsalzman/enet) - ENet reliable UDP networking library
* [mopemope/meinheld](https://github.com/mopemope/meinheld) - meinheld is a high performance asynchronous WSGI Web Server (based on picoev)
* [nanomsg/nanomsg](https://github.com/nanomsg/nanomsg) - nanomsg library
* [neilalexander/sigmavpn](https://github.com/neilalexander/sigmavpn) - Light-weight, secure and modular VPN solution which makes use of NaCl encryption (also available for Android using jnacl in "sigmavpn-android")
* [neutrinolabs/xrdp](https://github.com/neutrinolabs/xrdp) - xrdp: an open source RDP server
* [nicolasff/river](https://github.com/nicolasff/river) - A simple “comet” server in C, streaming data to web clients
* [obgm/libcoap](https://github.com/obgm/libcoap) - A CoAP (RFC 7252) implementation in C
* [opendp/dpdk-odp](https://github.com/opendp/dpdk-odp) - Open data plane on dpdk, TCP/IP stack for dpdk.
* [rockdaboot/mget](https://github.com/rockdaboot/mget) - Multithreaded metalink/file/website downloader (like Wget) and C library
* [rxi/dyad](https://github.com/rxi/dyad) - Asynchronous networking for C
* [sch3m4/libntoh](https://github.com/sch3m4/libntoh) - User-friendly C Library to perform TCP streams reassembly and IPv4/6 defragmentation
* [seanmiddleditch/libtelnet](https://github.com/seanmiddleditch/libtelnet) - Simple RFC-complient TELNET implementation as a C library.
* [shadeslayer/libnice](https://github.com/shadeslayer/libnice) - Implementation of the IETF's Interactive Connectivity Establishment (ICE) standard (RFC 5245) and the Session Traversal Utilities for NAT (STUN) standard (RFC 5389).
* [sustrik/msg_control](https://github.com/sustrik/msg_control) - Helper functions for dealing with socket ancillary data
* [tass-belgium/picotcp](https://github.com/tass-belgium/picotcp) - PicoTCP is a free TCP/IP stack implementation
* [stephane/libmodbus](https://github.com/stephane/libmodbus) - A Modbus library for Linux, Mac OS X, FreeBSD, QNX and Windows
* [udp/lacewing](https://github.com/udp/lacewing) - Cross-platform network I/O library for C/C++
* [verse/verse](https://github.com/verse/verse) - Network protocol for real-time sharing between graphical applications
* [the-tcpdump-group/libpcap](https://github.com/the-tcpdump-group/libpcap) - the LIBpcap interface to various kernel packet capture mechanism
* [the-tcpdump-group/tcpdump](https://github.com/the-tcpdump-group/tcpdump) - the TCPdump network dissector
* [unrealircd/unrealircd](https://github.com/unrealircd/unrealircd) - Official UnrealIRCd repository. Downloads are available from our site
* [vdloo/Beacontalk](https://github.com/vdloo/Beacontalk) - Peer to peer chat-program that sends data over Wi-Fi without associations.
* [vlm/asn1c](https://github.com/vlm/asn1c) - The ASN.1 Compiler
* [versatica/OverSIP](https://github.com/versatica/OverSIP) - OverSIP: the SIP framework you dreamed about
* [wolkykim/libasyncd](https://github.com/wolkykim/libasyncd) - Embeddable Event-based Asynchronous Message/HTTP Server library for C/C++
* [eam/libcrange](https://github.com/eam/libcrange) - Range parsing library for managing sets of hostnames, ips, clusters, roles and other operational data.
* [luohaha/CSpider](https://github.com/luohaha/CSpider) - A scalable and convenient crawler framework in C:).
* [nitrogenlogic/cliserver](https://github.com/nitrogenlogic/cliserver) - A sample libevent-based network socket server that presents a simple command line interface to multiple connecting clients.
* [bovine/datapipe](https://github.com/bovine/datapipe) - Network TCP port forwarding
* [hoxnox/rawsock_recv_example](https://github.com/hoxnox/rawsock_recv_example) - SOCK_RAW IPPROTO_UDP socket data transmission example
* [LiamBindle/MQTT-C](https://github.com/LiamBindle/MQTT-C) - MQTT protocol implementation.
* [google/gumbo-parser](https://github.com/google/gumbo-parser) - HTML5 parsing library in C99.
* [libsoup](https://wiki.gnome.org/action/show/Projects/libsoup?action=show&redirect=LibSoup) - GNOME HTTP client/server library. Uses GObject. [`GNU LGPL2.1`](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)

### RPC ###
* [hmng/jsonrpc-c](https://github.com/hmng/jsonrpc-c) - JSON-RPC in C (server only for now)
* [lopter/lightsd](https://github.com/lopter/lightsd) - A daemon with a JSON-RPC API to control your light bulbs
* [studio-ousia/mprpc](https://github.com/studio-ousia/mprpc) - A fast MessagePack RPC library

### Websockets ###
* [Wslay][248] - WebSocket library. Implements version 13 of the WebSocket
  protocol, as described in RFC 6455. [``MIT``][MIT]
* [libwebsock][241] - Easy-to-use and powerful web socket library. [``LGPL-3.0-only``][LGPL-3.0-only]
* [m8rge/cwebsocket](https://github.com/m8rge/cwebsocket) - cWebsocket is lightweight websocket server library
* [payden/libwebsock](https://github.com/payden/libwebsock) - C library for easy WebSockets server.
* [tatsuhiro-t/wslay](https://github.com/tatsuhiro-t/wslay) - The WebSocket library in C
* [zhaojh329/libuwsc](https://github.com/zhaojh329/libuwsc) - A Lightweight and fully asynchronous WebSocket client C library based on libubox for Embedded Linux.

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
* [Xfennec/progress](https://github.com/Xfennec/progress) - Linux tool to show progress for cp, rm, dd, ...
* [a0rtega/pafish](https://github.com/a0rtega/pafish) - Pafish is a demonstration tool that employs several techniques to detect sandboxes and analysis environments in the same way as malware families do.
* [adoxa/ansicon](https://github.com/adoxa/ansicon) - Process ANSI escape sequences for Windows console programs.
* [aidenbell/getdents](https://github.com/aidenbell/getdents) - Simple tool for listing large (millions) numbers of files on Linux systems without causing memory issues. Useful for shell scripting large data stores.
* [antirez/linenoise](https://github.com/antirez/linenoise) - A small self-contained alternative to readline and libedit
* [ardagnir/athame](https://github.com/ardagnir/athame) - Full vim for readline (bash, gdb, python, etc)
* [asamy/ksm](https://github.com/asamy/ksm) - A really simple and lightweight x64 hypervisor written in C.  Supports VMFUNC, EPTP switching, #VE EPT Violation, VT-x nesting and IDT shadowing.  VMFUNC backward compatibility also supported.
* [dtrace4linux/linux](https://github.com/dtrace4linux/linux) - dtrace for linux - kernel driver and userland tools
* [fancycode/MemoryModule](https://github.com/fancycode/MemoryModule) - Library to load a DLL from memory.
* [gentilkiwi/kekeo](https://github.com/gentilkiwi/kekeo) - A little toolbox to play with Microsoft Kerberos in C
* [jimon/osx_app_in_plain_c](https://github.com/jimon/osx_app_in_plain_c) - A simple showcase how to create a simple OS X app in plain C without any Objective-C
* [martinezjavier/ldd3](https://github.com/martinezjavier/ldd3) - Linux Device Drivers 3 examples updated to work in recent kernels
* [rvoicilas/inotify-tools](https://github.com/rvoicilas/inotify-tools) -   inotify-tools is a C library and a set of command-line programs for Linux providing a simple interface to inotify.
* [samuellab/InterProcess](https://github.com/samuellab/InterProcess) - A compact C library to share data between processes on Windows. Fast. Simple
* [tinyalsa/tinyalsa](https://github.com/tinyalsa/tinyalsa) - Tiny library to interface with ALSA in the Linux kernel
* [warmcat/libwebsockets](https://github.com/warmcat/libwebsockets) - canonical libwebsockets.org websocket library
* [wengkai/ACLLib](https://github.com/wengkai/ACLLib) - ACLLib is a bunch of C functions covers Win32API and provides simpler API to beginners for programming Windows GUI applications. It compiles with MinGW and MS Visual Studio Express
* [Keruspe/GPaste](https://github.com/Keruspe/GPaste) - Clipboard management system
* [zardus/preeny](https://github.com/zardus/preeny) - Some helpful preload libraries for pwning stuff.

## Procedural Generation ##
* [heman][382] - Tiny library of image utilities dealing with height maps,
  normal maps, distance fields and the like. [``MIT``][MIT]
* [JCash/voronoi](https://github.com/JCash/voronoi) - A C implementation for creating 2D voronoi diagrams

## Processes and IPC ##
* [D-Bus][430] - Interprocess communications bus. [``AFL-2.1``][AFL-2.1] or [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [WhisperSystems/libsignal-protocol-c](https://github.com/WhisperSystems/libsignal-protocol-c) - Signal Protocol C Library
* [bus1/dbus-broker](https://github.com/bus1/dbus-broker) - Linux D-Bus Message Broker
* [signalapp/libsignal-protocol-c](https://github.com/signalapp/libsignal-protocol-c) - Signal Protocol C Library
* [sharvil/flingfd](https://github.com/sharvil/flingfd) - A tiny library to send file descriptors across processes
* [sheredom/process.h](https://github.com/sheredom/process.h) - A simple one header solution to launching processes and interacting with them for C and C++.
* [troydhanson/kvspool](https://github.com/troydhanson/kvspool) - A library to support streaming data applications
* [xroche/coffeecatch](https://github.com/xroche/coffeecatch) - CoffeeCatch, a tiny native POSIX signal catcher (especially useful for JNI code on Android/Dalvik)

## Regex and Search ##
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
* [cesanta/slre](https://github.com/cesanta/slre) - Super Light Regexp engine for C/C++
* [k-takata/Onigmo](https://github.com/k-takata/Onigmo) - Onigmo is a regular expressions library forked from Oniguruma.
* [kkos/oniguruma](https://github.com/kkos/oniguruma) - regular expression library
* [mbornet-hl/hl](https://github.com/mbornet-hl/hl) - Highlight (colorize) text data using regular expressions
* [mptre/pick](https://github.com/mptre/pick) - A fuzzy search tool for the command-line
* [openresty/sregex](https://github.com/openresty/sregex) - A non-backtracking NFA/DFA-based Perl-compatible regex engine matching on large data streams
* [plusvic/yara](https://github.com/plusvic/yara) - The pattern matching swiss knife

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
* [Xsoda/struct](https://github.com/Xsoda/struct) - pack and unpack packet data like python struct module.
* [acg/lwpb](https://github.com/acg/lwpb) - Lightweight Protocol Buffers for C and Python
* [camgunz/cmp](https://github.com/camgunz/cmp) - An implementation of the MessagePack serialization format in C / msgpack.org[C]
* [cloudwu/atomdict](https://github.com/cloudwu/atomdict) - A data structure for data exchange between multi lua states.
* [cloudwu/pbc](https://github.com/cloudwu/pbc) - A protocol buffers library for C
* [cloudwu/sproto](https://github.com/cloudwu/sproto) - Yet another protocol library like google protocol buffers , but simple and fast.
* [dryman/opic](https://github.com/dryman/opic) - Fast serialization framework for C
* [fredrikbk/libpack](https://github.com/fredrikbk/libpack) - Library that packs/serializes or unpacks/deserializes user-defined data layouts. The data layouts are specified using datatypes similar to MPI Datatypes. The library compiles the datatypes into efficient vectorized pack/unpack code at commit time using an LLVM-based online compiler.
* [google/upb](https://github.com/google/upb) - a small protobuf implementation in C
* [greghaynes/Afproto](https://github.com/greghaynes/Afproto) - Serial data framing protocol
* [ludocode/mpack](https://github.com/ludocode/mpack) - MPack - A C encoder/decoder for the MessagePack serialization format / msgpack.org[C]
* [nanopb/nanopb](https://github.com/nanopb/nanopb) - Protocol Buffers with small code size
* [rfk/tnetstring](https://github.com/rfk/tnetstring) - data serialization using typed netstrings
* [troydhanson/tpl](https://github.com/troydhanson/tpl) - tpl - a small binary serialization library for C
* [alexanderchuranov/Metaresc](https://github.com/alexanderchuranov/Metaresc) - META data and RESource library for  C language

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
* [attractivechaos/klib](https://github.com/attractivechaos/klib) - A standalone and lightweight C library
* [breckinloggins/libuseful](https://github.com/breckinloggins/libuseful) - A collection of useful data structures, algorithms, and utilities for C programming
* [chadjoan/C-Survival-Kit](https://github.com/chadjoan/C-Survival-Kit) - A set of useful functions, data structures, and macros aimed at allowing more expressive and reliable C code.  Portability targets are OpenVMS and Linux.
* [clibs/clib](https://github.com/clibs/clib) - C package manager-ish
* [erimatnor/libckit](https://github.com/erimatnor/libckit) - A kit of C-based utilities and data structures.
* [floooh/sokol](https://github.com/floooh/sokol) - minimal cross-platform standalone C headers
* [gingerBill/gb](https://github.com/gingerBill/gb) - gb single-file public domain libraries for C & C++
* [gozfree/libraries](https://github.com/gozfree/libraries) - Basic libraries all written in c by gozfree, including network, event, config, log, hash, ipc, rpc, mem,  and so on
* [mackron/dr_libs](https://github.com/mackron/dr_libs) - A collection of public domain single-file libraries for C/C++.
* [mattiasgustavsson/libs](https://github.com/mattiasgustavsson/libs) - Single-file public domain libraries for C/C++
* [matteobertozzi/carthage](https://github.com/matteobertozzi/carthage) - Pure C Data Structure and Utils
* [napsy/libhelper](https://github.com/napsy/libhelper) - General functions and data structures for C
* [niklasfrykholm/nflibs](https://github.com/niklasfrykholm/nflibs) - A collection of interoperable minimalistic C libraries
* [nothings/stb](https://github.com/nothings/stb) - stb single-file public domain libraries for C/C++
* [prideout/par](https://github.com/prideout/par) - single-file C libraries from Philip Allan Rideout
* [rmitton/rjm](https://github.com/rmitton/rjm) - Various single-file C libraries.
* [rustyrussell/ccan](https://github.com/rustyrussell/ccan) - The C Code Archive Network
* [vurtun/mmx](https://github.com/vurtun/mmx) - single header libraries for C/C++
* [yl790/algorithms-and-data-structures](https://github.com/yl790/algorithms-and-data-structures) - for future reference
* [rofl0r/libulz](https://github.com/rofl0r/libulz) - a collection of useful functions and data structures to create C apps faster. focus on simplicity, ability to statically link and minimal binary size.
* [sdroege/snippets](https://github.com/sdroege/snippets) - Some algorithms and data structures
* [cirosantilli/cpp-cheat](https://github.com/cirosantilli/cpp-cheat) - C, C++, POSIX and Linux system programming minimal examples. Asserts used wherever possible. Hello worlds for cool third party libraries and build systems. Cheatsheets, tutorials and mini-projects.
* [lbrito1/cstuff](https://github.com/lbrito1/cstuff) - Algorithms & data structures in C
* [Krakonos/cutils](https://github.com/Krakonos/cutils) - C utilities and data structures
* [angelortega/mpdm](https://github.com/angelortega/mpdm) - Minimum Profit Data Manager
* [harnold/generic-c](https://github.com/harnold/generic-c) - A library of generic data structures and algorithms for C, in the spirit of the STL
* [pforemski/libpjf](https://github.com/pforemski/libpjf) - A C library of data structures with tools (based on libasn)
* [rgantt/compsci.c](https://github.com/rgantt/compsci.c) - data structures, algorithms, and musings in C
* [stevedekorte/basekit](https://github.com/stevedekorte/basekit) - C based OO portable data structure library
* [rampantpixels/foundation_lib](https://github.com/rampantpixels/foundation_lib) - Cross-platform public domain foundation library in C providing basic support data types and functions to write applications and games in a platform-independent fashion.

## Scientific ##
Math mostly located in *Calculations* category
* [GuillaumeHolley/BloomFilterTrie](https://github.com/GuillaumeHolley/BloomFilterTrie) - A data structure for pan-genome storage
* [noporpoise/seq_file](https://github.com/noporpoise/seq_file) - Library for Reading Bioinformatic Sequence Data in C
* [r0nk/corvus](https://github.com/r0nk/corvus) - Genetic BF programming
* [Netflix/dynomite](https://github.com/Netflix/dynomite) - A generic dynamo implementation for different k-v storage engines
* [XenonofArcticus/DynamicTrack](https://github.com/XenonofArcticus/DynamicTrack) - Access sources of dynamically-updated data about discrete entities like GPSes, INSes, ADS-B sources.
* [ericmandel/funtools](https://github.com/ericmandel/funtools) - A "minimal buy-in" FITS library and utility package for astronomical data analysis

## Special Purpose ##
* [Tulip Indicators][394] - Library of functions for technical analysis of
  financial data. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [libtrading][395] - Implementation of network protocols for communicating
  with exchanges, dark pools and other trading venues. Supports FIX, FIX/FAST
  and many proprietary protocols. [``BSD-2-Clause``][BSD-2-Clause]
* [AaronJackson/sage-in-c](https://github.com/AaronJackson/sage-in-c) - Simple library written in C for accessing invoices and company data created by Sage Accounts 50.
* [JayDDee/cpuminer-opt](https://github.com/JayDDee/cpuminer-opt) - Optimized multi algo CPU miner
* [MatthewLM/cbitcoin](https://github.com/MatthewLM/cbitcoin) - A low-level bitcoin library written in standard C.
* [RhysU/ESIO](https://github.com/RhysU/ESIO) - The ExaScale IO (ESIO) library provides simple, high throughput input and output of structured data sets using parallel HDF5. ESIO is designed to support reading and writing turbulence simulation restart files within C, C++, and modern Fortran applications.
* [TPSully/SRTM2STL](https://github.com/TPSully/SRTM2STL) - Create STL files from SRTM data for the purpose of creating 3D relief maps.
* [TravisWhitaker/FermiShell](https://github.com/TravisWhitaker/FermiShell) - Retrieve, compare, calculate, analyze, graph, simulate, and experiment with chemical data.
* [TulipCharts/tulipindicators](https://github.com/TulipCharts/tulipindicators) - Technical Analysis Indicator Function Library in C
* [Unidata/netcdf-c](https://github.com/Unidata/netcdf-c) - Official GitHub repository for netCDF-C libraries and utilities.
* [anza/metar](https://github.com/anza/metar) - METAR data fetcher and parser
* [cbuchner1/CudaMiner](https://github.com/cbuchner1/CudaMiner) - a CUDA accelerated litecoin mining application based on pooler's CPU miner
* [jgarzik/cpuminer](https://github.com/jgarzik/cpuminer) - CPU miner for bitcoin
* [jgarzik/picocoin](https://github.com/jgarzik/picocoin) - A bitcoin library in C, SPV wallet & more.
* [libtrading/libtrading](https://github.com/libtrading/libtrading) - Libtrading, an ultra low-latency trading connectivity library for C and C++.
* [nayuki/QR-Code-generator](https://github.com/nayuki/QR-Code-generator) - High-quality QR Code generator library in Java, JavaScript, Python, C++, C.
* [qiq/Czech-morphology](https://github.com/qiq/Czech-morphology) - Czech morphology library, using data files compatible with PDT 2.0
* [sleuthkit/sleuthkit](https://github.com/sleuthkit/sleuthkit) - The Sleuth Kit® (TSK) is a library and collection of command line digital forensics tools that allow you to investigate volume and file system data. The library can be incorporated into larger digital forensics tools and the command line tools can be directly used to find evidence.
* [hroptatyr/uterus](https://github.com/hroptatyr/uterus) - universal tick encoder library to efficiently transport huge amounts of tick data

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
* [marssaxman/startc](https://github.com/marssaxman/startc) - minimal freestanding C library for bare-metal i386 development
* [olibc/olibc](https://github.com/olibc/olibc) - Another C Library optimized for Embedded Linux
* [redjack/libcork](https://github.com/redjack/libcork) - A simple, easily embeddable cross-platform C library
* [wolkykim/qlibc](https://github.com/wolkykim/qlibc) - qLibc is a simple and powerful C library
* [lpsantil/rt0](https://github.com/lpsantil/rt0) - A minimal C runtime for Linux i386 & x86_64

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
* [utf8.h](https://github.com/sheredom/utf8.h) - Single header utf8 string functions. [`Unlicense`](http://unlicense.org/)
* [utf8proc](https://github.com/JuliaStrings/utf8proc) - Small, clean library for processing UTF-8 Unicode data. [`License`](https://github.com/JuliaStrings/utf8proc/blob/master/LICENSE.md)
* [JuliaStrings/utf8proc](https://github.com/JuliaStrings/utf8proc) - a clean C library for processing UTF-8 Unicode data
* [antirez/sds](https://github.com/antirez/sds) - Simple Dynamic Strings library for C
* [boyerjohn/rapidstring](https://github.com/boyerjohn/rapidstring) - Maybe the fastest string library ever.
* [clibs/buffer](https://github.com/clibs/buffer) - Tiny C string library
* [cloudwu/cstring](https://github.com/cloudwu/cstring) - A simple C string lib
* [chrisjmccormick/word2vec_commented](https://github.com/chrisjmccormick/word2vec_commented) - Commented (but unaltered) version of original word2vec C implementation.
* [flori/amatch](https://github.com/flori/amatch) - Approximate String Matching library
* [fontforge/libuninameslist](https://github.com/fontforge/libuninameslist) - A library with a large (sparse) array mapping each unicode code point to the annotation data for it provided in http://www.unicode.org/Public/UNIDATA/NamesList.txt
* [jasonmaclafferty/String](https://github.com/jasonmaclafferty/String) - A dynamic string data type implementation for C.
* [josephg/librope](https://github.com/josephg/librope) - UTF-8 rope library for C
* [sheredom/utf8.h](https://github.com/sheredom/utf8.h) - single header utf8 string functions for C and C++
* [sds](https://github.com/antirez/sds) - dynamic strings library
* [branchless-utf8](https://github.com/skeeto/branchless-utf8) - Branchless UTF-8 decoder

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
* [bvdberg/ctest](https://github.com/bvdberg/ctest) - ctest is a unit test framework for software written in C.
* [clear-code/cutter](https://github.com/clear-code/cutter) - An easy to write and debug unit testing framework for C and C++.
* [compiler-dept/speck](https://github.com/compiler-dept/speck) - A small unit testing framework for C
* [joewalnes/tinytest](https://github.com/joewalnes/tinytest) - A tiny unit-testing framework for C
* [libcheck/check](https://github.com/libcheck/check) - A unit testing framework for C
* [lpabon/cmockery2](https://github.com/lpabon/cmockery2) - Reviving cmockery unit test framework from Google
* [mcandre/qc](https://github.com/mcandre/qc) - qc - A C port of the QuickCheck unit test framework
* [mchochlov/Gnucash](https://github.com/mchochlov/Gnucash) - Data model unit testing - GSoC 2011
* [mortie/snow](https://github.com/mortie/snow) - A testing library for C.
* [orangeduck/ptest](https://github.com/orangeduck/ptest) - DRY Microtesting Framework for C
* [pozorvlak/libtap](https://github.com/pozorvlak/libtap) - Testing library for C, implementing the Test Anything Protocol. Written by Nik Clayton.
* [silentbicycle/greatest](https://github.com/silentbicycle/greatest) - A C testing library in 1 file. No dependencies, no dynamic allocation. ISC licensed.
* [silentbicycle/theft](https://github.com/silentbicycle/theft) - property-based testing for C: generate input to find obscure bugs, then reduce to minimal failing input
* [siu/minunit](https://github.com/siu/minunit) - Minimal unit testing framework for C
* [stephenmathieson/describe.h](https://github.com/stephenmathieson/describe.h) - Simple BDD describe test thingy for C
* [vmg/clar](https://github.com/vmg/clar) - What tests are made of.

## TUI ##
Textual User Interface
* [progressbar][371] - Easy-to-use library for displaying text progress bars. [``BSD-3-Clause``][BSD-3-Clause]
* [netbsd-curses][372] - Simplified and small version of ncurses, with the same
  interface. [``BSD-3-Clause``][BSD-3-Clause]
* [ncurses][373] - Coloured terminal UI library. [``MIT``][MIT]
* [termbox][374] - Library for writing text-based interfaces. [``MIT``][MIT]
* [bartobri/bmenu](https://github.com/bartobri/bmenu) - A generic terminal menu written in C.
* [doches/progressbar](https://github.com/doches/progressbar) - An easy-to-use C library for displaying text progress bars.
* [hpjansson/chafa](https://github.com/hpjansson/chafa) - 📺🗿 Terminal graphics for the 21st century.
* [jwerle/progress.c](https://github.com/jwerle/progress.c) - Progress display lib for c
* [nsf/termbox](https://github.com/nsf/termbox) - Library for writing text-based user interfaces
* [alandekok/recli](https://github.com/alandekok/recli) - A re-imagined CLI.  Customizable syntax, help, permissions, data types.

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
* [babelouest/ulfius](https://github.com/babelouest/ulfius) - Web Framework to build REST APIs, Webservices or any HTTP endpoint in C language. Can stream large amount of data, integrate JSON data with Jansson, and create websocket services
* [bitly/simplehttp](https://github.com/bitly/simplehttp) - a family of libraries and daemons for building scalable web infrastructure
* [boazsegev/facil.io](https://github.com/boazsegev/facil.io) - Your high performance web application C framework
* [ccxvii/mujs](https://github.com/ccxvii/mujs) - An embeddable Javascript interpreter in C.
* [cesanta/mongoose](https://github.com/cesanta/mongoose) - Embedded web server for C/C++
* [cesanta/smart.js](https://github.com/cesanta/smart.js) - Embedded Javascript engine for C/C++ with networking, file, database and device interfaces
* [cesanta/v7](https://github.com/cesanta/v7) - Embedded JavaScript engine for C/C++
* [criticalstack/libevhtp](https://github.com/criticalstack/libevhtp) - Create extremely-fast and secure embedded HTTP servers with ease.
* [danielwaterworth/Raphters](https://github.com/danielwaterworth/Raphters) - [DEPRECATED] A web framework for C.
* [davidmoreno/onion](https://github.com/davidmoreno/onion) - C library to create simple HTTP servers and Web Applications.
* [embedthis/appweb](https://github.com/embedthis/appweb) - Appweb Embedded Web Server
* [haiwen/ccnet](https://github.com/haiwen/ccnet) - Ccnet is a framework for writing networked applications in C.
* [haywire/haywire](https://github.com/haywire/haywire) - Haywire is an asynchronous HTTP server framework written in C that's built using the event loop based libuv platform layer that node.js is built on top of.
* [iafonov/cosmonaut](https://github.com/iafonov/cosmonaut) - Fast web server & micro framework implemented in C. Just for fun.
* [it4e/CHL](https://github.com/it4e/CHL) - C Hypertext Library - A library for writing web applications in C
* [jorisvink/kore](https://github.com/jorisvink/kore) - An easy to use, scalable and secure web application framework for writing web APIs in C.
* [kellabyte/Haywire](https://github.com/kellabyte/Haywire) - Asynchronous HTTP server framework written in C that's built using the event loop based libuv platform layer that node.js is built on top of.
* [monkey/duda](https://github.com/monkey/duda) - Duda I/O is an event-driven and high performant web services framework which exposes a friendly C API
* [oneoo/alilua](https://github.com/oneoo/alilua) - epoll/kqueue+lua based web server
* [riolet/WAFer](https://github.com/riolet/WAFer) - WAFer is a C language-based software platform for scalable server-side and networking applications. Think node.js for C programmers.
* [riolet/nope.c](https://github.com/riolet/nope.c) - nope.c is a C language-based software platform for scalable server-side and networking applications. Think node.js for C programmers.
* [lexborisov/Modest](https://github.com/lexborisov/Modest) - Modest is a fast HTML renderer implemented as a pure C99 library with no outside dependencies.
* [lexborisov/myhtml](https://github.com/lexborisov/myhtml) - Fast C/C++ HTML 5 Parser. Using threads.
* [htacg/tidy-html5](https://github.com/htacg/tidy-html5) - The granddaddy of HTML tools, with support for modern standards
* [mongrel2/mongrel2](https://github.com/mongrel2/mongrel2) - The Mongrel2 Web Server Project
* [shenfeng/tiny-web-server](https://github.com/shenfeng/tiny-web-server) - a tiny web server in C, for daily use.

## Web Service APIs ##
* [twitc][426] - Mini library for interacting with the Twitter OAuth API. [``MIT``][MIT]
* [dajobe/flickcurl](https://github.com/dajobe/flickcurl) - Flickr C API library
* [Cotix/cReddit](https://github.com/Cotix/cReddit) - CLI Reddit client written in C. Oh, crossplatform too!
* [HalosGhost/shaman](https://github.com/HalosGhost/shaman) - A small, native C library and utility to fetch weather
* [PromyLOPh/pianobar](https://github.com/PromyLOPh/pianobar) - Console-based pandora.com player
* [TOTBWF/SteamCurses](https://github.com/TOTBWF/SteamCurses) - A Basic NCurses Client for Steam
* [Yubico/yubico-c-client](https://github.com/Yubico/yubico-c-client) - Yubico C client library
* [adobkin/libcapn](https://github.com/adobkin/libcapn) - A simple C Library for interact with the Apple Push Notification Service (APNs)
* [andrewstone/AbqData](https://github.com/andrewstone/AbqData) - Tools to read ABQ Open Data Initiative city gov data
* [aws/aws-iot-device-sdk-embedded-C](https://github.com/aws/aws-iot-device-sdk-embedded-C) - SDK for connecting to AWS IoT from a device using embedded C.

[424]: http://coap.technology/

# Uncategorized #
* [tm][432] -  Timer and Timeline Utils for C. [``MIT``][MIT]
* [libgit2](https://libgit2.org/) - Pure C implementation of Git. [`GNU GPL2 only, with a linking exception`](https://github.com/libgit2/libgit2/blob/master/COPYING)
* [ThomasHabets/monotonic_clock](https://github.com/ThomasHabets/monotonic_clock) - Portable C library for getting monotonic time
* [ellson/graphviz](https://github.com/ellson/graphviz) - Graph Visualization Tools
* [elvismt/slope](https://github.com/elvismt/slope) - A library to create charts from raw data using cairo. Can be shown in GtkDrawingArea
* [h2non/semver.c](https://github.com/h2non/semver.c) - semantic version parser and serializer written in ANSI C
* [libical/libical](https://github.com/libical/libical) - Libical is an Open Source implementation of the iCalendar protocols and protocol data units.
* [jonpe960/ufsm](https://github.com/jonpe960/ufsm) - UML Statechart library in C and XMI importer
* [locasto/libdisorder](https://github.com/locasto/libdisorder) - A simple C library for entropy measurement of byte streams and other data.
* [lucasb-eyer/heatmap](https://github.com/lucasb-eyer/heatmap) - High performance C heatmap generation library. Supposed to be wrapped by higher-level languages.
* [tailhook/objpath](https://github.com/tailhook/objpath) - A library that allows to traverse data structures by path
* [vmg/houdini](https://github.com/vmg/houdini) - The Escapist
* [luke-jr/bfgminer](https://github.com/luke-jr/bfgminer) - Modular ASIC/FPGA miner written in C, featuring overclocking, monitoring, fan speed control and remote interface capabilities.
* [pornin/CTTK](https://github.com/pornin/CTTK) - Constant-Time Toolkit
* [juliettef/IconFontCppHeaders](https://github.com/juliettef/IconFontCppHeaders) - C, C++ headers and C# classes for icon fonts: Font Awesome, Fork Awesome, Material Design, Material Design icons, Kenney game icons and Ionicons.

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
[473]: https://computing.llnl.gov/tutorials/mpi/
[472]: https://computing.llnl.gov/tutorials/openMP/
[471]: https://www.youtube.com/playlist?list=PLLX-Q6B8xqZ8n8bwjGdzBJ25X2utwnoEG
[466]: http://blog.noctua-software.com/c-tricks.html
[465]: https://blogs.oracle.com/linux/8-gdb-tricks-you-should-know-v2
[464]: http://blog.pkh.me/p/20-templating-in-c.html
[462]: https://computing.llnl.gov/tutorials/pthreads/
[461]: https://web.archive.org/web/20170620131430/https://www.tedunangst.com/flak/post/memcpy-vs-memmove

[452]: http://c-faq.com/

[440]: https://github.com/alanxz/rabbitmq-c
[439]: https://github.com/dertuxmalwieder/libvldmail
[438]: https://github.com/nfc-tools/libnfc
[437]: https://github.com/cloudwu/pbc
[435]: https://gnu.org/software/gss/
[433]: https://github.com/antirez/linenoise
[432]: https://github.com/recp/tm
[427]: https://criu.org/Main_Page
[426]: https://github.com/sinemetu1/twitc
[425]: https://www.gnu.org/software/gnulib/
[422]: https://gnu.org/software/freeipmi/index.html
[421]: https://github.com/commonmark/cmark/blob/master/COPYING
[420]: https://github.com/commonmark/cmark
[417]: https://github.com/simplegeo/libgeohash


[409]: https://github.com/google/cpu_features
[408]: https://github.com/libimobiledevice/libimobiledevice
[407]: https://libusb.info/

[404]: https://github.com/atgreen/libffi

[403]: http://libcox.symisc.net/
[402]: https://github.com/dmw/caffeine
[401]: http://savannah.nongnu.org/projects/attr/

[398]: http://facebook.github.io/libphenom/index.html
[397]: http://libuv.org

[395]: http://libtrading.org/
[394]: https://tulipindicators.org/


[388]: https://github.com/mozilla/mozjpeg
[387]: http://www.vips.ecs.soton.ac.uk/index.php?title=VIPS
[385]: http://www.libpng.org/
[384]: https://libjpeg-turbo.virtualgl.org/
[383]: https://pngquant.org/lib/
[382]: https://github.com/prideout/heman

[378]: https://github.com/riolet/WAFer
[377]: http://www.pell.portland.or.us/~orc/Code/discount/
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

[329]: https://github.com/benhoyt/inih
[328]: https://lloyd.github.io/yajl/
[327]: https://github.com/netmail-open/wjelement/
[326]: https://github.com/sheredom/json.h
[325]: https://zserge.com/jsmn.html
[323]: http://www.digip.org/jansson/

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
[271]: https://github.com/cvxgrp/scs
[270]: http://www.mcs.anl.gov/petsc/
[269]: http://pari.math.u-bordeaux.fr/
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
[255]: http://www.feynarts.de/cuba/
[254]: https://scientificc.github.io/cmathl/
[253]: https://github.com/clMathLibraries/clBLAS
[252]: http://math-atlas.sourceforge.net/
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
[224]: http://libsound.io
[222]: https://mpv.io
[221]: https://gstreamer.freedesktop.org/
[220]: https://www.ffmpeg.org/
[219]: https://github.com/aubio/aubio

[215]: https://github.com/rampantpixels/rpmalloc
[213]: http://jemalloc.net

[211]: http://xforms-toolkit.org/
[210]: http://www.tcl.tk/
[208]: https://github.com/vurtun/nuklear
[207]: http://webserver2.tecgraf.puc-rio.br/iup/
[206]: https://www.gtk.org/

[205]: https://spdx.org/licenses/MPL-1.1.html
[204]: http://www.sgi.com/tech/opengl/?/license.html
[203]: https://www.opengl.org/
[202]: https://github.com/memononen/nanovg
[201]: https://github.com/ands/lightmapper
[197]: http://ebassi.github.io/graphene/
[196]: http://cairographics.org/

[194]: https://clover.moe/spearmint
[191]: https://www.libsdl.org/
[190]: https://www.libretro.com/
[189]: https://github.com/libretro/RetroArch
[188]: https://www.raylib.com
[187]: https://github.com/id-Software/Quake-2
[186]: https://github.com/id-Software/Quake
[185]: http://orx-project.org
[183]: https://xiph.org/ao/
[182]: https://github.com/Kazade/kazmath
[181]: https://ioquake3.org
[180]: https://www.glfw.org/
[179]: http://freeglut.sourceforge.net
[176]: https://icculus.org/twilight/darkplaces/
[175]: https://www.sfml-dev.org/index.php
[174]: https://www.sfml-dev.org/download/csfml/
[173]: https://github.com/orangeduck/Corange
[172]: http://chipmunk-physics.net
[171]: https://github.com/recp/cglm
[170]: https://liballeg.org

[169]: http://cyan4973.github.io/xxHash
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

[106]: http://troydhanson.github.io/uthash/
[99]: https://igraph.org/
[96]: https://github.com/jtsiomb/kdtree

[93]: https://unqlite.org/
[92]: https://www.sqlite.org/
[91]: https://github.com/spotify/sparkey
[90]: http://sophia.systems
[89]: https://redis.io/
[88]: https://www.postgresql.org/
[87]: https://symas.com/lightning-memory-mapped-database/
[85]: https://github.com/redis/hiredis
[83]: http://www.oracle.com/us/products/database/berkeley-db

[82]: https://github.com/trezor/trezor-crypto
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

[68]: https://tinycthread.github.io/
[67]: https://en.wikipedia.org/wiki/POSIX_Threads
[66]: https://gnu.org/software/pth/
[64]: https://www.open-mpi.org/
[63]: https://www.openmp.org/
[60]: http://libmill.org/
[57]: http://libdill.org/
[54]: http://concurrencykit.org
[52]: http://repo.hu/projects/cchan/

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
