# admetshiny v1.0.1.

### Visualizations

1.Added PERMANOVA statistics (R2, F, p-value) to PCA, t-SNE and UMAP plots via
vegan::adonis2(), computed on the original distance matrix. 

2.Added cumUlative R2 to the PCA subtitle. 

3.Added Shapiro-Wilk normality test and descriptive statistics (n, mean, SD, 
median, IQR) to plotMW, plotTPSA and plotLogP subtitles. 

4.Added Kruskal-Wallis test to plotHistogramCustom and plotViolinsubtitles, 
Wilcoxon, test for the two-group colour support. 

5.Improved the cluster heatmap with a labelled colour key (key.title, key.xlab),
finer colour breaks, and NA colour support. 

6.Fixed plotClusterHeatmap to handle NULL inputs from renderUI (method, palette,
scale_data) with safe defaults. 

7.Increased report figure resolution from 150 to 300 dpi. 

### Dark mode

1.Fixed the report preview container showing invisible text in dark mode (white 
background with light text).

### PubChem / Webchem compatibility update 

1. Updated pc_prop() property names for webchem 2.0: CanonicalSMILES is now 
ConnectivitySMILES. IsomericSMILES is now SMILES. Added column rename for 
backwards compatibility. 

### New dependencies

1.Added vegan to Imports for PERMANOVA computation. 

2.Added importFrom for stats::as.hclust, stats::cophenetic, stats::rect.hclust, 
stats::kruskal.test, stats::quantile, stats::shapiro.test, stats::wilcox.test. 

3.Added importFrom for vegan::adonis2()
