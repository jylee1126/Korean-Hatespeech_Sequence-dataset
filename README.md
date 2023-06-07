# Korean-Hatespeech_Sequence-dataset

## 소개

현 연구는 서울대학교 인문데이터과학 연계전공 졸업 발표를 위해 실시한 데이터셋 라벨링 프로젝트입니다. 

## 설명

> <b> 혐오표현이란? </b>
> <p> 인종, 종교, 성적 지향성, 정치적 지향성, 국적, 민족, 피부색, 성별 등의 속성에 따라 대상 그룹, 혹은 그 구성원에 대한 증오를 표현하기 위해 사용되는 언어 </p>

공개된 `Korean HateSpeech Dataset`의 `Unlabeled` 데이터를 1) `labeled` 2) `unlabeled` and 3) `news_title` 라벨 대신, <br>
앞선 혐오 표현의 정의에 따라 아래와 같은 라벨링을 통해 혐오 표현 탐지 모델의 성능을 향상시키고자 하였습니다. 

1) `gender`: 특정 성별에 대한 희화화된 표현, 혐오감을 담은 발언, 특정 성별을 고착화하는 표현 등
2) `age`: 특정 세대나 연령을 비하하는 표현
3) `nation (general + region)`: 국가 및 지역 단위의 혐오 표현
4) `religion`: 특정 종교에 대한 혐오 발언 및 차별성 발언을 포참하여, 특정 인종에 대한 차별성 발언을 초함
5) `others`: 위의 카테고리에 해당하지 않는 분류
6) `curse`: 특정인에 대한 혐오 표현

## Sequence-to-Sequence 성능 확인 코드

이번 데이터셋이 어떻게 작동하는지 확인하기 위한 코드를 Google Colab notebook으로 제공합니다. 

<a target="_blank" href="https://colab.research.google.com/drive/1Ls8Fi0ZPXSFo0juNtmRC70Btq8cRwOYA?usp=sharing">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

## References

Korean HateSpeech Dataset: https://github.com/kocohub/korean-hate-speech

UnSmile Dataset: https://github.com/smilegate-ai/korean_unsmile_dataset
