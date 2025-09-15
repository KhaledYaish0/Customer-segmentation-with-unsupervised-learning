# 🧑‍🤝‍🧑 Identify Customer Segments (Unsupervised Learning)

This project applies **unsupervised learning** to demographic data to identify segments of the population that form the core customer base for a mail-order sales company in Germany.  
It was developed as part of the Udacity Machine Learning Nanodegree, using real-world data provided by **Bertelsmann Arvato Analytics**.

---

## 📦 Data

The project works with four provided datasets:

- **`Udacity_AZDIAS_Subset.csv`**  
  Demographics data for the general population of Germany  
  (≈ 891,211 rows × 85 features)

- **`Udacity_CUSTOMERS_Subset.csv`**  
  Demographics data for the company’s customers  
  (≈ 191,652 rows × 85 features)

- **`AZDIAS_Feature_Summary.csv`**  
  Metadata file with feature attributes (85 rows × 4 columns)

- **`Data_Dictionary.md`**  
  Detailed documentation of all demographic features and codes

> Note: Data files are semicolon (`;`) delimited.

---

## 🛠️ Methods

1. **Data Preprocessing**
   - Handling missing values using codes from the feature summary
   - Converting categorical features to usable formats
   - Scaling and normalizing numerical features

2. **Dimensionality Reduction (PCA)**
   - Reduce 85 features to fewer components while retaining most variance
   - Interpret top principal components to understand main factors of variation

3. **Clustering (KMeans)**
   - Apply clustering on PCA-transformed data
   - Experiment with different numbers of clusters (k)
   - Use inertia, silhouette score, and interpretability to select the best k

4. **Customer vs. Population Comparison**
   - Assign clusters to both population and customer datasets
   - Identify **over-represented clusters** in the customer dataset
   - These clusters represent the company’s **core customer segments**

---

## 📊 Results

- PCA reduced dimensionality while keeping key variance in the data  
- KMeans clustering revealed distinct demographic groups  
- Certain clusters were found to be **significantly over-represented among customers**, pointing to the company’s main customer base  
- Insights can be applied for **targeted marketing campaigns** to maximize ROI

---
## 📁 Project Layout

Identify_Customer_Segments_project/
├── Identify_Customer_Segments.ipynb # Main analysis notebook
├── Identify_Customer_Segments.html # Exported notebook as HTML
├── README.md # Project documentation


---

## ⚙️ Setup

```bash
# (Optional) create a virtual environment first
pip install -r requirements.txt
```
## 📌 Requirements

pandas

numpy

scikit-learn

matplotlib

seaborn

(You can generate a requirements.txt with these libraries.)

##📜 License
For educational use only. Data provided by Bertelsmann Arvato Analytics.
