# 🚗 Predicción de Precios de Coches

Este proyecto tiene como objetivo predecir el precio de coches en función de diversas características como la marca, el modelo, el tipo de combustible, la transmisión y otras variables relevantes.

📊 Resultados del Modelo

Se ha entrenado un modelo de Regresión Lineal para predecir los precios, obteniendo los siguientes resultados:

Error Absoluto Medio (MAE): 793.48

Error Cuadrático Medio (MSE): 818,588.25

Coeficiente de Determinación (R² Score): 0.91

📌 Conclusión: El modelo tiene un buen rendimiento, ya que explica aproximadamente el 91% de la variabilidad del precio de los coches. Sin embargo, hay margen de mejora con modelos más avanzados como Random Forest o Gradient Boosting.

⚙️ Desarrollo del Proyecto

1️⃣ Carga y Exploración de Datos

Se ha utilizado pandas para cargar y analizar el dataset.

Se han identificado variables categóricas y numéricas.

Se han tratado valores faltantes y se ha realizado una exploración inicial.

2️⃣ Preprocesamiento de Datos

Se han codificado las variables categóricas (Brand, Model, Fuel_Type, Transmission) usando LabelEncoder.

Se ha realizado una división del dataset en datos de entrenamiento y prueba (train_test_split con 80%-20%).

3️⃣ Entrenamiento del Modelo

Se ha utilizado Regresión Lineal de sklearn.linear_model.

Se ha entrenado con el conjunto de datos de entrenamiento.

4️⃣ Evaluación del Modelo

Se han calculado métricas de error (MAE, MSE) y precisión (R² Score).

Se han obtenido buenos resultados con un R² de 0.91.

5️⃣ Guardado del Modelo

Se ha guardado el modelo con joblib para futuras predicciones.

🚀 Próximos Pasos

Mejorar el modelo con técnicas como Random Forest o Gradient Boosting.

Aplicar normalización y escalado en los datos para optimizar el rendimiento.

Probar otras métricas de evaluación y ajustar hiperparámetros.

¡Gracias por revisar este proyecto! 😊
