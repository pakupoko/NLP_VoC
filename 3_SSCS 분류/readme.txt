﻿CS추출 함수.ipynb
Ver1 - 190806
최초 업로드. csv를 받아, Review 칼럼의 값들을 (JJR,JJS,RBS,RBR)에 만족하는 경우 cs로 분리하여 cs 데이터프레임 완성
product_list가 없어서 해당 코드를 # 처리하여 남겨둠 추후 처리할 필요성있음.
Ver2 - 190807
아래 CS, SS 라벨링 문서에 통합되어 사용하지 않음. 앞으로 아래 함수 사용할 

=================================================
CS, SS 라벨링.ipynb
Ver1 - 190807
CS와 SS 라벨링하는 함수입니다. 라벨링한 데이터는 드라이브에^^
Ver2 - 190808
kw_list를 수작업으로 재정의했습니다
Ver3 - 190809
kw_list 가져오는 코드 함수화
cs, ss 라벨링 apply로 진행하는 코드 작성, 함수화
Ver3 - 190812
product list 가져오는 코드 함수화
product 사전을 통해 리뷰에서 타겟 제품을 찾고 라벨링하는 함수 설계
ver4 - 190813
CS 데이터 중 타겟 데이터와 제품명이 동일한 데이터들을 제거하는 코드 추가
ver5 - 190826
타겟 제품이 여러개 일 경우, 제품명과 동일한 모델명이 제거되지 않는 오류 수정
===================================================
labeling_feature.ipynb
Ver1 - 190807
feature_labeling하는 함수입니다. 라벨링한 데이터는 CS,SS 데이터를 포함하고 있습니다.
Ver2 - 190808
feature_labeling for문 말고 apply로 라벨링하는 코드를 작성했습니다.

===================================================
pNumber_preproc.ipynb
ver1 - 190812
최초 업로드. 제품 사전 엑셀 파일을 csv로 전환하는 함수입니다.
