Describe the Biology of your project? (one paragraph max).

Monitoring biodiversity is critical to assess the health of marine ecosystems. However, current marine biodiversity methods are costly, time-consuming, and require taxonomic expertise. Surveys via SCUBA can also unintentionally repel rare and secretive species. eDNA is a novel approach to rapidly and accurately survey marine biodiversity. eDNA is the freely dissociated DNA produced by organisms in the environment from processes such as waste removal (i.e. metabolic waste) and reproduction (i.e. external fertilization). This remnant DNA can then be filtered and sequenced to reconstruct the community of organisms present in the environment. Recent studies of eDNA in marine ecosystems have demonstrated that eDNA is a standardized, accurate, reliable, and cost-effective tool for measuring biodiversity and detecting the presence of rare and endangered species in an ecosystem. Additionally, trait information for species recovered from eDNA is critical for ecological analyses.  FishBase is a comprehensive database of fish (teleost and elasmobranch) information about distribution, behavior, diet, morphology, and habitat. This program will match species recovered from eDNA to their respective trait data from FishBase.


Describe the kind of data that you think you will be handling (one paragraph max).

The data we will be handling are species tables generated from the Anacapa bioinformatics pipeline. The Anacapa pipeline parses amplicon sequence variants (ASVs) and assigns taxonomy to the sequences based on a bootstrapped confidence score.The output is a list of ASVs and their assigned taxonomy with the taxonomic ranks delimited by semicolons. The table is count data of how many times an ASV appeared in a sample.  


What would you like to do with that data? (one paragraph max).

With data, we want to assign trait data from FishBase to the species recovered from eDNA. We want to then create tables of relevant traits for the species in a way that allows the user to specify the fields of interest.


What will be the output? (one paragraph max).
The output will be a .txt file of all the species and their data for the traits of interest. 

Is there any computational tool, package, etc. you would like to use? What would you do with that? For instance, you could mention shell scripts with sed or awk and will change the format of a table by replacing , with tabs. Also, you could mention tools that we haven’t seen in class yet but you herd that may be useful for your project. For instance, you could say I will use the package “GenomeGraphs” implement in the R software to visualize genome data. (a few sentences max).
The most important package for this project is rfishbase, a package to match species to the trait data from FishBase. R is the most important program for this script. The first part of this project is formatting the eDNA species table in a compatible format with rfishbase. The second part is creating a flexible script to allow users to specify trait fields of interest. 

What is your biggest concern regarding your project? (a few sentences max).
My biggest concern is making the script flexible enough that the user can input any field of interest and the program will print the relevant data. An rfishbase function has its own fields nested within the function, making it difficult to write a script that prints any field. 
