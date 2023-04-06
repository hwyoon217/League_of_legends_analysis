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
- grid search <br/>
<img src="https://github.com/hwyoon217/League_of_legends_analysis/blob/main/lol_data/xgb_f1.PNG" width="800" height="80"/><br/><br/>
- RandomizedSearchCV <br/>
<img src="https://github.com/hwyoon217/League_of_legends_analysis/blob/main/lol_data/random_f1.PNG" width="800" height="80"/><br/><br/>
- Permutation Importance<br/>
<img src="https://github.com/hwyoon217/League_of_legends_analysis/blob/main/lol_data/%EC%88%9C%EC%97%B4%EC%A4%91%EC%9A%94%EB%8F%84.PNG" width="800" height="500"/><br/>

- 분석 결과 승패에 큰 영향을 끼치는 3개 요인은 킬, 데스, 억제기를 먼저 깬 팀이다. <br/>
## 회고
- 기존 데이터가 어느정도 가공된 것이라 그런지 성능이 너무 좋게 나왔다. 그래서 내가 만든 모델의 성능을 제대로 파악할 수가 없었다.
- 리그오브레전드는 5인으로 구성되어 게임이 진행된다. 이번 프로젝트는 경기 결과만 가지고 분석을 했지만, 각 개인이 포지션별로 어떻게 플레이 해야하는지 분석을 해보고 싶다.
