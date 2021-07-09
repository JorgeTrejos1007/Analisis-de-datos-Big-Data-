### **Jorge Mario Trejos Barquero.**
### **B77676.**

#### **Resumen**

En estas últimas dos semanas se han visto múltiples temas, empezando con métodos de evaluación de resultados mencionando que si tenemos ground-truth entonces debemos usar métodos extrínsecos y si no tenemos ground-truth entonces debemos usar métodos intrínsecos. A continuación se vio el método de evaluación de silhuette, tiene de formula:

si = (bi-ai)/max(bi,ai)

1. Si el resultado es positivo, es que la asignación es buena.
2. Si el resultado es negativo, es que la asignación es mala.
3. Si el resultado es cercano a 0, asignación débil.

Podemos sacar el promedio de estos resultados para ver la evidencia de si estos clusters realmente existen:

1. Si x >= 0.5 buena evidencia.
2. Si 0.25 < x < 0.5 evidencia regular.
3. Si x <= 0.25 evidencia débil.

Luego se vio "self organising mal" (SOM) el cual es una técnica de segmentación y visualización basada en redes neuronales sin ser una, es un método no supervisado, se suele usar para reducción de dimensionalidad, es del tipo grid-based clustering e impone un orden topo-lógico a los centroides.

El algoritmo en pseudocódigo es:

1. Inicializa centroides
2. repetir
3. seleccione siguiente objeto
4. seleccione el centroide más cercano
5. actualiza los centroides
6. hasta que los centroides no cambien
7. asigne los objetos a su centroide y retorne clusters y centroides

Ahora se empezó con el tema de análisis de flujo de datos donde hay 2 categorías:

1. Batch processing: Almacenados en bases de datos, datos estáticos y las decisiones no tienen efecto inmediato
2. Stream processing: Datos de alto volumen y que cambian muy rápido, procesar sin almacenar datos, procesamiento en tiempo real y no es posible esperar a que un algoritmo de machine learning entrene para usarlo.

Tiene dos aspectos el stream processing: Cardinalidad (bounded, unbounded) y construcción (tablas y streams). Hay 3 clasificaciones según que tanto tiempo tarden:

1. Hard: micro-segundos - mili-segundos.
2. Soft: mili-segundos - segundos.
3. near: segundos - minutos.

Se vieron algunos algoritmos/estrategias para streaming tales como:

1. Time agnostic: Que puede ser filtering o inner joins.
2. Approximation: Que puede ser top-n o streaming k-means.
3. Windowing: Que puede ser fixed, sliding o sessions.
4. Windowing by event time.
5. Tumbling window (agrupa por cantidad y no por tiempo).

Ahora se vieron filtros, cuya lógica es que dejan pasar ciertos datos y retiene otros, o sea, es de selección, puede ser de membresía simple o compleja. Se vio el filtro de bloom el cual consiste en un arreglo binario inicializado en ceros y k funciones hash donde cada datos que se quiere meter al arreglo pasa por las k funciones hash y cambian ciertos valores del arreglo, esta es la lista blanca, datos que se aceptan. Al final la lógica consiste en que si un nuevo dato coincide con puros 1's en el arreglo después de pasar por las funciones hash este dato es aceptado, pero si al menos un valor que sale de una función hash cae en una casilla del arreglo que contiene un cero entonces se niega el dato y no pasa por el filtro.

Finalmente, se vieron tipos de análisis para streaming:

1. Filtros.
2. Enriching.
3. Aggregation.
4. Event detection.

#### **Aprendido**
Todo lo que se vio en estas 2 semanas es conocimiento nuevo ya que nunca había escuchado o visto estos temas.

#### **Dudas**
Ninguna de momento, todo va quedando bastante claro.

#### **Uso en el futuro**
Un ejemplo sería con el filtro de bloom que es algo que se puede usar en bases de datos NoSQL incluso varias bases de datos ya lo tienen implementado tales como Cassandra. Además, es una forma de crear filtros bastante usada en el mundo de la computación lo cual puede ser útil conocer para el futuro.

#### **Material extra**
No se consultó ninguna clase de material extra para el entendimiento de estos temas.