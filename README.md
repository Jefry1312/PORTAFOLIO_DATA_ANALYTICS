# 📊 Análisis de Rentabilidad y Sensibilidad de Precios: Sub-categoría "Mesas"

## 🎯 Contexto del Proyecto
En el análisis del dataset de retail, se detectó una **"Trampa de Volumen"**: la sub-categoría de Mesas genera ingresos significativos pero con pérdidas operativas constantes en casi todas las regiones. 

**El problema central:** Una política de descuentos agresiva aplicada para aumentar el volumen de ventas, sacrificando totalmente el margen de beneficio.

## 🛠️ Metodología Aplicada
Para resolver esto, utilicé **Python (Pandas & NumPy)** para modelar la relación entre los descuentos y el margen neto mediante una **Regresión Lineal Simple**.

### 🧪 Hallazgos Estadísticos
* **Ecuación del Negocio:** $y = mx + b$
* **Impacto:** Por cada 1% de descuento adicional, el margen de beneficio cae aproximadamente un **[X.XX]%** (Sustituye por tu valor de m*0.01).
* **Punto de Equilibrio (Breakeven):** Se identificó que el descuento máximo tolerable para no incurrir en pérdidas es del **17.5%**.

## 📈 Visualización Crítica
![Impacto del Descuento](./sensibilidad_descuento_mesas.png)

*Como se observa en el gráfico, regiones como **East (38% desc.)** operan en una zona de pérdida crítica, mientras que **West (16% desc.)** es la única región saludable.*

## 🚀 Recomendaciones Estratégicas
1. **Tope de Descuento:** Limitar los descuentos en mesas al 15% a nivel nacional.
2. **Estrategia de Precios:** Reclasificar las mesas como productos de bajo margen y evitar su uso como "líderes en pérdidas" con descuentos superiores al 18%.
3. **Optimización Regional:** Replicar el modelo de gestión de precios de la región West en las regiones East y Central.

## 🧰 Herramientas
* **Lenguaje:** Python 3.12
* **Librerías:** Pandas, NumPy, Matplotlib, Seaborn.
