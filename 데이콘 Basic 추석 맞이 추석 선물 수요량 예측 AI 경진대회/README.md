# <a href = "https://dacon.io/competitions/official/236166/overview/description" />데이콘 Basic 추석 맞이 추석 선물 수요량 예측 AI 경진대회
![image](https://github.com/18-12847/Competition/assets/118495919/2d7ce9e0-9487-49fe-b6c6-b2049fcef239)
- ### Autogluon 주요 파라미터(https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.fit.html)
  - presets : 전체 작동 방식(best_quality 등)
  - time_limit : 모델 훈련 및 튜닝에 할당된 시간 조절
  - refit_full : 최적의 모델을 찾은 후 전체 데이터셋을 사용하여 다시 훈련
  - num_bag_folds : stacking과 bagging을 사용할 때 fold 수 지정
  - hyperparameter_tune_kwargs : 하이퍼파라미터 튜닝 설정(searcher, scheduler, num_trials)
    ```
    tune_kwargs = {
    'searcher': 'random', #사용할 하이퍼파라미터 검색 알고리즘 지정(random, grid, bayesopt)
    'num_trials': 7,      #전체 튜닝 프로세스에서의 학습 룬의 최대 수 지정
    'scheduler' : 'local' #튜닝 작업 스케줄링 방식 지정(fifo, hyperband, local)
    }
    ```
