#bioinformatics #research #project #fun #goal

## Todo

This week:

> - [ ] look through other's github analysis for gene
> - [ ] have a draft of topic
> - [ ] take at least 2 lectures of each course
> - [ ] at least complete GEO analysis to get an idea of these analysis
> - [ ] play with TCGA
>   - [ ] play with GEO
>   - [ ] try the analysis tools listed in the research paper
# Definitions for Genetics ([source](https://www.ebi.ac.uk/training/online/courses/functional-genomics-i-introduction-and-design/what-is-functional-genomics/))
## Functional Genomics 
>- **Functional genomics**:  focuses on the ==dynamic expression== of gene products in a specific context
>     -   DNA level (genomics and epigenomics)
>     -   RNA level (transcriptomics)
>     -   Protein level (proteomics)
>     -   Metabolite level (metabolomics)
>     ![Functional genomics is the study of how the genome, transcripts (genes), proteins and metabolites work together to to produce a particular phenotype|400](https://www.ebi.ac.uk/training/online/courses/functional-genomics-i-introduction-and-design/wp-content/uploads/sites/60/2020/05/Figure01-1024x747.png "Functional genomics is the study of how the genome, transcripts (genes), proteins and metabolites work together to to produce a particular phenotype")
>- **Phenotype**: the set of observable characteristics of an individual resulting from the interaction of its genotype with the environment.

### Functional genomics case studies

Examples of biological questions that can be tackled using functional genomics experiments are:

-   Why do some cancer drugs only work effectively on a subset of patients with the disease?
-   Why are some cultivars of rice more resistant to drought than others?
-   What makes some individuals more susceptible to skin allergies?


# Tool
## Tool 1: GREIN ❌

![Figure 1|800](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41598-019-43935-8/MediaObjects/41598_2019_43935_Fig1_HTML.png)
⬆️ A schematic diagram for GREIN's workflow!

![[截圖 2021-11-16 下午10.16.33.png]]

However, the server seems to be shut down 🤧.

## Tool 2: GEO2R ✅

![[截圖 2021-11-16 下午10.46.27.png]]
I was greeted with this and it seems so interesting!

- [ ] look into what those plots mean
- [ ] see what log2 means to the data
- [ ] find the one that's most useful


# Analysis
## [Analysing data from GEO - Work in Progress](https://sbc.shef.ac.uk/geo_tutorial/tutorial.nb.html#Introduction)
### Print info
```r
library(GEOquery)
## change my_id to be the dataset that you want.
my_id <- "GSE33126"
gse <- getGEO(my_id)
pData(gse) ## print the sample information
fData(gse) ## print the gene annotation
exprs(gse) ## print the expression data
```
### Inspect Clinical Variables
I will need to inspect what variables will be useful

### Sample Clustering and Principal Component Analysis
```r
pheatmap()
```
![[Pasted image 20211121001334.png|500]]
#### Doing PCA
Need to first transpose the data so that we see how samples are related (and NOT GENES)
![[截圖 2021-11-21 下午1.53.26.png|500]]
![[截圖 2021-11-21 下午1.55.47.png|500]]
![[截圖 2021-11-21 下午2.00.30.png|500]]