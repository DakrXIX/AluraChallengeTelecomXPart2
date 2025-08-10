# 📊 Predicción de Cancelación de Clientes (Churn) – Proyecto TelecomX Latam

Este repositorio documenta el desarrollo de un proyecto de análisis y modelado predictivo enfocado en detectar los factores que impulsan la cancelación de clientes (*churn*) en una empresa ficticia del sector telecomunicaciones.

## 🔍 Propósito

La meta principal es identificar patrones y variables determinantes que influyen en la decisión de un cliente de abandonar el servicio. Esto permite proponer estrategias de retención más efectivas y anticiparse a la pérdida de usuarios.

---

## 🧱 Flujo del Proyecto

### 1. **Preparación de Datos**
- Procesamiento y normalización de datos originales.
- Limpieza de valores nulos y estandarización de formatos.
- Transformación de variables categóricas y numéricas.
- Creación de variables derivadas, como el gasto promedio diario.
- Consolidación de toda la información en un único DataFrame para facilitar el análisis.

### 2. **Análisis Exploratorio (EDA)**
- Revisión del *churn* según diferentes segmentos: tipo de contrato, método de pago, antigüedad, entre otros.
- Visualización y exploración de variables numéricas como:
  - `Charges.Total` (Gasto total acumulado)
  - `Tenure` (Meses como cliente)
- Detección de correlaciones relevantes y patrones de comportamiento.

### 3. **Modelado Predictivo**
Se desarrollaron y evaluaron diferentes modelos para estimar la probabilidad de cancelación:
- **Dummy Classifier** (modelo base)
- **Decision Tree Classifier**
- **Random Forest Classifier** (mejor desempeño, accuracy: 0.86)

### 4. **Variables Clave**
El análisis de importancia de variables reveló que los factores más influyentes incluyen:
- Tipo de contrato (`Contract_Month-to-month`)
- Antigüedad del cliente (`tenure`)
- Método de pago (`Electronic check`)
- Tipo de conexión a internet
- Servicios adicionales como soporte técnico y seguridad en línea

### 5. **Recomendaciones de Retención**
Basado en los resultados, se proponen acciones como:
- Mejorar la experiencia de incorporación de nuevos clientes.
- Incentivar contratos de mayor duración.
- Promover métodos de pago más confiables.
- Detectar clientes en riesgo y ofrecerles soluciones personalizadas.

---

## 🧠 Conclusión

La combinación de análisis estadístico y *machine learning* permitió no solo predecir la cancelación de clientes con alta precisión, sino también comprender qué factores tienen mayor impacto. Esto ofrece una base sólida para tomar decisiones estratégicas y reducir la tasa de *churn*.

---

## ⚙️ Herramientas Utilizadas

- Python 3.10
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 📬 Autor

Desarrollado por **Cesar Londoño**  
Para consultas o sugerencias, abre un *issue* o contáctame directamente.
