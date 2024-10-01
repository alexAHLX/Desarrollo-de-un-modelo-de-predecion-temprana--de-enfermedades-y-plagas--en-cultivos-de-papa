# Desarrollo de un Modelo de Detección Temprana de Plagas y Enfermedades en Cultivos de Papa Altoandina de Cusco mediante Redes Neuronales Convolucionales y Transfer Learning

## Resumen del Proyecto

Este proyecto se enfoca en desarrollar un modelo de detección temprana de plagas y enfermedades en cultivos de papa altoandina en Antapallpa, Cusco. El objetivo es mitigar las pérdidas en la producción, que pueden alcanzar hasta un 30% anual, mediante el uso de técnicas avanzadas de aprendizaje automático.

### Características Principales:
- Utilización de Redes Neuronales Convolucionales (CNN) y Transfer Learning.
- Dataset: 464 imágenes locales de hojas de papa, complementadas con datos internacionales de Kaggle.
- Técnicas de preprocesamiento: segmentación en espacio de color HSV y data augmentation.
- Evaluación de tres modelos: CNN personalizada, ResNet50 y ResNet101.

## Metodología

### 1. Preparación de Datos
- **Recolección**: Combinación de imágenes locales e internacionales.
- **Preprocesamiento**: 
  - Segmentación utilizando espacio de color HSV.
  - Aumento de datos para enriquecer el conjunto de entrenamiento.

### 2. Aumento de Datos
Aplicación de técnicas como:
- Rotación
- Escalado
- Recorte
- Cambios de color
- Flip horizontal/vertical

Objetivo: Mejorar la generalización del modelo y reducir el sobreajuste.

### 3. Modelos Evaluados
1. CNN Personalizada
2. ResNet50
3. ResNet101

### 4. Entrenamiento y Evaluación
- Entrenamiento inicial con datos internacionales.
- Fine-tuning con datos locales de Cusco.
- Evaluación de precisión y capacidad de generalización.

## Resultados

- Todos los modelos superaron el 85% de precisión.
- ResNet101 alcanzó la mayor precisión con 95.62%.
- La CNN personalizada mostró mejor ajuste a características locales.

## Impacto y Aplicaciones

- Mejora en la detección temprana de plagas y enfermedades.
- Potencial reducción de pérdidas en cultivos.
- Modelo replicable para otras regiones y cultivos en Perú.


## Estructura del Proyecto

- `data/`: Contiene los conjuntos de datos (raw, procesados, aumentados).
- `notebook_data_preparations/`: Notebooks para preparación y exploración de datos.
- `notebook_model/`: Implementación y entrenamiento de modelos.
- `notebook_predicciones/`: Scripts para realizar predicciones con los modelos entrenados.

## Próximos Pasos

- Ampliar el conjunto de datos locales.
- Explorar técnicas avanzadas de transfer learning.
- Implementar el modelo en una aplicación móvil para uso en campo.