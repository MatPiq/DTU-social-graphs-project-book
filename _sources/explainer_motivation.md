Motivation 
===========

In this project we decided to analyse five of the major social science diciplines and how they relate to each other. More specifically, we were guided by the following questions:

* *How and to what are the social science disciplines connected in terms of referencing each other?*
* *Are relationships reciprocal or are some fields more central and influential than others?*
* *How does the language differ between diciplines? Are some more similar than others?*
* *Is it possible to create an interpretable two dimensional latent representation of the diciplines using their nodes and textual features?*

**The Dataset**

 On the premise that a scientific field, in part, can be defined by its content—we used Wikipedia articles about of theories, subfields, methods and researchers corresponding to fields Economics, Sociology, Political Science, Anthropology and Psychology as our data source. In order to retain relevant articles we exploited that academic diciplines are organized hierarchically in groups, together with the open-source tool [petscan](https://en.wikipedia.org/wiki/Wikipedia:PetScan) through which all articles and sub-groups at a specificed depth relative to the parent node can be found. Moreover, petscan API is easily accesible programatically in Python and allows us to quickly get relevant urls without the need of webscraping. To avoid that the dataset becomes too big and to ensure a clear connection to the parent dicipline node we set the depth to one. While we think this is a reasonable strategy for the purpose of this assignment, it also suffers from bias stemming from parent nodes being organized differently. This means that the set of depth one articles we get might systematically differ in important ways such as count and type of content. This is discussed further in section 

**Why did we choose this data set?**

Research conducted at new university centers and departments focusing on Social Data Science or Computational Social Science is characterised by being highly interdiciplinary {cite}`sodas, alan, oxford, sage`. It is against this background, both interesting and of relevance to understand 

**Our goal for the end user's experience**

