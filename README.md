2016 Institut Curie

Author(s):

* avowinkel
* Jocelyn Brayet (Institut Curie)
* Nicolas Lapalu (INRA)

Avowinkel repository: https://toolshed.g2.bx.psu.edu/view/avowinkel/gatk/b80ff7f43ad1

Contact: jocelyn.brayet@curie.fr, nicolas.lapalu@versailles.inra.fr

## set PATH

```
export GATK_PATH_3_5="path to GenomeAnalysisTK.jar"
export PICARD_PATH="path to picard.jar"
```

## change PATH if necessary

In gatk.xml:

* line 48: java
* line 49: samtools

In gatk_macros.xml:

* line 11: java 

## Change data table:

In gatk.xml
* line 100: <options from_data_table="YOUR_FILE"/>

loc file example:

```
/YOUR_PATH/Human/hg19/gatk/hg19.fasta     hg19    hg19    /YOUR_PATH/Human/hg19/gatk/hg19.fasta
/YOUR_PATH/Mouse/mm9/gatk/mm9.fa  mm9     mm9     /YOUR_PATH/Mouse/mm9/gatk/mm9.fa
/YOUR_PATH/Mouse/mm10/gatk/mm10.fa        mm10    mm10    /YOUR_PATH/Mouse/mm10/gatk/mm10.fa
```

