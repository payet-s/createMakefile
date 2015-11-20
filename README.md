# createMakefile

An easy way to setup a Makefile for C and C++ projects. The script is compatible with Epitech's norm.

It spits out the Makefile on the standard output. You may redirect it to a Makefile using `./createMakefile [options] > Makefile` on the shell.

## How to use it

### Synopsis

Invoke the script with at least the `-S` option and valid source files, and a name (i.e. one of the following options : `-N`, `-A`, `-D`).

    ./createMakefile -S./src -I./include -Na.out
    
### Getting help

`./createMakefile --help` to get a full list of options :

    Options :
            -I<dir>         add include directory
            -S<dir>         add source directory
            -N<name>        set executable name
            -A<name>        set library name
            -D<name>        set dynamiclibrary name
            -C<flags>       add c++ flags
            -c<flags>       add c flags
            -f<flags>       add c and c++ flags
            -L<flags>       add ld flags
            -l<lib,makedir> add library as a dependance, with directory to call make in, and the directory
            -e<regex>       exclude files matching regex
## Features

* Creating compilation rules for `.c` and `.cpp` files.
* Source files have correct include dependancies (searched recursively in header files).
* Add a library as a dependance (will call all/clean/fclean/re when appropriate).

## Remarks and improvement

Feel free to report anything you think useful to florian.sabourin@epitech.eu.