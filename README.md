![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)

# **PROYECTO INDIVIDUAL Nº3**

### Marco de trabajo 

Este proyecto fue propuesto dentro de la estaoa de Labs del bootcamp de Henry, con el objetivo de hacer un ***Análisis de datos*** en base a una problemática planteada. El tiempo de preparación y entrega del proyecto fue de apróximadamente 72hs.

## **Contexto**
La **Organización de Aviación Civil Internacional (OACI)**, organismo de la Organización de las Naciones Unidas, quiere investigar en profundidad los accidentes producidos desde inicios del siglo XX. Para ello, les solicita la elaboración de un informe y un dashboard interactivo que recopile tal información. 

La OACI únicamente cuenta con un dataset sobre datos de accidentes de aviones, pero insta a la consultora de datos -de la que forman parte- que intente cruzar esta información con otras fuentes de su interés. Esto con el objetivo de obtener mayor claridad y consistencia en los fundamentos del estudio.

## **Que encontraran en el repositorio**

+ Dataset original llamado AvvidentesAvions
+ EDA del dataset provisto junto con sus pertinentes transformaciones para el análisis en main.ipnb
+ Un reporte de calidad y diccionario de datos 
+ Archivo .sql creado en la base de datos. Dicha información se consume en tiempo real por power BI
+ Dos dataset adiccionales, Entregas y Pedidos. Se muestran la cantidad de aviones pedidos y entregados de los dos fabricante comerciales más importantes

Stack tecnológico:

+ `Python`: EDA + transformaciones 
+ `SQL`: base de datos
+ `Power BI`  análisis de datos
+ `GitHub`: control de versiones


## ** Pasos del proyecto **

Se hizo un primer acercamiento al dataset con Python. Creando un notebook que contiene un análisis exploratorio, transformaciones y el preprocesamiento pertinentes. El notebook .ipynb se encuentra documentado en cada línea para una mejor comprensión. 

Luego se hizo una búsqueda de distintos enfoques. Luego de leer mucho, se llegó a la conclusión que nos vamos a centrar sólo en aviones comerciales. Se encontrö un dataset que proveé información de los dos competidores más grandes de fabricación de este tipo de aviones: Boeing y Airbus. Se trabajará el análisis con dicho enfoque. 

Para trabajar los datos de forma fácil, se ingestaron en tablas a tráves de MySQL

##### Elección de herramientas y solución de problemas #######

En principio se intentó trabajar con la versión gratuita de Looker (ex google data studio). El problema es que la versión gratuita sólo permite cargar una tabla de gestores SQL. Se plantea la posibilidad de trabajar con una tabla principal y cosumimr las otras convertidas a CSV directamente. El siguiente problema es que la base de datos debe poder ser conectada de forma remota. Se investigaron algunas alternativas como Heroku y Firebase pero tienen un límite de almacenamiento.

Por esto se procede a utilizar Power BI, que es una herramienta muy potente pero su versión gratuita no permite compartir dashboard online cömo lo hace Looker. 

Power BI presentó algunos problemas de conección con MySQL, dado un fallo genral en el conector de MySQL. Se probó con Postgress y no hubo problemas de conexión.
- - -

## ***Conclusiones finales***

Se han visto distintos enfoques en los aún se puede investigar más. Por el tiempo en el que se requiere este informe, no hubo posibilidad de hacerlo y se recomienda seguir abordando el tema con más herramientas para un mejor análisis. 


