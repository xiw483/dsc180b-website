# Multiple Testing Method with Empirical Null Distribution in Leukemia Studies
By Raymond Wang and Jacob Benson

## Introduction
Multiple testing analysis is a commonly used statistical practice in genetic research, often used to separate significant genes from a large pool of candidates. For example, in genome-wide association studies (GWAS), the multiple testing approach can be used to identify particular genes responsible for a certain disease. This is achieved through simultaneously conducting a large number of hypothesis tests between the control and experimental groups on each individual gene. With each hypothesis test’s t-statistics recorded, we can search through the data for anomalies and identify genes that might be correlated with the disease of our interest. 

Acute Lymphocytic Leukemia (ALL) and Acute Myelogenous Leukemia (AML) are two common types of leukemia. According to the [Children's Hospital of Pittsburgh](https://www.chp.edu/our-services/cancer/conditions/leukemia/types), ALL acounts for about 75 percent of childhood leukemia. It affects the growth of lymphocytes, a type of white blood cells that is normally responsible for one's immunity, causing it to overproduce and crowding out other types of blood cells. On the other hand, AML causes the overproduction of granulocytes, another type of white blood cells. Identifying genes responsible for each of the two types of leukemia helps us to better understand their pathology as well as allows build statistical models adaptable for future studies and applications.


![Sample images of AML, ALL, and other types of leukemia](/aml_all.jpeg)

[Sample images of AML, ALL, and other types of leukemia](https://www.mdpi.com/2075-4418/9/3/104/htm)


In our study, we will apply a multiple testing model to a leukemia gene dataset to identify genes that are expressed differently between the two groups of leukemia. We will use both a theoretical null distribution and an empirical null distribution and compare and contrast the results between the two. We hypothesize that the empirical null distribution will yield more meaningful result than the theoretical null distribution.

## Exploratory Data Analysis
The dataset we will be using is collected by Harvard Professor of Pediatric, Todd Golub. It contains the gene expressions of 47 AML patients and 25 ALL patients. It is seperated into a training set and a test set. We will use these genetic data to perform pairwise t-tests between the ALL patients and the AML patients for every single gene. We will then transform the resulting t-statistics into standardized z-scores and apply quantile transformation. 

![Countplot of AML and ALL patients](/all_aml_pie.png)



## Theory and Methods
## Results
## References
Ahmed N, Yigit A, Isik Z, Alpkocak A. Identification of Leukemia Subtypes from Microscopic Images Using Convolutional Neural Network. Diagnostics. 2019; 9(3):104. https://doi.org/10.3390/diagnostics9030104

Efron, B., Tibshirani, R., Storey, J.D., Tusher, V., 2001. Empirical Bayes analysis of a microarray experiment. J. Am. Stat. Assoc. 96 (456), 1151-1160.

Golub TR, Slonim DK, Tamayo P, Huard C, Gaasenbeek M, Mesirov JP, Coller H, Loh ML, Downing JR, Caligiuri MA, Bloomfield CD, Lander ES. Molecular classification of cancer: class discovery and class prediction by gene expression monitoring. Science. 1999 Oct 15;286(5439):531-7. doi: 10.1126/science.286.5439.531. PMID: 10521349.

Schwartzman,A., Dougherty, R., Lee, J., Ghahremani, D., & Taylor, J. (2009). Empirical null and false discovery rate analysis in neuroimaging. NeuroImage, 44(1), 71–82.

“Types of Leukemia: Children's Hospital Pittsburgh.” Children's Hospital of Pittsburgh, www.chp.edu/our-services/cancer/conditions/leukemia/types. 
