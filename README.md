# CUAI-2022-Summer-CV-3-team
segmentation은 image 크기가 달라도 학습할 수 있다
근데 코드들 보면 사람들이 다 iamge size 256x256으로 맞추던데?
FCN은 이미지 크기 달라도 학습 할 수 있다

rand augment의 경우 epoch을 돌릴때 augmentaion 종류 중에 하나가 랜덤으로 사용된다
따라서 epoch을 늘릴 때 augmentation을 늘린 게 효과를 발휘한다

fastai, w&b





data loader + converting + augmentation / model(unet, swim transformer) / train / inference


1. Unet Fastai baseline 코드 error 고쳐나가면서 실행해보기
2. model 자리에 swim transformer 적용해보기
<Swim Transformer>
imports / paths / additionals / random choice / augmentations / Dataset / image patching / model(swim transformer) / window functionalities / Upent_Net+MLP / configuration / Folds  / competition Metric  / validation / initialization / training
3. 속성데이터 추가(aspp)
4. dataaugmentation 방법 추가해보기
5. loss function (lovasz)(dice) 
6. fastai를 pytorch 로 바꿔보기
