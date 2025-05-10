🎬 Predicción de Ratings de Películas y Series con Red Neuronal (PyTorch)
Este proyecto implementa una red neuronal en PyTorch para predecir la categoría del rating IMDb de películas y series (Mal, Bien, Muy bien, Excelente), utilizando características como:

Tipo (película o serie)

Año de lanzamiento

Número de votos en IMDb

Géneros codificados (Drama, Comedia, Otro)

📊 Flujo del proyecto
Carga y limpieza de datos:

Dataset real procesado desde Kaggle (vía Google Drive).

Eliminación de columnas irrelevantes, valores nulos y outliers.

Estandarización de variables numéricas.

Preprocesamiento:

Codificación de géneros en variables binarias.

Clasificación del rating IMDb en 4 categorías.

División en conjunto de entrenamiento y test (80% / 20%).

Construcción de la red neuronal:

Arquitectura fully connected con 2 capas ocultas (64 y 32 neuronas).

Función de activación: ReLU.

Salida: 4 neuronas (una por clase).

Entrenamiento:

Optimización con Stochastic Gradient Descent (SGD).

Tuning automático de hiperparámetros (learning rate y momentum).

Función de pérdida: CrossEntropyLoss.

Evaluación:

Precisión del modelo en el test set.

Comparación de predicciones reales vs predichas.

Métricas: Accuracy y matriz de confusión.

Predicciones nuevas:

El modelo puede usarse para predecir la categoría IMDb de nuevas películas introduciendo sus atributos.
