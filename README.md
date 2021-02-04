# Keras rede neural WEIGHT REGULARIZATION

Neste Notebook estudaremos como reduzir o **sobreajuste de uma rede neural de aprendizado profundo** usando a **regularização de peso**.

Um modelo com pesos grandes é mais complexo do que um modelo com pesos menores. É um sinal de uma rede que pode ser excessivamente especializada em dados de treinamento.

O algoritmo de aprendizagem pode ser atualizado para encorajar a rede a usar pequenos pesos.


Uma forma de fazer isso é alterar o cálculo da **função de perda (Loss)** usado na otimização da rede para considerar também o tamanho dos pesos. **Isso é chamado de regularização de peso ou redução de peso**.

**Keras** oferece suporte à regularização de peso por meio do argumento ``kernel_regularizer`` em uma camada, que pode ser configurada para usar a norma do vetor ``L1`` ou ``L2``, por exemplo:

model.add(Dense(500, input_dim=2, activation='relu', kernel_regularizer=l2(0.01)))

O exemplo a seguir demonstra um modelo de **Perceptron multicamadas** com redução de peso em um problema de classificação binária.




**NOTA:**
O site deste código pode ser encontrado [aqui](https://machinelearningmastery.com/better-deep-learning-neural-networks-crash-course/).
