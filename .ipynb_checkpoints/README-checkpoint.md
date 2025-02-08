📌 Nota **_Importante_**: Este proyecto es meramente académico y formativo. No está diseñado como un sistema de software robusto ni sigue estrictamente los principios de arquitectura software, por eso y por simplicidad, entre otras cosas, solo existe una rama main donde se sube todo el contenido. Su objetivo principal es la exploración y experimentación con modelos de predicción.

# 🚗 Predicción de Precios de Coches  

Este proyecto tiene como objetivo comparar el rendimiento de los algorítmos **Linear Regression y Gradient Boosting Regressor**. También te permite predecir el precio que tendrá un coche que crees fusionando marcas, modelos, kilometraje, etc.. Si quieres saber como, revisa el apartado: **"🔧 Configuración del Entorno"**, el cual se encuentra más abajo.

---

## 📂 Estructura del Proyecto

📁 **Performance** → Compara el rendimiento de ambos algorítmos.  
📁 **GB** → Sistema de Gradient Boosting.  
📁 **LR** → Sistema de Regresión Lineal.  
📜 **car_price_dataset.csv** → Conjunto de datos con información de los coches.  

---  

## ❓ ¿Por qué tiene sentido la comparación?

✅ **Regresión Lineal (LR)**  

Funciona bien si el precio de los coches tiene una relación lineal con las características (por ejemplo, si el precio aumenta de manera constante con la potencia del motor o el año del modelo). Es fácil de interpretar y entrenar rápido.  

✅ **Gradient Boosting (GB)**  

Puede capturar relaciones no lineales entre características y precio (por ejemplo, si un coche muy viejo baja mucho de precio, pero los clásicos pueden subir).
Es más preciso en datasets complejos, pero puede ser más lento y requerir ajuste de hiperparámetros.

**¿Cómo compararlos?**  
- Métricas de error: Usa MSE, RMSE o MAE para ver cuál predice mejor.
- Distribución de Errores: Si un modelo hace buenas predicciones, la distribución de errores tiende a parecerse a una curva normal.
- Importancia de variables: Si el modelo es perfecto, los puntos deberían alinearse en la diagonal y = x.

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
🔹 Entrenamiento con los datos procesados.  

### 4️⃣ Guardado del Modelo  
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
📂 Abre la carpeta del algorítmo que quieras probar.
📜 Abre el archivo **Predict_X.ipynb**.  
▶️ Ejecuta las celdas paso a paso para cargar el modelo y hacer predicciones.  

---

🎉 **¡Gracias por revisar este proyecto!** 😊