# Clasificación de Patologías Pulmonares mediante Vision Foundation Models

Este proyecto implementa un sistema de diagnóstico asistido por computadora (CAD) para la identificación de patologías en radiografías de tórax. Se explora el uso de **Self-Supervised Learning (SSL)** y modelos fundacionales como **DINOv2** para la extracción de características robustas en imágenes médicas.

## Tecnologías y Frameworks
- **Deep Learning:** TensorFlow / Keras
- **Modelos de Visión:** DINOv2 (Vision Transformers)
- **Procesamiento de Imágenes:** OpenCV, PIL
- **Análisis Estadístico:** Scikit-learn (Métricas de clasificación)
- **Entorno:** Python 3.x / Google Colab

## Metodología Detallada
El pipeline de este proyecto sigue los estándares de la investigación en IA Médica:
1. **Preprocesamiento:** Normalización y redimensión uniforme para el procesamiento de imágenes de TC/Rayos X.
2. **Feature Extraction:** Evaluación de características visuales robustas sin supervisión (DINOv2).
3. **Fine-tuning:** Adaptación de modelos pre-entrenados para tareas específicas de diagnóstico radiológico.
4. **Regularización:** Implementación de técnicas para prevenir el sobreajuste en datasets médicos de alta variabilidad.

## Evaluación y Resultados
El modelo fue evaluado bajo métricas de alta sensibilidad, críticas en el entorno clínico:
- **Matriz de Confusión:** Para el análisis de falsos negativos (críticos en medicina).
- **ROC / AUC:** Evaluación de la capacidad de discriminación del modelo.
- **Comparativa:** El uso de modelos fundacionales mostró una mejora significativa en la generalización frente a CNNs tradicionales desde cero.

## Estructura
- `/notebooks`: Contiene el flujo completo de entrenamiento y validación.
---

