# Lab 4: Descriptive assessment of datasets

<!-- NOTE: 
You can preview this README.md document by clicking the 'Preview' button in the RStudio toolbar. 
-->

## Preparation

- Read/ annotate: [Recipe \#4](https://lin380.github.io/tadr/articles/recipe_4.html). You can refer back to this document to help you at any point during this lab activity.
- Note: do your best to employ what you've learned and use other existing resources (R documentation, web searches, etc.). If, however, you get stuck you are encouraged to view the lab model (`lab_4_model.Rmd`) for hints to get back on track.

## Objectives

- Read and inspect the structure of a dataset.
- Identify and apply the appropriate descriptive methods for a vector's informational value.
- Descriptively assess both single variables and multiple variables with the appropriate statistical, tabular, and/ or graphical summaries. 

## Instructions

### Setup

1. Create a new R Markdown document. Title it "Lab #4" and provide add your name as the author. 
2. Edit the front matter to have rendered R Markdown documents print pretty tabular datasets.
3. Delete all the material below the front matter.
4. Add a code chunk directly below the header named 'setup' and add the code to load the following packages
  - tidyverse
  - janitor
  - skimr

### Tasks

1. Create four level-1 header sections named: "Read and inspect", "Single variables", "Multiple variables", and "References". 
2. Follow the instructions that follow adding the relevant prose description and code chunks to the corresponding sections.

*Remember:*

- Add code comments (`# code comments...`) to your code lines to clarify what each step of your code does. 
- Use Markdown syntax as necessary to format your responses
- Use keyboard shortcuts inside code chunks/ the R Console (`<-`, `%>%`, code completion hints, etc.)

**Read and inspect**

In this lab you will be working with a curated dataset drawn from the [CEDEL2 Corpus](http://cedel2.learnercorpora.com/) (L2 Spanish written corpus). The observations in this dataset represent compositions written by L1 English-L2 Spanish learners. 

- Cite the dataset adding `bibiliography: references.bib` in the front matter and using the correct citation key (found in `references.bib`). 
- Read the dataset (`data/derived/cedel_dataset.rds`) and describe the dataset:
  - How many compositions (observations) are in this dataset?
  - How many measures (variables) are in this dataset?
    - What type informational values does each contain?
    - What describe the type of measure of each variable. 

**Single variables**

Categorical: 

- Summarize the categorical variables `sex` and `proficiency`.
  - Use tabular and/ or graphical methods, as appropriate.
- In a prose description, describe any notable aspects of these two variables.

Continuous: 

- Summarize the any two of the four variables `placement_test_score_percent`, `num_tokens`, `num_types`, or `ttr`. 
  - Use statistical and/ or graphical methods, as appropriate.
- In a prose description, describe any notable aspects of these two variables.

**Multiple variables**

Consider what you have learned about this dataset by exploring the previous variables. With this in mind, summarize at least two relationships that involve two variables. 

- Use tabular, statistical and/ or graphical methods, as appropriate.
- In a prose description, describe any notable aspects of these two relationships.

### Assessment

Add a section which describes your learning in this lab.

Some questions to consider: 

  - What did you learn?
  - What was most/ least challenging?
  - What resources did you consult? 
  - What more would you like to know about?

## Submission

1. To prepare your lab report for submission on Canvas you will need to Knit your R Markdown document to PDF or Word. 
  - Note: you will have to add the front matter line to pretty-print tables under the `pdf_document:` or `pdf_document2:` (if you want cross-references to tables or figures) output. 

```yaml
output:
  pdf_document:
    df_print: kable
```
  
2. Download this file to your computer.
3. Go to the Canvas submission page for Lab #4 and submit your PDF/Word document as a 'File Upload'. Add any comments you would like to pass on to me about the lab in the 'Comments...' box in Canvas.

