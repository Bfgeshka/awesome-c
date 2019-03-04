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
* [AI](#ai)
* [Tooling](#tooling)
	* [Build Systems](#build-systems)
	* [Compilers](#compilers)
	* [Utilities](#utilities)

## Contents ##

### Meta ###
#### Standart ####

* [Draft C89 standard][1]
* [Draft C99 standard][2]
* [Draft C11 standard][3]
* [Draft C18 standard][4]

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

### Tooling ###
Compilers and other tooling.

#### Build Systems ####
* [CMake][11] - Cross-platform family of tools designed to build, package and
  test software. Written in C++11. [``BSD-3-Clause``][BSD-3-Clause]
* [GNU Make][12] - Tool which controls the generation of executables and other
  non-source files of a program. [``GPL-3.0-or-later``][GPL-3.0-or-later]
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

#### Utilities ####
* [ccache][22] - Compiler cache designed to speed up recompilation. [``GPL-3.0-or-later``][GPL-3.0-or-later]
* [distcc][23] - Program that allows builds to be distributed among several
  machines. [``GPL-2.0-or-later``][GPL-2.0-or-later]
* [Firm][24] - Library that provides a graph-based intermediate
  representation, optimizations and assembly code generation suitable for use in
  compilers. Comes with an example C front-end under the same
  license. [``LGPL-2.1-only``][LGPL-2.1-only]


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
