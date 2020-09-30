# Geoffrey Hinton's summary of finding up to today <br>
왜 잘 안되었을까? <br><br>

datasets이 너무 적었다. <br>
computer의 속도가 너무 느렸다. <br>
초기값 설정이 잘 안되어있었다. <br>
sigmoid function의 문제 <br><br>

초기값 설정과 sigmoid function 문제를 해결하기 위한 방법은? <br><br>

## We used the wrong type of non-linearity. <br>
### Vanishing gradient <br>
초반의 입력값이 sigmoid function에 의해 0에 가까워져 뒤의 값에 거의 영향을 미치지 못하는 문제. <br><br>

### ReLU:Rectified Linear Unit <br>
![figure1](https://user-images.githubusercontent.com/57740560/94715631-b4e0d080-0388-11eb-89c1-210a3a53956b.png) <br>
sigmoid의 Vanishing gradient 해결을 위해 제안됨 <br><br>

### Other Activation functions <br>
![figure2](https://user-images.githubusercontent.com/57740560/94715390-5e739200-0388-11eb-9bfa-9582717049c6.png) <br><br>

## We initialized the weights in a stupid way. <br>
### Initialization method <br>
![figure2](https://user-images.githubusercontent.com/57740560/94715903-0ab57880-0389-11eb-9548-73d27612c929.png) <br><br>

# Overfitting <br>
Training dataset에 최적화되어 Training data에서는 높은 accuracy를 보이지만, test dataset에서 accuracy가 낮음. layer가 많을 수록 overfitting 가능성 높음. <br><br>

Solutions of overfitting <br><br>

1. More training data <br>
2. Regularization <br><br>

+ Dropout <br>
![figure2](https://user-images.githubusercontent.com/57740560/94718814-3b97ac80-038d-11eb-9426-17b87418d375.png) <br>
node를 random하게 선택하여 연결을 끊는다. dropout rate를 설정할 수 있다. 단, 학습할때만 dropout을 사용하고 test에서는 전체 node를 사용해야 함. <br><br>

# Ensemble <br>
학습시킬 수 있는 기기가 많을 때 독립된 여러개의 NN으로 학습시켜 마지막에 combine. Ensemble 모델 사용시 2~4-5% 성능 향상. <br><br>

[참고 자료 및 이미지 출처] <br>
모두를 위한 딥러닝 시즌1 
