# AWS Spot Instances without losing data
벡터 계산이 많은 경우 GPU를 사용하면 10~30배 가량 속도가 빠름 <br>
하지만 GPU를 빌리려면 금액이 발생 <br>
Spot Instance는 비교적 저렴한 가격으로 GPU 사용 가능 <br><br>

## On-Demand VS Spot Instances
![figure1](https://user-images.githubusercontent.com/57740560/95966829-8eba3680-0e46-11eb-9021-008c5b689dde.png) <br>
On-Demand 의 경우 항상 사용가능하지만, Spot Instances는 다른 사용자의 요청이 있을 경우 사라질 수 있음 <br><br>

=> Solution : Spot Instance + EBS Volume(do not delete on termination) <br> 
![figure2](https://user-images.githubusercontent.com/57740560/95967696-80204f00-0e47-11eb-875b-c05b042b9ff4.png) <br> 
이렇게 하면 중간에 instance가 사라지더라도 데이터 보존 가능 <br><br> 

## Work with screen
ssh <br>
screen : open a new screen <br>
- python train.py ..; echo "Done"|mail-s"Finished" 이메일 <br>
- Ctrl-a d (to exit screen) <br>
srceen -r: attach the screen <br>






