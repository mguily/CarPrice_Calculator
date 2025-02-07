# 📊 Resultados con Gradient Boosting

A continuación, se presentan los resultados obtenidos con el algoritmo básico de Gradient Boosting.

### 📈 Métricas de rendimiento  
- 🔹 **R² Score: 0.9987**  
- 🔹 **MSE (Error Cuadrático Medio): 12325.64**  
- 🔹 **RMSE (Raíz del Error Cuadrático Medio): 111.02**  
- 🔹 **MAE (Error Absoluto Medio): 84.32**  

### 🔍 Distribución de Errores  
El siguiente gráfico muestra la distribución de los errores (diferencia entre los valores reales y las predicciones):  

![📉 Distribución de Errores](https://github.com/user-attachments/assets/21b596f6-16ef-4484-ac00-efb5eb503e32)

### 🎯 Predicciones vs Valores Reales  
El gráfico siguiente representa la relación entre las predicciones del modelo y los valores reales:  

![📊 Predicciones vs Valores Reales](https://github.com/user-attachments/assets/93f72e16-484b-4022-b40c-25408bd102ab)

📌 **Conclusión:** Un R² de 0.9987 es casi perfecto, ya que logra predecir casi todas las variaciones de precio en función de las variables dadas. Analizando los gráficos:  

**Distribución de Errores**: La diferencia entre los valores reales y las predicciones sigue una distribución normal perfecta, centrada en 0, lo que indica que los errores son aleatorios y sin sesgo. Esto es una señal de que el modelo no está sobreajustado ni infraajustado y generaliza bien sobre los datos.  

**Predicciones vs Valores Reales**: El gráfico de predicciones contra valores reales muestra una alineación prácticamente perfecta, lo que sugiere que el modelo hace predicciones 'exactas' sin sesgo sistemático.   
