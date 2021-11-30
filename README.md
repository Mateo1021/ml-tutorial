# Solucion Taller 3
# script de forest fires:
## ¿Se desea resolver el problema utilizando aprendizaje supervisado o no supervisado? <br/><br/>
![alt text](https://github.com/Mateo1021/ml-tutorial/tree/master/img/imagen_2021-11-30_003844.png)
Se puede determinar que es un problema de aprendizaje supervisado ya que el modelo trata de hacer una predicción de los incendios teniendo en cuenta un histórico de registros de incendios que se han evidenciado y una serie de variables que puede ayudar a la predicción. 
## ¿Es un problema de clasificación o de regresión?<br/><br/>
Durante la ejecucion de problema se puede ver que se hace un proceso de regresion ademas son problemas de regresión cuando el resultado a predecir es un atributo numérico.
![alt text](https://github.com/Mateo1021/ml-tutorial/tree/master/img/imagen_2021-11-30_011826.png)
## ¿Qué interpretación le puede dar a los resultados obtenidos?<br/><br/>
Se puede evidenciar que los resultados da el error de media absoluta, con el fin de calcular las predicciones por medio de la regresion lineal. 
# recursos humanos (rrhh)
## ¿Cuál es la clase para la que el modelo más se equivoca? ¿Por qué?
#### promotion_last_5years
Ya que los datos después de hacer un describe muestra que solo toma los valores entre 0 y 1 y aun así y la gran mayoría de los datos están en 0 esto puede decir que la variable es innecesaria y se podría omitir para cualquier evaluación.
![alt text](https://github.com/Mateo1021/ml-tutorial/tree/master/img/imagen_2021-11-30_014617.png)
## ¿Cuál cree que es el propósito del parámetro max_depth usado al momento de instanciar el modelo de árbol de decisión?
El max_depth se utiliza para determinar la La profundidad máxima del árbol esto se hace con el fin de pre podar el árbol y asegurarse de que no tenga una profundidad mayor que 5
![alt text](https://github.com/Mateo1021/ml-tutorial/tree/master/img/imagen_2021-11-30_013619.png)
## Para este caso particular, ¿por qué cree que es difícil obtener un buen clasificador?
no existe una Relacion directa entre los datos y el salario ademas se puede ver que en la matriz de confusion el uncio dato que esta siendo relacionado es salario low por la gran cantidad de veces que este parametro low se repite en la variable de salary.
![alt text](https://github.com/Mateo1021/ml-tutorial/tree/master/img/imagen_2021-11-30_015236.png)
# Identificación de géneros musicales
## Para el caso binario (jazz and blues vs. soul and reggae) ¿Es posible obtener mejores métricas entrenando un modelo basado en Random Forest?
## Escoja otro par de géneros, entrene un conjunto de modelos y documente los resultados del mejor que se haya obtenido.
## Para el caso multi-clase, ¿cuál es la clase para la que el modelo más se equivoca? ¿Por qué?
## Para el caso multi-clase, el modelo basado en red neuronal parece estar mayoritariamente sesgado hacia un género particular. ¿Cuál género cree que es?

# Segmentación de cajas de compensación familiar (subsidio)
## ¿Qué cajas de compensación parecen ser mayoritariamente diferentes a las demás?
### Caja de Compensacion Familiar de Antioquia COM...
### Caja Colombiana de Subsidio Familiar COLSUBSIDIO	
### Caja de Compensacion Familiar COMPENSAR	
### Caja de Compensacion Familiar del Valle del Ca...
### Caja de Compensacion Familiar CAFAM	
Se puede ver que estas 5 cajas de compensación están en los cluster 1 y 2, estas se puede determinar que son las mas diferentes ya que no se pudo encajar dependiendo de sus características en grupos mas grandes. 
## ¿A partir de qué características utilizadas para el entrenamiento del modelo se podría explicar la razón por la que las cajas anteriores fueron agrupadas en clusters tan pequeños?
En el cluster 1 se puede evidenciar en todas las variables y en sus respectivas descripciones tiene unos valores muy atípicos comparados con los demás cluster, Por ejemplo, en la variable (Total Población Cubierta) el valor máximo es de 3455041.00 muy por encima de los máximos de los demás cluster. Además de que en ninguno de los valores tiene un 0 como promedio o mínimo valor a diferencia de los otros que tiene como valor 0 en varias variables 
## ¿Se pueden obtener resultados más homogéneos utilizando cantidades diferentes de clusters para el entrenamiento? Entienda homogeneidad como clusters con cantidades similares de instancias de datos.
NO. Ya que primero que todo la cantidad de datos en muy poca y segundo existen cajas de compensación con valores muy atípicos como las cajas que estaban en el cluste 1 al inicio del ejercicio. 
![alt text](https://github.com/Mateo1021/ml-tutorial/tree/master/img/imagen_2021-11-30_023050.png)
si se disminuyen se puede ver como almacena estas cajas con valores atípicos en un solo grupo y las demás en un grupo mas general. y si se aumenta 
![alt text](https://github.com/Mateo1021/ml-tutorial/tree/master/img/imagen_2021-11-30_023217.png) se puede ver como se mantienen estas 4 cajas de compensación con valores atípicos en grupos diferentes
