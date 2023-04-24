# Arabi.Computational
Singularity containers for Alya Research Lab

## Note
Before building singularity containers, please note that you have enough disk space for singularity tmpdir

> Do the below checks to make sure which folder has enough free space to build singularity container

* Issue `df -h` command and find out where the free space is
* Create a tmp directory where you have free space. example `mkdir /opt/tmp` if you have free space in `/opt`
* Redirect singularity tmpdir to `/opt/tmp`. example `export SINGULARITY_TMPDIR=/opt/tmp`

## Avogadro
`avogadro.def` file is used to build avogadro container. 

In order to build avogadro container, execute command ` singularity build avogadro.sif avogadro.def`

> **_NOTE:_** This will take 10-15 minutes to complete

## Amber
`amber.def` file is used to build amber container. 

Download `Amber22` and `AmberTools22` from website `https://ambermd.org/GetAmber.php`

Download `openmpi` from website `https://www.open-mpi.org/software/ompi/v4.1/`

There are 3 packages needed to build this container. `Amber22.tar.bz2`, `AmberTools22.tar.bz2` and `openmpi-4.1.5.tar.gz`

Copy all these files to the directory where `amber.def` is present

In order to build amber container, execute command ` singularity build amber.sif amber.def`

> **_NOTE:_** This will take around 30 minutes to complete

## Gnuplot
`gnuplot.def` file is used to build gnuplot container. 

In order to build gnuplot container, execute command ` singularity build gnuplot.sif gnuplot.def`

> **_NOTE:_** This container does not need to change the terminal type to X11



