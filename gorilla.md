---
type: page
title: GOrilla
author: Alex Gibbs
---


Gene Ontology enRIchment anaLysis and visuaLizAtion tool ([GORILLA](https://cbl-gorilla.cs.technion.ac.il/)) is a tool that does what it says - identifies and visualises enriched GO terms in ranked lists of genes. 
It is important that users know that the input gene list for this tool must be ranked, which is usually by expression.

**Running GOrilla**

Everything needed to run the analysis is on the homepage.

*Step 1: Choose organism*

Select the organism that you have been working on in the drop-down menu

*Step 2: Choose running mode*

There are two modes to choose from: Single ranked list of genes and Two unranked lists of genes(target and background lists. The mode we will be using for our ranked gene list is Single ranked list of genes.

*Step 3: Paste a ranked list of gene/protein names*

This is one of the tools that prefers gene symbols as input, but does accept Ensemble ID. Users need to copy and paste their gene IDs (either gene symbol or Ensemble ID) into the box. 
Genes must be separated by a new line, i.e. each gene is on a new line. If you have your gene list as a column in excel, simply copy the column (minus the column title/header) and paste it in.

*Step 4: Choose an ontology*

There are four options to choose here: Process_, Function, Component, and All. Select which one you want. 
I would suggest All as you wont have to come back an rerun the analysis if you wanted to see the other ontologies. Once you have done this, click the Search Enriched GO terms button below.

**Results**

Once you have submitted the job, a new page will load with a real-time process indicator. This will tell you what has been processed and what is left to do. 
The analysis takes around 10-20 seconds to run on a gene list of ~2000 genes. Once the analysis has completed, the page will refresh and load the results. 
If you have run All ontologies, there will be three tabs at the top of the screen, one for each ontology. In each tab will be a graphical representation in the term of a network of the GO terms highlighted by significance. 
There will also be a table below the network will be a table of each GO term and its associated values. Below the graph is the information that you may need to interpret the results.

***Optional Extras***

If you have a very large gene list to run, this may in turn produce a very large list of enriched GO terms, making your interpretation difficult. 
To fight this, there is an option in the *Advanced parameters* section below Step 4 when submitting your analysis to **Show output also in REViGO**. 
If you select this tick-box before running the analysis, it will give you another clickable link below the results table: *Visualise output in REViGO*. 
Clicking this link will take you to **REduce and VIsualise Gene Ontology ([REViGO](revigo.md))** website with your results already pasted into the input box. 
Scroll down the page and click on the Start Revigo box to run the analysis. This analysis attempts to reduce the number of redundant GO terms in your results, making it easier to interpret your data. 

There are a number of tabs in the results. Taking GOrilla Function analysis as en example, the outermost tabs are Molecular Function, Tag Clouds, and Report. 

*Molecular Function* tab contains six additional tabs: Description, Table, Scatterplot, 3D Scatterplot, Interactive Graph, and Tree Map. 

*Description* tab provides an overview on the GO Molecular Function terms. The other tabs provide the user with different visual representations of the results. 

*Tag Clouds* generates two tag clouds, one for frequent keywords within the GO terms associated with your data, and one for keywords that correlate with the values associated with the GO terms. 

*Report* tab provides the user with any messages or warnings generated during the REViGO analysis. Check my [REViGO](revigo.md) tutorial for more information.

