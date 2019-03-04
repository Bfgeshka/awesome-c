# Awesome C #

A curated list of C good stuff.

**An important note:** first and foremost linked resources are for C, therefore
C++ is an afterthought.

**Note:** there are several awesome-c lists already, but they are having
somewhat different sets of libraries in them. This list tries to incorporate
them all, and many more other resources. Consider it my personal cheat sheet and
index for easier search instead of github stars.


## Index ##

* [Meta](#meta)
	* [Standarts](#standarts)
	* [Tooling](#tooling)
		* [Build Systems](#build-systems)
		* [Compilers](#compilers)
		* [Debugging And Analysis](#debugging-and-analysis)
		* [Documentation Generation](#documentation-generation)
		* [Editors](#editors)
		* [Profiling](#profiling)
		* [Text Editor Extensions](#text-editor-extensions)
		* [Utilities](#utilities)

--------------------------------------------------------------------------------

* [AI](#ai)
* [Compression](#compression)
* [Concurrency And Parallelism](#concurrency-and-parallelism)
* [Crypto](#crypto)
* [Databases](#databases)
* [Data Structures](#data-structures)
* [Hashing](#hashing)
* [Multiple Purpose Libraries](#multiple-purpose-libraries)

--------------------------------------------------------------------------------

## Meta ##

### Standarts ###
* [Draft C89 standard][1]
* [Draft C99 standard][2]
* [Draft C11 standard][3]
* [Draft C18 standard][4]

### Tooling ###
Compilers and other tooling.

#### Build Systems ####
* [CMake][11] - Cross-platform family of tools designed to build, package and
  test software. Written in C++11. [``BSD-3-Clause``][BSD-3-Clause]
* [GNU Make][12] - Tool which controls the generation of executables and other
  non-source files of a program. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GMSL][146] - GNU Make Standard Library; a collection of additional
  functionality for GNU Make. [``BSD-3-Clause``][BSD-3-Clause]
* [Meson][13] -  Build system based on Ninja and Python. [``Apache-2.0``][Apache-2.0]
* [Premake][14] - Generates project files for Visual Studio, Xcode and GNU Make.
  Targets suppport can be extended via modules. [``BSD-3-Clause``][BSD-3-Clause]
* [SCons][15] - Software construction tool based on Python. [``MIT``][MIT]
* [xmake][16] - Cross-platform build utility based on Lua. [``Apache-2.0``][Apache-2.0]
* [zproject][17] - Project generator and build system support tool for ZeroMQ
  project. [``MPL-2.0``][MPL-2.0]

#### Compilers ####
* [GCC][18] - Provides a C compiler as part of its compiler set. Supports C11. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Clang][19] - Compiler for LLVM. Supports C11. [``NCSA``][NCSA]
* [PCC][20] - Venerable compiler. Supports C99. [Various licenses][21], all
  open source.

#### Debugging And Analysis ####
* [C-Reduce][108] - Tool that takes a large C file with a property of interest
  and automatically produces a much smaller C file that has the same property.
  Intended to help create minimal bug-demonstrating cases in complex code. [``BSD-3-Clause``][BSD-3-Clause]
* [CBMC][109] - C Bounded Model Checker; a tool for verification of array
  bounds, pointer safety and user-specified assertions. [``BSD-4-Clause``][BSD-4-Clause]
* [GNU cflow][110] - Analyzes a collection of source files and prints a graph
  charting control flow in the program. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GNU Complexity][111] - Tool for measuring the complexity of source code. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [CScout][112] - Source code analyzer and refactoring browser for C programs. [``GPL-3.0-only``][GPL-3.0-only]
* [GNU DDD][113] - Graphical front-end for a range of command-line debuggers. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GDB][114] - GNU Project debugger. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [lldb][115] - LLVM debugger. [``NCSA``][NCSA]
* [rr][116] - Debugger that records non-deterministic executions to allow for
  deterministic debugging. [``BSD-2-Clause``][BSD-2-Clause]
* [Valgrind][117] - Range of dynamic analysis tools, including a leak checker. [``GPL-2.0-only``][GPL-2.0-only]
* [address-sanitizer][138] - Fast memory error detector. [``Apache-2.0``][Apache-2.0]
* [ClangCheck][144] - Static analysis tool, designed to work with Clang. [``NCSA``][NCSA]
* [Cppcheck][145] - Static analysis tool. Despite the name, works well with C. [``GPL-3.0-or-later``][GPL-3.0-or-later]

#### Documentation Generation ####
* [Cxref][118] - Generates documentation in either LaTeX, HTML, RTF or SGML. [``GPL-2.0-only``][GPL-2.0-only]
* [DocOnce][119] - Modestly tagged markup language that can be used to generate
  a range of formats. [``BSD-3-Clause``][BSD-3-Clause]
* [Doxygen][120] - De-facto standard tool for generating documentation from
  annotated sources. Can generate a large range of formats. [``GPL-2.0-only``][GPL-2.0-only]

#### Editors ####
IDEs and text editors with good support of C specifics.

* [Anjuta DevStudio][121] - GNOME IDE. [``GPL-2.0-only``][GPL-2.0-only]
* [Code::Blocks][122] - Extendable, configurable IDE supporting C. [``GPL-3.0-only``][GPL-3.0-only]
* [CodeLite][123] - Cross-platform IDE. [``GPL-2.0-only``][GPL-2.0-only]
* [Geany][124] - Small and fast IDE. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [KDevelop][125] - KDE IDE. [``GPL-2.0-only``][GPL-2.0-only]

#### Profiling ####
* [gperftools][126] - Collection of utilities for measuring and improving
  performance. [``BSD-3-Clause``][BSD-3-Clause]
* [gprof][127] - Performance analysis tool. Part of GNU binutils. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [OProfile][128] - Statistical profiler for Linux. Can profile any code
  (including the kernel!) with low overhead and without recompilation. [``GPL-2.0-only``][GPL-2.0-only]
* [perf][129] - Linux kernel-based profiler with a lot of functionality. [``GPL-2.0-only``][GPL-2.0-only]

#### Text Editor Extensions ####
* [CCompletion][130] - Notepad++ autocompletion plugin. Works with all
  identifiers recognized by Ctags. This is a download link. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [CEDET][131] - Collection of Emacs Development Environment Tools; designed to
  provide IDE-like features to Emacs. Built-in. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Flycheck][132] - Modern syntax checking for Emacs. For C, it can use either
  GCC or Clang as a back-end. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [Neomake][133] - Async :make and linting framework for Neovim/Vim. [``MIT``][MIT]
* [Syntastic][134] - Syntax checking and linting for Vim. [``WTFPL``][WTFPL]
* [YASnippet][135] - Emacs code template system, with C templates for common
  snippets. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [YouCompleteMe][136] - Code completion engine for Vim. [``GPL-3.0-only``][GPL-3.0-only]

#### Utilities ####
* [ccache][22] - Compiler cache designed to speed up recompilation. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [distcc][23] - Program that allows builds to be distributed among several
  machines. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [Firm][24] - Library that provides a graph-based intermediate representation,
  optimizations and assembly code generation suitable for use in compilers.
  Comes with an example C front-end under the same license. [``LGPL-2.1-only``][LGPL-2.1-only]
* [Artistic Style][137] - Fast and small automatic source code formatter that
  supports C. [``LGPL-3.0-only``][LGPL-3.0-only]
* [biicode][139] - Dependency manager. [``MIT``][MIT]
* [c][140] - Compile and execute C "scripts" in one go on the command line. Also
  has shebang support. [``MIT``][MIT]
* [c99sh][141] - Run C files using hash-bang. [``BSD-2-Clause``][BSD-2-Clause]
* [cdecl][142] - Online service to translate C declarations into English and
  vice versa. Public domain.
* [cinclude2dot][143] - Graphs include dependencies in a project using Graphviz. [GPL-1.0-or-later][335] or [``GPL-2.0-or-later``][GPL-2.0-or-later] or [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [GNU Global][147] - Source code tagging tool. [``GPL-3.0-only``][GPL-3.0-only]
* [GPP][148] - General-purpose preprocessor. More versatile than the C
  preprocessor, but more flexible than m4. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [Highlight][149] - Converts source code to formatted text with highlighting. [``GPL-3.0-only``][GPL-3.0-only]
* [include-what-you-use][150] - Helps find unecessary inclusions and make
  suggestions for fixing them. Based on LLVM/Clang (and only works with it). [``NCSA``][NCSA]
* [indent][151] - Formats C source code automatically to make it easier to
  read. Also converts from one style of source to another. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [SMACK][152] - Modular software verification toolchain and a self-contained
  software verifier. Currently only works with programs compiled using Clang. [``MIT``][MIT]
* [unifdef][153] - Removes #ifdef and #if directives with their delimited text
  without touching any other part of the file. [``BSD-3-Clause``][BSD-3-Clause] or [``BSD-2-Clause``][BSD-2-Clause]

--------------------------------------------------------------------------------

## Contents ##

### AI ###
Computer vision, neural nets, machine learning, and other similar things.
Basically, if your university calls it AI, it lives here.

* [ccv][5] - C-based/Cached/Core Computer Vision library; modern computer
  vision. [``BSD-3-Clause``][BSD-3-Clause]
* [Cranium][6] - Portable, header-only ANN library in C99. [``MIT``][MIT]
* [FANN][7] - Fast Artifical Neural Network library; an implementation of neural
  networks. [``GPL-2.0-only``][GPL-2.0-only]
* [Genann][8] - Simple ANN in C89, without additional dependencies. [``Zlib``][Zlib]
* [KANN][9] - Two-file ANN library. [``MIT``][MIT]
* [LibDEEP][10] - Deep learning library. [``BSD-3-Clause``][BSD-3-Clause]

### Compression ###
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

### Concurrency And Parallelism ###
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

### Crypto ###
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

### Databases ###
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

### Data Structures ###
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

### Multiple Purpose Libraries ###
* [pal][65] - Optimized library for maths, parallel processing and data
  movement. [``Apache-2.0``][Apache-2.0]
* [APR][154] - Apache Portable Runtime; another library of cross-platform utility
  functions. [``Apache-2.0``][Apache-2.0]
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


-=-=-=-=-=-=-=-=-=-
UNSORTED
* [debug][467] - One-header library for easier 'printf debugging'. [``MIT``][MIT]
* [Glade][328] - RAD tool to enable quick development of GTK+ GUIs. [``GPL-2.0-only``][GPL-2.0-only]



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

[153]: http://dotat.at/prog/unifdef/
[152]: https://github.com/smackers/smack
[151]: https://www.gnu.org/software/indent/
[150]: https://github.com/include-what-you-use/include-what-you-use
[149]: http://www.andre-simon.de/doku/highlight/en/highlight.php
[148]: https://logological.org/gpp
[147]: https://www.gnu.org/software/global/
[146]: https://gmsl.sourceforge.net/
[145]: http://cppcheck.sourceforge.net/
[144]: https://clang.llvm.org/docs/ClangCheck.html
[143]: https://www.flourish.org/cinclude2dot/
[142]: https://cdecl.org/
[141]: https://github.com/RhysU/c99sh
[140]: https://github.com/ryanmjacobs/c
[139]: https://biicode.github.io/biicode/
[138]: https://github.com/google/sanitizers
[137]: http://astyle.sourceforge.net/

[136]: http://valloric.github.io/YouCompleteMe/
[135]: http://joaotavora.github.io/yasnippet/
[134]: https://github.com/vim-syntastic/syntastic
[133]: https://github.com/neomake/neomake
[132]: https://github.com/flycheck/flycheck
[131]: http://cedet.sourceforge.net/
[130]: http://freeweb.siol.net/rmihor/NppCCompletionPlugin.zip

[129]: https://perf.wiki.kernel.org/index.php/Main_Page
[128]: http://oprofile.sourceforge.net/news/
[127]: https://www.gnu.org/software/binutils/
[126]: https://github.com/gperftools/gperftools

[125]: https://www.kdevelop.org/
[124]: https://www.geany.org/
[123]: https://www.codelite.org/
[122]: http://www.codeblocks.org/
[121]: http://anjuta.org/

[120]: http://www.doxygen.nl/
[119]: https://hplgit.github.io/doconce/doc/web/index.html
[118]: http://www.gedanken.org.uk/software/cxref/

[117]: http://www.valgrind.org/
[116]: https://rr-project.org/
[115]: https://lldb.llvm.org/
[114]: https://www.gnu.org/software/gdb/
[113]: https://www.gnu.org/software/ddd/ddd.html
[112]: https://www.spinellis.gr/cscout/
[111]: https://www.gnu.org/software/complexity/
[110]: http://www.gnu.org/software/cflow/
[109]: https://www.cprover.org/cbmc/
[108]: https://embed.cs.utah.edu/creduce/

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

[24]: https://pp.ipd.kit.edu/firm/
[23]: https://github.com/distcc/distcc
[22]: https://ccache.samba.org/
[21]: http://pcc.ludd.ltu.se/licenses/
[20]: http://pcc.ludd.ltu.se/
[19]: https://clang.llvm.org/
[18]: https://gcc.gnu.org/

[17]: https://github.com/zeromq/zproject
[16]: https://xmake.io/
[15]: https://www.scons.org/
[14]: https://github.com/premake/premake-core
[13]: http://mesonbuild.com/
[12]: https://www.gnu.org/software/make/
[11]: https://cmake.org/

[10]: https://github.com/jppbsi/LibDEEP/wiki
[9]: https://github.com/attractivechaos/kann
[8]: https://codeplea.com/genann
[7]: http://leenissen.dk/fann/wp/
[6]: https://github.com/100/Cranium
[5]: http://libccv.org

[4]: https://web.archive.org/web/20181230041359if_/http://www.open-std.org/jtc1/sc22/wg14/www/abq/c17_updated_proposed_fdis.pdf
[3]: https://port70.net/~nsz/c/c11/n1570.html
[2]: https://port70.net/~nsz/c/c99/n1256.html
[1]: https://port70.net/~nsz/c/c89/c89-draft.html

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
