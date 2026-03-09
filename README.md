# 📊 Telecom X: Predicción de Evasión de Clientes (Churn) con Machine Learning

## 📝 Descripción del Proyecto
Este proyecto de Ciencia de Datos analiza la base de clientes de la empresa de telecomunicaciones **Telecom X** con el objetivo de entender y predecir la evasión de clientes (*Churn*). Retener a un cliente es más rentable que adquirir uno nuevo, por lo que este análisis busca identificar los factores clave que llevan a la cancelación del servicio y proponer estrategias de retención basadas en datos.

## 🛠️ Tecnologías y Librerías Utilizadas
* **Lenguaje:** Python
* **Manipulación de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Regresión Logística, Random Forest)
* **Balanceo de Clases:** Imbalanced-learn (SMOTE)

## 🚀 Estructura y Fases del Proyecto

El análisis se dividió en dos grandes etapas documentadas en los cuadernos de Jupyter:

### Parte 1: Exploración y Limpieza de Datos (EDA)
* Extracción de datos desde formato JSON vía API.
* Limpieza de datos nulos y eliminación de variables no predictivas (`customerID`).
* Ingeniería de características (creación de la métrica `Cuentas_Diarias`).
* Análisis visual del comportamiento de los clientes cruzando variables demográficas y financieras con la tasa de evasión.

### Parte 2: Modelado Predictivo (Machine Learning)
* **Preprocesamiento:** Transformación de variables categóricas mediante *One-Hot Encoding* y escalado de variables numéricas (*StandardScaler*).
* **Balanceo de Datos:** Aplicación de la técnica **SMOTE** para corregir el desbalanceo en la variable objetivo (Churn) y evitar sesgos en el modelo.
* **Entrenamiento:** Creación y ajuste de dos modelos de clasificación:
  1. *Regresión Logística* (sensible a la escala, excelente para inferencia y análisis de coeficientes).
  2. *Random Forest* (basado en árboles, excelente para manejar relaciones complejas y extraer la importancia de las variables).
* **Evaluación:** Medición del desempeño utilizando métricas clave como Exactitud (Accuracy), Precisión, Sensibilidad (Recall), F1-Score y Matrices de Confusión.

## 💡 Principales Hallazgos (Insights)
A través de la extracción de importancia de variables (*Feature Importance*) y el análisis de coeficientes, descubrimos que los factores que más influyen en la cancelación son:

1. **Tiempo de Contrato (Tenure):** El riesgo de abandono es crítico durante los primeros meses. La lealtad aumenta significativamente con el tiempo.
2. **Tipo de Contrato:** Los clientes con modalidad "Mes a mes" presentan la mayor tasa de evasión en comparación con los contratos anuales.
3. **Cargos Mensuales:** Existe una correlación directa entre cuotas mensuales altas y la decisión de buscar alternativas en la competencia.

## 🎯 Recomendaciones Estratégicas
Basado en los modelos predictivos, se sugiere a Telecom X:
* Implementar un programa de atención prioritaria (*Onboarding*) durante los primeros 90 días del cliente.
* Crear campañas de *upselling* ofreciendo beneficios para incentivar la transición de contratos mensuales a contratos de 1 o 2 años.
* Monitorear a los clientes con cargos mensuales elevados y ofrecer reestructuraciones antes de que decidan cancelar.

---
*Desarrollado por Axel Edwin Serrano Ruiz*
| ![Imagen](https://github.com/user-attachments/assets/b056c417-64ea-47ef-a64e-144917396f74) |
| :---: |
