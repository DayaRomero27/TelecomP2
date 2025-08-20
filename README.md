Propósito del Análisis
Este proyecto tiene como objetivo principal predecir el churn (cancelación) de clientes en la empresa Telecom X mediante el uso de técnicas de machine learning. El análisis identifica patrones y variables predictoras que permiten anticipar qué clientes tienen mayor probabilidad de cancelar sus servicios, enabling la implementación de estrategias proactivas de retención.

Objetivos específicos:

Identificar las variables más influyentes en la decisión de cancelación

Desarrollar un modelo predictivo con alta precisión

Proporcionar insights accionables para el equipo de retención

Reducir la tasa de churn mediante intervenciones dirigidas

Estructura del Proyecto
telecom-x-churn-prediction/
│
├── notebooks/
│   └── TelecomX_Churn_Analysis_Parte2.ipynb  # Cuaderno principal de análisis
│
├── data/
│   ├── raw/
│   │   └── TelecomX_Data(2).csv              # Datos originales
│   ├── processed/
│   │   ├── TelecomX_Data_Limpio.csv          # Datos después de limpieza
│   │   └── TelecomX_Data_Preprocesado.csv    # Datos listos para modelado
│   └── models/
│       └── best_churn_model.pkl              # Modelo entrenado
│
├── visualizations/
│   ├── churn_distribution.png
│   ├── feature_importance.png
│   ├── correlation_matrix.png
│   └── model_performance.png
│
├── reports/
│   └── insights_report.pdf                   # Reporte ejecutivo
│
└── README.md



1. Clasificación de Variables
Variables Categóricas:

Gender: Género del cliente (Male/Female)

Contract: Tipo de contrato (Month-to-month/One year/Two year)

InternetService: Tipo de servicio de internet

PaymentMethod: Método de pago

MultipleLines: Múltiples líneas telefónicas

OnlineSecurity: Seguridad en línea

TechSupport: Soporte técnico

Variables Numéricas:

Tenure: Antigüedad del cliente (meses)

MonthlyCharges: Cargos mensuales

TotalCharges: Cargos totales

SeniorCitizen: Cliente senior (0/1)

2. Etapas de Preprocesamiento
Limpieza Inicial:

Eliminación de columnas irrelevantes (IDs, información personal)

Manejo de valores nulos

Detección y tratamiento de outliers

Codificación:

One-Hot Encoding para variables categóricas nominales

Label Encoding para variables ordinales

Target Encoding para categorías con muchos niveles

Normalización:

StandardScaler para variables numéricas

Preservación de la distribución original cuando fue necesari
