# Reporte del Modelo Final

## Resumen Ejecutivo

El modelo que se implemento fue una red LSTM de 117.619 parámetros, el resumen de las principales métricas se observa en la siguiente tabla:

| M étrica  | Valor |
| ------------- | ------------- |
| MAE  | 23.810577542069577  |
| MSE  | 1399.8180107374865  |
| MAPE  | 0.13537180600439117  |
| R²  | 0.8858916094211834 |

## Descripción del Problema

El objetivo es predecir el precio de bolsa promedio ponderado de la energía eléctrica en función del precio de las energías de generación tales como el agua, el gas, el carbón y combustibles líquidos.

## Descripción del Modelo

El modelo fue el siguiente:

![image](https://github.com/FaSaSu20/MLD6_Proy/assets/65478386/cf442f85-71c2-4351-9833-008f84d5da3c)

Se utilizo un modelo de red neuronal LSTM, debido a que estamos trabajando con una serie de tiempo, es decir el dato siguiente depende del anterior y asi sucesivamente, por lo tanto es necesario una arquitectura de NN que tenga "memoría", las redes LSTM nos permiten esta caracteristica.

## Evaluación del Modelo

El MAE de 23.81 indica que el promedio se aleja ese valor respecto a los valores reales. el MSE indica que hay puntos de la serie de tiempo donde el error es mayor, recordemos que entre mas grande sea la diferencia entre la predicción y la real se penaliza mas el error. el MAPE indica un error porcentual del 13%. el R² de 0.88 es un valor cercano a 1, lo que indica que el ajuste es bueno y el modelo tiene buena explicabilidad respecto a las variabilidades lineales (multivariables) del modelo.

## Conclusiones y Recomendaciones

El modelo es una red neuronal de 4 capas (2 LSTM) con 117.619 parámetros. Tenemos un error porcentual del 13%, a consideración una muy buena aproximación para ser el primer experimento. Aún no se han aplicado técncias adicionales de proprocesamiento de los datos, no se han modificado hiperparámetros y tampco se ha probado una red de mayor complejidad, por lo tanto para ser el primer modelo, considero que funciona de manera correcta.

Se recomienda explorar técnicas de proprocesamiento de datos, modificar hiperparamétros o probar redes mas grandes o robustas.

## Referencias

- https://www.tensorflow.org/api_docs/python/tf/keras/layers/LSTM

- https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_absolute_error.html#sklearn.metrics.mean_absolute_error

- https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_squared_error.html#sklearn.metrics.mean_squared_error

- https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_absolute_percentage_error.html#sklearn.metrics.mean_absolute_percentage_error

- https://scikit-learn.org/stable/modules/generated/sklearn.metrics.r2_score.html#sklearn.metrics.r2_score
