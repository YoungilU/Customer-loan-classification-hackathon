# 고객 대출등급 분류 해커톤
## 주제
고객의 대출등급을 예측하는 AI 알고리즘 개발
<br>
<br>
## **데이터**
https://dacon.io/competitions/official/236214/data
<br>
<br>
## **프로젝트 배경**
[Dacon 해커톤 39회, 고객 대출등급 분류 해커톤]
이번 데이콘 해커톤은 고객의 대출등급을 예측하는 인공지능 모델을 개발하는 것을 목표로 합니다.  
제공된 데이터를 통해 고객정보와 대출현황 데이터를 분석합니다.  
<br>
## **프로젝트 과정**
#### 1.EDA 수행
#### 2.라이브러리와 데이터 불러오기
#### 3.전처리
##### - 주택소유상태=='ANY' Drop
##### - 근로기간=='Unknown' Drop
##### - 범주형 변수('대출기간', '주택소유상태', '대출목적', '근로기간') category type으로 변경
##### - 수치형 변수('대출금액', '연간소득', '부채_대비_소득_비율', '총계좌수', '최근_2년간_연체_횟수', '총상환원금', '총상환이자', '총연체금액', '연체계좌수') MinMaxScaling 
#### 4.대출등급 예측 모델 생성
##### - 분석 모델 선정 -> RandomForest, Catboost, Xgboost, Lightgbm 중 더 나은 성능을 보이는 Lightgbm 채택
#### 5.하이퍼파라미터 그리드 설정(GridSearchCV)
#### 6.모델 학습
#### 7.학습한 모델로 예측한 DataFrame 생성  
