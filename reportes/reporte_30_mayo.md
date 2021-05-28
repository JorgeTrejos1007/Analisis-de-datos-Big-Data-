### **Jorge Mario Trejos Barquero.**
### **B77676.**

#### **Resumen**
En estas dos semanas del curso se ha visto en profundidad el tema de la redes neuronales. 

Se empezó hablando de los modelos lineales, tanto de sus ventajas como desventajas, tales como: que no funcionan bien con poca dimensionalidad, son mejores con alta dimensionalidad, son sensibles a la escala de los atributos, etc.

Luego se habló de la regularización, que es el proceso de penalizar la complejidad de un modelo para disminuirla. Aquí se hablaron de técnicas como: costo, L1 o Lasso, L2 o Ridge y Elastic net que es una combinación de L1 y L2.

Se habló un poco de la regresión logística ya que este tema no es nada nuevo, y pasamos ahora si a hablar sobre redes neuronales, las cuales tienen varios niveles o capas de procesamiento, tiene perceptrones o neuronas y cada neurona tiene una función de activación. Estas funciones de activación son ReLU, tangente hiperbólica, identidad y sigmoidal. Estas funciones de activación que se mencionaron ya fueron explicadas a profundidad en otros trabajos como la práctica 5 asi que no entraremos en detalle de como es cada una de estas funciones, lo único importante a tener presente es que no todas estas funciones son utilizables en cada capa, hay 3 tipos de capas, la de entrada, la salida y las ocultas, para cada una de estas capas la función de activación puede ser diferente dependiendo de lo que se este haciendo.

Todo lo que se ha mencionado hasta ahora forman parte del control de complejidad, capas ocultas, numero de nodos por capa, parámetros de regularización, pesos iniciales de la red, etc. En scikitlearn existen redes neuronales de clasificación y regresión.

Ahora que se vio las partes de una red y las partes de una neurona se pasó a hablar de como entrenar una red neuronal, para esto se tiene que preparar la data, se usa stochastic gradient descent que es el método de training más común para las redes neuronales, se actualizan los pesos (este proceso se puede hacer en cada iteración del training o cada x cantidad de iteraciones) y finalmente se usa la red neuronal para hacer predicciones.

Una vez acabado y explicado el tema de las redes neuronales pasamos al tema del análisis de asociación, el cual consiste en buscar patrones de la forma a -> b, o sea, que a implica b. Este análisis se hace con datasets tabulares o transaccionales y se busca encontrar patrones para poder sacar provecho de estos, como por ejemplo: saber si es conveniente hacer una promoción de cereal y galletas en un supermercado ya que se ve que mucha gente que compra cereal también compra galletas (cereal -> galletas). Para este proceso hay que definir unas reglas las cuales se definen siguiendo estos pasos:

1. Definir la granularidad.
2. Definir las prioridades (general o detallado).
3. Encontrar itemsets frecuentes.
4. Generar reglas de asociación que satisfagan support y confidence.

Ahora se estudió el principio a priori, esto lo que nos dice es que si un itemset es frecuente todos sus subconjuntos también. Los atributos pueden ser: binarios asimétricos, binarios simétricos, categóricos, continuos, multi-dimensionales, multi-nivel y secuenciales.

Finalmente se habló de las reglas no útiles que son las actionable rules, trivial rules y inexplicable rules. Además, se mencionaron las medidas de utilidad tales como: support, confidence y lift.

#### **Aprendido**
Todo lo visto de redes neuronales es conocimiento nuevo. Respecto al análisis de asociación ya se conocía el concepto, pero no se sabía nada de medidas de utilidad.

#### **Dudas**
Ninguna, las que se tienen sobre todo del área de redes neuronales ya fueron hechas en otro trabajo.

#### **Uso en el futuro**
Se puede usar junto a almacenes de datos los cuales son transaccionales para su análisis tanto con redes neuronales como para análisis de asociación y con esto ayudar a una posible futura compañía.

#### **Material extra**
La documentación de scikitlearn sobre los métodos y librerías para hacer redes neuronales.