DependencyTest
==============

This project illustrates what seems to be a header-file dependency issue with
Intel's C++ XE 14 compiler combined with Xcode 5.0.2 running on OS X Mavericks.

Steps to reproduce:

1. Open the project and build the single target/scheme.
2. Re-build and note that no extra work is incurred.
3. Modify the header file `module.h`.
4. Re-build and note that `module.cpp` is not rebuilt.