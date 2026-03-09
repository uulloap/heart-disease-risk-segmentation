# Heart Disease Segmentation: PCA & Cluster-Based Risk Analysis

![R](https://img.shields.io/badge/Language-R-blue.svg)
![Topic](https://img.shields.io/badge/Domain-Healthcare_/_Bioinformatics-red.svg)
![Method](https://img.shields.io/badge/Method-Unsupervised_Learning-orange.svg)

## 📌 Project Overview
This project applies unsupervised machine learning techniques to the Cleveland Heart Disease dataset to identify distinct patient risk profiles. By implementing dimensionality reduction and clustering, the analysis simplifies complex clinical data into actionable patient segments for targeted medical screening.

## 📊 Business Problem
Clinical datasets often contain highly correlated variables, making it difficult to isolate the primary drivers of cardiac risk. This project aims to consolidate these variables into "Risk Dimensions" to help healthcare providers prioritize screenings for the most vulnerable patient populations.



## 🛠️ Technical Stack
- **Language:** R
- **Libraries:** `tidyverse`, `cluster`, `factoextra`, `GGally`, `stats`
- **Techniques:** Principal Component Analysis (PCA), K-Means Clustering, Elbow Method, Silhouette Analysis.

## 🚀 Key Features
- **Dimensionality Reduction:** Used **PCA** to reduce 14 clinical features (e.g., cholesterol, max heart rate, ST depression) into 5 principal components explaining **[X]%** of total variance.
- **Patient Segmentation:** Implemented **K-Means Clustering** to group patients into distinct "Risk Tiers" based on their PCA scores.
- **Feature Correlation:** Conducted multivariate analysis to visualize the relationship between chest pain types, age, and asymptomatic indicators.
- **Optimal Cluster Selection:** Utilized the **Elbow Method** and **Average Silhouette Width** to mathematically determine the most stable number of patient segments.



## 📈 Key Insights & Results
- **Dominant Risk Factors:** PCA revealed that "Major Vessels Colored by Flourosopy" and "ST Depression" were the strongest contributors to the primary risk dimension.
- **Clinical Profiles:** Identified a specific "High-Risk" cluster characterized by high resting blood pressure and age, which significantly correlated with positive heart disease diagnoses.
- **Visualization:** Created a biplot to visualize how specific clinical variables (like Max Heart Rate vs. Age) drive patient separation in the feature space.

## 📂 Project Structure
```text
├── data/               # Cleveland Heart Disease dataset
├── notebooks/          # .Rmd file with PCA and Clustering implementation
├── output/             # PCA Scree plots, Biplots, and Cluster visualizations
├── Final_Report.pdf    # Statistical interpretation of clinical segments
└── README.md           # Project documentation
