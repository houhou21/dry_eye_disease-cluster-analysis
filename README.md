# 👁️ Dry Eye Disease Clustering Analysis 

## 🏗️ Project Context  
This was a research project developed as teamwork for the third term of the Post-Degree Diploma in Data Analytics at Langara College.  

## 📌 Project Overview  
This project explores clustering methods to identify potential subgroups within individuals diagnosed with or at risk of Dry Eye Disease (DED). Using lifestyle, health, and behavioral data, the analysis investigates whether unsupervised machine learning can reveal patterns associated with DED outcomes.  

## 🎯 Objective  
- Identify distinct clusters based on lifestyle choices and assess their correlation with Dry Eye Disease outcomes.  
- Examine whether BMI and physical health contribute to DED development, and whether clustering can highlight higher-risk subgroups.  

## 🛠 Tools & Technologies  
- **Language & Libraries:** R (tidyverse, factoextra, cluster, fpc, mclust, dendextend, writexl)  
- **Techniques:** Data preprocessing, stratified sampling, PCA, k-means, PAM, hierarchical clustering, DBSCAN, hybrid HKMeans, cluster validation (Rand, VI, Silhouette, Gap Statistic), Wilcoxon tests  
- **Visualization:** ggplot2, factoextra  
- **Data Source:** Kaggle Dry Eye Dataset ([link](https://www.kaggle.com/datasets/dakshnagra/dry-eye-disease/data))  

## 📊 Key Steps  
1. **Data Preparation**  
   - Cleaned and transformed raw dataset (20,000 observations, 26 features).  
   - Stratified sampling of 200 records for analysis.  
   - Created derived features (e.g., BMI, split systolic/diastolic).  

2. **Exploratory Data Analysis**  
   - Numerical: distributions, correlations, PCA.  
   - Categorical: bar plots for lifestyle/health factors.  

3. **Clustering Analysis**  
   - Applied k-means, PAM, hierarchical (Ward, complete), hybrid HKMeans, DBSCAN.  
   - Evaluated number of clusters using WSS, Silhouette, Gap Statistic.  
   - External validation with Rand Index and VI.  

4. **Statistical Analysis**  
   - Compared clusters using Shapiro and Wilcoxon tests.  
   - Reviewed categorical and numerical distributions per cluster.  

## 🚀 Results  
| Aspect                 | Findings                                                                 |
|-------------------------|--------------------------------------------------------------------------|
| Lifestyle choices       | Alcohol consumption + Blue-light filter use linked to higher DED risk.   |
| Physical health         | Females with sleep disorders, eye strain, and irritation showed higher risk. |
| Clustering tendency     | Hopkins statistic ≈ 0.49 → data had low clustering tendency.             |
| Algorithm performance   | No clustering method significantly outperformed random assignment.       |
| Statistical validation  | Wilcoxon test revealed differences in numerical features, but categorical distributions were similar across clusters. |  

## 📂 Repository Structure  
```
├── Data/              # Raw data
├── Src/           # rmd file for analysis and modelling
├── Documentation/   # Project Proposal, Final project report and presentation
└── README.md          # Project description

## 🙌 Acknowledgments  
Developed by:  
- Javier Merino  
- Meyliani Sanjaya  
- Angeli De los Reyes  
- Nay Zaw Lin  
