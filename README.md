# eBay Product Price Intelligence — Web Scraped Data Mining & Prediction

An end-to-end machine learning project focused on **predicting product prices** using a real-world dataset scraped from eBay. The project follows the **CRISP-DM** framework, combining **data mining**, **predictive modeling**, and **data visualization** to support smarter pricing strategies for sellers and businesses.

---

## 🌐 Dataset Origin

The dataset was collected through **ethical web scraping** of live eBay product listings. It includes over **1,990 records** with product names, ratings, number of ratings, and categories.  
To promote transparency and reproducibility, the dataset was cleaned, documented, and uploaded to Kaggle:

📎 **Kaggle Dataset**: [eBay Scraped Products](https://www.kaggle.com/datasets/topvirus/ebay-scraped-products)

---

##  Project Objectives

- Identify the most influential features affecting **product pricing** on eBay.
- Build a predictive model that can estimate prices with a **Mean Absolute Error (MAE) < 30**.
- Support sellers in making better **data-driven pricing decisions**.
- Deploy an explainable ML pipeline that is **fair, scalable, and actionable**.

---

##  CRISP-DM Pipeline Overview

| Phase               | Highlights |
|---------------------|-----------|
| **Business Understanding** | Reduce pricing inefficiencies & improve sales against competitors. |
| **Data Collection** | Scraped live data from eBay using Python scraping tools. |
| **Data Preparation** | Cleaned missing values, engineered `Rating_Factor`, normalized data, stratified binning. |
| **Modeling**         | Trained and compared **Random Forest** and **XGBoost** regressors. |
| **Evaluation**       | Achieved MAE of **25**; used **SHAP** for interpretability. |
| **Deployment**       | Created price prediction function + Power BI dashboard for sellers. |

---

## 📂  Dataset Summary

| Attribute            | Description                        |
|----------------------|------------------------------------|
| `Product_Name`       | Name of the listed item            |
| `Price` *(target)*   | Actual listed price (float)        |
| `Rating`             | Average rating out of 5 (may be missing) |
| `Number_of_Ratings`  | Total count of user ratings        |
| `Category`           | eBay product category              |

---

##  Models & Results

- **Best Model**: `XGBoost Regressor`
- **Performance**:
  - MAE: `25`
  - RMSE: `32`
- **Interpretability**:
  - Used `Feature Importance` from Random Forest
  - Applied `SHAP` for model transparency

---

##  Visualizations & Dashboard

- Built an interactive **Power BI dashboard** to help sellers visualize:
  - Predicted vs. actual prices
  - Price distribution by category
  - Rating effects on pricing

- Developed Python price prediction function that accepts new data inputs and returns estimated prices instantly.

---

## 🔒 Ethics & Fairness

-  **Ethical scraping** with no personal identifiers.
-  Compliant with data privacy principles (e.g., GDPR).
-  Addressed **data imbalance** with oversampling/undersampling.
-  Used **fair metrics** across multiple subgroups.


---

## 📂 Repository Contents

| File/Folder               | Description                                      |
|---------------------------|--------------------------------------------------|
| `code.ipynb`              | Full notebook with scraping, preprocessing, modeling |
| `ebay_scraped_products.csv` | Cleaned dataset uploaded to Kaggle             |
| `README.md`               | Project documentation                            |

---

## 📌 Key Takeaways

- Product **rating** and **category** are strong price influencers.
- Transparent pricing insights can boost seller trust and pricing accuracy.
- The project pipeline is modular and can be extended to other e-commerce platforms.

---

## 🔗 Useful Links

- 📊 [Kaggle Dataset](https://www.kaggle.com/datasets/topvirus/ebay-scraped-products)

---

##  Conclusion

This project successfully demonstrates the application of CRISP-DM principles in a real-world e-commerce scenario. It delivers a fully functional pricing prediction system that is not only accurate but also explainable and business-relevant. With ethical data handling and model fairness at its core, this solution holds promise for wider deployment in intelligent retail systems.

