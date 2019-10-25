# NLP_VoC
## 개요
아마존 제품 리뷰와 매출 순위의 상관 관계를 파악하는 Voice of the Customers 논문을 구현해보는 것이 이번 프로젝트의 목적이었습니다.
해당 논문 링크는 다음과 같습니다.
<br/>
<br/>
<br/>
https://www.semanticscholar.org/paper/Voice-of-the-Customers%3A-Mining-Online-Customer-for-Zhang-Narayanan/5aa2b53b342211258a2d996d50dae120fb791f3a -> Voice of the Customers: Mining Online Customer Reviews for Product Feature-based Ranking
<br/>
<br/>
<br/>
다만 논문과의 조사방법과 저희 조사 방법이 약간 차이가 있을 수 있습니다.
<br/>
<br/>
- 해당 논문에서는 디지털 카메라와 TV 이 두 가지 제품군으로 데이터를 수집, 분석하였으나 저희는 디지털 카메라 품목만 활용하였습니다.
- 논문에서의 결과 도출 방식과 저희 프로젝트의 결과 도출 방식에 차이가 있습니다. 논문에서는 리뷰의 Feature 언급 정도와 고객들이
가장 중요하게 여기는 Feature 순서를 비교하여 모델의 정확도를 측정하였습니다.
- 저희 모델에서는 리뷰 자체가 제일 많은 인기 품목 10개의, feature 별 랭킹 순서와 제품들의 특정 feature에 대한 품질 기반 순위의 상관도를 분석하여
모델의 정확도를 측정하였습니다.


## 설명

순서는 다음과 같이 진행되었습니다.
<br/>
<br/>
- API를 통해 아마존 리뷰 데이터, 메타 데이터 수집
- 리뷰를 Sentence 형태로 토큰화
- 특정 feature(배터리, 화소, LCD 등) 10가지가 포함된 리뷰만 추출
- 타 제품 비교 리뷰와 제품 자체 리뷰를 구분, 타 제품 비교 리뷰의 경우 타 제품 명 또한 추출
- 리뷰의 극성 분류
- PageRank 알고리즘을 통해 feature 별 제품 랭크를 산출

<br/>
<br/>
분석 결과 및 성과 등 자세한 설명은 git에 업로드 된 발표 PDF를 통해 확인 하실 수 있습니다.
