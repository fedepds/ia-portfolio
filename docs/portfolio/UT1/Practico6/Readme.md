# Práctico 6 - Mall Customer Segmentation

## 🎯 Objetivo
Realizar un **análisis exploratorio y segmentación de clientes** a partir del dataset *Mall Customers* con el fin de:
1. Comprender las características principales de los clientes (edad, ingresos, puntaje de gasto).
2. Detectar outliers y analizar distribuciones.
3. Aplicar **clustering (K-Means)** para agrupar clientes en segmentos con patrones de consumo diferenciados.

---

## 📊 Dataset
- **Fuente**: [Mall Customer Segmentation Dataset](https://www.kaggle.com/datasets/shwetabh123/mall-customers)  
- **Columnas principales**:  
  - `CustomerID` → identificador único del cliente.  
  - `Genre` → género del cliente.  
  - `Age` → edad.  
  - `Annual Income (k$)` → ingreso anual (en miles de dólares).  
  - `Spending Score (1-100)` → puntaje de gasto asignado por el shopping.  

---

## 🔧 Proceso

### 1. Análisis Exploratorio
- Estadísticas descriptivas de las variables numéricas.  
- Distribución por género (balance relativo entre hombres y mujeres).  
- Análisis de **rangos y promedios** en edad, ingreso e índice de gasto.  
- Detección de **outliers con IQR** en las variables numéricas.  

### 2. Visualización
- Histogramas de las variables principales (`Age`, `Annual Income`, `Spending Score`).  
- Gráficos de dispersión para observar correlaciones.  
- Mapas de calor (heatmaps) para visualizar patrones.  

### 3. Clustering (K-Means)
- Normalización de variables para mejorar la separación de clusters.  
- Aplicación de **método del codo (Elbow Method)** para determinar el número óptimo de clusters.  
- Entrenamiento del modelo K-Means y asignación de etiquetas de cluster.  
- Visualización de los grupos formados en 2D (por ejemplo, Ingreso vs Spending Score).  

---

## 📈 Resultados
- Se identificaron **segmentos de clientes** con características distintas en función de ingresos y puntaje de gasto.  
- Ejemplo típico de clusters encontrados:  
  - Clientes de **alto ingreso pero bajo gasto**.  
  - Clientes de **bajo ingreso y bajo gasto**.  
  - Clientes de **alto gasto con ingresos medios** (potenciales clientes premium).  
- Los clusters permiten al shopping **diseñar estrategias de marketing personalizadas**.  

---

## 🔍 Reflexión
- El dataset es pequeño (200 clientes), pero suficiente para ilustrar el poder de la segmentación.  
- El clustering demostró que hay **patrones claros de consumo** que pueden aprovecharse.  
- Posibles mejoras:  
  - Usar más variables de comportamiento (por ejemplo, frecuencia de visitas, compras reales).  
  - Comparar con otros algoritmos de clustering (DBSCAN, jerárquico).  
  - Aplicar reducción de dimensionalidad (PCA) para visualizar mejor los grupos.  

---
