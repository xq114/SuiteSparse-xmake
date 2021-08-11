# SuiteSparse-xmake
xmake port for SuiteSparse, supporting windows, macosx, linux and a range of other platforms.

## Usage

- Make sure a working compiler (MSVC, gcc, clang, etc.) is present;
- Copy xmake.lua to the root directory in SuiteSparse (along with README.md);
- Execute `xmake` to build the library.
- (Optional) Run `xmake install -o dist` to install library files.

## Notes

- Linking shared library with mkl on linux is currently erroreous, please use OpenBLAS instead or use original makefile instead.
- On windows GPU build is not officially supported. If you need an unofficial GPU build, apply msvc.patch and config with `xmake f --with_cuda=on && xmake`
