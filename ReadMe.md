# A fine-tuned global distribution dataset of marine forests

J. Assis, E. Fragkopoulou, Frade, D., Neiva, J., A. Oliveira, D. Abecasis, S. Faugeron, E.A. Serrão

### Abstract

Species distribution records are a prerequisite to follow climate-induced range shifts across space and time, yet, data collection can be costly and time consuming. Synthesizing information from various sources, such literature, herbaria, digital repositories and citizen science is challenging, as data are scattered, may comprise thematic and taxonomic errors and lacks standardized formats to enable interoperability. 

To address this gap, we gathered ~1,5 million records of 2166 important marine ecosystem structuring species of fan corals, large brown algae and seagrasses. We provide a curated dataset, taxonomically standardized, dereplicated and treated according to the physiological and biogeographical trait of species. Specifically, a flagging system was developed to sign potentially biased records occurring on land, in regions with limiting light or oxygen, or outside ecological niches and dispersal capacities. Experts were further consulted to validate the accuracy of records, relatively to the known distributional range of species. 

We document the procedure and provide a ready to use dataset, alongside with a set of functions in R language for data management and visualization. 


### R functions for data management and visualization

We provide a set of functions in R language to facilitate extraction, listing and visualization of occurrence records. The functions can be easily installed by entering the following line into the command prompt:

source("https://raw.githubusercontent.com/jorgeassis/marineforestsDB/master/sourceMe.R")

<br>
List of functions available for management and visualization:
<br><br>

Function | Description | Arguments
------------ | ------------- | -------------
extractDataset() | Imports data to R environment | group (character), pruned (logical)
listTaxa() | Lists available taxa | --
listData() | Lists data available in a dynamic table | data (character), taxa (character), status (character)
listDataMap() | Lists data available in a map | data (character), taxa (character), status (character),radius (integer), color (character), zoom (integer)
exportData() | Exports available data to a text delimited file | data (character), taxa (character), status (character), file (character)

<br>
Example [1]
<br>
dataset <- extractDataset("fanCorals",pruned=TRUE)<br>
listData(dataset,taxa="Paramuricea clavata",status="accepted")<br>
listDataMap(dataset,taxa="Paramuricea clavata",status="accepted",radius=2,color="Black",zoom=2)<br>
exportData(dataset,taxa="Paramuricea clavata",status="accepted",file="myfile.csv")
<br><br>
Example [2]
<br>
dataset <- extractDataset("fanCorals",pruned=TRUE)<br>
listData(dataset)<br>
listDataMap(dataset,radius=2,color="Black",zoom=2)<br>
exportData(dataset,file="myfile.csv")
