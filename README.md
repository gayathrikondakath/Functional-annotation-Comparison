# Functional Annotation Method Comparison
Code snippets to compare three functional annotation methods (BLAST, eggNOG-Mapper, and InterProScan) in their ability to assign Gene Ontology terms in two species of Insecta with differing levels of annotation, Bombyx mori and Manduca sexta. 


**for .annot converter**

*Aim*: Convert into an annotated .annot file compatible with OmicsBox

*Description*: This code allows you to convert a gene ID and GO tag data file into an annotated .annot file that is compatible with OmicsBox. The resulting .annot  file will contain gene IDs and their associated GO terms separated by commas.

*Input*: There is a sample input file in the file named “sample_input_converter.tsv”

*Caution*: the outfile file does not remove redundant GO tags for unique genes.

**for Jaccard Index and non-overlapping GO terms**

*Aim*: Calculate Jaccard Similarity Index and #Non-overlapping GO terms

*Description*:This code calculates the Jaccard similarity index and the number of non-overlapping Gene Ontology (GO) terms for a given dataset. It compares the GO terms derived from two types of files: one derived from BLAST and another from EggNOG/InterPro. The code provides insights into the similarity and dissimilarity of GO terms between the two sources.

*File Structure*:The code assumes that the input files are located in the specified file_path directory or its subdirectories. The files should be of two types: one derived from BLAST and the other from EggNOG/InterPro.

*Caution*: ‘AnnotationDbi’ package does not run optimally when ‘dplyr’ package is installed. 

**for Mean Number of GO tags**
*Aim*: Mean Number of GO Terms

*Description*: This code calculates the mean number of Gene Ontology (GO) terms for different annotation approaches, i.e. BLAST, EggNOG, and InterPro. It assumes that there are three types of input files derived from these approaches.

*File Structure*: The code expects the input files to be located in the "R:\RNAseq2022\Method Comparison" directory. You may need to modify the file path based on your system. 
It assumes that there are three types of input files derived from BLAST, EggNOG and InterPro approaches.
There is a sample input file in the file named “sample_input_file_comparison.xlsx”
