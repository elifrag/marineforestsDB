# A fine-tuned global distribution dataset of marine forests

J. Assis, E. Fragkopoulou, Frade, D., Neiva, J., A. Oliveira, D. Abecasis, E.A. Serrão


### Abstract

Species distribution records are a prerequisite to follow climate-induced range shifts across space and time, yet, data collection can be costly and time consuming. Synthesizing information from various sources, such as peer-reviewed literature, herbaria, repositories and citizen science is challenging, as data are scattered, may comprise thematic and taxonomic errors and there are no standardized formats to enable interoperability. 

To address this gap, we gathered ~1,5 million records of 2166 important marine ecosystem structuring species of fan corals, large brown algae and seagrasses. We provide a curated dataset, taxonomically standardized, dereplicated and treated according to the physiological and biogeographical trait of species. Specifically, a flagging system was developed to sign potentially biased records occurring on land, in regions with limiting light or oxygen, or outside ecological niches and dispersal capacities. Experts were further consulted to validate the accuracy of records, relatively to the known distributional range of species. 


### R functions for data management and visualization

We provide a set of functions in R language to facilitate extraction, listing and visualization of occurrence records. The functions can be easily installed by entering the following line into the command prompt:

source("https://raw.githubusercontent.com/jorgeassis/marineforestsDB/master/sourceMe.R")

<br><br>
Table. List of functions available for management and visualization.

Function | Description | Arguments
------------ | ------------- | -------------
function() | Importing data to R environment | Datasets (character) (logical); (default)
function() | Subsetting data | Layercodes (character)
function() | Listing data in a table | Layercodes (character)
function() | Listing data in a map | Layercodes (character)
function() | Exporting data to file | Layercodes (character)

