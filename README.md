# ST_Insurance
Sure Tomorrow Insurance Company - Customer Management with Machine Learning.

### Descripción y Objetivos del Proyecto

La compañía de seguros Sure Tomorrow quiere resolver varias tareas con la ayuda de machine learning:

  - Tarea 1: encontrar clientes que sean similares a un cliente determinado. Esto ayudará a los agentes de la compañía con el marketing.
  - Tarea 2: predecir la probabilidad de que un nuevo cliente reciba una prestación del seguro. ¿Puede un modelo de predictivo funcionar mejor que un modelo dummy?
  - Tarea 3: predecir el número de prestaciones de seguro que un nuevo cliente pueda recibir utilizando un modelo de regresión lineal.
  - Tarea 4: proteger los datos personales de los clientes sin afectar al modelo del ejercicio anterior.

Es necesario desarrollar un algoritmo de transformación de datos que dificulte la recuperación de la información personal si los datos caen en manos equivocadas. 

### Etapas del Proyecto
  - Preprocesamiento y exploración de datos
  - Carga de datos
  - Análisis exploratorio de datos
    - Tarea 1. Clientes similares
    - Tarea 2. ¿Es probable que el cliente reciba una prestación del seguro?
    - Tarea 3. Regresión (con regresión lineal)
    - Tarea 4. Ofuscar datos
  - Prueba de que la ofuscación de datos puede funcionar con regresión lineal
  - Prueba de regresión lineal con ofuscación de datos
  - Conclusiones

### Herramientas Tecnológicas Implementadas

  - numpy as np
  - pandas as pd
  - math
  - seaborn as sns
  - sklearn.linear_model
  - sklearn.metrics
  - sklearn.neighbors
  - sklearn.preprocessing
  - train_test_split
  - IPython.display
  - StandardScaler
  - KNeighborsClassifier
  - DummyClassifier
  - mean_squared_error, r2_score
  - LinearRegression
  - NearestNeighbors

### Conclusiones

Con respecto al ejercicio de buscar clientes similares con distintas métricas, es un código muy práctico para por ejemplo encontrar clientes similares a un cliente en particular. Esto nos puede permitir por ejemplo generar campañas de marketing a estos clientes similares, podemos ofrecerles la compra con algún beneficio de los mismos productos o anticiparnos a alguna decisión que pueda tomar el cliente.

El escalado de datos parece mejorar el rendimiento del modelo KNN en comparación con el modelo sin escalar, como se evidencia por los valores más altos de F1-score y una matriz de confusión más equilibrada.

En general, tanto el modelo KNN escalado como el sin escalar superan al modelo aleatorio en términos de rendimiento de clasificación, lo que sugiere que estos modelos están aprendiendo patrones significativos en los datos y son capaces de hacer predicciones más precisas.

Con respecto al modelo de regresión lineal, los resultados demuestran que la regresión lineal es robusta frente al escalado de datos, manteniendo las mismas métricas de rendimiento, debido a que el RMSE y R2 tienen el mismo valor, lo que indica que el modelo se comporta de manera similar independientemente de si los datos están escalados o no.

Con respecto a la ofuscación de datos, en base a los resultados obtenidos y con la demostración analítica, comprobamos que la ofuscación de datos no afecta la capacidad predictiva de la regresión lineal.
