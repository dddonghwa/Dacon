# parking_demand
### 대회명 
DACON 주사추요 예측 AI 경진대회 [링크](https://dacon.io/competitions/official/235745/data) (2021.06.10 ~ 2021.07.30)

### 데이터셋 :
  - train.csv
  - test.csv
  - sample_submission.csv
  - age_gender_info.csv

### 배경
아파트 단지 내 필요한 주차대수는 ①법정주차대수 ②장래주차수요 중 큰 값에 따라 결정하게되어 있어, 정확한 ②장래주차수요의 산정을 필요로 합니다.
현재 ②장래주차수요는 ‘주차원단위’와 ‘건축연면적’을 기초로하여 산출되고 있으며, ‘주차원단위’는 신규 건축예정 부지 인근의 유사 단지를 피크 시간대 방문하여 주차된 차량대수를 세는 방법으로 조사하고 있습니다.
이 경우 인력조사로 인한 오차발생, 현장조사 시점과 실제 건축시점과의 시간차 등의 문제로 과대 또는 과소 산정의 가능성을 배제할 수 없습니다.

### 주제
🏠 유형별 임대주택 설계 시 단지 내 적정 🅿️ 주차 수요를 예측

### 주최 / 주관
주최 : 한국토지주택공사
주관 : 데이콘

### 참가 대상
일반인, 학생 누구나 👩‍🎓👨🏻‍⚖️👩🏼‍💻

### 제출 모델 
|일자| 사용 모델| 사용 피처 | 과정/특징 |  결과(랭킹) | 링크 |
|:--:|:--:|:--:|:--|:--:|:--:|
|2021.07.12| LinearRegression | '총세대수' | - '자격유형' 결측치 처리 <br> - 각 데이터별 등록차량수 예측치의 평균을 각 단지별 등록차량수 'null'으로 저장 후 제출 | 246.91677 (336위) | [LINK](https://github.com/dddonghwa/Dacon/blob/main/parking_demand/class28_0712_1.ipynb) |
|2021.07.12 | RandomForestRegression |  '총세대수', '전용면적', '전용면적별세대수', '공가수',  '단지내주차면수', '자격유형', '지역' | - '자격유형' 결측치 처리 <br> - '자격유형'&'지역' 라벨인코딩 <br> - - 각 데이터별 등록차량수 예측치의 평균을 각 단지별 등록차량수 'null'으로 저장 후 제출 | 137.84508(305위) | [LINK](https://github.com/dddonghwa/Dacon/blob/main/parking_demand/class28_0712_2.ipynb)|
|2021.07.14|LinearRegression | '총세대수', '전용면적', '전용면적별세대수', '공가수','단지내주차면수' | - '자격유형' 결측치 처리 <br>  |[LINK](https://github.com/dddonghwa/Dacon/blob/main/parking_demand/class29_0714_3.ipynb)|
 
