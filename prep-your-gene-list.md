---
type: page
title: Prepping Your Gene List
Author: Alex Gibbs
---
We must first prepare the gene list.

We need the following from the list:
- Gene ID
- Gene Symbol
- Expression Value (LogFC/Log2FC)
- Adjusted P Value

**Gene ID**
We must have the gene ID, as most tools only accept this. The gene ID is a unique identifier for the gene. 
We often come accross genes that have unusual names, such as *SEPT4* and *MARCH1* which are commonly autocorrected to *Sept-04* and *Mar-01* in spreadsheet softwares such as Microsoft Excel. 
There are a plethora of different gene ID formats available, but the most common is Ensembl ID, which starts with ENS for Ensemble, and then G for gene, followed by the unique identifier number. 
For example, *ENSG00000139618* is the Ensembl gene ID for human *BRCA2*. In the case of a different species, a three letter code is inserted into the ID. For example, *ENSMUSG00000041147* is the Ensembl gene ID for murine *BRCA2* (Mus Musculus).

To obtain Ensembl gene IDs, copy and paste your gene symbols into g:Profilers convert tool (https://biit.cs.ut.ee/gprofiler/convert). Select *ENSG* in the *Target namespace* dropdown and then click *Run Query*. 
Copy the 'converted alias' tab and paste it into your gene list as a new column.

**Gene Symbol**
The gene symbol is the conventional name for the gene, such as *BRCA2*. I like to include the gene symbols in with analyses as it allows you to read your results in real-time.

**Expression Value (LogFC/Log2FC)**
Depending on the analyses you will be performing, it is also necessary to include your expression values so that you can see the directionality of your results. 
Values used here would be the log-fold change or log2-fold change that you get from performing differential gene expression.

**Adjusted P Value**
This value is needed as when we perform multiple significance testing, our rate of false positives increases staggeringly. 
Differential gene expression tools account for this by performing multiple test correction which produces an adjusted p value.
I would reccommend creating a new Excel spreadsheet and copying and pasting the required data into it and saving this as a new file. 
From here, you can filter based on significance (Adjusted P Value < 0.05) and either sort by significance or expression.
