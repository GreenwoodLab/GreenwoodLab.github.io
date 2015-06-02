Genomics Ranges
========================================================
author: VOISIN Greg
date:  May, 19 , 2015


Specific data structures in R/BioConductor
========================================================

Some specific data structures are been developped by Bioconductor team:

ExpressionSet/methylSet: Matrix-like dataset plus experiment/sample/feature metadata..
SummarizedExperiment: Analogous to ExpressionSet, but features defined in genomic coordinates.
GRanges :Genomic coordinates and associated qualitative and quantitative information, e. g., gene symbol, coverage, p-value.

S3 and S4 structures: particular structures in R to manage a complex data structure.


R package
========================================================

Lawrence M, Huber W, PagEs H, Aboyoun P, Carlson M, Gentleman R, Morgan M and Carey V (2013).  
"Software for Computing and Annotating Genomic Ranges."  
PLoS Computational Biology, 9.

[Available here](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3738458/pdf/pcbi.1003118.pdf)


Goal
========================================================

* manipulate efficently genomic annotations and alignments in high-throughput data  
* store informations such as genomic intervals, score ...



Three Data structures
========================================================

* Iranges, describes one interval   
* Granges, describes one transcript (for exemple)  
* GrangesList, describes all transcripts of a given gene (for exemple)   


Basic information (not optional) of Granges object
========================================================

**seqnames**: define the chromosome  
**ranges**: define the boundaries of the element ( gene, exons, TFBS...). start/end  
**strand** : +/-/*  

Note1: the start is always the left position and the end the right, even when the range is on the minus strand.  
Note2: seqnames/interval/strand are used for Granges objects comparison.  

metadata informations included in Granges object
========================================================

Extra column of informations. 
accessor mcols()


Basic operations on Granges object
========================================================
GRanges objects are considered vector-like objects

* length()
* names()
* subsetting
* c()
* comparison : ==, !=, match(), %in%, duplicated(), unique()
...

Complex Operations on Granges object  
========================================================

![alt text](img/genomicRange_presentation.png)


GRangeList  
========================================================
storing a list of compatible GRanges objects.

Compatible : 
relative to the same genome
same metadata columns

GRanges objects are considered list-like objects

Some functions work very well with this kind of list: 
elementLengths(GRangeList obj) 
shift()
reduce()
...



Bioconductor tutorial  
========================================================

[here](http://www.bioconductor.org/help/course-materials/2015/SeattleApr2015/B_GenomicRanges.html)



