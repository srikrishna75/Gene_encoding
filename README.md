## Data Contributor GENEBOX
#### My sincere thanks to GENEBOX

# PROBLEM 1 

The file was generated from GenomeStudio software. The data fields in the attached files are: 

                  rsID      Chromosome    Location     Genotype

* rsID: The unique ID assigned to a change in single nucleotide in the DNA at specific location of the chromosome. May be repeated for quality control. (Look out for weird cases). 
* Chromosome: chromosome no on which the variation is located. 
* Location: Location of the variation on the chromosome. 
* Genotype: Humans have two sets of each chromosomes. Genotype (say GG) tells us about what nucleotides are present on each chromosome for the given variant location (In this case, G is present on both copies). The second part is the genotype call score which is calculated with specified threshold for the genotypes. 
	
#### A. Find unique rsIDs and chromosome and location with genotype keeping in mind the following things: 
	
1. Keep observations with higher call rates 
2. Remove no calls represented as ‘--’ but if all repeated observation are no calls keep one observation with no call (to imply that rsID has no call in the data). 
	   * Prepare a summary of the duplications. (how many unique rsIDs are there with different genotypes? Is there any relation with the duplicates?) 
	   * How will you report a final version of the data? 
	   * Visualize the data. 

##### Related topics you might want to read: Single Nucleotide Polymorphism, Strand orientations in DNA raw data

# PROBLEM 2 


* Note that the file doesn’t contain the header fields mentioned here. 

* For first row if 1 is present in column 1 then output should be TT
* For first row if 1 is present in column 2 then output should be TC
* For first row if 1 is present in column 3 then output should be CC

* Transform the data to obtain the 

following output:    SNP 	S1 	S2 
                    Rs123 	CC 	TT 
                    Rs124 	GG 	AG 

