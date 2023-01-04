![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png) 

# PROYECTO INDIVIDUAL III

## Descripción del proyecto: </br>  
En este proyecto realizaremos un EDA (Análisis Exploratorio de Datos) sobre un dataset que tiene información sobre el sector de telecomunicaciones en Argentina desde el año 2014, hasta el año 2022. </br>

Nuestro dataset de trabajo original sera 'Internet_Penetracion.csv' pero usaremos datasets adicionales para complementar el analisis y la investigación del sector de telecomunicaciones en Argentina.</br>

A estos cuatro datasets adicionales no se les realizara una transformaciòn en python, dentro de power bi vamos a ir adecuando y limpiando estos datasets, para adecuarlos a nuestro modelo de negocios.

Dividiremos el proyecto en diferentes fases que nos permitiran realizar correctamente el EDA, adicional a esto realizaremos un reporte de calidad de los datos que nos permitira informar el estado en el cual recibimos los datos y que manejo le dimos a estos, un diccionario de datos donde especificaremos la informacion que almacena cada dimension, y su tipo de dato, y por ultimo realizaremos un dashboard interactivo donde evidenciaremos los diferentes analisis que se realizaron en la investigación.</br>

Principalmente vamos a estar evaluando el siguiente KPI: El aumento o disminución de la variación porcentual trimestral del servicio de internet, cada 100 hogares por provincia.

https://datosabiertos.enacom.gob.ar/home <---- Datasets obtenidos de esta pagina 


## Descripción del dataset de origen: </br>
Internet_Penetracion.csv : Contiene 4 dimensiones y 792 registros.</br> 
Nuestro dataset contiene la siguiente información sobre el sector de telecomunicaciones especificamente internet fijo banda ancha en Argentina por cada provincia en el periodo(2014- 2022) por cada 100 hogares

## Descripción de las dimensiones del dataset de origen: </br> 

+  Año: Año de la toma de información
+  Trimestre: Trimestre perteneciente al año de la toma de información
+  Provincia: Lugar de la toma de información
+  Accesos por cada 100 hogares: Valor numerico que indica la cantidad de acceso por hogar 

## Fases de realización del proyecto

1. Carga de los datasets
2. EDA (Análisis Exploratorio de Datos)
    + Transformación y limpieza de los datos
    + Resumen estadistico
    + Distribuicion de frecuencia
    + Boxplots
    + Correlación
3. Realizacion del reporte de calidad y diccionario de datos    
4. Creacion del dashboard interactivo

Frameworks usados
+ `Python`: EDA 
+ `Power BI`: dashboard 
