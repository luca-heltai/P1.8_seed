============================
D6-Hands-on: Openstack 
===========================

To access the CNR/IOM OpenStack dashboard
::

  http://nimbo.escience-lab.it/dashboard


To login on the virtual machines
::

	ssh centos@<ip>


Note
====

To access the OpenStack dashboard and the virtual machine you need to be inside the SISSA network

==========================
Elasticluster installation
==========================


Do on your local system (Ubuntu-Debian)::

 sudo apt-get install gcc g++ git libc6-dev libffi-dev libssl-dev python-dev virtualenv

or (Red-Hat based)::

 yum install gcc gcc-c++ git libffi-devel openssl-devel python-devel python-virtualenv

Create a virtualenv and clone and install::

 virtualenv elasticluster
 . elasticluster/bin/activate
 cd elasticluster
 git clone git://github.com/gc3-uzh-ch/elasticluster.git src
 cd src
 pip install -e .

Then::

 elasticluster start slurm

 elasticluster list

 elasticluster stop slurm


To exit the virtual environment
::

  deactivate  

