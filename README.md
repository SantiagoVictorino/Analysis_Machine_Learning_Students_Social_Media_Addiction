# 🚀 Analysis Machine Learning Students Social Media Addiction



**Author:** Santiago Nahuel Victorino
**Course:** Data Science
**Date:** 10/2025

[![Open In Colab](https://colab.research.google.com/drive/1xwCea1d-5q-M-VJYtyD3yR4aAza7rFWl?usp=sharing)](https://colab.research.google.com/github/SantiagoVictorino/Analysis_Machine_Learning_Students_Social_Media_Addiction/blob/main/[Proyect_Data_Science_Students_Media_Addiction.ipynb)

---

## 📝 Project Description

> This project analyzes a database on the consequences of social media use among students. The objective is to address the influence of average hours of social media use on average hours of sleep per night, building a machine learning model to discover the magnitude of that influence.

---

## 🎯 Problem Statement and Objectives

### Research question
En este proyecto se intentará resolver la siguiente pregunta: ¿Qué influencia tiene el promedio de horas de uso de las redes sociales diarias sobre el promedio de las horas de sueño nocturno?

### Objetivos

1.  **Exploratory Aata Analysis (EDA):** Identificar las características y las variables que pueden llegar a ser afectadas por el uso diario de las redes sociales.
2.  **Statistical Analysis:** Hacer un análisis estadístico utilizando el coeficiente de correlación r de Pearson para medir la fuerza y dirección de la relación entre las variables.
3.  **Machine Learning model:** Implementar y entrenar un modelo de machine learning para conocer en profundidad la relación y determinar que tan significativa es.

---

## 📊 Dataset

* **Dataset source:** Kaggle - (https://www.kaggle.com/datasets/adilshamim8/social-media-addiction-vs-relationships).
* **Size** 705 rows x 13 columns.
* **Description:** Cada fila representa un estudiante único mientras que las columnas indican distintas caracateristicas de cada estudiante como por ejemplo la ubicacion geografica, la edad, el promedio de uso de redes sociales, el promedio de horas de sueño nocturnas, etc.

---

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Python 3.
* **Librerías Principales:**
    * **Pandas:** Para la manipulación y limpieza de datos.
    * **NumPy:** Para operaciones numéricas eficientes.
    * **Matplotlib & Seaborn:** Para la visualización de datos.
    * **Scikit-learn:** Para el modelado de Machine Learning (preprocesamiento, entrenamiento y evaluación).
* **Entorno:** Google Colab

---

## ⚙️ Instalación y Use

Explica cómo otra persona puede ejecutar tu proyecto. Dado que usaste Colab, la forma más fácil es enlazar directamente a tu notebook.

1.  **Clonar el repositorio (opcional):**
    ```bash
    git clone [https://github.com/](https://github.com/)[TU_USUARIO_GITHUB]/[TU_REPOSITORIO].git
    ```
2.  **Abrir en Google Colab:**
    La forma más sencilla de ejecutar este proyecto es haciendo clic en el siguiente botón para abrir el notebook directamente en Google Colab:

    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/[TU_USUARIO_GITHUB]/[TU_REPOSITORIO]/blob/main/[NOMBRE_DE_TU_NOTEBOOK].ipynb)

3.  **Instalar dependencias:**
    Si hay alguna librería que no venga por defecto en Colab, indica cómo instalarla:
    ```python
    !pip install -r requirements.txt
    ```
    *(Asegúrate de tener un archivo `requirements.txt` en tu repositorio).*

---

## 🔬 Methodology: The Step-by-Step

This project followed a defined structure to clean, analyze, model, and draw conclusions from the data.

### 1. Dataset Loading and Selection
* **Library Imports:** Necessary libraries for analysis were imported, including `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, and `sklearn`.
* **Data Loading:** The dataset (`Students Social Media Addiction.csv`) was loaded into a pandas DataFrame from Google Drive.
* **Variable Definition:** A variable dictionary was established to provide a clear reference for the meaning of each column in the dataset.

### 2. Data Cleaning and Preprocessing
An exhaustive cleaning process was performed to ensure data quality before analysis:
* **Null Values:** `df.isnull().sum()` was used to check for missing values. The analysis determined there was no null data in the set.
* **Categorical Inconsistencies:** The unique values (`.unique()`) of all categorical columns (like 'Gender', 'Academic_Level', etc.) were reviewed for typos or inconsistencies. None were found.
* **Whitespace Removal:** The `.str.strip()` function was applied to all object-type columns to remove leading or trailing whitespaces that could affect the analysis.
* **Outlier Handling:**
    * Box plots were generated for all numerical variables.
    * Using the Interquartile Range (IQR) method, 3 outliers were identified in the `Avg_Daily_Usage_Hours` column.
    * These outliers were removed, creating a new clean dataframe (`df_cleaned`) with 702 rows for the analysis.
* **Final Verification:** A final check was run on `df_cleaned` to confirm the absence of nulls, the consistency of categories, and the removal of outliers.

### 3. Statistical and Exploratory Data Analysis (EDA)
This phase focused on understanding the data and discovering relationships between variables.

* **Descriptive Analysis (Numerical):**
    * Descriptive statistics (`.describe()`) were calculated for key numerical variables, such as 'Age', 'Avg_Daily_Usage_Hours', 'Sleep_Hours_Per_Night', 'Mental_Health_Score', 'Conflicts_Over_Social_Media', and 'Addicted_Score'.
    * Histograms and ECDF (Empirical Cumulative Distribution Function) plots were generated to visualize the distribution of each of these variables.

* **Descriptive Analysis (Categorical):**
    * Frequency and proportion counts (`.value_counts()`) were calculated for categorical variables.
    * Count plots (`sns.countplot`) were created to visualize the distribution of 'Gender', 'Academic_Level', 'Most_Used_Platform', 'Affects_Academic_Performance', and 'Relationship_Status'. For the 'Country' variable, a Top 15 chart was plotted.

* **Bivariate and Correlation Analysis:**
    * The Pearson correlation coefficient between `Avg_Daily_Usage_Hours` and `Sleep_Hours_Per_Night` was calculated, resulting in **-0.79**, indicating a strong negative relationship.
    * A scatter plot (`sns.scatterplot`) was generated between these two variables to visually observe this relationship.

### 4. Machine Learning Modeling (Linear Regression)
To quantify the impact of social media hours on sleep, a linear regression model was implemented.

* **Problem Definition:** The research question was posed: "How do daily social media usage hours affect nightly sleep hours among students?".
* **Feature Selection:**
    * The predictor variable (X) was defined as `Avg_Daily_Usage_Hours`.
    * The target variable (y) was defined as `Sleep_Hours_Per_Night`.
* **Data Splitting:** The `df_cleaned` dataset was split into training (80%) and test (20%) sets using `train_test_split`.
* **Model Training:**
    * A `LinearRegression` model instance from `sklearn` was imported and created.
    * The model was trained on the `X_train` and `y_train` data using the `.fit()` method.

### 5. Evaluation and Communication of Results
* **Prediction and Evaluation:**
    * The trained model was used to make predictions (`.predict()`) on the test set (`X_test`) [cite: uploaded:Proyect_Data_Science

---

## 💡 Resultados y Conclusiones

Resume los hallazgos clave de tu análisis y el rendimiento de tu modelo final.

* **Resultados del EDA:** ¿Qué patrones interesantes encontraste? (Ej: "Los clientes con contratos mes a mes y fibra óptica tienen una tasa de abandono significativamente mayor").
* **Rendimiento del Modelo:** ¿Cuál fue el mejor modelo y qué métricas obtuvo? (Ej: "El modelo Random Forest alcanzó una precisión del 82% en el conjunto de prueba").
* **Conclusiones Finales:** ¿Qué respondiste de la pregunta de negocio inicial? Ofrece recomendaciones basadas en tus datos.

---

## 🚀 Trabajo Futuro

(Opcional, pero muy recomendado)

Enumera posibles mejoras o siguientes pasos para el proyecto. Esto demuestra que piensas a largo plazo.
* Probar con modelos más complejos (ej: redes neuronales).
* Recolectar más datos para mejorar la predicción.
* Desplegar el modelo como una API web.

