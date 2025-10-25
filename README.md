# 🚀 Analysis Machine Learning Students Social Media Addiction



**Autor:** Santiago Nahuel Victorino
**Curso:** Data Science
**Fecha:** 10/2025

[![Open In Colab](https://colab.research.google.com/drive/1xwCea1d-5q-M-VJYtyD3yR4aAza7rFWl?usp=sharing)](https://colab.research.google.com/github/SantiagoVictorino/Analysis_Machine_Learning_Students_Social_Media_Addiction/blob/main/[Proyect_Data_Science_Students_Media_Addiction.ipynb)

---

## 📝 Descripción del Proyecto

> This project analyzes a database on the consequences of social media use among students. The objective is to address the influence of average hours of social media use on average hours of sleep per night, building a machine learning model to discover the magnitude of that influence.

---

## 🎯 Planteamiento del Problema y Objetivos

### Pregunta de investigación
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

## ⚙️ Instalación y Uso

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

## 🔬 Metodología: El Paso a Paso

Esta es la sección más importante. Detalla las fases de tu proyecto de forma clara y ordenada.

### 1. Limpieza y Preprocesamiento de Datos
* Manejo de valores nulos (missing values).
* Corrección de tipos de datos.
* Codificación de variables categóricas (ej: One-Hot Encoding, Label Encoding).
* Detección y tratamiento de outliers (si aplica).

### 2. Análisis Exploratorio de Datos (EDA)
* Análisis univariado y bivariado para entender la distribución de las variables.
* Visualización de las relaciones entre las características y la variable objetivo (`Churn`).
* **Incluye aquí 1 o 2 de tus gráficos más importantes.** Puedes hacer una captura de pantalla del gráfico en tu Colab, subirla a tu repositorio de GitHub y enlazarla así:
    ```markdown
    ![Distribución de Churn por tipo de contrato](imagenes/grafico1.png)
    ```

### 3. Feature Engineering
* Creación de nuevas características a partir de las existentes.
* Escalado de datos numéricos (ej: StandardScaler, MinMaxScaler).

### 4. Modelado y Entrenamiento
* División del dataset en conjuntos de entrenamiento y prueba (`train_test_split`).
* Modelos probados (ej: Regresión Logística, Random Forest, XGBoost).
* Explicación breve de por qué elegiste esos modelos.
* Menciona si usaste técnicas como Cross-Validation para asegurar la robustez del modelo.

### 5. Evaluación del Modelo
* Métricas utilizadas para evaluar el rendimiento (Accuracy, Precisión, Recall, F1-Score, Curva ROC).
* Presentación de los resultados, por ejemplo, con una matriz de confusión.
    ```markdown
    ![Matriz de Confusión del Modelo Final](imagenes/matriz_confusion.png)
    ```

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

