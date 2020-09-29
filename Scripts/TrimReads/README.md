#### Trimming reads using Trimmomatic tool

trimmomatic.sh file contains the command line script for using the trimmomatic tool. The inputs files used for this example are from the directory: 
**/data/reddylab/Flowcells/GGR/rna_seq/Reddy_4557_171219A3**. 

The fastq files used ares: A549_FOXO3_OE-RNA_seq-dex-00h-rep1_S1_L001_R1_001.fastq.gz as the input forward strand and A549_FOXO3_OE-RNA_seq-dex-00h-rep1_S1_L001_R2_001.fastq.gz as the input reverse strand. 

#### Trimming reads using trimmomatic.cwl

The below given command is used to execute trimmomatic.cwl script:

`cwltool /data/reddylab/software/cwl/GGR-cwl/v1.0/trimmomatic/trimmomatic.cwl [input-job-settings]`

Input-job-settings can be given in seperate .yml file which makes the script look clean or can be input directly in the command line.

**trim_input.yml** is such a sample .yml file with all the input parameters needed for the execution of the cwl pipeline. The fastq files used for this task is same as the that of the above one.

More information and explanations can be found in the [Wiki page](https://github.com/DukeCAGT/bioinfo_tasks/wiki/Trimming-reads). 
