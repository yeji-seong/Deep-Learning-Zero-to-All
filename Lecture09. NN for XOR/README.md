# XOR using NN <br>
![figure1](https://user-images.githubusercontent.com/57740560/94712423-6f220900-0384-11eb-9341-6c833057d1e6.png) <br><br>

K(**X**) = sigmoid(**X** **W_1** + **b_1**)  <br>
hypothesis = sigmoid(K(**X**)**W_2** + b_2) <br><br>

# Backpropagation <br>
![figure1](https://user-images.githubusercontent.com/57740560/94713186-6ed63d80-0385-11eb-8dfc-72dcaa14c350.png)  <br><br>
Chain rule을 통해 output에 대한 입력값의 미분값을 구할 수 있다. Tensorflow는 backpropagation을 사용해 단순한 방법으로 미분값(기울기)를 구할 수 있다.<br><br>

# Tensorboard  <br>
Tensorflow 시각화 도구로 loss, accuracy 시각화, 모델 그래프 시각화, weight, biases, 기타 텐서의 히스토그램 확인 등 다양한 기능을 제공한다.  <br> <br>

[참고 자료 및 이미지 출처] <br>
모두를 위한 딥러닝 시즌1 
