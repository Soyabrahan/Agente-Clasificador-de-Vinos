# Agente Clasificador de Vinos con Backpropagation

Este proyecto implementa una red neuronal multicapa desde cero en NumPy para clasificar vinos según sus características fisicoquímicas, utilizando el algoritmo de backpropagation. El código está diseñado para ejecutarse en Google Colab y permite cargar datasets en formato CSV, preprocesar los datos, entrenar la red y evaluar su desempeño.

## Características principales

- **Carga de datos:** Permite subir un archivo CSV con los datos de vinos.
- **Preprocesamiento:** 
  - Elimina columnas irrelevantes (`free sulfur dioxide`, `density`).
  - Normaliza las características con Z-score.
  - Codifica la variable objetivo (`quality`) en formato one-hot.
- **División de datos:** Separa el dataset en entrenamiento (60%) y prueba (40%) de forma aleatoria.
- **Red neuronal:** 
  - Dos capas ocultas (ReLU) y una capa de salida (Softmax).
  - Entrenamiento con descenso de gradiente y ajuste de tasa de aprendizaje.
- **Evaluación:** 
  - Calcula precisión (accuracy) y matriz de confusión.
  - Muestra ejemplos de predicciones reales vs. predichas.

## ¿Cómo usarlo?

1. Abre el notebook en Google Colab:  
   👉 [Abrir en Google Colab](https://colab.research.google.com/drive/1b9x-YbIQy_bSA3bCDDgDZUJRePO3cjDB?authuser=1#scrollTo=GeH-LRoS6mHM)

2. Sube tu archivo CSV de vinos cuando se solicite.

3. Ejecuta las celdas para entrenar y evaluar el modelo.

## Estructura del código

- **Carga y limpieza de datos:**  
  Se eliminan columnas seleccionadas y filas con datos faltantes o no numéricos.
- **Normalización y codificación:**  
  Se normalizan las características y se codifica la salida en one-hot.
- **Entrenamiento:**  
  Implementación manual del forward pass, cálculo de la función de pérdida (cross-entropy), backpropagation y actualización de pesos.
- **Evaluación:**  
  Se calcula la precisión y la matriz de confusión sobre el conjunto de prueba.

## Ejemplo de resultados

- Precisión del modelo: ~81%
- Matriz de confusión y ejemplos de predicción incluidos en la salida.

---

**Autores:**  
Abrahan Ramirez y Jesus Merlin

**Repositorio:**  
[GitHub - Agente-Clasificador-de-Vinos](https://github.com/tu_usuario/Agente-Clasificador-de-Vinos)
