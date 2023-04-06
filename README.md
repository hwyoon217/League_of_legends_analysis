# League_of_legends_analysis

## 프로젝트 개요
우리나라에서 인기가 많은 게임인만큼 많은 사람들이 즐기고 있는데, 이 게임에서 어떻게 하면 티어(등급)를 올릴 수 있을지 궁금했다.<br>
따라서 리그오브레전드 상위권 유저의 데이터를 이용하여 어떤 요인들이 게임 승패에 큰 영향을 끼치는지 머신러닝을 사용하여 분석하였다. <br/>


## 프로젝트 구조
 - 데이터는 캐글에 있는 데이터를 이용 <br/>
   <https://www.kaggle.com/datasets/gyejr95/league-of-legends-challenger-ranked-games2020> <br/>
 - 구조<br>
    - 데이터 전처리 및 EDA
    - xgboost를 활용한 성능 평가
    - grid search와 RandomizedSearchCV를 이용하여 최적 하이퍼파라미터 확인
    - 특성중요도, 순열중요도를 이용하여 승패에 중요한 요인 확인<br/>
    
## 결과


