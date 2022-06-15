<h1 align="center">Grupo 7 - Algoritmos 2022-1</h1>
<p align="center"><strong>Laboratorio 6</strong> </p>
<br>

<p>El laboratorio 6 consistió en crear un perceptron que pudiera clasificar entre dos clases de uva (Kecimen y Besni)</p>
<p>Para realizar el laboratorio se uso el dataset Raisin, el cual incluye datos sobre 2 variedades de uvas pasas (Kecimen y Besni). El Dataset contiene 900 registros, de los cuales la mitad corresponden a uvas Kecimen y la otra mitad a uvas Besni. Cada registro contiene los siguientes datos:
Area, Perimeter, MajorAxisLength, MinorAxisLength, Eccentricity, ConvexArea, Extend y Class (Kecimen, Besni).

En este caso solo se utilizaron los datos MajorAxisLength y Extent como datos de entrada del perceptron, a partir de ellos se intento clasificar las uvas como tipo Besni o Kecimen.

El dataset esta disponible en https://archive.ics.uci.edu/ml/datasets/Raisin+Dataset</p>
<br>
<p>
<h2>Requerimientos del programa:</h2>
✅ Parámetros del Perceptron: eta (tasa de aprendizaje defualt = 0.1), n_iter número de iteraciones que se realizan en el entrenamiento,
x cantidad de registros y numero_caracteristicas es la cantidad de características de un registro.<br>
✅ Graficas de los datos de cada clase de uva. (Disponibles en el archivo Lab6.ipynb)<br>
✅ Calcular error del perceptron en la clasificación (51%).<br>


<h2>Analisis de complejidad especifica y generalizada</h2>
<p> 
Analisis de complejidad especifica: O(n_iter) * O(x) * O(numero_caracteristicas)

El proceso de mayor complejidad durante la ejecución del programa es el entrenamiento del perceptron, es decir, la ejecución del metodo train() en la clase Perceptron.

Entonces el metodo train() es el que determina la complejidad del programa. La complejidad de dicho metodo se puede representar en terminos de los parametros de entrada como O(n_iter) * O(x) * O(numero_caracteristicas)

Es decir que la complejidad de este metodo depende principalmente de 3 valores:

**n_iter:** Este valor representa la cantidad de iteraciones que se realizaran en el entrenamiento. Si unicamente se incrementa el valor de **n_iter**, el tiempo de ejecucion del programa incrementara linealmente acotado por O(n_iter).

**x:** Este valor representa la cantidad de registros que se utilizaran para entrenar el perceptron. Si unicamente se incrementa el valor de **x**, el tiempo de ejecucion del programa incrementara linealmente acotado por O(x).

**numero_caracteristicas:** Este valor representa la cantidad de caracteristicas que tiene cada registro que se usa para entrenar el perceptron, en el caso del perceptron utilizado en el laboratorio son 2 (MajorAxisLength y Extent). Si unicamente se incrementa el valor de **numero_caracteristicas**, el tiempo de ejecucion del programa incrementara linealmente acotado por O(numero_caracteristicas).

Cabe resaltar que el perceptron tambien recibe otro paramentro de entrada el cual es **eta** que representa el valor de la tasa de aprendizaje del perceptron, pero dicho valor no afecta en la complejidad del programa al solo ser usada como una constante en las operaciones de entrenamiento.

Si se generaliza la complejidad del programa obtenida en la anterior seccion, se obtiene que el programa tiene una complejidad de O(n^3), es decir que si se incrementan al tiempo los parametros **n_iter**, **x** y **numero_caracteristicas** el tiempo de ejecución del programa puede crecer en gran medida.
</p>


<h2>Analisis de los resultados en función de la separabilidad de los datos</h2>
<p>
En el dataset utilizado, las dos caracteristicas tomadas (MajorAxisLength y Extent) no son lo suficientemente distinguibles entre las uvas Kecimen y las uvas Besni como para que el perceptron pueda clasificarlas. 

Los datos de las Uvas Kecimen y Besni no son separables, esto se puede observar cuando se graficaron las uvas en funcion de las caracteristicas MajorAxisLength y Extend las uvas eran muy parecidas entre si y sus puntos se ubicaban en casi la misma region. (Graficas disponibles en el archivo Lab6.ipynb)

Ademas puede observar que en todas las iteraciones en el entrenamiento el perceptron comete muchos errores (entre 345 y 348) lo cual hace que actualice muchas veces su pesos, y se puede observar que no hay una tendencia a que la cantidad de errores disminuya, ya que es muy dificil distinguir los dos tipos de uvas a pesar del entrenamiento.

Es por ello que el perceptron tiene un porcentaje de error alto del **51**% al realizar las pruebas, las uvas son muy parecidas entre si, entonces el perceptron no puede ajustar los pesos de sus conexiones para poder distinguirlas y se equivoca al intentar clasificarlas.
</p>

<h2>Referencias</h2>

*   https://web.archive.org/web/20190213060442/https://www.llipe.com/2017/04/19/programando-un-clasificador-perceptron-en-python/

*   https://machinelearningmastery.com/standard-machine-learning-datasets/

*   https://archive.ics.uci.edu/ml/datasets/Raisin+Dataset

<h2>Integrantes del grupo</h2>

Luis Fernando Mendez Marques | <a href = "mailto: lumendezm@unal.edu.co" target="_blank">Email</a>
Santiago Cassiano Rozo | <a href = "mailto: scassiano@unal.edu.co" target="_blank">Email</a>
juan Esteban Oviedo Garcia | <a href = "mailto: joviedog@unal.edu.co" target="_blank">Email</a>
Juliana Catalina De Castro Moreno | <a href = "mailto: jdec@unal.edu.co" target="_blank">Email</a>
Ivan Alexander Morales Muñoz | <a href = "mailto: imorales@unal.edu.co" target="_blank">Email</a>
Nicolas Mauricio Rincon Vija | <a href = "mailto: nrinconv@unal.edu.co" target="_blank">Email</a>

<h6>Ingeniería de Sistemas y Computación</h6>
<h6>Universidad Nacional de Colombia</h6>
