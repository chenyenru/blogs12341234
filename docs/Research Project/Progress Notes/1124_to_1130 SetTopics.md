## Todo

This week:
>- [ ] look into the journals listed above
>- [ ] draft potential research topics for each of them
>- [ ] **REMEBER!** to evaluate each of them's practicality

## Paper and methods (**from last time**)

### [Integrative Bioinformatics and Functional Analyses of GEO, ENCODE, and TCGA Reveal FADD as a Direct Target of the Tumor Suppressor BRCA1](https://www.mdpi.com/1422-0067/19/5/1458/htm)

1.  Tumor Suppressor [BRCA1](https://www.ntuh.gov.tw/gene-lab-mollab/Fpage.action?muid=4048&fid=3866)
2.  **Identification of Potential BRCA1 Target Genes from ENCODE, GEO, and TCGA Data Analysis**

### Survival Analysis of Cancer Patients with the TCGA Datasets

1.  [Journals](https://www.google.com/search?q=survival+analysis+journal+tcga&client=firefox-b-d&biw=1280&bih=687&ei=vmKaYYG4Eabm2roPq4y9sA4&ved=0ahUKEwiBj9Dp36n0AhUms1YBHStGD-YQ4dUDCA0&uact=5&oq=survival+analysis+journal+tcga&gs_lcp=Cgdnd3Mtd2l6EAM6BwgAELADEBM6CwgAELADEAgQHhATOgQIABATOgYIABAeEBM6BQghEKABSgQIQRgBUNUBWMcfYIEhaAJwAHgAgAHZAYgBkgmSAQU0LjQuMZgBAKABAcgBA8ABAQ&sclient=gws-wiz)

### [Statistically identifying tumor suppressors and oncogenes from pan-cancer genome-sequencing data](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4757952/)


### [Bioinformatics prediction of differential miRNAs in non-small cell lung cancer](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0254854)
**aim**: screen miRNAs associated with 非小細胞肺癌(_NSCLC_) ... 非小細胞肺癌是最常見的肺癌種類 85% of all lung cancer
**method**: 
	- **dataset**: tcga and geo dataset. --> wow! this is exactly what i could do
	- **analysis**: ROC analysis, survival analysis, and enrichment analysis (GO term and KEGG pathway).
	
21 meaningful differentially expressed miRNAs were identified from NSCLC tissues and adjacent tissues. 
- **ROC Analysis**: The receiver operating characteristic (ROC) curve was used to analyze the sensitivity and specificity of the 4 miRNAs with the most differences, including hsa-mir-30a, hsa-mir-338, hsa-mir-451a, and hsa-mir-4732. 
- **Survival Analysis**: In addition, we also performed survival analysis, gene ontology (GO) terminology, and KEGG function prediction analysis on hsa-mir-30a, which is the most differentially expressed, to determine the related expression functions and pathways of hsa-mir-30a. Differentially expressed miRNAs were identified from NSCLC tissues and paracancerous tissues. And we hope to provide a potential development direction for the treatment of NSCLC.

In this study, we obtained all miRNAs in NSCLC tissues and paracancerous tissues from the TCGA database and GEO database. 21 meaningful differentially expressed miRNAs were identified from NSCLC tissues and adjacent tissues. The receiver operating characteristic (ROC) curve was used to analyze the sensitivity and specificity of the 4 miRNAs with the most differences, including ==hsa-mir-30a, hsa-mir-338, hsa-mir-451a, and hsa-mir-4732==. In addition, we also performed *survival analysis*, gene ontology *(GO) terminology*, and *KEGG function prediction analysis* on hsa-mir-30a, which is the most differentially expressed, to determine the related expression functions and pathways of hsa-mir-30a. Differentially expressed miRNAs were identified from NSCLC tissues and paracancerous tissues. And we hope to provide a potential development direction for the treatment of NSCLC.


#### 2.1. Data selection

We screened 52 NSCLC tissue specimens and 8 normal specimens from the TCGA database ([https://portal.gdc.cancer.gov/](https://portal.gdc.cancer.gov/)). The RNA-seq data of these samples were downloaded and analyzed. Furthermore, the raw sequencing data of 5 NSCLC tissue samples and 5 normal samples were downloaded from the National Center for Biotechnology Information (NCBI) GEO database ([http://www.ncbi.nlm.nih.gov/geo/](http://www.ncbi.nlm.nih.gov/geo/)) (GSE135918).

--> Hmm, maybe I can use a similar approach 🤓

#### 2.2. MiRNA screening and visualization
- Bioconductor DESeq2 package
- volcano maps (hehe used it last time)
#### 2.3. ROC diagnosis and survival curve
#### 2.4. GO and KEGG pathway enrichment analysis
