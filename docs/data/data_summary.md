# Reporte de Datos

Este documento contiene los resultados del análisis exploratorio de datos.

## Resumen general de los datos

Hay un total de 2647, entre 1ro de enero de 2015 hasta el 31 de marzo del 2022. Se tienen 6 columnas:

  - Fecha: Variable de tipo datetime.
  - Agua: Variable númerica.
  - Carbón: Variable númerica.
  - Gas: Variable númerica.
  - Líquidos: Variable númerica.
  - Precio bolsa: Variable númerica.

No hay datos faltantes, en todas las fechas se tiene registros.

Distribución estadisticas de las variables:

![image](https://github.com/FaSaSu20/MLD6_Proy/assets/65478386/aeebb165-a86c-453b-a15b-3228c39619b2)

## Resumen de calidad de los datos

No hay valores faltantes. Los valores extremos se identifican en la tabla anterior. Tampoco existen duplicados, ni inconsistencias ni errores evidentes. Por lo tanto la calidad de los datos es buena.

### Relación entre variables explicativas y variable objetivo

## Variable objetivo & Variables individuales

La siguente serie de tiempo evidencia el comportamiento de las variables individuales y su relación con la variable objetivo, se observa que el agua se comporta muy cerca a la variable objetivo.

![image](https://github.com/FaSaSu20/MLD6_Proy/assets/65478386/da384c03-e392-45e1-b0e8-0b53c7020ddc)

## Ranking de variables

El siguiente mapa de calor de correlación, muestra la relación entre las variables indivudales y su relación con la variable objetivo, se evidencia que el agua tiene una correlación positiva alta y el gas y el liquido una correlación negativa.

![image](https://github.com/FaSaSu20/MLD6_Proy/assets/65478386/6cdff55a-7189-4667-a0b1-57cc741108a5)

No se uso ningún método de extracción de características ni de trasnformación de datos.
