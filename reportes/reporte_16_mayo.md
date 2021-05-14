### **Jorge Mario Trejos Barquero.**
### **B77676.**

#### **Resumen**
Estas dos semanas de clases empezaron con el tema de los árboles de decisión y sus tipos tales como binarios, nominales categóricos, nominales ordinales, etc. También los tipos de atributos que pueden ser binarios, en umbrales o por rangos, y que los árboles de decisión también pueden sufrir de problemas tales como overfitting y underfitting.

Ventajas de los árboles de decisión:
1. Simples.
2. No sensible a falta de datos.
3. Son numéricos y categóricos.
4. Tienen un entrenamiento eficiente.
5. Previene el overfitting con algunos parámetros.

Desventajas de los árboles de decisión:
1. Sensible a cambios en el dataset
2. Puede llegar a hacerse un árbol muy grande.
3. Más profundidad usualmente es igual a más efectivo pero esto es menos entendible.
4. Se tiende al overfit ya que, aunque hayan parámetros para evitarlo igual se tiende a hacer overfit.

Luego se habló de los random forest los cuales son muchos árboles que se usan para dar resultados distintos y sacar una media de ellos por ejemplo. Estos se construyen por selección de observaciones (filas) o por selección de atributos (columnas), además pueden ser con reemplazo o sin reemplazo.

Ventajas de un random forest:
1. Da mejores resultados que un solo árbol de decisión.
2. Reduce las probabilidades hacer overfit.
3. Es paralelizable entre los procesadores que se dispongan para poder ejecutar el código.

Desventajas de un random forest:
1. No son fáciles de interpretar.
2. Tienen un entrenamiento lento.
3. No funciona con datos dispersos.

Gradient boosting consiste en poner los arboles de decisión de forma serial (uno detrás de otro), con esto se busca que cada árbol corrija el error del anterior, suelen ser árboles pequeños llamados weak learner y como desventajas tienen que son más sensibles a parámetros y el training es muy lento.

Ahora se habló de cross validation el cual consiste en dividir un dataset en splits y folds, también se conoce como k-fold y de este se derivan muchos otros métodos tales como:

1. Stratified k-fold.
2. Leave one out (LOOCV)
3. Shuffle split
4. Con grupos
5. Repeated stratified k-fold

De estos métodos se puede mencionar que hay más aún y que cada uno funciona en una situación diferente, es por esto que tenemos que realizar un análisis de los datos antes de elegir uno de estos métodos mencionados, por ejemplo: En caso de que haya varios datos con un mismo origen se usa "Con grupos" (es usado sobre todo en el área de médica o medicina).

Finalmente, se habló sobre grid_search el cual es un método que busca los parámetros óptimos para hacer cross validation y del método nested cross validation, el cual hace todo el proceso de primero encontrar los parámetros óptimos y luego corre el cross validation.

#### **Aprendido**
En general todo lo visto en estas semanas es conocimiento nuevo y que se me hace súper interesante. Se había investigado un poco sobre los métodos de k-fold pero no estaba claro como funcionaban, pero ya ahora habiéndolo visto en clase ya quedó claro.

#### **Dudas**
Ninguna, todo sobre estos temas se entendió bien, además de que ya anteriormente se había investigado un poco de estos temas.

#### **Uso en el futuro**
Es posible usar estos temas para realizar estudios predictivos sobre como mejorar un servicio de TI basado en las experiencias de usuario que existan por ejemplo, que sea un modelo que pueda ser predictivo hace que su uso sea muy amplio y flexible a muchos ámbitos. Ninguna, todo sobre estos temas se entendió bien, además de que ya anteriormente se había investigado un poco de estos temas.

#### **Material extra**
No se consultó ninguna clase de material extra para el entendimiento de estos temas.