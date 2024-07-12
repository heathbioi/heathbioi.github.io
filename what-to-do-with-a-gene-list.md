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

![WebGestalt!](/assets/img/webgestalt.png)

WEB-based Gene SeT AnaLysis Toolkit. Functional enrichment analysis web tool.

***

### [ShinyGO](http://bioinformatics.sdstate.edu/go/) 

A graphical tool for gene enrichment analysis. Neat tool. 

***

### [Gene Set Enrichment Analysis (GSEA)](https://www.gsea-msigdb.org/gsea/index.jsp) 

![Gene Set Enrichment Analysis (GSEA)!](/assets/img/gsea.png)

This is a downloadable tool that performs GSEA on your gene list. GSEA is a computational method that determines whether a priori defined set of genes shows statistically significant, concordant differences between two biological states. 

***

### [GO-Elite](http://www.genmapp.org/go_elite/)

![GO-Elite!](/assets/img/go-elite.png)

Application designed to identify non-redundant set of ontology terms, gene sets and pathways to describe a particular set of genes or metabolites. Downloadable software.

***

### [BiNGO - Biological Network Gene Ontology Tool](https://www.psb.ugent.be/cbd/papers/BiNGO/Home.html)

![BiNGO - Biological Network Gene Ontology Tool!](/assets/img/bingo.png)

Java-based tool to determine which GO categories are statistically overrepresented in a set of genes. 

***

### [Gorilla](https://cbl-gorilla.cs.technion.ac.il/)

![Gorilla!](/assets/img/gorilla.png)

Gene ontology enrichment analysis and visualisation tool. Identifies and visualises enriched GO terms in ranked lists of genes. I have also made a quick [tutorial](gorilla.md).
I have also made a quick [video tutorial](https://cardiff.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=a74d5ae4-d4d3-4f55-a045-b0540081405f) for this tool:

***

### [ReViGO - Reduce and Visualise Gene Ontology](http://revigo.irb.hr/)

![ReViGO - Reduce and Visualise Gene Ontology!](/assets/img/revigo.png)

This tool takes long lists of GO terms and summarizes them by removing redundant GO terms. good for tools that produce GO results, like GOrilla. I have also made a quick [tutorial](revigo.md).

***

### [Gonet](https://tools.dice-database.org/GOnet/)

![Gonet!](/assets/img/gonet.png)

Constructs interactive graphs containing enriched GO terms and genes. I also made a quick [tutorial](gonet.md). 

***

### [EnrichR](https://maayanlab.cloud/Enrichr/)

![EnrichR!](/assets/img/enrichr.png)

Enrichment analysis web tool. I have also made a quick [video tutorial](https://cardiff.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=008340c5-afd1-49b9-965e-b05a00fccfe0) for this tool:
Link to the [About page](https://rummagene.com/about).

***

### [Rummagene](https://rummagene.com)

![Rummagene!](assets/img/rummagene.png)

Rummage through 658,108 gene sets extracted from supporting tables of 124,773 articles to find the most similar gene sets that match your query.

***

### [DAVID - Database for Annotation, Visualisation and Integrated Discovery](https://david.ncifcrf.gov/)

![DAVID!](/assets/img/david.png)

Functional annotation of your gene list. I also made a quick [tutorial](david.md).

***

### [PANTHER - Protein Analysis Through Evolutionary Relationships](https://pantherdb.org/)

![PANTHER!](/assets/img/panther.png)

Classifys proteins and their genes in order to facilitate high-throughput analysis. I also made a quick [tutorial](panther.md).

***

### [PARADIGM - Pathway Representation and Analysis by Direct Reference on Graphical Models](https://sbenz.github.io/Paradigm/) 

Downloadable software.

***

### [Pathway Commons](http://www.pathwaycommons.org/)

![Pathway Commons!](/assets/img/pathway-commons.png)

Access and discover data integrated from public pathway and interactions databases. Can paste your gene list into the search bar and click the search button. 

***

### [Reactome](https://reactome.org/PathwayBrowser/#TOOL=AT) 

![Reactome!](/assets/img/reactome.png)

Open-source, open-access, manually curated and peer-reviewed pathway database. Can perform enrichment analysis on your gene list by clicking on analysis tools from the homepage. I also made a quick [tutorial](reactome.md).

***

### [g:Profiler](https://biit.cs.ut.ee/gprofiler/gost) 

![g:profiler!](/assets/img/gprofiler.png)

Maps genes to known functional information resources and detects statistically significant enriched terms. I also made a quick [tutorial](g-profiler.md) and [video tutorial](https://cardiff.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=540e51c1-71cc-4817-97cf-b05a00de7832) for this tool:

***

### [pathDIP](http://ophid.utoronto.ca/pathDIP/)

![pathDIP!](/assets/img/pathdip.png)

Annotated database of signalling cascades in human and non-human organisms, comprising core pathways from major curated pathways databases, and pathways predicted based on orthology, and by using physical protein interactions. 

***

### [GeneTrail](https://genetrail.bioinf.uni-sb.de/start.html) 

![GeneTrail!](/assets/img/gene-trail.png)

Advanced high throughput enrichment analysis. Gene expression data can be uploaded and enrichment analysis can be performed.

***

### [PathVisio](https://pathvisio.org/)

![PathVisio!](/assets/img/path-visio.png)

Pathway analysis and drawing software which allows drawing, editing, and analysing biological pathways. 

***

### [Cytoscape](https://cytoscape.org/)

![Cytoscape!](/assets/img/cytoscape.png)

Network data integration, analysis, and visualisation in a box. Also has NDEx iQuery box on the homepage which you can copy and paste your list into. [ClueGO](https://apps.cytoscape.org/apps/cluego) is a plug-in that visualises the non-redundant biological terms for large clusters of genes in a functionally grouped network. 

***

### [Integrated interactions database (IID)](http://iid.ophid.utoronto.ca/)

![IID!](/assets/img/iid.png)

Tissue specific PPI networks across species. 

***

### [STRING-DB](https://string-db.org/)

![STRING-DB!](/assets/img/stringdb.png)

PPI networks functional enrichment analysis.

***

### [GeneMANIA](https://genemania.org/)

![GeneMANIA!](/assets/img/genemania.png)

Predict function of your gene list. 

***

### FOR WINDOWS USERS: [FunRich](http://funrich.org/index.html) 

![FunRich!](/assets/img/funrich.png)

Downloadable software for functional enrichment analysis. 

***

### [iDEP.96](http://bioinformatics.sdstate.edu/idep/)

Integrated Differential Expression and Pathway analysis) integrated web application for differential expression and pathway analysis of RNAseq data. 

***

### [Kinase Enrichment Analysis 2](https://www.maayanlab.net/KEA2/) 

Predict kinase activity from your list of input set of phosphosites.

***

### [chEA3](https://maayanlab.cloud/chea3/)

![chEA3!](/assets/img/chea3.png)

ChIP-X enrichment analysis version 3. performs transcription factor enrichment analysis on your list of DEGs. 

***

### [MetaboAnalyst](https://new.metaboanalyst.ca/home.xhtml)

![MetaboAnalyst!](/assets/img/metaboanalyst.png)

User-friendly, streamlines metabolomics data analysis tool. Performs enrichment, pathway, and network analyses. 

***

### [GREAT - Genomic Regions Enrichment of Annotations Tool](http://great.stanford.edu/public/html/)

![GREAT!](/assets/img/great.png)

Many coding genes are well annotated with their biological functions. Non-coding regions typically lack such annotation. GREAT assigns biological meaning to a set of non-coding genomic regions by analyzing the annotations of the nearby genes. Thus, it is particularly useful in studying cis functions of sets of non-coding genomic regions. Also available as an [R package](https://bioconductor.org/packages/release/bioc/html/rGREAT.html).

***
