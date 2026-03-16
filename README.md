# 📊 Análisis de Rentabilidad y Optimización de Margen - Superstore 📉

## 📋 Descripción del Proyecto
Este proyecto consiste en un análisis exhaustivo de los datos de ventas de una "Superstore" para identificar fugas de rentabilidad. A través de la exploración de datos y el modelado estadístico, se detectó que la subcategoría de **Mesas (Tables)** presentaba pérdidas críticas debido a una política de descuentos ineficiente.

El objetivo principal fue determinar el **punto de equilibrio (breakeven)** para los descuentos, permitiendo que la categoría vuelva a ser rentable.

## 🛠️ Herramientas Utilizadas
* **Lenguaje:** Python 3.12
* **Librerías:** * `Pandas` & `NumPy`: Procesamiento de datos y cálculos estadísticos.
    * `Matplotlib` & `Seaborn`: Visualización avanzada de datos.
    * `np.polyfit`: Implementación del modelo de Regresión Lineal.

## 🔍 Hallazgos Clave

### 1. El Problema del Lunes (Monday)
Al segmentar por día de la semana, se identificó que la categoría **Furniture (Muebles)** es la menos rentable los lunes, con un margen de apenas **2.91%**, comparado con el **22.40%** de Office Supplies.

### 2. La "Trampa de Descuento" en Mesas
Dentro de Furniture, las **Mesas (Tables)** mostraron un margen negativo del **-6.39%**. Al profundizar, se encontró una correlación negativa agresiva: a mayor descuento, el margen se desploma de forma no sostenible.

## 📈 Modelado: Regresión Lineal y Breakeven
Utilicé un modelo de regresión lineal ($y = mx + b$) para encontrar el límite de descuento que el negocio puede soportar.

![Análisis de Sensibilidad de Descuento](./sensibilidad_descuento_mesas.png)

### Resultados del Modelo:
* **Punto de Equilibrio:** El descuento máximo tolerable es del **17.5%**.
* **Impacto:** Por cada 1% que se aumenta el descuento, el margen cae aproximadamente un **1.62%** (basado en la pendiente del modelo).
* **Situación Crítica:** La región **East** opera con un 38% de descuento, lo que explica su pérdida neta masiva.

## 🚀 Recomendaciones Estratégicas
1. **Tope de Descuento:** Implementar un límite máximo de descuento del **15%** para la subcategoría de Mesas.
2. **Revisión Regional:** Intervenir la estrategia comercial de la región **East**, alineándola con el modelo de la región **West** (que opera con descuentos del 16% y mantiene márgenes positivos).
3. **Monitoreo de Lunes:** Ajustar las promociones automáticas de los inicios de semana para evitar la erosión del margen en productos de mobiliario.

---
**Autor:** [Tu Nombre o Usuario de GitHub]  
**LinkedIn:** [Link a tu perfil]
