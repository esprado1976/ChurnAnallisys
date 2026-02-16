📊 Predicción de Churn en Servicios de Hogar con Random Forest

Este proyecto desarrolla un modelo de Machine Learning capaz de identificar clientes en riesgo de abandono (Churn). El objetivo es proporcionar una herramienta accionable para que los equipos de Customer Experience (CX) puedan intervenir proactivamente.

🎯 Contexto y Objetivos
El abandono de clientes es uno de los desafíos más críticos en las empresas de servicios. Este análisis se enfoca en:

Identificar los disparadores (drivers) principales del Churn.

Predecir con alta sensibilidad (Recall) qué clientes tienen mayor probabilidad de irse.

Optimizar la retención mediante la segmentación por probabilidad de riesgo.

🛠️ Stack Tecnológico
Lenguaje: Python 3.x

Entorno: Google Colab / Jupyter Notebooks

Librerías principales:

Pandas y NumPy para manipulación de datos.

Scikit-Learn para el modelado y optimización (Random Forest, GridSearchCV).

Seaborn y Matplotlib para el Análisis Exploratorio (EDA).

📈 Hallazgos Principales (EDA)
A través del análisis exploratorio, detectamos que:

Soporte Técnico: Los clientes sin soporte técnico muestran una tasa de abandono significativamente mayor, lo que sugiere una oportunidad para la implementación de agentes de IA de soporte.

Antigüedad (Tenure): El riesgo es crítico en los primeros meses de contratación.

Cargos Mensuales: Existe una correlación positiva entre cargos más altos y la probabilidad de fuga.

🤖 El Modelo
Se implementó un Random Forest Classifier optimizado mediante GridSearchCV.

Métricas de Performance
Tras el ajuste de hiperparámetros y el balanceo de clases, logramos:

Recall (Clase 1): 0.77 — El modelo detecta exitosamente al 77% de los clientes en riesgo.

F1-Score: 0.61 (Equilibrio optimizado para sensibilidad).

🚀 Implementación y Resultados
El modelo genera un archivo clientes_en_riesgo.csv que incluye la probabilidad de Churn para cada cliente. Esto permite:

Acciones Preventivas: Automatización de contactos vía agentes de IA para clientes con riesgo > 80%.

Eficiencia en CX: Priorización de la fuerza de ventas y soporte en los casos de mayor impacto económico.

Cómo ejecutar
Clona el repositorio.

Sube tu archivo CSV de datos o monta tu Google Drive.

Ejecuta las celdas del notebook para entrenar el modelo o utiliza el archivo .pkl guardado para predicciones directas.
