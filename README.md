# Nombre candidato: Valeria Arias González
# Fecha: 19 de Julio de 2022
# Cargo: Científico de Datos

## Prueba técnica

### Objetivo

Cree un regresor que recomiende el tamaño de la "tripulación" para los posibles compradores de barcos.

### Instrucciones

Esta prueba debe ser desarrollada con el lenguaje de programación python. El resultado debe ser cargado en un Jupyter notebook y debe ser cargado en un repositorio de github para su entrega.

### Datos

Los datos para la prueba deben ser descargados de aquí.

### Pasos a seguir para el desarrollo de la prueba

1. Leer el archivo 
2. Mostrar las columnas
3. Calcular estadísticas básicas de los datos, interpretarlos y enunciar sus observaciones
  - **Realizando las estadísticas básicas se puede observar que cada columna tiene un rango de valor bastante diferenciado a las demás.**
4. Seleccionar las columnas que se consideran importantes para predecir el tamaño de la tripulación (crew)
5. Si eliminas columnas explica la razón de la decisión tomada
  - **Se realizó una matriz de covarianza para encontrar la correlación de cada columna con la columna de tripulación (crew). Con esto se puede notar que hay una correlación muy fuerte con cuatro columnas: Tonnage, passengers, length y cabins, por lo que se utilizaron estas para la regresión.**
6. Utiliza “one-hot encoding” para las características categóricas
7. Crea conjuntos de entrenamiento y prueba (utilice el 60 % de los datos para el entrenamiento y el restante para prueba).
8. Cree un modelo de aprendizaje automático para predecir el tamaño de la tripulación. 
9. Calcula el coeficiente de correlación de Pearson para el conjunto de entrenamiento y los conjuntos de datos de prueba.
10. Describa los hiperparámetros en su modelo y cómo los cambiaría para mejorar el rendimiento del modelo.
  - **Los hiper parámetros utilizados para el entrenamiento fueron alpha y fit_intercept. Para mejorar el rendimiento se puede cambiar el parámetro alpha para regularizar mejor el modelo.**
11. ¿Qué es la regularización? ¿Cuál es el parámetro de regularización en su modelo?
  - **La regularización es un método el cual sirve para que el modelo no se sobreajuste y de esta manera de mejores resultados. Para esto se usó la regularización Ridge (L2), variando alpha.**
12. Trazar el valor del parámetro de regularización frente a la correlación de Pearson para los conjuntos de prueba y entrenamiento, y ver si su modelo tiene un problema de sesgo o de varianza.

