---
type: page
title: REViGO
author: Alex Gibbs
---

**Reduce & Visualise Gene Ontology ([REViGO](http://revigo.irb.hr/))**

REViGO is a tool that takes GO enrichment results and trys to better summarise them by removing redundant terms. T
his tools requires GO terms and their associated enrichment p-values. To get these, I reccommend inputting your gene list into the GOrilla enrichment tool and exporting the results to use here.

**Running REViGO**

Users need to copy and paste their enrichment results into the provided input box. For examples of how the input should look, click on the three examples above the box. 
Note that the examples have a paragraph above the data describing what it is and what paper its come from etc. 
Every line here starts with a % which is used to tell the system to not read these lines. You can add comments above your GO terms in the same manner. 
If you do not want to add any comments, just paste in the GO terms and the p-values.
You can also choose how large you would like the resulting list to be, I would suggest sticking with the default of Medium (0.7).
You must tell the system what your accompanied values represent, if these values have come from REViGO, they represent the p-value.

***Advanced options:***

I would reccomend you keep these options to default. If you would like to change any of them and dont know what the option does, click the small i symbol next to the option.
Once you have everything ready, click on the Start Revigo button at the bottom of the page.

**Results**

Clicking Start Revigo will load up the results page. 
Taking Example #1 as example, the results page gives us five outer tabs: *Biological Process (103), Cellular Component (51), Molecular Function (45), Tag Clouds,* and *Report (21 Warning(s))*.

Each GO-related tab (*Biological Process, Cellular Component,* and *Molecular Function*) has six daughter tabs: *Description, Table, Scatterplot, 3D Scatterplot, Interactive Graph,* and *Tree Map*.

The *Description* tab tells you all the information about that particular GO category. This tab also gives you a brief outline of what the other tabs show.

*Table* shows a table of the GO terms along with the statistical data.

*Scatterplot* applies multidimensonal scaling to the similarity matrix of the GO terms and displays the results in a scatterplot. The more similar the GO terms are, the closer together they will be on this plot.

*3D Scatterplot* shows the Scatterplot data, but with another dimension added. This further splits the GO terms to give a better understanding of how similar/dissimilar they are.

*Interactive Graph* displays the GO terms as a network. Each node (GO term) can be click-and-dragged.

*Tree Map* shows two-level hierarchy of the GO terms.

*Tag Clouds* generates two tag clouds, one for frequent keywords within the GO terms associated with your data, and one for keywords that correlate with the values associated with the GO terms.

*Report* provides the user with any messages or warnings generated during the REViGO analysis.

