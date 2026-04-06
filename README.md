# 🚚 Análisis Predictivo de SLA: Optimización de Logística Inversa

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

## 📋 Descripción del Proyecto
Este proyecto nace de la necesidad de entender los desvíos en el cumplimiento del **SLA (Service Level Agreement)** en una operación de logística inversa con más de 60,000 registros. 

A través de un **EDA (Exploratory Data Analysis)** profundo y modelos de **Machine Learning**, se identificaron fallas sistémicas de trazabilidad y desfasajes entre los acuerdos comerciales y la capacidad operativa real.

## 🚀 Hallazgos Principales

### 1. Auditoría de Trazabilidad (Caso Pickit)
Se detectó un volumen crítico de pedidos con entrega final (POD) pero sin registro de imposición inicial. 
* **Insight:** El canalizador "Pickit" realiza cargas masivas de estados finales, omitiendo la trazabilidad intermedia y afectando artificialmente los indicadores de performance.

### 2. Feature Importance (Machine Learning)
Utilizando un modelo de **Random Forest**, se determinó que el factor con mayor peso en la generación de "Delays" es el **Objetivo de Días SLA** configurado en el sistema, por encima de la eficiencia de las sucursales o el volumen diario.

### 3. Detección de Anomalías
Mediante el algoritmo **Isolation Forest**, se aislaron casos atípicos donde la demora superaba los 60 días para SLAs de 48hs, identificando errores críticos de proceso y pérdidas de piezas.

## 📊 Visualizaciones Destacadas
* **Heatmaps:** Concentración de demoras por Sucursal y Día de la semana.
* **Dumbbell Charts:** Brecha entre el SLA exigido vs. el promedio real histórico.
* **Scatter Plots:** Identificación de anomalías detectadas por IA.

## 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python (Google Colab)
* **Librerías de Datos:** Pandas, Numpy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (RandomForestClassifier, IsolationForest)

## 📈 Conclusiones de Negocio
El proyecto permitió elevar recomendaciones estratégicas a la gerencia:
1. **Renegociación de SLA:** Ajuste de metas comerciales inalcanzables.
2. **Auditoría de Proveedores:** Exigencia de trazabilidad completa a canalizadores externos.
3. **Saneamiento de Datos:** Depuración de anomalías sistémicas para mejorar la visibilidad del tablero de control (Power BI).

---
*Proyecto desarrollado por [Tu Nombre/Usuario de GitHub]*
