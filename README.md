# RNAseq

## Instructions for analysis

The goal of this analysis is to perform a differential expression analysis at gene level (mRNA isoforms are *not* taken into account).

The following instructions are short in purpose: additional information or tools can be deduced, or retrieve from public databases. 

1. Download 4 sequence datasets deposited to the EBI [ENA](http://www.ebi.ac.uk/ena):

 `ERR990557`
    
 `ERR990558`
    
 `ERR990559`
    
 `ERR990560`
 
These datasets have been generated in a work published in Embo Reports :

Molla-Herman A, Vallés AM, Ganem-Elbaz C, Antoniewski C, Huynh J-R. tRNA processing defects induce replication stress and Chk2-dependent disruption of piRNA transcription. EMBO J. 2015;34: 3009–3027. doi:10.15252/embj.201591006

2. Extract fastq files
3. for each file, select 8,000,000 (8 millions) of sequence reads and generate the following sample files:

 `ERR990557s.fastq`
    
 `ERR990558s.fastq`
    
 `ERR990559s.fastq`
    
 `ERR990560s.fastq`

4. Align these read datasets to the reference genome by any appropriate mean, and generate a sorted bam alignment file.
5. Count reads aligning to genome's genes by any appropriate mean
6. Perform a statistical differential expression analysis and report using any appropriate figure(s)/graph(s)
7. select a list of genes likely to be differentially expressed with a p-adj value < 0.01
8. Code a simple script that parse the table of differential expressions (from *6.*) and return the genes with a p-adj value < 0.01 for rejection of H0 (non differential expression)

## Reporting

Each analyst will report her/is analysis by any mean s/he feels appropriate (pdf, text, markedown, jpg, URL, etc.).

The only constraint is that analysis outputs will be deposited in a personal [fork](https://help.github.com/articles/fork-a-repo/) of this repository in a *new* directory named analysis.01, analysis.02, etc. (see analysis.00 for an example). Keep track of the analysis.xx directories already existing and chose another name for your directory.

Final submission of the results will be made through a [pull request](https://help.github.com/articles/creating-a-pull-request/) from the analyst to the [original repo](https://github.com/drosofff/RNAseq.git).

Please do not neglect the reporting and follow the requested process, it is a part of the analysis.
