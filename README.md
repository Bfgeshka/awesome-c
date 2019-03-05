# Awesome C #

A curated list of C good stuff.

**An important note:** first and foremost linked resources are for C, therefore
C++ is an afterthought.

**Note:** there are several awesome-c lists already, but they are having
somewhat different sets of libraries in them. This list tries to incorporate
them all, and many more other resources. Consider it my personal cheat sheet and
index for easier search instead of github stars. Also, original list categories
are a mess.


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
* [Calculations](#calculations)
* [Compression](#compression)
* [Concurrency And Parallelism](#concurrency-and-parallelism)
* [Crypto](#crypto)
* [Databases](#databases)
* [Data Structures](#data-structures)
* [Game Development](#game-development)
* [Graphics](#graphics)
* [GUI](#gui)
* [Hashing](#hashing)
* [Memory Management](#memory-management)
* [Multimedia](#multimedia)
* [Multiple Purpose Libraries](#multiple-purpose-libraries)
* [Networking](#networking)
* [Regex](#regex)
* [Serialization](#serialization)
* [Source Code Collections](#source-code-collections)
* [Standard Libraries](#standart-libraries)
* [String Manipulation](#string-manipulation)

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

## AI ##
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

## Concurrency And Parallelism ##
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
* [uastar][195] - Minimal A\* implementation. [``ZLib``][Zlib]

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

## GUI ##
Widget toolkits, or things meant to be used in a similar way to them.

* [GTK+][206] - Cross-platform widget toolkit. [``LGPL-2.1-only``][LGPL-2.1-only]
* [IUP][207] - Another cross-platform widget toolkit. [``MIT``][MIT]
* [nuklear][208] - Small, C89, single-header widget toolkit. Public domain.
* [tinyfiledialogs][209] - Single-file library for simple dialogs. Compatible
  with many other toolkits and OSes. [``Zlib``][Zlib]
* [Tk][210] - Basic widget toolkit. Part of Tcl/Tk. [``TCL``][TCL]
* [XForms Toolkit][211] - Widget toolkit designed for the XWindow system. [``LGPL-2.1-only``][LGPL-2.1-only]

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

## Multimedia ##
Audio and video processing

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

## Networking ##
* [asnlc][227] - Compiler of ASN.1 specifications into C source code. [``BSD-2-Clause``][BSD-2-Clause]
* [CHL][228] - C Hypertext Library - A library for writing for web in C. [``GPL-3.0-only``][GPL-3.0-only]
* [GNU adns][229] - Advanced, easy-to-use, asynch-capable DNS client library
  and utilities. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [http-parser][230] - HTTP request/response parser. [``MIT``][MIT]
* [ldns][231] - Library to simplify DNS programming. [``BSD-3-Clause``][BSD-3-Clause]
* [libcurl][232] - Client-side URL transfer library, supporting a wide range of
  formats. [``curl``][curl]
* [LibEtPan][233] - Mail library providing an efficient network for IMAP, SMTP,
  POP and NNTP. [``BSD-3-Clause``][BSD-3-Clause]
* [libhttpd][234] - Library to add basic web server capabilities to an
  application or embedded device. [``GPL-2.0-only``][GPL-2.0-only]
* [libidn][235] - Implementation of the Stringprep, Punycode and IDNA
  specifications. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [libmicrohttpd][236] - Small library that makes it easy to run an HTTP
  server as part of another application. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libonion][237] - HTTP server library, designed to be easy to use. [``Apache-2.0``][Apache-2.0]
* [libquickmail][238] - Library intended to give developers a way to send email
  from their applications. Supports multiple To/Cc/Bcc recipients and
  attachments without size limits. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [libsagui][239] - Library for cross-platform HTTP servers. [``LGPL-3.0-or-later``][LGPL-3.0-or-later]
* [LibVNCServer][240] - Cross-platform libraries to implement VNC server and/or
  client functionality. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [libwebsock][241] - Easy-to-use and powerful web socket library. [``LGPL-3.0-only``][LGPL-3.0-only]
* [lwan][242] - Experimental, scalable, high-performance HTTP server. [``GPL-2.0-only``][GPL-2.0-only]
* [mongoose][243] - Embedded web server. [``GPL-2.0-only``][GPL-2.0-only]
* [nanomsg][244] - C-based implementation of ZeroMQ. [``MIT``][MIT]
* [NNG][245] - nanomsg-next-generation - lightweight brokerless messaging. [``MIT``][MIT]
* [oSip][246] - SIP implementation without additional dependencies. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [socket99][247] - C99 wrapper for the BSD sockets API. [``ISC``][ISC]
* [Wslay][248] - WebSocket library. Implements version 13 of the WebSocket
  protocol, as described in RFC 6455. [``MIT``][MIT]
* [zyre][249] - Framework for proximity-based peer-to-peer applications. [``MPL-2.0``][MPL-2.0]

## Regex ##
* [Onigmo][275] - Fork of Oniguruma, supporting more advanced regexps. [``BSD-2-Clause``][BSD-2-Clause]
* [Oniguruma][276] - Regex library supporting a wide range of encodings, and
  incorporating many security-oriented fixes. [``BSD-2-Clause``][BSD-2-Clause]
* [PCRE][277] - Implementation of regexes identical to that of Perl 5. [``BSD-3-Clause``][BSD-3-Clause]
* [SLRE][278] - Super Light Regular Expression library; a small implementation
  of a subset of Perl regex syntax. [``GPL-2.0-only``][GPL-2.0-only]
* [TRE][279] - POSIX-compliant, feature-full regex library. [``BSD-2-Clause``][BSD-2-Clause]

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

-=-=-=-=-=-=-=-=-=-
UNSORTED
* [debug][467] - One-header library for easier 'printf debugging'. [``MIT``][MIT]
* [Glade][328] - RAD tool to enable quick development of GTK+ GUIs. [``GPL-2.0-only``][GPL-2.0-only]
* [giflib][401] - Library for reading and writing gif images. [``MIT``][MIT]
* [heman][365] - Tiny library of image utilities dealing with height maps,
  normal maps, distance fields and the like. [``MIT``][MIT]
* [libgd][402] - Library for the dynamic creation of images by programmers. [``MIT``][MIT]
* [libimagequant][300] - Small, portable library for high-quality conversion of
  RGBA images to 8-bit indexed colour images. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [libjpeg-turbo][193] - Faster library for reading and writing JPEG files. [Various licences][194].
* [libpng][382] - Official PNG reference library. [``Libpng``][Libpng]
* [libRSVG][417] - Library to render SVG files using Cairo. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [libvips][511] - Image processing library. [``LGPL-2.1-or-later``][LGPL-2.1-or-later]
* [mozjpeg][200] - Improved JPEG encoder. [``BSD-3-Clause``][BSD-3-Clause]
* [lodepng][69] - Simple PNG image decoder and encoder, requiring no other
  dependencies. [``BSD-3-Clause``][BSD-3-Clause]
* [gumbo-parser][196] - HTML5 parsing library in C99. [``Apache-2.0``][Apache-2.0]
* [libev][144] - Yet another event loop. [``BSD-2-Clause``][BSD-2-Clause]
* [libevent][124] - Event loop replacement for network servers. [``BSD-3-Clause``][BSD-3-Clause]
* [twitc][237] - Mini library for interacting with the Twitter OAuth API. [``MIT``][MIT]
* [gnulib][46] - Collection of common GNU code. Various licenses, all
  open source.





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
