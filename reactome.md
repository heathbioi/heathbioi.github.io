---
type: page
title: Reactome
author: Alex Gibbs
---

[REACTOME](https://reactome.org/PathwayBrowser/#TOOL=AT) is an open-source, open access, manually curated and peer-reviewed pathway database.

There is a free [course](https://www.ebi.ac.uk/training/online/courses/reactome-tools-for-analysing-biological-pathways/#vf-tabs__section--overview) offered by the European Bioinformatics Institute (EBI) which nicely covers the Reactome analysis tools .

**Querying the Reactome database with your gene list**

Clicking the above link will take you to the Analysis tools page. Along the left side of the page is four different tools: *Analyse gene list, Analyse gene expression, Species Comparison,* and *Tissue Distribution*. 
The two most useful tools here are *Analyse gene list* and *Analyse gene expression*. For the sake of simplicity, we will only cover the Analyse gene list tool, as the Analyse gene expression tool requires specific data that you may/may not have. 
If you would like to use this tool, please let us know and I can go through it with you.

**Analyse gene list**

Clicking the link above takes you to this tool by default. This tool accepts multiple gene IDs, so you can choose to use Ensemble IDs (**reccommended**) or gene symbol. 
You have two options to input your data, *click and browse* or *copy and paste*. If you are unsure about how the list should look, click on the *examples* on the right hand side of the page. 
Once you have your data in, click on Continue. This will take you to the Options menu where you have two tick boxes to consider. I would reccommend running with the default parameters. 
Once you are ready, click on *Analyse!* at the bottom right of the page.

**Results**

Once your data has been analysed, you will be taken to a new page with your results. There are three sections to this results page. 

The main window shows all the reactome pathways with your results overlaid in shades of yellow (stronger yellow indicates more significant findings). 

The main pathways are labelled as circles, with the sub-pathways branching off as 'spider webs'. You can zoom in and out of each pathway using your scrool wheel.

At the top left of this main window is a search bar where you can search for your favourite gene. Searching for a gene will produce a small results box below where you can select your gene. 
This will highlight which pathways your gene is involved in on the diagram. 

To the right of the search box is three view options: *Show all, Open pathway diagram,* and *Open voronoi visualisation*. 
*Show all* adjusts the page so that all pathways are visible. 
*Open pathway diagram* is selectable if you click on a specific pathway. To do this, click on a pathway of interest, which highlights it blue, then select the Open pathway diagram. 
This zooms into the selected pathway and shows you a nice diagram of the pathway. 
*Open voronoi visualisation* changes the layout of the results to a voronoi visualisation.

On the left hand side of the page is a window with Event Hierarchy. Hovering your mouse over each of the pathways will highlight it in the main window. 
Clicking on a pathway will zoom into it on the main window. Next to each pathway is a small + symbol, clicking on this will expand the pathway to show the sub-pathways. 
Clicking on the pathway will display it in the main window. Each sub-pathway can be further expanded using the + option next to it, and clicking on the results will further zoom into it on the main window.

At the bottom of the page is a window with six tabs: *Description, Molecules, Structures, Expression, Analysis,* and *Downloads*. 

*Description* tab provides a description of each pathway if you click on it in the main window or in the Event Hierarchy. 

*Molecules* tab gives details of all the molecules involved in a certain pathway once it is selected. 

*Structures* tab shows the user the structure of the molecules in a specific reaction of a pathway when selected. 
To view molecules, the user must select a reaction at the very end of a pathway (for example: Immune system > Innate immune system > Complement cascade > Activation of C3 and C5 > Activation of C5). 

*Expression* tab gives the user a human (male, female, and brain) diagram highlighting the areas of expression along with an associated table for the genes associated with the selected pathway. 
Clicking on a particular gene in the table takes the user to the genes page on Ensembl. 

*Analysis* tab provides the user with a table of the pathway results along with the associated statistics. To the left of the table is a further 3 tabs: *Results, Not found,* and *Downloads*. 

The *Results* tab is already loaded, the *Not found* tab shows the user the genes that were not found in the reactome database, and the *Downloads* tab allows the user to download various pieces of results. 
The main Downloads tab allows the user to download selected pathway diagrams and formats.

If you need a visual guide to the results, select the *Tour* tab at the very top of the page, which loads a Youtube video.
