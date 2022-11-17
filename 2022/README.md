#GSOC 2022

## Configurable feature visualization to improve the user experience and performance of the feature viewer
### neXtProt

[neXtProt](www.nextprot.org) is an open source discovery platform for human genes and proteins developed at the Swiss Institute of Bioinformatics (ELIXIR-CH). The neXtProt team would like to develop a web based user interface for the VEP neXtProt plugin and include it as one of the  community tools hosted on the neXtProt portal, in order to improve its accessibility.

### neXtProt system overview
neXtProt is a public portal accessible at www.nextprot.org. neXtProt exposes different ways for the users to view and use data. 
High level overview of neXtProt components can be found here. ![here](./images/np.png).

* Web User Interface (nextprot.org)
Web User Interface is developed in Angular and Polymer as the main technologies. It also integrates several other web components to add more features.

* SPARQL web interface (snorql.nextprot.org)
SPARQL is a semantic query language, which can be used to query a semantic knowledge base. neXtProt exposes its as a semantic model for SPARQL users and exposes a simple web interface for the users play with SPARQL queries over neXtProt data.

* API (api.nextprot.org)
neXtProt exposes a public API for the users to use neXtProt data in a more advanced and programmatic way. Both the main UI and SPARQL UI utilize the API to fetch the required data.


### Project Description

#### Configurable feature visualization to improve the user experience and performance of the feature viewer

Analyzing positional features/annotations in sequences is important in bioinformatics. Visualizing such data is quite a challenging task, considering the large amount of data to be displayed. The feature viewer is an open source javascript library developed to visualize biological data (referred to as features) mapped to a linear sequence (Paladin et al., 2020). For instance, it can be configured to visualize the location of protein domains or amino acid variations in a protein sequence. The feature viewer is being used in several popular bioinformatics resources such as [neXtProt](http://www.nextprot.org) and [COSMIC 3D](https://cancer.sanger.ac.uk/cosmic3d/).

#### Objective

Currently, the feature viewer supports limited configurability options in the features displayed, such as the color, shape and on-click behavior. This is too restrictive for some of the possible use cases of the feature viewer, where more flexibility is required in the display of features. One such instance is when different types of amino acid variants should be displayed in a color-specific manner in the same feature track.

The overall goal of this project is to improve the configurability of the feature viewer, such that it allows greater flexibility in the visualization of detailed biological data.  Specific aims of the project are:

##### Development steps

#### Simplify the configuration of new tracks

The current version of the feature viewer requires new tracks to be hard-coded. Implementing a solution allowing new tracks to be added or existing tracks to be modified or deleted would ease the use of the viewer.  

#### Add graphical representations of numerical features

Protein sequences can have features/annotations which are numerical. For instance, the frequency observed in a population of amino acid variants at a specific position. Such numerical data can be visualized as graphs of different types, such as line graphs or histograms.

#### Configure the visualization of certain features in a class of feature

Currently all the features displayed on a single track have the same color and/or shape;  interesting features can not be highlighted using a different color or shape.

#### Improve the speed of display by first displaying a summary or message

Currently all the data displayed has to be provided before display, which results in slow loading and rendering time when there are tens of thousands of features. In order to improve the user experience, it is possible to initially show a message summarizing the data  and only fetch and display the data on-demand by the user.

#### Enable the user to download a snapshot of the current display

The user community has requested a download button which generates a snapshot of the feature viewer. This feature will allow users to include an image of the data displayed in the feature viewer in a publication or elsewhere.

#### Preparation

Students can start exploring the neXtProt tools by referring to www.nextprot.org and the resources mentioned below. A warm-up exercise would be to write a simple javascript (any related platform) program to call the nextprot API and list/visualize the data returned. 

#### Tentative timeline

* Week 1-2:  Initial preparation, familiarizing with the repository and project
* Week 3-5: Define a representative configuration by analyzing the biological data
* Week 6-10: Implement, test and release, numerical feature visualization
* Week 11-16: Implement, test and release, configurability of visualization within feature
* Week 17-21: Implement, test and release, configurability of the initial data load for a feature
* Week 21-23: Implement a demo use case and document
* Week 23-24: Final report


### References

* Overview of the [neXtProt Concept](https://www.nextprot.org/about/nextprot)
* [Technical Corner](https://www.nextprot.org/help/technical-corner)
* [neXtProt github](https://github.com/calipho-sib)
* neXtProt features visualization [Feature viewer](https://github.com/calipho-sib/feature-viewer)

### Contributor

Chalith Tharuka Gunasekara (Tampere University)
[Github] : (https://github.com/chaliya96)

### Contact
kasun Samarasinghe [kasun.wijesiriwardana@unige.ch](mailto:kasun.wijesiriwardana@unige.ch)
