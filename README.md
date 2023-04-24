# Arabi.Computational
Singularity containers for Alya Research Lab

## Note
Before building singularity containers, please note that you have enough space for singularity tmpdir
Do the below to check where you have space

* Issue `df -h` command and find out where the free space is
* Create a tmp directory where you have free space. example `mkdir /opt/tmp` if you have free space in /opt
* Redirect singularity tmpdir to /opt/tmp. example `export SINGULARITY_TMPDIR=/opt/tmp`

## Avogadro
`avogadro.def` file is used to build avogadro container. In order to build avogadro container, execute command
` singularity build avogadro.sif avogadro.def`

> **_NOTE:_** This will take 10-15 minutes to complete

