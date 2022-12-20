## Model description
### 사용한 모델 : U-Net
- U-Net : 분야에서 이미지 분할(Image Segmentation)을 목적으로 제안된 End-to-End 방식의 Fully-Convolutional Network 기반 모델 
- End-to-End Learning: 어떤 문제를 해결할 때 필요한 여러 스텝을 하나의 신경망을 통해 '재배치'하는 과정. 데이터 크기가 클 때 효율적. 즉 데이터가 클 때 두 단계로 나누어 각각 네트워크를 구축한 후 학습한 후 그 결과를 합치는 방법이다. 이렇게 하는 이유는 스텝을 나누는 것이 성능이 더 좋기 때문이다.

