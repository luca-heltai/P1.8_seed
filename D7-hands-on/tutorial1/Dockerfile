FROM ubuntu:latest

RUN apt-get update && apt-get install -y libatlas-base-dev make mpich wget

RUN cd /opt && wget http://www.netlib.org/benchmark/hpl/hpl-2.2.tar.gz && tar -xvf hpl-2.2.tar.gz && mv hpl-2.2 hpl

ADD Make.Linux_ATHLON_CBLAS /opt/hpl

RUN cd /opt/hpl && make arch=Linux_ATHLON_CBLAS
ADD HPL.dat /opt/hpl/bin/Linux_ATHLON_CBLAS
CMD cd /opt/hpl/bin/Linux_ATHLON_CBLAS && mpirun -np 4 ./xhpl HPL.dat
