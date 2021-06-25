### **Jorge Mario Trejos Barquero.**
### **B77676.**

#### **Resumen**
En estas 2 semanas empezamos a ver el tema de la segmentación más específicamente clustering, del cual se dijo algunas de sus características, tales como:

1. Busca dividir el dataset en grupos.
2. Crea clases o grupos que comparten características en común.
3. Necesita una métrica de similitud.
4. Necesita que se codifiquen atributos categóricos.
5. Necesita que se transformen los atributos numéricos.
6. En algunos casos hay que decir cuantos cluster se quieren.

Existen 4 tipos: partition (k-means), hyerarchical (BIRCH), density-based (DBSCAN, OPTICS, DENCLUE, etc) y grid-based (STING, CLIQUE, etc).

Lo siguiente que se hizo fue hablar en profundidad sobre k-means, se dijo que sus inputs son: "K" que es el numero de clusters buscados y un "D" que es el dataset; de output tenemos los "K" clusters ya creados.

El algoritmo lo que hace es:

1. Seleccionar lo k centroides iniciales aleatoriamente.
2. Formar k cluster asignando los diferentes puntos a el centroide más cercano.
3. Re-calcular el centroide de cada cluster.
4. Repetir paso 2 y 3 hasta que ya no cambien los centroides.

Limitantes:

1. No se sabe si el numero de k dado es el correcto.
2. Supone clusters con el mismo diámetro.
3. Supone que direcciones de los puntos son igual de importantes.
4. Cluster con forma convexa.

Luego se habló sobre los algoritmos de aglomeración, se mencionó que tiene 3 métodos: 

1. Ward: Tiende a producir clusters de tamaño similar. 
2. Average: Funciona mejor cuando los cluster tienen una cantidad distinta de elementos.
3. Comlete: igual que average.

Ahora se habló de clustering jerárquico y dendogramas, en este tipo de clustering lo que se busca es todos los posibles clusters que se pueden realizar y con los dendogramas se puede visualizar esto de manera muy sencilla. El algoritmo al cual se le dio profundidad en esta categoría fue al DBSCAN, algunas características de este algoritmo son:

1. Es lento pero funciona bien con datasets grandes.
2. No requiere de un k (cantidad de clusters) inicial.
3. Formas complejas de los clusters.
4. Puede tener puntos que no pertenecen a ningún cluster.

Requiere de 2 parámetros, uno es "min_samples" (cantidad mínima de puntos para que algo se considere como un cluster) y "eps" que es el tamaño del vecindario. Para ambos parámetros existe una forma de encontrar valores óptimos, para "min_samples" se puede hacer un factor mayor o igual 2 multiplicado por la cantidad de columnas y para "eps" se puede hacer el método del codo. Existen 3 tipos de puntos: noise, boundary, core.

Dentro de los datos que se usan para este método se busca que haya una alta dimensionalidad, suelen tener ruido y outliers, se tiene que conocer la escala de los datos, hay que conocer la dispersión, etc.

#### **Aprendido**
De k-means ya se sabía la mayoría de los puntos mencionados, aunque no todo, el resto de lo temas todo fue conocimiento nuevo y muy interesante.

#### **Dudas**
De momento ninguna, solo que me gustaría saber como se aplica esto en código, pero estoy seguro de que haremos esto más adelante.

#### **Uso en el futuro**
Algoritmos de clustering en el área de TI son muy importantes ya que sirven para realizar estudios de datos que pueden estar almacenados en data warehouses por ejemplo.

#### **Material extra**
Ninguno.