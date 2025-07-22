# 🏠 Property Price Prediction in CABA (Buenos Aires, Argentina)

![banner](images/properati_banner.jpeg)

## 📌 Objective

This project aims to build a machine learning model capable of predicting residential property prices in **CABA (Ciudad Autónoma de Buenos Aires)** using real estate listing data. The model is designed to support buyers, sellers, and real estate professionals in making data-driven decisions by providing pricing insights based on property features and location.


📄 Full analysis available in [property_price_prediction](https://github.com/ybarnatan/property_price_prediction/blob/main/Property_price_prediction_Properati_Buenos_Aires.ipynb)

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

<pre>├── properties_price_prediction_properati.ipynb  # Notebook principal del proyecto
├── data/  # Carpeta general de datos
│   ├── hospitals/  # Datos georreferenciados de hospitales
│   ├── neighborhoods/  # Archivos shapefile de distritos/barrios
│   ├── parks/  # Datos georreferenciados de parques
│   ├── precios_ref_ZP_Ene2020/  # Precios referenciales de Zona Prop, enero 2020
├── images/
│   └── properati_banner  # Imagen/banner del proyecto
├── README.md  # Documentación principal del repositorio </pre>

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
* Segmenting the data pero district or propery type to reduce the error due to high variability of prices per district/property types.


---

## 🚀 Instructions

1. Clone the repository: `git clone https://github.com/tu_usuario/properties_price_prediction_properati.git`
2. Open jupyter notebook: `properties_price_prediction_properati.ipynb`

Note: Data should be downloaded from data source provided and hosted in the `data` folder with names `df_train` = entrenamiento.csv and `df_test` = a_predecir.csv 

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

