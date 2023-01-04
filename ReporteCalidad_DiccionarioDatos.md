 >Reporte de calidad y diccionario de datos

* REPORTE DE CALIDAD

Al realizar el proceso de ETL con el csv descargado de la **ENACOM** se evidencio al realizar el EDA que el dataset recibido debia ser normalizado en algunas de las columnas (dimensiones), el archivo se descargo de la fuente en un tipo .csv y el delimitador mantenia la coherencia de los datos y todas las dimensiones contaban con la misma cantidad de datos</br>

En este caso el dataset no contaba con valores faltantes, ni valores duplicados por lo cual no se realizo ningun tipo de normalización en el dataset para estas problematicas</br>

El dataset contaba con valores que parecian atipicos con respecto a los demas datos, al analizarlos y visualizarlos se evidencio que estos valores aunque representaban una anormalidad, no generaban tanto ruido con respecto a los demas y que al momento de hacerles un manejo o corrección se podria perder valores de gran importancia para el analisis e investigación del caso. </br>

En la columna 'Acceso por cada 100 hogares' los valores tenian una ',' y esto ocasionaba un error al hacer la conversión al tipo de dato que corresponde, el manejo dado a este problema fue reemplazar ese caracter por un '.' sin afectar el dato y su formato. </br>

El tipo de dato en las columnas 'Provincia', 'Año', y 'Acceso por cada 100 hogares' fue cambiado ya que estas columnas venian con un tipo de dato que no correspondia al dato que almacenaban

No se realizo el descarte de ninguna columna ya que todas revelaban información importante para el analisis de los datos, la resolución de las incognitas propuestas y la investigación a realizar con estos </br>

* DICCIONARIO DE DATOS

Columna 1 : Año
* Descripción: Año de la toma de información sobre el acceso a internet fijo
* Tipo: String

Columna 2: Trimestre
* Descripción: Trimestre perteneciente al año de la toma de información sobre el acceso a internet fijo
* Tipo: int

Columna 3: Provincia
* Descripción: Provincia donde se tiene acceso a internet fijo
* Tipo: String

Columna 4: Acceso por cada 100 hogares
* Descripción: Cantidad hogares con acceso a internet fijo 
* Tipo: Float


