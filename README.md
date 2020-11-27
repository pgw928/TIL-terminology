# TIL-terminology

> 오늘 배운 IT 관련 용어를 정리한다.



## Machine Learning 관련 용어
> 머신러닝 관련 용어들을(method, platform 등) 정리 한다.


#### 1. ONNX

: Open Neural Network Exchange 의 줄임말로 Tensorflow, Pytorch와 같이 서로 **`다른 DNN 프레임워크 환경에서 만들어진 모델들을 호환`**되게 사용되도록 만들어진 **`공유 플랫폼`**이다. 

예를 들어, Tensorflow에서 만든 모델을 ONXX 그래프로 export하고 PyTorch에서 그 모델을 import하여 사용이 가능하다.  ONXX는 크게  두가지의 장점을 지닌다.

* Framework Interoperability

  특정환경에서 생성된 모델을 다른 환경에서 자유롭게 import 할 수 있다는것이 최대 장점이다.

  Tensorflow에서 빠르게 학습 시킨 뒤 모바일로 옮겨서 사용하는 방식도 가능하다.

* Shared Optimization

  하드웨어 제조업체(HW vendor)의 입장으로 ONNX와 같은 프레임워크 간 공유되는 포맷이 존재하면, HW 설계시 ONXX representation을 기준으로 최적화 하면 되기 때문에 효율적이다. (예를 들어 ONXX라는 합의된 DNN 모델 포맷이 존재한다고 생각하면 된다.)

#### 참고 사이트

####  [onnx github tutorials](github.com/onnx/tutorials)



## 통신 관련 용어

> 프로토콜 등의 관련 용어들을 정리한다.



#### 1. SSH

: Secure Shell Protocal의 줄임말이다.  **`네트워크 프로토콜`**  중 하로 컴퓨터와 컴퓨터가 인터넷과 같은 **`Public Network를 통해 서로 통신할 때 보안적으로 안전`**하게 통신하기 위해 사용하는 **`프로토콜`**이다.

대포적 사용의 예

* 데이터 전송 

* 원격 제어





## 파일 확장자 용어

> 새로 배운 파일 확장자 용어들을 정리한다.



#### 1. PPK 파일

: PuTTY Private Key로 PuTTY를 이용해 아마존 AWS 관련한 것들을 사용하기 위해 필요한 파일이다.