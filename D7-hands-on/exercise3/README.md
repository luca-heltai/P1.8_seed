==============
Exercise 3
==============

The aim of this exercise is to "dockerize" LAMMPS, a classical molecular dynamics code.

You can download the code from [the official LAMMPS web page](http://lammps.sandia.gov) (select the stable version).

Use ubuntu:16.04 or centos:7.2.1511 as starting image.

To complete this exercise, you are expected to delivery a Dockerfile that generates a working image with LAMMPS installed (compile the serial version).

By default, a container created from this image must execute the in.lj test (lj means Lennard-Jones): you can find it in the bench directory.
To execute the test, put the content of that file in the standard input of the executable that "make" creates in the src directory

