# ML Test de Noviazgo

## Introduccion

El gobierno de la ciudad de Buenos Aires a traves del portal [data.buenosaires.gob.ar](https://data.buenosaires.gob.ar/) facilita la busqueda, acceso y descubrimiento a los datos que produce la ciudad, tambien incentiva la generacion de valor con los mismos. En este sentido, se disponibilizan el dataset [Test de Alerta sobre un noviazgo violento](https://data.buenosaires.gob.ar/dataset/test-alerta-sobre-noviazgo-violento) que contiene respuestas anonimas a una encuesta que busca concienciar a las personas respecto relaciones que pueden tender hacia la violencia. Esta encuesta esta compuesta por 13 preguntas que se pueden consultar en el [github del gobierno de la ciudad](https://github.com/datosgcba/test_alerta_noviazgo_violento). En este trabajo implementamos y presentamos un clasificador que puede predecir la respuesta de la pregunta 13 utilizando el resto de las preguntas, con la posibilidad de que en futuros trabajos se pueda enriquecer el clasificador con mas datos.

Para implementar este clasificador, escogimos la metrica de AUC como guia a la hora de escoger el modelo, tanto para hyperparameter tuning como para la evaluacion entre distintos modelos. La metrica de AUC nos permite ver el performace general tomando distintos umbrales de decision, estos ultimos no son parte de este proyecto.

## Motivación

Los datasets presentes en [data.buenosaires.gob.ar](https://data.buenosaires.gob.ar/) resultan de suma importancia para el análisis de problemáticas sociales en la Ciudad de Buenos Aires, entre ellas, la violencia de parejas. En la pandemia, diferentes medios, revistas y canales de televisión hicieron énfasis en el recrudecimiento de este tipo de violencia exacerbada en un contexto de encierro inusual para la sociedad toda, donde problemas tales como el hacinamiento o los problemas de infraestructura estuvieron presentes en numerosos hogares de la Capital.

Poder trabajar con estos datos es, además de una posibilidad enorme de analizar una problemática presente en muchos hogares porteños, un puntapié para la formulación de nuevas preguntas. La existencia de trabajos previos, señalados a continuación, nos da la pauta que es un tema ya revisado y estudiado, pero que sin embargo, y a pesar de no ser especialistas, nos convoca como ciudadanos. 

## Resultados de la exploración de datos

### Barrios de las personas encuestadas

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/barriosdelosencuestados.png)

### Género de las personas encuestadas

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/generoencuestados.png)

### Outliers de edad

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/outliersedad.png)

### Densidad de población por Comuna

![] (https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/map.png)

### Encuestas completas por Comuna

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/encuestascompletasporcomuna.png)

### Porcentaje de mujeres por Comuna

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/porcentajedemujeresporcomuna.png)

### Promedio de edad de varones que completaron la encuesta por Comuna

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/promediodeedaddevaronesquecompletaronlaencuesta.png)

### Promedio de edad de mujeres que completaron la encuesta por Comuna

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/promediodeedaddemujeresquecompletaronlaencuesta.png)

## Resultados

### True Positive Rate vs False Positive Rate

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/tpr-vs-fpr.png)

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/matrixconfusion.png)

### ROC Curve

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/roc-auc-final.png)

![](https://github.com/cnexans/ml-test-noviazgo/blob/master/Imagenes/ROC%20AUC.png)

## Equipo

* [David G. Nexans](https://github.com/cnexans)
* [Guido Mitolo](https://github.com/guidomitolo)
* [Thomas Artopoulos](https://github.com/thomasartopoulos)
* [Jonatan Smith](https://github.com/John31991)


## Trabajos previos

Existen diversidad de trabajos previos relacionados con este, en primera instancia [el test en si mismo](https://data.buenosaires.gob.ar/dataset/test-alerta-sobre-noviazgo-violento) y otros que listamos a continuacion:

* [Noviazgos violentos en la Ciudad de Buenos Aires, 2019](https://datosgcba.github.io/curso-datos/trabajos/noviazgos.html)
* [¿En qué barrios las mujeres sufren más violencia en sus noviazgos?, 2018](https://blog.properati.com.ar/en-que-barrios-las-mujeres-sufren-mas-violencia-en-sus-noviazgos/)



