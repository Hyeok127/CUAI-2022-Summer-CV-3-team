* 이 문서에서 글을 지우는 건 pull request로 해주세요

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

# pull reqeust 하는 법
1. origin repo를 fork
2. fetch upstream
3. modify
4. pull request
5. origin repo에서 merge
6. repeat 2-5
 * 모든 사람이 봐야 할 수정사항이 있다면 pull request로 작성하기 (새로운 버전의 코드 등)

# data
|dataset|volume|number of data|
|------|---|---|
|origin|9.39g|351|
|256|318m|2791|
|512|1.32g|2895|
|128|87m|3148|

# code
 * https://www.kaggle.com/code/iafoss/hubmap-pytorch-fast-ai-starter 
  * baseline 코드가 참고했던 baseline
