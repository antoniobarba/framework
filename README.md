## Introduction

This is very early... I don't have anything special to show for, right now. I'm experimenting with C++ and modern web technologies. The goal is to build a fast and memory efficient web backend framework using C++ and HTTP/3.

We'll see!

## Compilation

You'll need Conan2, CMake 3.29 and a compiler capable of c++20.

```
$ git clone something somewhere
$ cd somewhere
$ conan install .
$ cd build
$ ccmake ..
Enable testing if you want Google Test enabled
$ make -j16
$ ./blog 
$ (optional) test/test_framework
```

