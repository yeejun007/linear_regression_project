# linear_regression_project
### 한국 개봉영화 관람객 예측 프로젝트
<br/>

### 팀구성
김민혜, 배빛나, 송이준
#
<br/>

### `Goal`
개봉한 영화의 관람객 수 예측하기 
<br/>

### `Technical Skills`
python, scikit-learn, statsmodels, matplotlib, pandas
<br/>

### `Procedure`
1. 주제선정
2. 기존의 연구동향 파악(선행연구 논문 읽기) 
3. 데이터수집&EDA
4. 회귀분석 모델링
5. 최종 모델을 통한 에측
<br/>
<br/>

### `Project Details`
#### 1. 영화흥행 예측모델 생성을 목표로 정하고, 종속변수는 관객수로 하기로한다. (독립변수는 2015~2019년간의 반기별 top100 영화)
  - 영화 흥행의 척도는 크게 매출액 or 관객수
  - 하지만 매출액을 기준으로 하면 프라임 시간대를 배정받는 영화와 그렇지 않은 영화를 구분해야 할 뿐 아니라, 물가 상승률 또한 고려해야 한다(정확한 예측이 힘들다)
  - 따라서 관객수를 종속변수로 하기로 한다
  <br/>
  <br/>
  
#### 2. 선행 연구논문들을 통해 영화흥행에 영향을 미치는 요인들에 어떤한 것들이 있는지 파악하고 관련 데이터를 수집한다.(최대한 많은 컬럼을 수집하는 것을 1차 목표로 한다)
  - 배우 파워, 감독 파워, 장르, 국적, 마케팅(신문 기사 홍보 등..), 배급사 파워, 개봉시점, 원작여부, 실화바탕 여부, 관람객 평점, 할당받은 상영관 갯수 등...
  <img width="864" alt="스크린샷 2020-07-07 오후 3 14 06" src="https://user-images.githubusercontent.com/46306443/86725348-86db4100-c064-11ea-9a12-9b8efbfc43bd.png">
<br/>
<br/>

#### 3. EDA를 통해 수집한 데이터들을 한번 더 재 가공한다.
  - 범주형 변수의 경우, 특징(컬럼)의 갯수를 줄여서 과접합을 막고 모델이 복잡해지는 것을 방지한다
  - 도메인에 대한 서칭을 통해 이 과정이 적합한지, 해서는 안될 특별한 이유가 없는지 확인함
  - 또한 실제로 모델간 비교를 통해 이러한 범주형 변수의 범위 축소과정이 더 나은 선택이라는 것을 확인하였음
  <img width="853" alt="스크린샷 2020-07-07 오후 3 29 24" src="https://user-images.githubusercontent.com/46306443/86727743-a96e5980-c066-11ea-9227-6caddb0fe129.png">
  <img width="748" alt="스크린샷 2020-07-07 오후 3 31 22" src="https://user-images.githubusercontent.com/46306443/86727989-ee928b80-c066-11ea-9a9b-812eeb8046fb.png">
  <br/>
  <br/>

#### 4. try&error 과정을 통해 모델링을 진행한다.
- statsmodels의 r-squared, kfold 교차검증 r-squared, test r-squared를 향상시키는 방향으로 모델을 발전시켜나간다
<img width="726" alt="스크린샷 2020-07-07 오후 3 37 29" src="https://user-images.githubusercontent.com/46306443/86728865-ceaf9780-c067-11ea-9376-90c90355c726.png">
<br/>

#### 5. 완전히 새로운 데이터로 영화 관객수 예측해보기(최종 모델 사용)
  - 생각보다 굉장히 잘나와서 놀람...
  <img width="796" alt="스크린샷 2020-07-07 오후 3 40 26" src="https://user-images.githubusercontent.com/46306443/86729255-3bc32d00-c068-11ea-9411-a33883985c04.png">
<br/>
<br/>


### `Presentation ppt`
https://bit.ly/3dYX7cV
<br/>


