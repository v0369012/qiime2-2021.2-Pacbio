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

### Add Pacbio processing codes
#### Download the files
`git clone https://github.com/sixvable/q2-dada2-CCS.git`
#### replace the original files
`cp ./q2-dada2-CCS/*.py /yourqiime2path/envs/qiime2-2021.2-Pacbio/lib/python3.6/site-packages/q2_dada2/`
`cp ./q2-dada2-CCS/run_dada_ccs.R /yourqiime2path/envs/qiime2-2021.2-Pacbio/bin`

#### Refresh qiime2
`qiime dev refresh-cache`

#### Check dada2 for Pacbio long reads
`qiime dada2 denoise-ccs --help`

#### Remove the downloaded folder
`rm -r ./q2-dada2-CCS`
