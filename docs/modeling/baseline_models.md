# Reporte del Modelo Baseline

## Descripción del modelo

El primer modelo sera una red neuronal LSTM (Long-Short Term Memory), la cúal es uan arquitectura de red recurrente que posee memoría de corto y largo plazo.

## Variables de entrada

Las variables de entrada son el precio de los recursos de generación disponibles:

- AGUA.
- CARBÓN.
- GAS.
- LÍQUIDOS.

## Variable objetivo

La variable objetivo es el precio de bolsa a la que se vende la energía:

-PPP Bolsa diario.

## Evaluación del modelo

### Métricas de evaluación

- Error medio abosluto (MAE): Proporciona una medida del tamaño promedio de los errores.
- Error cuadrático medio (MSE): Media de los errores al cuadrado.
- Error porcentual absoluto medio (MAPE): Medida de la precisión porcentual del modelo.
- Coeficiente de determinación (R²): Mide que tan bien se ajustan los valores predichos a los valores reales.

### Resultados de evaluación

![image](https://github.com/FaSaSu20/MLD6_Proy/assets/65478386/3880300b-570b-4dfe-a235-275bcfc87d1f)

MAE = 23.810577542069577
MSE = 1399.8180107374865
MAPE = 0.13537180600439117
R² = 0.8858916094211834

## Análisis de los resultados

El MAE de 23.81 indica que el promedio se aleja ese valor respecto a los valores reales. el MSE indica que hay puntos de la serie de tiempo donde el error es mayor, recordemos que entre mas grande sea la diferencia entre la predicción y la real se penaliza mas el error. el MAPE indica un error porcentual del 13%. el R² de 0.88 es un valor cercano a 1, lo que indica que el ajuste es bueno y el modelo tiene buena explicabilidad respecto a las variabilidades lineales (multivariables) del modelo.

## Conclusiones

El modelo es una red neuronal de 4 capas (2 LSTM) con 117.619 parámetros. Tenemos un error porcentual del 13%, a consideración una muy buena aproximación para ser el primer experimento. Aún no se han aplicado técncias adicionales de proprocesamiento de los datos, no se han modificado hiperparámetros y tampco se ha probado una red de mayor complejidad, por lo tanto para ser el primer modelo, considero que funciona de manera correcta.

## Referencias

- https://www.tensorflow.org/api_docs/python/tf/keras/layers/LSTM

- https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_absolute_error.html#sklearn.metrics.mean_absolute_error

- https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_squared_error.html#sklearn.metrics.mean_squared_error

- https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_absolute_percentage_error.html#sklearn.metrics.mean_absolute_percentage_error

- https://scikit-learn.org/stable/modules/generated/sklearn.metrics.r2_score.html#sklearn.metrics.r2_score

