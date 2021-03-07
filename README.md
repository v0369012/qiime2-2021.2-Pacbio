# qiime2-2021.2-Pacbio-git

This file allows users to create a conda virtual evironment which has qiime2-2021.2 with the ability to process Pacbio long reads.

The codes processing long reads are from https://github.com/sixvable/q2-dada2-CCS.

#### Download .yml file
`git clone https://github.com/v0369012/qiime2-2021.2-Pacbio-git.git`

#### Create the environment
`cd ./qiime2-2021.2-Pacbio-git`
`conda env create -n qiime2-2021.2-Pacbio --file qiime2-2021.2-Pacbio.yml`

#### Start the environment
`conda activate qiime2-2021.2-Pacbio`
