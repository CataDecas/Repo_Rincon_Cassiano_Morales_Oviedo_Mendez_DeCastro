<h1 align="center">Grupo 7 - Algoritmos 2022-1</h1>
<p align="center"><strong>Laboratorio 5</strong> </p>
<br>

<p>El laboratorio 5 consistió en maximizar una función no lineal a partir de algoritmos genéticos.
<br>
  
<p>
<h2>Requerimientos:</h2> <br>
✅ Parámetros: Tamaño_genoma_Individuos, Tamaño_población, Probabilidad_Mutación, Generaciones, Función_a_Optimizar, Rango_de_Busqueda.<br>
✅Calculo y graficado de Error promedio de la población actual, en función de las generaciones. <br>
✅Almacenamiento y graficado del mejor individuo por generación. <br>
<br>
</p>
<p>
<h2>📌 Problemas planteados: </h2> <br>
  <h2>1. ¿Como influyen diferentes parametros en el tiempo de ejecucion? </h2><br>
  Solución: <br>
  📍 Parámetro Genoma:<br>
  - Para parametro genoma 10 > 0:00:00.906180 <br>
  - Para parametro genoma 100 > 0:00:05.961513 <br>
  - Para parametro genoma 1000 > 0:01:01.429062 <br>
  - Para parametro genoma 2000 > 0:02:05.462562 <br>
  <br>
   📍 Parámetro Tamaño Población:<br>
  - Para parametro tamaño poblacion 10 > 0:00:00.129723  <br>
  - Para parametro tamaño poblacion 100 > 0:00:01.209316  <br>
  - Para parametro tamaño poblacion 1000 > 0:00:15.966701  <br>
  - Para parametro tamaño poblacion 2000 > 0:00:25.712003  <br>
  <br>
   📍 Parámetro Probabilidad de Mutación:<br>
  - Para parametro probabilidad de mutacion 0.01 > 0:00:01.212672 <br>
  - Para parametro probabilidad de mutacion 0.1 > 0:00:01.339554 <br>
  - Para parametro probabilidad de mutacion 0.5 > 0:00:02.343851 <br>
  - Para parametro probabilidad de mutacion 0.8 > 0:00:03.183847 <br>
  - Para parametro probabilidad de mutacion 1 > 0:00:03.867119 <br>
  -  <br>
   📍 Parámetro Generaciones:<br>
  - Para parametro generaciones 10 > 0:00:00.124242 <br>
  - Para parametro generaciones 100 > 0:00:01.226541 <br>
  - Para parametro generaciones 1000 > 0:00:11.809732 <br>
  - Para parametro generaciones 2000 > 0:00:22.985334 <br>
  -  <br>
   📍 Parámetro Rango de Busqueda:<br>
  - Para parametro rango de busqueda [0, 1] > 0:00:01.130410 <br>
  - Para parametro rango de busqueda [0, 2] > 0:00:01.140615 <br>
<h2>2. Análisis de la complejidad del logarítmo:</h2><br>
  Al hacer un analisis de complejidad del algoritmo, la complejidad simplificada que se obtiene es de O(n^3).<br>
  Aunque, especificamente, la complejidad del algoritmo en funcion de sus parametros podria describirse como: O(Generaciones⋅TamañoPoblacion⋅LongitudDelGenoma).<br>
<h2>3. ¿Qué parámetro es más relevante para acelerar la convergencia de la búsqueda?</h2> <br>
  Para acelerar la velocidad de convergencia, los tres parametros mas importantes a disminuir son la cantidad de generaciones, el tamaño de la poblacion, o el tamaño del genoma. Aunque cabe resaltar que a pesar de que la velocidad de convergencia sera menor, tambien puede hacer que la busqueda sea menos precisa, ya que a medida que es mayor el valor de dichos parametros, el algoritmo prueba mas posibilidades de individuos, lo cual puede llevar a encontrar una mejor solución.
<br>
</p>
<br>
<h2>Integrantes del grupo</h2>

Luis Fernando Mendez Marques | <a href = "mailto: lumendezm@unal.edu.co" target="_blank">Email</a>
Santiago Cassiano Rozo | <a href = "mailto: scassiano@unal.edu.co" target="_blank">Email</a>
juan Esteban Oviedo Garcia | <a href = "mailto: joviedog@unal.edu.co" target="_blank">Email</a>
Juliana Catalina De Castro Moreno | <a href = "mailto: jdec@unal.edu.co" target="_blank">Email</a>
Ivan Alexander Morales Muñoz | <a href = "mailto: imorales@unal.edu.co" target="_blank">Email</a>
Nicolas Mauricio Rincon Vija | <a href = "mailto: nrinconv@unal.edu.co" target="_blank">Email</a>

<h6>Ingeniería de Sistemas y Computación</h6>
<h6>Universidad Nacional de Colombia</h6>
