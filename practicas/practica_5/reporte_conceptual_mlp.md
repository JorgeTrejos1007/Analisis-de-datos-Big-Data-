### **Jorge Mario Trejos Barquero.**
### **B77676.**

#### **Resumen** 
Primero se habló de los multi layered perceptrons los cuales en el fondo son los mismo que una red neuronal, se dijo que un perceptron es el equivalente a una neurona. Una neurona tiene: una salida, una función de activación y n entradas con un peso cada una de ellas. Los pesos de las neuronas son incializados con valores pequeños, entre 0 y 0.3. 

Luego se habló de la redes nuronales la cuales se componen de: input layer, output layer y n capas ocultas (hidden layers) con n neuronas cada capa. El tipo de función de acticación que vaya a tener la output layer dependera directamente del estilo de análisis que se este haciendo.

Ahora se habló de entrenar la red una vez ya está hecha esta misma. Preparar la data es lo primero que tenemos que hacer antes de empezar a entrenar la red, hay que convertir datos a numericos mediante codificaciones para poder usarlos en el entrenamiento. El metodo normalmente para entrenar la red es el de Stochastic Gradient Descent donde se pasa una a una las lineas del dataset y al final produce un output, este se compara con el output esperado para calcular el error y entonces poder recalcular los pesos (este calculo de los pesos se puede actualizar apenas se realiza una comparacion de la salida obtenida con la salida esperada o se puede realizar hasta el final, a esto se le conoce como batch learning). Finalmente, una vez entrenada la red, ya se puede usar para que pueda realizar predicciones.

#### **Aprendido**
Todo lo que se vio en este primer tutorial es nuevo ya que no se tenia conocimientos previos de como funcionaba una red neuronal.

#### **Dudas**
¿Como se re-calculan los pesos de la red? Esta duda me surge ya que en teoría se compara un output y un input, ¿entonces como sé que partes de la red debo re-calcular? y si la re-calculo toda, ¿como se si debo aumentar o disminuir los pesos de cada una de las neuronas? 