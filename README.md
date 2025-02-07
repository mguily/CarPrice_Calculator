📌 Nota Importante: Este proyecto es meramente académico y formativo. No está diseñado como un sistema de software robusto ni sigue estrictamente los principios de arquitectura software. Su objetivo principal es la exploración y experimentación con modelos de predicción.

# 🚗 Predicción de Precios de Coches  

Este proyecto tiene como objetivo predecir el precio de coches en función de diversas características como la marca, el modelo, el tipo de combustible, la transmisión y otras variables relevantes.  

---  

## 📊 Resultados con Regresión Lineal (Performance_LinearRegression.ipynb)

A continuación, se presentan los resultados obtenidos con el algoritmo básico de regresión lineal.

### 📈 Métricas de rendimiento  
- 🔹 **R² Score: 0.9163**  
- 🔹 **MSE (Error Cuadrático Medio): 811222.33**  
- 🔹 **RMSE (Raíz del Error Cuadrático Medio): 900.68**  
- 🔹 **MAE (Error Absoluto Medio): 791.46**  

### 🔍 Distribución de Errores  
El siguiente gráfico muestra la distribución de los errores (diferencia entre los valores reales y las predicciones):  

![📉 Distribución de Errores](https://github.com/user-attachments/assets/1f8e47a6-e93f-476e-8120-482412995e37)

### 🎯 Predicciones vs Valores Reales  
El gráfico siguiente representa la relación entre las predicciones del modelo y los valores reales:  

![📊 Predicciones vs Valores Reales](https://github.com/user-attachments/assets/7f2e2b2c-ee3c-4383-8fbd-88544272c153)  

📌 **Conclusión:** El modelo no tiene un mal rendimiento, ya que explica aproximadamente el **91%** de la variabilidad del precio de los coches. Sin embargo, analizandio los gráficos:  

**Distribución de Errores**: No parece ser completamente normal, lo que sugiere que el modelo podría no estar capturando bien ciertos patrones en los datos.  
La línea roja en 0 sugiere que el modelo tiene un sesgo bajo, pero hay errores dispersos en ambos lados.  

**Predicciones vs Valores Reales**: La mayoría de los puntos están cercanos con la línea roja (valor ideal), lo que indica que el modelo predice bien en general.  
Sin embargo, hay cierta dispersión en valores más altos, lo que podría significar que el modelo tiene más dificultad para predecir valores extremos.   

---  

## ⚙️ Desarrollo del Proyecto  

### 1️⃣ Carga y Exploración de Datos  
✅ Se ha utilizado `pandas` para cargar y analizar el dataset.  
✅ Identificación de variables categóricas y numéricas.  
✅ Tratamiento de valores faltantes y exploración inicial.  

### 2️⃣ Preprocesamiento de Datos  
🔹 Codificación de variables categóricas (`Brand`, `Model`, `Fuel_Type`, `Transmission`) con `LabelEncoder`.  
🔹 División del dataset en datos de entrenamiento y prueba (`train_test_split` con **80%-20%**).  

### 3️⃣ Entrenamiento del Modelo  
🔹 Uso de **Regresión Lineal** (`sklearn.linear_model`).  
🔹 Entrenamiento con los datos procesados.  

### 4️⃣ Evaluación del Modelo  
📉 Cálculo de métricas: **MAE, MSE, R² Score**.  
📊 **R² obtenido:** **0.91** (buen resultado).  

### 5️⃣ Guardado del Modelo  
💾 Modelo guardado con `joblib` para futuras predicciones.  

---  

## 🔧 Configuración del Entorno  

Para ejecutar este proyecto, utilizaremos **Anaconda** con su entorno base y **Jupyter Notebook**.  

### 1️⃣ Instalar Anaconda (si no lo tienes instalado)  
📥 Puedes descargar e instalar Anaconda desde su página oficial:  
🔗 [https://www.anaconda.com/products/distribution](https://www.anaconda.com/products/distribution)  

### 2️⃣ Abrir Jupyter Notebook desde Anaconda Navigator  
🔹 Abre **Anaconda Navigator**.  
🔹 En la pestaña **Home**, selecciona el entorno `base (root)`.  
🔹 Busca **Jupyter Notebook** y haz clic en **Launch**.  

### 3️⃣ Abrir el Notebook de Predicción  
📂 Navega hasta la carpeta donde hayas clonado este repositorio.  
📜 Abre el archivo **Predict.ipynb**.  
▶️ Ejecuta las celdas paso a paso para cargar el modelo y hacer predicciones.  

---  

## 📘 Ejemplo de ejecución:

💸 Este coche debería valer (Mirando el csv: Kia,Sportage,2014,2.6,Hybrid,Manual,98700,3,4) -> **9926$**

El sistema de predicción ha mostrado un resultado cercano, pero no exacto, por eso hay margen de mejora. ⬇️

![image](https://github.com/user-attachments/assets/e7c6b710-205c-4c5c-9137-daeddff063f9)

---

## 📂 Estructura del Proyecto

📜 **CarPrice_NB.ipynb** → Entrena el modelo de regresión lineal y lo guarda en un archivo.  
📜 **Predict.ipynb** → Carga el modelo guardado y realiza predicciones.  
📁 **car_price_dataset.csv** → Conjunto de datos con información de los coches.  
📁 **car_price_model.pkl** → Modelo de regresión lineal entrenado.  
📁 **label_encoders.pkl** → Codificadores de variables categóricas para la predicción.  

---

## 🚀 Próximos Pasos

✅ Mejorar el modelo con técnicas como **Random Forest (Árboles de decisión en paralelo)** o **Gradient Boosting (Entrenar secuencialmente los árboles)**.  
✅ Aplicar **normalización y escalado** en los datos para optimizar el rendimiento.  
✅ Probar otras métricas de evaluación y **ajustar hiperparámetros (Parámetros del modelo configurados antes del entrenamiento)**.  

---

🎉 **¡Gracias por revisar este proyecto!** 😊
