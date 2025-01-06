# **ML-Model: Customer Segmentation and CLV Prediction**

This project focuses on clustering and customer segmentation using machine learning models, specifically **K-Means** and **Gaussian Mixture Model (GMM)**. The dataset used is **TheLook**, an e-commerce dataset from Google BigQuery, which provides insights into customer behavior. The goal is to identify distinct customer segments to enhance marketing strategies and predict **Customer Lifetime Value (CLV)** for informed business decisions.

---

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Project Structure](#project-structure)
4. [How to Run the Project](#how-to-run-the-project)
5. [Dependencies](#dependencies)
6. [Key Results](#key-results)
7. [Next Steps](#next-steps)

---

## **Project Overview**

The project consists of two major components:
1. **Customer Segmentation**:
   - Clustering customers based on **RFM (Recency, Frequency, Monetary)** metrics.
   - Comparing two clustering algorithms: **K-Means** and **Gaussian Mixture Model (GMM)**.
   - Evaluating the quality of clusters using metrics like **Silhouette Score**.
   - Visualizing clusters using **3D PCA** for interpretability.

2. **Customer Lifetime Value (CLV) Prediction**:
   - Predicting the expected lifetime value of customers using regression models.
   - Features such as RFM metrics and customer demographics are utilized.

---

## **Features**

- **Clustering**:
  - Determining the optimal number of clusters using the **Elbow Method**.
  - Implementing K-Means and GMM for customer segmentation.
  - Cluster visualization using **PCA** (Principal Component Analysis).

- **Evaluation**:
  - Comparing clustering methods with **Silhouette Scores**.
  - Interpreting and labeling clusters into tiers such as **Platinum**, **Gold**, **Silver**, and **Bronze**.

- **Prediction**:
  - Predicting **CLV** to prioritize high-value customers.

---

## **Project Structure**

```plaintext
ML-MODEL/
├── data/                     # Contains raw and processed data files
├── notebooks/                # Jupyter notebooks for clustering and CLV prediction
│   ├── clustering-model.ipynb
│   ├── predictive-clv-model.ipynb
├── venv/                     # Virtual environment (ignored in Git)
├── config.py                 # Configuration file for sensitive credentials (ignored in Git)
├── requirements.txt          # Python dependencies for the project
├── README.md                 # Project documentation
```
## **How to Run the Project**

### **Clone the Repository**
```bash
git clone <repository-url>
cd ML-MODEL
```
### **Set Up a Virtual Environment**
``` python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```
### **Install Dependencies**
```
pip install -r requirements.txt
```
### **Set Up Google BigQuery**
Add your Google credentials JSON file and set the path in your environment variables:
```
export GOOGLE_APPLICATION_CREDENTIALS="path_to_your_credentials.json"
```
### ** Run Notebooks**

## **Key Results**
### Clustering Results
- Optimal Clusters (K-Means): 4
Silhouette Scores:
- K-Means: 0.44
- GMM: 0.33
### Cluster Labels:
- Platinum: High-value customers with high spending.
- Gold: Moderate spenders with frequent purchases but higher return rates.
- Silver: Infrequent, low spenders.
- Bronze: Dormant customers with minimal spending.
### CLV Prediction
Models trained to predict Customer Lifetime Value using regression techniques. (THIS IS STILL IN DEVELOPMENT)

