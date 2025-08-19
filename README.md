
README

# 📊 Telecom X_ML - Parte 2: Predicción de Churn

Este proyecto forma parte del análisis de **Telecom X**, cuyo propósito principal es **predecir la cancelación de clientes (Churn)** a partir de un conjunto de variables relevantes. El estudio busca identificar patrones de comportamiento en los usuarios y apoyar la toma de decisiones estratégicas en la retención de clientes.

---

## 🗂️ Estructura del Proyecto

TelecomX_Parte2/
│── data/
│ ├── Obtenemos la data de la URL = "https://raw.githubusercontent.com/FelipeOctavio87/Proyecto_TelecomX_ML/refs/heads/main/preprocessed_TelecomX_data.json"
│
│── notebooks/
│ ├── TelecomX_ML.ipynb # Cuaderno principal del análisis
│
│── visualizations/
│ ├── *.png / *.jpg # Gráficos generados en el EDA y modelización
│
│── README.md # Documentación del proyecto


---
## 🔎 Proceso de Preparación de los Datos

1. **Clasificación de variables**  
   - **Categóricas:** Género, tipo de contrato, servicio telefónico, servicio de internet, métodos de pago, entre otras.  
   - **Numéricas:** Tenencia en meses, cargos mensuales, cargos totales, edad, entre otras.

2. **Transformaciones aplicadas**  
   - **Codificación:** Variables categóricas transformadas mediante **One-Hot Encoding** o **Label Encoding** dependiendo del caso.  
   - **Normalización:** Escalado de variables numéricas para mejorar el desempeño de los algoritmos sensibles a la escala (ej. Regresión Logística, SVM).

3. **División de datos**  
   - **Entrenamiento:** 70-80% de los datos.  
   - **Prueba:** 20-30% de los datos.  
   - Se utilizó estratificación para mantener la proporción de clientes que cancelan y los que permanecen.

---

## ⚙️ Modelización y Justificación

Durante la construcción de modelos se consideraron diferentes algoritmos, destacando:

  
- **Random Forest:** manejo robusto de variables categóricas y no linealidades.  
- **Support Vector Machine (SVM):** útil para identificar fronteras complejas de decisión.  

Cada elección fue motivada por el balance entre interpretabilidad, capacidad predictiva y desempeño con datos desbalanceados.  
Para mitigar el **desbalance de clases**, se aplicaron técnicas como **SMOTE** (Synthetic Minority Oversampling Technique).

---

## 📈 Exploración de Datos (EDA)

Se realizaron análisis exploratorios para comprender el comportamiento de los clientes. Algunos insights relevantes fueron:

- **Tipo de contrato:** Los contratos mensuales presentan mayor tasa de churn.  
- **Servicios adicionales:** Clientes con múltiples servicios tienden a cancelar menos.  
- **Cargos mensuales:** Montos elevados se asocian a una mayor probabilidad de churn.  

Ejemplos de visualizaciones generadas:  
- Histogramas de distribución de cargos.  
- Boxplots comparativos entre clientes que permanecen y que cancelan.  
- Matriz de correlación entre variables numéricas.  
- Gráficos de barras para variables categóricas y su relación con el churn.  

---

## 🚀 Visualización del Proyecto

1. **Clonar o entrar al repositorio: https://github.com/FelipeOctavio87/Proyecto_TelecomX_ML**

2. Abrir notebooks/TelecomX_ML.ipynb en Jupyter Notebook o JupyterLab.



📌 Conclusiones

El churn puede predecirse con buena precisión utilizando modelos basados en árboles y técnicas de balanceo de clases.

Las variables relacionadas con contratos, cargos mensuales y servicios adicionales son las más relevantes.

El proyecto proporciona un marco de análisis aplicable a problemas similares en la industria de telecomunicaciones y otros sectores.

👤 Autor

Felipe Rebolledo
Proyecto académico/profesional de análisis de datos y machine learning aplicado al sector telecomunicaciones.
