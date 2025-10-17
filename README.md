# Análisis Predictivo de Hospitalizaciones con Datos de VAERS COVID-19

Proyecto final para el curso de Data Science de la UTN-BA.

## Problema
El objetivo de este proyecto es construir un modelo de Machine Learning capaz de predecir la probabilidad de que un reporte de evento adverso a una vacuna (dataset VAERS) resulte en una hospitalización.

## Metodología
El flujo de trabajo consistió en:
1.  **Limpieza de Datos:** Tratamiento de valores nulos y corrección de tipos de datos.
2.  **Ingeniería de Características:** Se aplicaron técnicas de extracción manual para variables de texto y consolidación de categorías para reducir la dimensionalidad (de más de 500 a ~350 características).
3.  **Modelado:** Se entrenó un modelo de Regresión Logística.
4.  **Evaluación:** Se analizaron métricas como la matriz de confusión, exactitud, sensibilidad y especificidad.

## Resultados Clave
- El modelo final alcanzó una **exactitud del 92.82%**.
- El análisis reveló un fuerte desbalance de clases, resultando en una **baja sensibilidad (48%)**, lo que indica una debilidad para detectar casos de hospitalización.
- El gráfico de importancia de características mostró que los predictores más fuertes para la hospitalización son `HOSPDAYS`, `ER_ED_VISIT_Y` y `L_THREAT_Y`.

## Próximos Pasos
Las futuras iteraciones deberían enfocarse en técnicas para manejar el desbalance de datos (como SMOTE) para mejorar la sensibilidad del modelo.
