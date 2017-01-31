==============
Exercise 1
==============

The aim of this exercise is to "dockerize" RegCM, a REGional Climate Model system currently maintained in the Earth System Physics (ESP) section of the ICTP.

You can download the code from [GForge](http://gforge.ictp.it/gf/project/regcm/frs/) (select the version 4.5).

Use ubuntu:16.04 or centos:7.2.1511 as starting image.

To complete this exercise, you are expected to delivery a Dockerfile that generates a working image with RegCM installed.

To test if the image works as expected, run it in a container and use the following command from the directory where you have installed RegCM

```
./regcmMPI /regcm_input/test_001.in
```

When you run the docker container, use the following parameters to have some valid input files (it will mount some input directories inside your container)

```
-v /lustre/mhpc/regcm_input_samples:/regcm_input -v /lustre/mhpc/regcm_output_samples:/regcm_output
```
