# Hierarchical-Clustering
"Advanced Unsupervised Learning project implementing Hierarchical Clustering (Ward Linkage) on customer demographic data to extract strategic business segments."
# Customer Analytics & Segmentation using Advanced Unsupervised Learning

This repository features an advanced data science and marketing analytics project that segments a population of 2,000 consumers based on their socio-demographic and economic attributes. By implementing feature scaling, correlation analysis, and **Hierarchical Agglomerative Clustering**, this project groups consumers into distinct actionable clusters to assist businesses in formulating hyper-targeted marketing and VVIP customer retention strategies.

## 📊 Dataset & Features Overview
The project processes a comprehensive consumer dataset (`segmentation data.csv`) containing the following behavioral attributes:
* **Sex & Marital Status**: Demographic baseline metrics.
* **Age & Education**: Professional and maturity lifecycle indicators.
* **Income**: Quantitative annual earning power.
* **Occupation**: Segmented into Unemployed/Entry-level, Skilled, and Management/Self-employed.
* **Settlement Size**: Classified by community type (Small town, Mid-sized city, Metropolitan).

## 🚀 Key Framework & Workflow
1. **Exploratory Data Analysis (EDA)**: Investigating dataset distribution and high-level statistical properties.
2. **Correlation Matrix & Heatmap**: Mapping linear dependencies (e.g., strong relationships between Education vs Age, and Income vs Occupation).
3. **Feature Scaling**: Utilizing `StandardScaler` to uniformize metrics and avoid variance dominance during distance metrics optimization.
4. **Hierarchical Clustering**: Computing Euclidean distances using the **Ward Linkage Method** to structure a descriptive cluster tree (Dendrogram).
5. **Cluster Profiling**: Translating multivariate statistical means into real-world buyer personas.

## 📈 Consumer Personas & Business Action Plan

An optimal allocation of $K=4$ clusters was extracted from the dendrogram analysis, resulting in the following target segments:

| Cluster ID | Market Segment Name | Core Characteristics | Core Geo-Demographics | Strategic Corporate Actions |
| :---: | :---: | :---: | :---: | :---: |
| **Cluster 0** | **Budget-Conscious Young Starters** | Lowest Income, Entry-level or Unemployed jobs | ~35 Yrs Old, Majority Females, Rural/Small Towns | Focus on value-driven marketing, standard consumer credit lines, and seasonal sales. |
| **Cluster 1** | **Affluent Single Professionals** | High Income, Fast-tracked Skilled Careers | ~37 Yrs Old, 100% Single Males, Mega Cities / Metros | High conversion potential for luxury lifestyle products, performance electronics, and global travel. |
| **Cluster 2** | **The Wealthy Elite / Seniors** | Highest Income, Highest Education & Top Management | ~55 Yrs Old, Mixed Gender, Metropolitan Areas | **VVIP Tier**. Focus on asset management, luxury estate investments, and premium concierge services. |
| **Cluster 3** | **Affluent Young Couples** | High Income Growth, Solid Professional Trajectory | ~28 Yrs Old, 100% Married, Mid-to-Large Cities | Ideal demographic for automated home appliance plans, automotive loans, and nuclear family products. |

## 🛠️ Tech Stack & Dependencies
* **Python 3**
* **Pandas & NumPy**: Structural data handling and multi-dimensional matrices.
* **SciPy**: For executing hierarchical clustering trees and linkages.
* **Matplotlib & Seaborn**: For plotting correlation matrices and dendrograms.
* **Scikit-Learn**: For preprocessing scalers and training automated models.

## ⚙️ How to Initialize and Run
1. Clone this repository to your local runtime ecosystem:
   ```bash
   git clone https://github.com
   ```
2. Set up dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the processing script:
   ```bash
   python customer_segmentation_adv.py
   ```
