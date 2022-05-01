# CNN-Image-Predict
CNN을 통한 이미지 부분 예측

AI 부트캠프 3기 백경렬의 네번째 프로젝트입니다.

section4에서는 CNN을 이용해서 이미지의 비어있는 부분을 예측하였습니다.

예측한 이미지는 치아 X-ray 이미지를 스펙트럼화 시켜놓은 이미지를 사용하였습니다.

GAN을 통해서도 예측을 해보려 했지만..

영상 : https://youtu.be/w9T9M1Ygbnw

학습 데이터들의 소유권이 저에게 없기에 공유가 불가능한 점을 미리 말씀드립니다 !
#

아래 이미지의 노란색 부분을 CNN으로 예측 해 보려고 했습니다.

![image](https://user-images.githubusercontent.com/40240766/166127449-d58666aa-5594-4da8-a0b2-5e036bf8ffd6.png)

위(빨간색 Data1), 아래(파란색 Data2) 데이터들을 가지고 가운데 노란색 부분을 예측하기 위해

![image](https://user-images.githubusercontent.com/40240766/166127715-b3c05245-ce8e-4d30-abd7-7c0f6eaff908.png)

아래와 같이 이미지들을 움직여 줍니다.

![image](https://user-images.githubusercontent.com/40240766/166127671-ec6bc300-6bf7-4bf0-ac89-19a5f6335f0d.png)

데이터들을 모아 학습 시킨 후 예측을 원하는 부위를 예측 시켜 채워 넣습니다.

![image](https://user-images.githubusercontent.com/40240766/166127735-d6ac2c26-7f71-48df-9893-6ba13527c20f.png)

비어 있는 부분의 이미지를 거의 비슷하게 예측 해냈음을 볼 수 있습니다.

![image](https://user-images.githubusercontent.com/40240766/166127782-bf6da7a6-360d-4845-9053-4c448aa8d725.png)

#

다음은 GAN을 이용해서 예측을 해보려 했습니다만..

![dcgan](https://user-images.githubusercontent.com/40240766/166127806-20dab048-e255-4146-8041-4c415ecf0065.gif)

실패..

# 

이번 프로젝트는 원래 데이터를 한줄씩 받아와서 가운데 부분을 예측 하려 했었다.

예측된 부분이 양옆으로 서로 어울리지 못해 이상하게 결과가 나왔었습니다.

양과 범위를 Data1, Data2의 범위처럼 넓게 잡고 학습 시킨 후 예측을 하니까,

예측된 데이터들이 서로 잘 어울리는 모습을 볼 수 있었습니다.

지금은 차원이 1차원 예측이지만 3차원까지 늘릴 수 있다면 컬러 이미지도 부분 예측이 가능하지 않을까 싶습니다 !

이미지의 한 부분이 훼손 되어도 그 부분을 주변 이미지와 어울리는 이미지로 채워 넣을 수 있게 만들게 하는 프로젝트이었습니다.

감사합니다.
