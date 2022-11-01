## Easy way to configure environment in anaconda (miniconda)

### Anaconda env
env는 Python의 독립적인 가상의 실행 환경(Environment)를 말합니다.

아나콘다 패키지로 설치한 경우 conda 명령어를 이용해서 env를 생성/삭제 및 관리할 수 있습니다.

### env 생성
` conda create -n env_tf python=3.7 `

Python 3.9 버전의 ‘env_tf’라는 이름으로 env를 생성합니다. (현재 Windows에서 Keras를 설치할 거면 Python 버전을 3.6이 아닌 3.5로 해야 합니다.)

### env 리스트 보기
` conda env list` 

### env 활성화
` activate env_tf` 

### env 비활성화
` deactivate` 

### env 삭제
` conda env remove -n env_tf ` 


### env에 Tensorflow, Keras 설치
` activate env_tf ` 

` pip install tensorflow ` 

` pip install keras ` 
Tensorflow와 Keras의 설치 확인은 다음 명령어를 이용해서 확인할 수 있습니다.

``` python  

import tensorflow as tf  
import keras

print(tf.__version__)   

``` 
