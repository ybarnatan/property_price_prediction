# 🏠 Property Price Prediction in CABA (Buenos Aires, Argentina)

![banner](images/properati_banner.jpeg)

## 📌 Objective

This project aims to build a machine learning model capable of predicting residential property prices in **CABA (Ciudad Autónoma de Buenos Aires)** using real estate listing data. The model is designed to support buyers, sellers, and real estate professionals in making data-driven decisions by providing pricing insights based on property features and location.

---

## 📊 Summary of Findings

- The dataset included thousands of property listings in CABA with detailed attributes such as surface area, number of rooms and neighborhood.
- After cleaning and exploring the data, a **Random Forest Regressor** was used to model property prices.
- The final model achieved an **RMSE of 51,958 ARS**, indicating that on average, predicted prices deviate from actual values by around 52,000 ARS — an acceptable margin considering the natural price variability in the Buenos Aires market and that this model accounts for different property types.
- Key predictors included **covered surface area**, **number of rooms**, **neighborhood**, and **property type**.
- Error analysis revealed that most large errors occurred for properties with extreme values or unusual characteristics.

---

## 🧠 Model Details

- **Model Used**: Random Forest Regressor (`sklearn.ensemble`)
- **Why Random Forest?**
  - Handles non-linear relationships
  - Robust against overfitting
  - Provides feature importance metrics
    
- **Best Parameters**: Conducted using custom `grid search`
  - `n_estimators`: 500
  - `max_depth`: 50
  - `min_samples_split`: 10
  - `min_samples_leaf`:20
 
---

## 🗂️ Project Structure
├── properties_price_prediction_properati.ipynb #Project
│
├── data/             #Data hosted after downloading from source.
│   ├── hospitals/               # Hospitals georef. data
│   ├── neighborhoods/           # District shapefile
│   ├── parks/                   # Parks georef. data
│   ├── precios_ref_ZP_Ene2020/  # Referential prices from Zona Prop - Jan 2020
│
├── images/
│   ├── properati_banner # Banner image
│
├── README.md

---

##  💻 Tech Stack

* `Python`

* `Jupyter Notebook`

 - Data wrangling: `pandas`, `numpy`, `time`
 - Visualization: `matplotlib`, `seaborn`
 - Spatial/cartographic analysis: `geopandas`, `shapely`
 - Text mining: `re`, `unidecode`, `unicodedata`
 - ML Model implementation: `sklearn`


---

## 📌 Future Improvements

* Experiment with advanced models like XGBoost, LightGBM, or CatBoost (academic limitation: RF)
* Include temporal features such as listing date and market trends


---

## 🎓 Academic Context

* This project was developed as part of the Data Mining course within the Master’s in Data Exploitation and Knowledge Discovery program at [Universidad de Buenos Aires]. 
* The objective was to apply supervised machine learning techniques to a real-world problem, involving data preprocessing, model selection, hyperparameter tuning, and performance evaluation — with a strong emphasis on interpretability and error analysis.

---
  
## 📚 Data Source

[Data source](https://www.kaggle.com/competitions/fcen-dm-2025-prediccion-precio-de-propiedades/leaderboard) 

---

## ✍️ **Author**  

**Yair Barnatan**

[LinkedIn](https://www.linkedin.com/in/yair-barnatan/) | [GitHub](https://github.com/ybarnatan)

📧 Email: ybbarnatan@gmail.com

