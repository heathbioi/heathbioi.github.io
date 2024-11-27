---
type: page
title: g:Profiler
Author: Alex Gibbs
---
This is a public web server that performs statistical enrichment analysis on your gene lists to find over-representation from various GO terms, biological pathways etc. 
The home page takes you straight to the enrichment tool, g:GOSt. 
There are also three other tools available: g:Convert, g:Orth, and g:SNPense. g:Convert is used to convert gene IDs, g:Orth is used for gene orthology searches, and g:SNPense maps a list of human SNPs to gene names.

**g:GOSt Enrichment Tool**

There are three tabs that the researcher can use depending on the format of gene list they want to upload: *Query*, *Upload Query*, and *Upload bed file*. This tutorial will focus on the Query function.

**Upload Query**

This tab allows users to drag and drop or upload a query file. To do this, the user must first create a new Microsoft Excel
spreadsheet, copy and paste the gene list column, and save the worksheet as a tab-delimited file (.txt). This .txt file can then be uploaded.

**Upload bed file**

This tab allows the user to upload a .BED file which contains 3-12 columns of data. The first three columns of this data must contain chrom, chromStart, and chronEnd. 
This file can be dragged and dropped or uploaded.

**Query**

This tab allows users to copy and paste their gene list from Microsoft Excel. Pasting your list in here should be whitespace-separated. i.e. each gene should be on a new line. For example:

|GeneA|
|:----|
|**GeneB**|
|**GeneC**|
|**...**|

**Options**

Once you have pasted their gene list into the Query box, you now need to check the Options parameters on the right hand side of the box.

**Ordered query**

Most users wil be using default parameters, however, if you have ordered your gene list based on expression or significance in a decreasing manner, then you should tick the Ordered query box (clicking on the quesiton mark symbol next to the tick-box will provide the user with a detailed explanation of what this option does).

**Run as multiquery**

In some cases, users may only be interested in significantly up- or down-regulated genes, or even just have more than one gene list to run. 
If this is the case, and you dont want to perform the analysis twice, then a multiquery can be performed.
To run a multiquery, the user must first create the multiquery file. To do this, create a new Microsoft Excel spreadsheet and paste the first list into the first column. 
The first cell (A1) will be the title of your gene list and must start with '>'. For example,

 |>Gene List 1|
 |:-----------|
|GeneA|
|GeneB|
|GeneC|

The second gene list must be inserted underneath the first list, again with a title beginning with '>'. For example,
	
|>Gene List 1|
|:-----------|
|GeneA|
|GeneB|
|GeneC|
|**>Gene List 2**|
|GeneD|
|GeneE|
|GeneF|

Further gene lists are added in this manner. Now save this as a tab-delimited text (.txt) file and either copy and paste, or import it into g:profiler and select the Run as multiquery tick-box.

**Results**

Once you have uploaded your gene list and selected the desired options, click Run query. Most of the time, you will be asked about genes that have ambiguous names. 
You can choose to remove these from your analysis by ignoring, or you can select the correct gene by selecting "Select the Ensembl ID with the most GO annotations" and then click Rerun. 
Be aware that some of these Ensembl IDs will have the same number of GO annotations, and therefore you may have to manually select the correct one.
The user will now be shown an overview of the results in the form of a Manhattan-like-plot. This plot is an interactive plot that shows the enrichment results. 
The x axis represents the functional terms, which are grouped and colour coded by the data source. The y axis shows the adjusted p-values in a negative log-10 scale. 
The circles in the plot represent the various enrichment terms. If there are any circles that are light/transparent, this indicates that they are not significant. 
The size of the circles corresponds to the size of the terms, i.e. bigger circles have more genes are associated with that term. 
Users can hover their mouse over the circles to obtain the relevant information for that enrichment term. Users can click on circles to generate a table underneath of the results.
For more information on the results, users can select the Detailed Results tab. Before digging into your results, click on the Legend option, which provides you with information regarding the various evidence codes for your results. 
Above the Legend option, there is also options to download the results and a filter box. The detailed results gives you a table for each data source.
There are many different ways in which you can re-run this enrichment analysis, such as measuring under-representation, using different multiple testing methods, and visualising your results as a GO interaction network. 

The authors have a really good documentation page describing how to do all of this, plus a nice section on how the adjusted p-values are calculated [link](https://biit.cs.ut.ee/gprofiler/page/docs).

For more hardcore users, g:Profiler can also be queried through [R](https://biit.cs.ut.ee/gprofiler/page/r) and [Python](https://biit.cs.ut.ee/gprofiler/page/apis). 
This is something we can provide assistance/training on, so please contact us if you would like to do this.
