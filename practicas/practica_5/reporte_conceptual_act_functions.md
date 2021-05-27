### **Jorge Mario Trejos Barquero.**
### **B77676.**

#### **Resumen** 
Una función de activación es la forma en la que se van a sumar los valores de las entradas para producir una salida. Se mencionó que cada una de la hidden layers suelen tener la misma función de activación, mientras que la output layer suele tener una distinta que las hidden layers. Para las funciones de activación de las hidden layer se suele usar una de las siguientes funciones:

1. Rectified Linear Activation (ReLU) = max(0.0 x) Esto significa que si x es mayor a 0 retorna esta valor y si es menos retorna 0.
2. Logistic (Sigmoid) = 1.0 / (1.0 + e^-x) La función toma cualquier valor real como valores de entrada y de salida en el rango de 0 a 1. Cuanto mayor sea la entrada (más positiva), más cerca estará el valor de salida a 1.0, mientras que cuanto más pequeña sea la entrada (más negativa), más cerca estará la salida será 0.0.
3. Hyperbolic Tangent (Tanh) = (e^x – e^-x) / (e^x + e^-x) Muy parecida a la Sigmoid. 

Hace años lo más normal era usar Sigmoid para la hidden layer, en los tiempo más recientes se ha utilizado más Tanh. Uno se puede guiar de la siguiente manera para elegir que función de activación usar en la hidden layer.

1. Multilayer Perceptron (MLP): ReLU.
2. Convolutional Neural Network (CNN): ReLU.
3. Recurrent Neural Network: Tanh and/or Sigmoid.

Para la output layer se puede usar como función de activación.

1. Linear = retorna x
2. Logistic (Sigmoid) = Igual que en la hidden layer.
3. Softmax = e^x / sum(e^x) 

Para elegir que función usar uno se puede guiar con esto:

1. Regression: linear activation.
2. Binary Classification: sigmoid activation.
3. Multiclass Classification: softmax activation.
4. Multilabel Classification: sigmoid activation.

#### **Aprendido**
Nuevamente todo lo visto aquí es conocimiento nuevo que no se había visto nunca antes.

#### **Dudas**
No me quedó del todo calro como funciona la función Softmax.