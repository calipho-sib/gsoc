#GSOC 2021 

## Development of a user interface for the Ensembl Variant Effect Predictor neXtProt plugin as one of the  community tools hosted on the neXtProt portal

### neXtProt

[neXtProt | www.nextprot.org] is an open source discovery platform for human genes and proteins developed at the Swiss Institute of Bioinformatics (ELIXIR-CH). The neXtProt team would like to develop a web based user interface for the VEP neXtProt plugin and include it as one of the  community tools hosted on the neXtProt portal, in order to improve its accessibility.

### Variant Effect Predictor

In order to be able to interpret human genomic variation data, several open source tools such as the Ensembl Variant Effect Predictor (VEP) have been developed to predict the structural and functional effects of variants (SNPs, insertions, deletions, CNVs or structural variants) on genes, transcripts, and protein sequences, as well as regulatory regions. The VEP tool takes input variants in different formats such as VCF, HGVS and variant identifier formats such as SNPs, and produces the output with the predicted effect on the selected biological entities. The VEP tool has numerous plugins including a neXtProt plugin, which was made public last november as a command line. This plugin improves the accuracy of predictions  about coding single nucleotide polymorphisms by integrating manually curated information from neXtProt about domains, PTMs, interacting regions etc. associated with the affected amino-acid positions. 
The proposed user interface visualizes the predicted variant effect output for all variants within a neXtProt entry. It has to handle the possibly large number of variants in the neXtProt entry and handle the corresponding large VEP output in an optimal manner. The student is expected to have knowledge in REST APIs and to utilize the neXtProt API to get the variants given a neXtProt accession. The student has the choice of the web technology to use to implement the UI (Javascript based technologies recommended). The UI has to handle large amounts of prediction data and visualize them in an efficient and user friendly manner.

### Tentative Use Case

A first use case which has to be implemented is as follows;


A sample timeline:
Week 1-2: Review the VEP neXtProt plugin (In a docker setup), neXtProt REST API 
Week 3-4: Design the UI considering the VEP output and the data to be visualized, Lazy loading of data if required and implement the first version of the UI
Week 5-8: Implement the data bindings to the UI by calling the API
Week 9-10: Optimize the API calls and UI and deploy it following the neXtProt community tool to integrate it with www.nextprot.org.
