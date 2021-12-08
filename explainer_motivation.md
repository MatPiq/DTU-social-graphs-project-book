Motivation 
===========

In this project, we analyse five of the major social science disciplines and how they relate to each other. More specifically, we are guided by the following questions:

* *How and to what are the social science disciplines connected in terms of referencing each other?*
* *Are relationships reciprocal or are some fields more central and influential than others?*
* *How does the content differ between disciplines? Are some more similar than others?*

**The Dataset**

 On the premise that a scientific field, in part, can be defined by its content—we used Wikipedia articles about theories, subfields, methods and researchers corresponding to the fields Economics, Sociology, Political Science, Anthropology and Psychology as our data source. In order to retain relevant articles we exploited that academic disciplines are organized hierarchically in groups, together with the open-source tool [PetScan](https://en.wikipedia.org/wiki/Wikipedia:PetScan) through which all articles and sub-groups at a specified depth relative to the parent node can be found. Moreover, petscan's API is easily accessible programmatically in Python and allows us to quickly get relevant urls without the need of web scraping. To avoid that the dataset becomes too big and to ensure a clear connection to the initial parent discipline node we set the depth to two for all other disciplines than anthropology. While we think this is a reasonable strategy for the purpose of this project, it also suffers from bias stemming from the fact that parent nodes are organized slightly differently. This means that the set of depth one article we get might systematically differ in important ways such as count and type of content affecting our results (see also our [data collection](explainer_data_collection) for a further elaboration of our sampling strategy). 

**Why did we choose this data set?**

Research conducted at new university centers and departments focusing on Social Data Science or Computational Social Science is characterised by being highly interdisciplinary {cite}`sodas, alan, oxford`. It is against this background, both interesting and of relevance to understand the commonalities and differences between the fields. We think that a better understanding could enhance collaboration in two important ways. First of all, having a basic understanding of central theories and methodological approaches used in other fields is a first step for a fruitful collaboration in an interdisciplinary project. Second of all, finding possible overarching topics and methods across disciplines can be used to facilitate complementary and diverging perspectives regarding the same issues. 

**Our goal for the end user's experience**

We want to give users the possibility to interact with the data through plots or by running code cells directly on the website, while at the same time ensuring that the reading experience is pleasing and upholds a good academic standard. On this basis we employ a [`jupyter book`](https://jupyterbook.org/) hosted on github pages. Although taking some initial time to set up properly, it offers the possibility to build the website directly from `jupyter notebooks` and has built-in support for `bibtex`, table of contents and linking to source code on github. This allows us to organize the website into a main stand-alone part, consisting of our main results visualized interactively and a part consisting of our explainer notebooks for the curious visitor. For convenience and ease of use, these can be run on a cloud server and forked directly from the website.