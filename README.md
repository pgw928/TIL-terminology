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



## 데이터 베이스 용어

> DB 관련 용어들을 정리한다.



#### 1. BLOB

: Binary Large Object의 줄임말로 **데이터베이스 관리 시스템의 하나의 엔티티로** 저장한느 이진 데이터의 모임이다. 영어 단어를 보면 Large Object를 문자 그대로 큰 객체로 주로 이미지, 비디오, 사운드 등과 같은 멀티 미디어를 binary 형태로 저장할 것이라는것을 추축할 수 있다.



## 컴퓨터 기초 용어

> 컴퓨터 관련 기초용어들을 정리한다.



#### 1. 아스키(ASCII)코드

: American Standard Code Information Interchange의 줄임말로, 1960년대 미국에서 정의한 표준화한 부호체계이다.

1바이트(byte) = 8비트(bit)은 2의 8승인 256개의 고유한 값을 저장할 수있다.

아스키 코드의 경우 7비트만 활용한다. 즉 128개의 고유값을 사용한다. 이는 1비트를 **통신** **에러** **검출**을 위해 사용하기 때문이다.

<img src="markdown-images/image-20201221002921929.png" alt="image-20201221002921929" style="zoom:67%;" />

(0~32, 127 : 인쇄와 제어용 용어, 33~126 : 숫자, 알파벳, 특수기호)



#### 2. ANSI 코드

: American National Standards Institute 8비트로 아스키코드를 확장한 코드이다.

아스키 코드에서 1비트 늘어났기 때문에 기존 아스키 코드보다 128개를 더 사용가능 하다.

이때, 1바이트만으로 표현되는 경우를 SBCS(Single Byte Character Set)이라고 한다.

반대의 경우는 MBCS(Multi-Byte Character Set)이라고 한다.



#### 3. 유니코드

: 아스키 코드만으로 다른 언어들을 표현할 수 없기 때문에 2바이트(65536개)의 유니코드가 등장했다.

유니코드 3.0버전까지는 2바이트 영역을 기본다중언어판(BMP, Basic Multilingual Plane)이라 불렀다.

그러나 65536개로 이세상의 모든 문자를 담을 수 없어 유니코드 3.0부터 보충언어판(Supplementary Plane)을 정의했다.



## 정리할 내용

* backporting

* 카멜표기법, 뱀표기법

* 디코딩, 인코딩

