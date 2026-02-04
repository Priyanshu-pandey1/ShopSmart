# 🛒 ShopSmart: E-commerce Revenue Prediction

ShopSmart is a machine learning project designed to predict whether a website visitor will generate revenue based on their browsing behavior. By utilizing a **Decision Tree Classifier** integrated into a **Scikit-Learn Pipeline**, this project identifies key patterns in customer sessions to help businesses optimize their conversion rates.

## 🚀 Project Overview

The goal of this project is to classify customer sessions as "Revenue Generating" (1) or "Non-Revenue Generating" (0). The model addresses the challenge of **class imbalance** (where most visitors do not buy) by using balanced class weights and strategic pruning.

### Key Features:
* **Automated Preprocessing:** Uses `ColumnTransformer` to handle numerical scaling (`StandardScaler`) and categorical encoding (`OneHotEncoder`) simultaneously.
* **ML Pipeline:** Implements a robust `Pipeline` to prevent data leakage and ensure clean, reproducible code.
* **Hyperparameter Tuning:** Optimized using `GridSearchCV` to find the best balance between model depth and leaf size.
* **Imbalance Handling:** Utilizes `class_weight='balanced'` to improve recall for the minority class (actual buyers).

## 🛠️ Tech Stack

* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn
* **Algorithm:** Decision Tree Classifier

---

## 📊 Model Performance

After optimization, the model achieved a strong balance between precision and recall, ensuring that we capture as many potential buyers as possible.

| Metric | Score |
| :--- | :--- |
| **Best F1-Score (Tuned)** | **0.634** |
| **Accuracy** | **0.85** |
| **Recall (Class 1)** | **0.83** |

### Confusion Matrix Insights:
The model is particularly strong at identifying potential customers, achieving a **83% Recall** for the revenue class, which is vital for marketing targeting.

---

## 📂 Repository Structure

* `ShopSmart.ipynb`: The main Jupyter Notebook containing data analysis, pipeline construction, and model evaluation.
* `shop_smart_ecommerce.csv`: The dataset containing visitor session attributes.

## ⚙️ How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/Priyanshu-pandey1/ShopSmart.git](https://github.com/Priyanshu-pandey1/ShopSmart.git)
