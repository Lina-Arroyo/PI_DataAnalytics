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
Nuestro dataset contiene la siguiente información sobre el sector de telecomunicaciones especificamente internet fijo banda ancha en Argentina por cada provincia en el periodo(2014- 2022) por cada 100 hogares. </br>
Este dataset cuenta con las siguientes dimensiones: </br>
+  Año: Año en el cual se registraron los accesos al internet fijo
+  Trimestre: Trimestre del año en el cual se registraron los accesos a internet fijo
+  Provincia: Provincia en la cual se registraron los accesos al internet fijo
+  Accesos por cada 100 hogares: Cantidad de accesos a internet fijo por hogar 

## Fases de realización del proyecto

1. Carga de los datasets
2. EDA (Análisis Exploratorio de Datos)
    + Transformación y limpieza de los datos
    + Resumen estadistico
    + Distribuicion de frecuencia
    + Boxplots
    + Correlación   
3. Creacion del dashboard interactivo
--------------------------------------------------------------------------------------

# Reporte de calidad y diccionario de datos

* REPORTE DE CALIDAD

Al realizar el proceso de ETL con el csv descargado de la base de datos abierta de **ENACOM** se evidencio al realizar el EDA que el dataset recibido debia ser normalizado en algunas de las columnas (dimensiones), el archivo se descargo de la fuente en un tipo .csv y el delimitador mantenia la coherencia de los datos y todas las dimensiones contaban con la misma cantidad de datos</br>

En este caso el dataset no contaba con valores faltantes, ni valores duplicados por lo cual no se realizo ningun tipo de normalización en el dataset para estas problematicas</br>

El dataset contaba con valores que parecian atipicos con respecto a los demas datos, al analizarlos y visualizarlos se evidencio que estos valores aunque representaban una anormalidad, no generaban tanto ruido con respecto a los demas y que al momento de hacerles un manejo o corrección se podria perder valores de gran importancia para el analisis e investigación del caso. </br>

En la columna 'Acceso por cada 100 hogares' los valores tenian una ',' y esto ocasionaba un error al hacer la conversión al tipo de dato que corresponde, el manejo dado a este problema fue reemplazar ese caracter por un '.' sin afectar el dato. </br>

El tipo de dato en las columnas 'Provincia', 'Año', y 'Acceso por cada 100 hogares' fue cambiado ya que estas columnas venian con un tipo de dato que no correspondia al dato que almacenaban

No se realizo el descarte de ninguna columna ya que todas revelaban información importante para el analisis de los datos, la resolución de las incognitas propuestas y la investigación a realizar con estos </br>

El dataset contaba con los siguientes tipos de datos: Int64(2), object(2) y ocupaba la siguiente cantidad espacio en memoria: 24.9+ KB </br>


* DICCIONARIO DE DATOS

Columna 1 : Año
* Descripción: Valor numerico que representan el año en el cual se registraron los accesos al internet fijo
* Nulos: 0
* Duplicados: 0
* Tipo: String

Columna 2: Trimestre
* Descripción: Valor numericos que representan el trimestre del año en el cual se registraron los accesos a internet fijo
* Nulos: 0
* Duplicados: 0
* Tipo: int

Columna 3: Provincia
* Descripción: Valor cualitativo que representa la provincia en la cual se registraron los accesos al internet fijo
* Nulos: 0
* Duplicados: 0
* Tipo: String

Columna 4: Acceso por cada 100 hogares
* Descripción: Valor numerico que representa la cantidad hogares con acceso a internet fijo 
* Nulos: 0
* Duplicados: 0
* Tipo: Float

Frameworks usados
+ `Python`: EDA 
+ `Power BI`: dashboard 
