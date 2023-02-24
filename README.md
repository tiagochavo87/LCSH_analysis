# LCSH_analysis
The code is written in Python and makes use of the Pandas library to manipulate and filter a dataset consisting of regions of the human genome (identified by a chromosome, start and end positions, and size).

The code reads in the dataset from a CSV file and applies a series of filters to extract specific regions of interest. The extracted regions are then written to new CSV files. The filters applied include: excluding regions on chromosomes X and Y, filtering for autosomes with a size greater than 10,000,000 and 3-5 MB regions, filtering for 3-5 MB regions with a total size of at least 10,000,000 and only one region per file, filtering for regions greater than 5,000,000 with a total size of at least 10,000,000 and only one chromosome per file, and filtering for cases with at least one region greater than 5 MB.

The code then calculates the total size of human autosomal DNA and the proportion of each case's LCSHs greater than 3 MB to autosomal DNA. It defines a set of F values and calculates the F value closest to each case's proportion. It then transposes the cases to the columns corresponding to the F values and writes the output to a CSV file.
