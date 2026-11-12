# Obesity Analysis: Clustering, Factorial Methods and Classification

Final project for *Quantitative Marketing Techniques* (MESIO UPC-UB, 2025), written in R.
It applies factorial, clustering and classification methods to a dataset on obesity levels (2,111 individuals, 17 variables on eating habits, physical condition and demographics).

## Methods
1. **Text analysis:** corpus cleaning and word cloud from a WHO web page on obesity
2. **Factorial methods:** correspondence analysis, multiple correspondence analysis (MCA) and PCA
3. **Clustering:** hierarchical clustering and k-means, with the number of clusters chosen using several validation criteria (2 vs 3 clusters compared)
4. **Classification:** k-nearest neighbours (plain, PCA-reduced and kernel versions), plus other supervised methods covered in the report

## Structure
```
data/obesity.csv   dataset
report/report.Rmd  full report with all code (in Spanish)
```

## How to run
```r
rmarkdown::render("report/report.Rmd")
```
Main packages: FactoMineR, factoextra, cluster, NbClust, clValid, flexclust, dendextend, caret, class, kknn, e1071, randomForest, nnet, tm, wordcloud, rvest, tidyverse.
The text analysis section scrapes a WHO web page, so it needs an internet connection.

## Data
The dataset appears to be the UCI "Estimation of obesity levels based on eating habits and physical condition" dataset (Palechor & De la Hoz Manotas, 2019). Check the original source's licence before reuse.

## Author
Mohammed Essabaouni
