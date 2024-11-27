---
layout: page
title: What to do with a gene list
author: Alex Gibbs
---

The Database for Annotation, Visualisation and Integrated Discovery ([**DAVID**](https://david.ncifcrf.gov/home.jsp)) provides a comprehensive set of functional annotation tools for users to understand their gene lists. 
There are a number of tools available on this website: **Functional annotation tools, Gene functional classification tool, Gene ID conversion tool,** and **Gene name batch viewer**. 
We will cover the functional annotation tools and gene classification tool in this tutorial.

**Analysis Overview**

With the Functional Annotation Tools, users can perform functional annotation mapping (Functional Annotation Table), functional annotation enrichment analysis (Functional Annotation Chart), and functional annotation clustering based on the relationship of genes to annotation within the user's list (Functional Annotation Clustering). 
The Gene Functional Classification Tool generates a gene-to-gene similarity matrix of the genes in the user's list based on shared functional annotation from multiple functional annotation categories. 
This novel clustering algorithm classifies highly related genes into functionally related groups.


**Performing DAVID Analysis**

Clicking on the Start Analysis tab at the top of the page will take you to the Analysis Wizard page. On this page, there is a box on the left side of the page with three tabs: *Upload, List, and_Background_*.

**Upload**

*Step 1 :Enter Gene List*

Users will first need to paste their gene list into the Paste a list box, or upload using the Browse button.
In some cases, users may have more than one gene list to run. If this is the case, and you dont want to perform the analysis more than once, then a multiquery can be performed. 
To run a multiquery, the user must first create the multiquery file. To do this, create a new Microsoft Excel spreadsheet and paste each list into a new column. The first
row of each column must be the name of the list. For example:

|Gene List 1 |Gene List 2 |Gene List 3|
|:-----------|:-----------|:----------|
|GeneA|GeneB|GeneC|
|GeneD|GeneE|GeneF|
|.....|.....|.....|

Save this file as a **tab-delimited text (.txt)** file, upload it using the Browse button, and then select the Multi-List File option below.

*Step 2: Select Identifier*

In the drop-down menu, select the gene identifier that you have used in your list (i.e. Ensemble_Gene_ID).

*Step 3: List Type*

Select the Gene List option and then click Submit List underneath.

**Analyze**

selecting Submit List will take you to the second page of the analysis wizard and also to the List tab on the left of the page. 
In the List tab, users can select the species that the gene list belongs to and also rename their list (if they want to). 
In the middle of the page is the second step of the Analysis Wizard. 
This step asks you to choose which analysis you want to perform: Functional Annotation Tool (Functional Annotation Clustering, Functional Annotation Chart, and Functional Annotation Table), Gene Functional Classification Tool, Gene ID Conversion Tool, and Gene Name Batch Viewer.

**Functional Annotation Tool**

To use this tool for analysis, click on it on the Analysis Wizard. This will take you to a new page with Annotation Summary Results. 
At the top of this page is a list of all the categories that DAVID can use for its analyses. Each category can be expanded to show the different databases that can be used. 
Clicking on the Chart button next to each one will open a new window with a table of the different gene sets for each one. 
Categories that are highlighted in red are what DAVID uses by default. Users can add or remove these categories by expanding each section and selecting/de-selecting the databases they want/don't want.

**Functional Annotation Clustering**

Clicking on this button at the bottom of the page will load a new window of the results. This tool attempts to cluster related gene sets to give you a better overview of biological themes. 
There are a number of different options the user can change by selecting Options at the top of the page. If any options are changed, select Rerun using options button below to rerun the analysis.

**Functional Annotation Chart**

This tools analyses each gene list independently and lists the results in a table. Again, options can be changed for this analysis by clicking on Options at the top of the page. 
If any options are changed, click on the Rerun Using Options button below to rerun the analysis.

**Functional Annotation Table**

This tool loads a new window with a table of every term that each gene in your list is associated with.

**Gene Functional Classification Tool**

Clicking on this tool will load a new page with the Gene Functional Classification Results. This analysis clusters genes into functional groups. 
Options can be changed by clicking on Options at the top of the page. If the options are changed, select Rerun using options button below.

