---
type: page
title: GOnet
author: Alex Gibbs 
---

[GOnet](https://tools.dice-database.org/GOnet/) generates interactive graphs containing GO terms and genes.

GOnet works on Human and Mouse data and can be run using gene names as well as expression values.

**Running GOnet**

Everything needed to run the analysis is on the homepage. Note that GOnet does not accept Ensembl IDs, so you will need the gene symbols instead. 
You can also choose to upload just gene symbols to perform GO term annotation or gene symbols with their accompanied expression values to perform GO term enrichment.

**Input Parameters**

Select the organism that you are working with, then either upload your gene list as a **comma-separated value (.csv)** file or copy and paste your gene symbols. 
To make a .csv file, create a new Microsoft Excel Worksheet, copy and paste your gene symbols (and expression values) in, and then save as comma-separated values (.csv). 
You can give your analysis an optional job name in the provided box, too. 
If you have copied and pasted your gene symbols and expression values from Excel, these will be separated by a tab, so select *{tab}* in the Contrast value separator section. 
If you have uploaded a .csv file, select *{,}*.

**Job parameters**

Users can choose which GO terms to run against by using the drop-down box in the GO namespace section. 
Next, Select analysis type. If you have uploaded only gene symbols, choose the GO term annotation option, if you have accompanying expression values, you can choose GO term enrichment. 
Enrichment analysis options and Annotation analysis options are usually kept as default, but can be changed depending on the users preferences.

**Output parameter*

There are three output types from this analysis: *Interactive Graph, Hierarchical Text,* or *CSV*8. 
I would reccommend running the Interactive Graph as it gives a nice visual network of your data. The latter two options produce downloadable files.
Once you have selected your analysis, click *Submit* below to submit the analysis. This will take you to a new page where you can see the progress of the job.

**Results**

Depending on the size of your gene list, this may take some time to run. Also note that the bigger your gene list, the slower this will make your browser.
Once the job has run, you will get a Warnings window appear, this usually just tells you that there are a lot of genes present so they will only show the GO terms to reduce rendering time. 
You can shoose to export at this stage if you dont want to wait a long time for the browser to render by clicking on the Export data tab. Otherwise, click on the *Show network tab*.
A network of your data will now load, there is a window on the right hand side of the screen where users can change parameters. 
To change the layout of the network, select between *Cose, Hierar,* or *Euler* in the *Choose layout* tab. 
To gain a more clear insight, users can also choose to hide gene-unconnected terms by selecting the *Hide gene-unconnected terms* tab or changing the p-value threshold by using the associated drop-down box.
To navigate around the network, simply click and drag with your mouse. The scrool wheel can be used to zoom in and out. 
To obtain information on a GO term, click it and new information will pop up in the window on the right hand side. 
This will give you information on the GO term, such as p-value, total genes of that GO term, and how many of your genes are in that GO term.
Finally, to export the results, use the Export data tab which gives you a range of export options. 
If using the network for a paper, I would reccommend using the View as png (high def) option.

