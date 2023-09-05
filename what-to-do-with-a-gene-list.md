---
layout: page
title: What to do with a gene list
author: Alex Gibbs
---
Have you performed a sequencing experiment which generated a list of differentially expressed genes and are now left wondering 'what can I do or find out about my list of genes?'. Then look no further! 

I have scoured the internet for tools that will allow you to perform a range of analyses on your gene list, such enrichment analysis, gene ontology, network analysis and so on.

This list contains mostly tools that only require a web browser and an active internet connection to run. However, some tools are downloadable as an application, and some can be run through R.
Clicking on the name of the tool will direct you to a mini-tutorial that I wrote for that tool. I am also making short tutorial videos for each tool - please email me to be granted access to those videos.

If you have any questions, problems, or suggestions - please contact me @ GibbsA@cardiff.ac.uk!

***

# Prepare Your Gene List

I would first suggest that you take the time to [prep your gene list](prep-your-gene-list.md) so that it saves you time.

***

# Gene List Analysis Tools

***

### [WebGestalt](https://www.webgestalt.org/#) 

WEB-based Gene SeT AnaLysis Toolkit. Functional enrichment analysis web tool.

***

### [ShinyGO](http://bioinformatics.sdstate.edu/go/) 

A graphical tool for gene enrichment analysis. Neat tool. 

***

### [Gene Set Enrichment Analysis (GSEA)](https://www.gsea-msigdb.org/gsea/index.jsp) 

This is a downloadable tool that performs GSEA on your gene list. GSEA is a computational method that determines whether a priori defined set of genes shows statistically significant, concordant differences between two biological states. 

***

### [GO-Elite](http://www.genmapp.org/go_elite/)

Application designed to identify non-redundant set of ontology terms, gene sets and pathways to describe a particular set of genes or metabolites. Downloadable software.

***

### [BiNGO - Biological Network Gene Ontology Tool](https://www.psb.ugent.be/cbd/papers/BiNGO/Home.html)

Java-based tool to determine which GO categories are statistically overrepresented in a set of genes. 

***

### [Gorilla](https://cbl-gorilla.cs.technion.ac.il/)

Gene ontology enrichment analysis and visualisation tool. Identifies and visualises enriched GO terms in ranked lists of genes. I have also made a quick [tutorial](gorilla.md).
I have also made a quick video tutorial for this tool:
<iframe src="https://cardiff.cloud.panopto.eu/Panopto/Pages/Embed.aspx?id=a74d5ae4-d4d3-4f55-a045-b0540081405f&autoplay=false&offerviewer=true&showtitle=true&showbrand=true&captions=false&interactivity=all" height="405" width="720" style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>

***

### [ReViGO - Reduce and Visualise Gene Ontology](http://revigo.irb.hr/)

This tool takes long lists of GO terms and summarizes them by removing redundant GO terms. good for tools that produce GO results, like GOrilla. I have also made a quick [tutorial](revigo.md).

***

### [Gonet](https://tools.dice-database.org/GOnet/)

Constructs interactive graphs containing enriched GO terms and genes. I also made a quick [tutorial](gonet.md). 

***

### [EnrichR](https://maayanlab.cloud/Enrichr/)

Enrichment analysis web tool. I have also made a quick video tutorial for this tool:
<iframe src="https://cardiff.cloud.panopto.eu/Panopto/Pages/Embed.aspx?id=008340c5-afd1-49b9-965e-b05a00fccfe0&autoplay=false&offerviewer=true&showtitle=true&showbrand=true&captions=false&interactivity=all" height="405" width="720" style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>

***

### [DAVID - Database for Annotation, Visualisation and Integrated Discovery](https://david.ncifcrf.gov/)

Functional annotation of your gene list. I also made a quick [tutorial](david.md).

***

### [PANTHER - Protein Analysis Through Evolutionary Relationships](https://pantherdb.org/)

Classifys proteins and their genes in order to facilitate high-throughput analysis. I also made a quick [tutorial](panther.md).

***

### [PARADIGM - Pathway Representation and Analysis by Direct Reference on Graphical Models](https://sbenz.github.io/Paradigm/) 

Downloadable software.

***

### [Pathway Commons](http://www.pathwaycommons.org/)

Access and discover data integrated from public pathway and interactions databases. Can paste your gene list into the search bar and click the search button. 

***

### [Reactome](https://reactome.org/PathwayBrowser/#TOOL=AT) 

Open-source, open-access, manually curated and peer-reviewed pathway database. Can perform enrichment analysis on your gene list by clicking on analysis tools from the homepage. I also made a quick [tutorial](reactome.md).

***

### [g:Profiler](https://biit.cs.ut.ee/gprofiler/gost) 

Maps genes to known functional information resources and detects statistically significant enriched terms. I also made a quick [tutorial](g-profiler.md).
I hace also made a quick video tutorial for this tool:
<iframe src="https://cardiff.cloud.panopto.eu/Panopto/Pages/Embed.aspx?id=540e51c1-71cc-4817-97cf-b05a00de7832&autoplay=false&offerviewer=true&showtitle=true&showbrand=true&captions=false&interactivity=all" height="405" width="720" style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>
***

### [pathDIP](http://ophid.utoronto.ca/pathDIP/)

Annotated database of signalling cascades in human and non-human organisms, comprising core pathways from major curated pathways databases, and pathways predicted based on orthology, and by using physical protein interactions. 

***

### [GeneTrail](https://genetrail.bioinf.uni-sb.de/start.html) 

Advanced high throughput enrichment analysis. Gene expression data can be uploaded and enrichment analysis can be performed.

***

### [PathVisio](https://pathvisio.org/)

Pathway analysis and drawing software which allows drawing, editing, and analysing biological pathways. 

***

### [Cytoscape](https://cytoscape.org/)

Network data integration, analysis, and visualisation in a box. Also has NDEx iQuery box on the homepage which you can copy and paste your list into. [ClueGO](https://apps.cytoscape.org/apps/cluego) is a plug-in that visualises the non-redundant biological terms for large clusters of genes in a functionally grouped network. 

***

### [Integrated interactions database (IID)](http://iid.ophid.utoronto.ca/)

Tissue specific PPI networks across species. 

***

### [STRING-DB](https://string-db.org/)

PPI networks functional enrichment analysis.

***

### [GeneMANIA](https://genemania.org/)

Predict function of your gene list. 

***

### FOR WINDOWS USERS: [FunRich](http://funrich.org/index.html) 

Downloadable software for functional enrichment analysis. 

***

### [iDEP.96](http://bioinformatics.sdstate.edu/idep/)

Integrated Differential Expression and Pathway analysis) integrated web application for differential expression and pathway analysis of RNAseq data. 

***

### [Kinase Enrichment Analysis 2](https://www.maayanlab.net/KEA2/) 

Predict kinase activity from your list of input set of phosphosites.

***

### [chEA3](https://maayanlab.cloud/chea3/)

ChIP-X enrichment analysis version 3. performs transcription factor enrichment analysis on your list of DEGs. 

***

### [MetaboAnalyst](https://new.metaboanalyst.ca/home.xhtml)

User-friendly, streamlines metabolomics data analysis tool. Performs enrichment, pathway, and network analyses. 

***
