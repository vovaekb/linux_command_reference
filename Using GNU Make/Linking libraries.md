# Linking system libraries

Assume the task in hand is to compile some C/C++ project, which uses a system libraries (e.g., OpenCV). We need to link proper header files when compiling the project.

Firstly, we can figure out which flags (cflags) we need to use with the compiler:

```bash
pkg-config --cflags opencv
```
and which libs to include:
```bash
pkg-config --libs opencv
```


The input will be like that:
```bash
-I/usr/local/include/opencv -I/usr/local/include
```

Then let`s create a Makefile with content:

```bash
CFLAGS=`pkg-config --cflags opencv`
LIBS=`pkg-config --libs opencv`


example: example.cpp
        g++ -o example example.cpp $(CFLAGS) $(LIBS)
```
