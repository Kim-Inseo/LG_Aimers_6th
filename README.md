# LG_Aimers_6th

## 경진대회 주제
- 난임 환자 대상 임신 성공 여부 예측
- https://dacon.io/competitions/official/236452/overview/description

## 결과
- 229등/794
- 상위 29%

## 사용한 방법
- EDA
  - target 비율 확인
  - 결측치 확인
  - 그래프 시각화
- Data preprocessing
  - 결측치 채우기
  - 범주형 데이터 인코딩
- Train
  - CatBoostClassifier
  - Optuna

## 아쉬운 점 및 보완해야 할 점
- 파생변수를 적극적으로 사용해볼 시도를 하지 못한 것이 아쉬움이 남는다.
- 전처리를 하는 데에 상당한 시간을 들였지만, 어떤 전처리가 합리적일지 여러 가능성을 시험해보지는 못했는데 다양한 경우를 시도해보았으면 더 좋았을 것이다.
- CatBoostClassifier 이외의 다른 모델과 앙상블을 시도해보았다면 어땠을까?
  - 그러나 이러면 해석력을 어떻게 개선할지 (SHAP Value 등?) 고민해봐야 한다.
- Optuna를 GPU에서 사용할 때 결과값이 완전하게 고정되지는 않는 모습을 보였다.
  - 이 부분의 오차를 최대한 줄이기 위해서 어떻게 해야 하는지 고민이 필요하다.
