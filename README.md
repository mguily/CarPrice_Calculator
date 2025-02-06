# 🚗 Predicción de Precios de Coches  

Este proyecto tiene como objetivo predecir el precio de coches en función de diversas características como la marca, el modelo, el tipo de combustible, la transmisión y otras variables relevantes.  

---  

## 📊 Resultados del Modelo  

Se ha entrenado un modelo de **Regresión Lineal** para predecir los precios, obteniendo los siguientes resultados:  

- **Coeficiente de Determinación (R² Score):** 0.91
- **Error Absoluto Medio (MAE):** 793.48  
- **Error Cuadrático Medio (MSE):** 818,588.25  

📌 **Conclusión:** El modelo tiene un buen rendimiento, ya que explica aproximadamente el **91%** de la variabilidad del precio de los coches. Sin embargo, hay margen de mejora con modelos más avanzados como **Random Forest** o **Gradient Boosting**.  

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

## 📘 Guía para Usar el Notebook de Predicción  

### 🔍 Cómo utilizar los valores  

- **Brand (Marca):** Marca del coche (Ej: Audi, BMW, Ford).  
- **Model (Modelo):** Modelo del coche (Ej: Q5, X5, Focus).  
- **Year (Año):** Año de fabricación del coche.  
- **Fuel_Type (Tipo de combustible):**  
  - `Electric` → Eléctrico  
  - `Petrol` → Gasolina  
  - `Diesel` → Diésel  
- **Transmission (Transmisión):**  
  - `Automatic` → Automática  
  - `Manual` → Manual  
- **Mileage (Kilometraje):**  
  - Número de **millas** que ha recorrido el coche.  
  - 📏 **Conversión:** 1 milla = **1.60934 km**  
  - Ejemplo: **680,000 millas** → **1,094,353.2 km**  
- **Engine_Size (Tamaño del motor):** Tamaño del motor en litros (Ej: 1.6, 2.0, 3.5).  
- **Doors (Número de puertas):** Número de puertas (Ej: 2, 4).  
- **Owner_Count (Número de propietarios):** Número de propietarios anteriores (Ej: 1, 2, 3).  

### ✏️ ¿Cómo modificar los valores?  

Para hacer una predicción sobre un coche, simplemente reemplaza los valores en el diccionario `nuevo_coche` con los datos correspondientes.  

Ejemplo de entrada en **Predict.ipynb**:  

```python
nuevo_coche = {
    'Brand': 'Kia',  # Sustituye con valores reales
    'Model': 'Sportage',
    'Year': 2014, 
    'Fuel_Type': 'Hybrid',
    'Transmission': 'Manual',
    'Mileage': 98700,
    'Engine_Size': 2.6,
    'Doors': 3,
    'Owner_Count': 5
}
```

💸 Este coche debería valer (Mirando el csv) -> Kia,Sportage,2014,2.6,Hybrid,Manual,98700,3,4 -> **9926$**

El sistema de predicción ha mostrado un resultado cercano, pero no exacto, por eso hay margen de mejora. ⬇️

💸 ![image](https://github.com/user-attachments/assets/e1de418c-ac4a-437f-b348-f2ff117f2baf)

---

## 📂 Estructura del Proyecto

📜 **CarPrice_NB.ipynb** → Entrena el modelo de regresión lineal y lo guarda en un archivo.  
📜 **Predict.ipynb** → Carga el modelo guardado y realiza predicciones.  
📁 **car_price_dataset.csv** → Conjunto de datos con información de los coches.  
📁 **car_price_model.pkl** → Modelo de regresión lineal entrenado.  
📁 **label_encoders.pkl** → Codificadores de variables categóricas para la predicción.  

---

## 🚀 Próximos Pasos

✅ Mejorar el modelo con técnicas como **Random Forest** o **Gradient Boosting**.  
✅ Aplicar **normalización y escalado** en los datos para optimizar el rendimiento.  
✅ Probar otras métricas de evaluación y **ajustar hiperparámetros**.  

---

🎉 **¡Gracias por revisar este proyecto!** 😊
