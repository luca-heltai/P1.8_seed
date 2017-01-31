==============
Exercise 4
==============

The aim of this exercise is to create a docker container with GCC and the OpenBlas library installed, that can be used as a
starting image for other containers. GCC can be installed using the package manager, but the openblas must be compiled by hand.
To make your image portable, please compile them for Nehalem or newer CPUs!

You can download the OpenBlas libraries from [www.openblas.net](http://www.openblas.net/) (select the last version).

Use ubuntu:16.04 or centos:7.2.1511 as starting image.

By default, a container created from this image must write on the standard output a message like the following:

    OPENBLAS + GCC container
    *+*+*+*+*+*+*+*+*+*+*+*+*
    
    In this container you will find gcc version #.## and OpenBLAS version ##.##.
    The OpenBLAS library are saved in /#####/#####/####



