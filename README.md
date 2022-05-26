## BUBBLEing: 한식 인식을 위한 딥러닝 모델 학습
### 모델 학습 및 변환 프로세스
<img src="https://user-images.githubusercontent.com/76741915/170532651-7f658622-5e9e-4633-944f-284e08a6cca5.png" width="700" height="200"/>

### 학습 환경
- Google Colab
- Tensorflow 2
### 학습 데이터
(1) 직접 제작한 한국 음식 데이터셋

-> 58종 클래스에 대해 총 21,895개 이미지로 구성

(2) 한국의 대중적인 식문화를 반영해 아래의 기준으로 음식 선정
- 한식진흥원 포털의 한국 음식 아카이브 
- 외국인에게 인기있는 한식 메뉴
- 한국인이 좋아하는 한식 메뉴
### 학습 방법
- COCO 2017 Dataset으로 pre-trained된 SSD MobileNect v2 모델로 전이 학습 수행

- 실시간 모델 검증을 위해 training / evaluation terminal 병렬 수행
<img src="https://user-images.githubusercontent.com/76741915/170534667-633efe10-4c92-4f11-8fc4-6ac527b21f9d.png" width="700" height="120"/>

### 학습 결과
<img src="https://user-images.githubusercontent.com/76741915/170534952-d93d72ca-5c1d-4ed3-bac9-e1fb47ff52ae.png" width="300" height="250"/>

- 실제 서비스에 적용한 모델은 Bubbleing-Tensorflow.js-Model 레포지토리에 위치함.
