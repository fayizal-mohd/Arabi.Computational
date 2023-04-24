# Arabi.Computational
Singularity containers for Alya Research Lab

## Note
Before building singularity containers, please note that you have enough disk space for singularity tmpdir

> Do the below checks to make sure which folder has enough free space to build singularity container

* Issue `df -h` command and find out where the free space is
* Create a tmp directory where you have free space. example `mkdir /opt/tmp` if you have free space in /opt
* Redirect singularity tmpdir to /opt/tmp. example `export SINGULARITY_TMPDIR=/opt/tmp`

## Avogadro
`avogadro.def` file is used to build avogadro container. In order to build avogadro container, execute command
` singularity build avogadro.sif avogadro.def`

> **_NOTE:_** This will take 10-15 minutes to complete

## Amber
`amber.def` file is used to build amber container. 
There are 2 packages needed to build this container. `Amber22.tar.bz2` and `AmberTools22.tar.bz2`. Copy both these files to the directory where `amber.def` is present.



