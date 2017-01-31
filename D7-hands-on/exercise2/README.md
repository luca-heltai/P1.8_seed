==============
Exercise 2
==============

The aim of this exercise is to "dockerize" QuantumESPRESSO, a software suite for ab initio quantum chemistry methods of 
electronic-structure calculation and materials modeling.

You can download the code from [QEForge](http://www.qe-forge.org/gf/project/q-e/frs/?action=FrsReleaseBrowse&frs_package_id=18) (select the version 6.0).

Use ubuntu:16.04 or centos:7.2.1511 as starting image.

To complete this exercise, you are expected to delivery a Dockerfile that generates a working image with QuantumESPRESSO installed.

Execute a 

```
make all
```
to compile the code.


By default, a container created from this image must execute "make test-suite" in the main directory!
Your image is expected to pass all the test but two (that end in an unknown status by design).
