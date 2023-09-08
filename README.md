# Fall-Detection-Using-GRU
GRU를 사용하여 낙상 감지 모델 구현

## 요양 병원에서의 낙상 사고 혹은 복도에서의 거동이 불편한 환자들의 낙상 사고를 감지하는 것을 목표로 합니다.

낙상 사고 발생 시 혼자인 경우 즉각적인 대처가 필요하며, 주변에 사람이 있어도 도움을 요청하기 어려운 경우 문제가 발생할 수 있습니다.
이러한 상황에서는 관리자(, 관계자)의 빠른 상황 인식이 필요한데, 사람이 직접 감지하는 것은 제한 사항이 있을 수 있기 때문에 자동화 도구를 만들어 신속한 알림을 주고자 하였습니다.

### 사용 Skill : 
1. PoseNet을 이용한 Skeletal Data 추출
2. Tensorflow의 RNN 레이어 중 하나인 GRU를 이용하여 시계열 데이터 학습
3. sklearn과 matplotlib를 통한 시각화 및 데이터 분석
4. (추가 예정) React와 Tensorflow.js를 활용한 실시간 데이터 처리 및 낙상 감지 연구

### 사용 Dataset
1. URFD Dataset(이미지 파일을 영상으로 변환 후 사용)
2. 자체 제작 Dataset(영상)

![image](https://github.com/bk123477/Fall-Detection-Using-GRU/assets/59231609/55a70605-fcff-4e96-ad3e-69e3a6e92120)

100 epoch 수행 시 모델의 train 정확도 99%, 모델의 validation 정확도 98.5%

![image](https://github.com/bk123477/Fall-Detection-Using-GRU/assets/59231609/dc8ccf2a-2588-49ac-8fce-0b7d0e5affb9)

모델의 정확도, 정밀도, 재현율, 특이도

![image](https://github.com/bk123477/Fall-Detection-Using-GRU/assets/59231609/f24b9d69-c1fd-439a-815a-1b72d6bc84b1)

모델의 F1-Score, 위양성율, ROC-curve 및 AUC
