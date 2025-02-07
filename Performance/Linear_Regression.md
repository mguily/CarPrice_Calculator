# 📊 Resultados con Regresión Lineal (Performance_LinearRegression.ipynb)

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

📌 **Conclusión:** Un R² de 0.9163 indica que el modelo no es del todo malo. Sin embargo, analizando los gráficos:  

**Distribución de Errores**: No parece ser completamente normal, lo que sugiere que el modelo podría no estar capturando bien ciertos patrones en los datos.

**Predicciones vs Valores Reales**: La mayoría de los puntos están relativamente cercanos con la línea roja (valor ideal), lo que indica que el modelo no realiza predicciones exageradamene desviadas. Sin embargo, hay cierta dispersión en valores más altos, lo que podría significar que el modelo tiene más dificultad para predecir valores extremos.   
