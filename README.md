mruby-test
==========
An example on how to embedded mruby into an C++ program.
It is a playground where I tried different ways to use a ruby script and
how ruby and C++ can interact. This is my first experience in embedding mruby.
I hope I can put more effort into it in the near future.

Installation
============
Currently only a MSVC version is available.
- Install [mruby](http://www.mruby.org/downloads/)
- Set the environment variable `MRUBY_INCLUDE` to the location of the include folder.
- Set the environment variable `MRUBY_LIB` to the location of the generated lib folder.
- To compile and run use the visual studio solution file.

Hint
====
The current project is only use w/ the debug x64 configuration. It is assumed that the mruby compilation is done w/ the compilation flags /D_DEBUG /On /MDd.
If /MDd is not set (which is the default in mruby) the linker complains about not matching 
CRT versions.

