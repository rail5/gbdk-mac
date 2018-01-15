GBDK
====

"The GameBoy Developer's Kit (GBDK), is a set of tools that enable to
develop programs for the Nintendo GameBoy system, either in C or in
assembly. GBDK includes a set of libraries for the most common
requirements and generates image files for use with a real GameBoy or
with an emulator like VGB or no$gmb. [...]

GBDK features:
  * An ANSI C compiler.
  * An assembler that generates relocatable code.
  * A peephole optimiser.
  * A linker that produces GameBoy image files.
  * Support for multiple-bank images.
  * Smart linking.
  * A set of libraries, with source code.
  * Example programs in assembly and in C."

From http://gbdk.sourceforge.net

Quick summary
=============

The base version (2.96a) was downloaded from the official site. Although
this is the latest version, it was released quite a while ago (back in
April 2002).

The code can be compiled in an up-to-date macOS environment

Original sites:
  * http://gbdk.sourceforge.net
  * http://sourceforge.net/projects/gbdk

Building
========

Tested only on macOS 10.13

The environment will need a few packages, all of them can be installed
using homebrew
```
brew install make
brew install gcc
brew install g++
brew install bison
brew install flex
```

After downloading the source you can use the Makefile to compile the
binaries:
```
cd /path/where/you/extracted
make
```

Installing the compiled binaries can be done via make as well:
```
sudo make install
```

Compiling the examples:
```
cd ./gbdk-lib/examples/gb
make
```

Note: compiling the examples requires you to install the binaries you
just built in the previous steps.
