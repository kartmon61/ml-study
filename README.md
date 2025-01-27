# ml-study

## 1. Machine Learning
This is a repository for studying machine learning.

### 1. pandas and numpy
### 2. scikit-learn
### 3. evaluation
개요: 모델의 성능을 평가하는 방법은 다양하다. 모델의 성능을 평가하는 방법은 모델의 목적에 따라 달라진다. 모델의 성능을 평가하는 방법은 다음과 같다.
- confusion matrix
- accuracy
- precision
- recall
- f1 score
- roc_auc

### 4. classification
개요 : 분류는 이산적인 출력 변수(예: 클래스, 변수)를 예측하기 위해 입력 변수와 출력 변수 사이의 관계를 모델링하는 기법이다.
주로 데이터가 특정 범주나 클래스에 속하는지 예측하는 데 사용된다.

분류를 사용하는 이유는 다음과 같다.
- 데이터를 범주로 나누기 위해 사용된다. 예를 들어 스팸 메일과 정상 메일을 구분하는 경우
- 새로운 데이터의 소속 클래스를 예측할 수 있다. 예를 들어 질병 여부를 예측하는데 사용된다.
- 데이터의 패턴을 학습하여 정확한 분류를 가능하게 한다.

분류 모델의 성능을 평가하는 방법은 다음과 같다.
- confusion matrix : 실제 클래스와 예측 클래스를 비교하여 TP, TN, FP, FN을 계산한다.
- accuracy : 전체 데이터 중에서 정확하게 예측한 데이터의 비율을 계산한다.
- precision : 양성 클래스로 예측한 데이터 중에서 실제 양성 클래스인 데이터의 비율을 계산한다.
- recall : 실제 양성 클래스인 데이터 중에서 양성 클래스로 예측한 데이터의 비율을 계산한다.
- f1 score : precision과 recall의 조화 평균을 계산한다.
- roc_auc : ROC curve의 면적을 계산한다.

- decision tree
- ensemble model
  - random forest
  - gradient boosting
  - xgboost
  - lightgbm
- stacking with ensemble model
- hyperparameter tuning
  - grid search
  - random search
  - bayesian optimization

### 5. regression
개요 : 회기는 연속적인 출력 변수(예: 숫자 값)를 예측하기 위해 입력 변수오 출력 변수 사이의 관계를 모델링하는 기법이다. 주로 숫자 값을 예측하거나 추정하는 데 사용된다.
회기를 사용하는 이유는 다음과 같다.
- 연속적인 값(예: 주가, 집값 등)을 예측하는 데 사용된다.
- 입력 변수와 출력 변수 사이의 관계를 파악하고 모델링하여 예측력을 높인다.
- 데이터의 경향성을 분석하고, 이를 기반으로 미래의 값을 예측하는 데 도움이 된다.

회귀 모델은 크게 선형 회귀와 비선형 회귀로 나눌 수 있다.
- 선형 회귀 : 입력 변수와 출력 변수 사이의 관계가 선형적인 경우 사용된다.
- 비선형 회귀 : 입력 변수와 출력 변수 사이의 관계가 비선형적인 경우 사용된다.

선형 회귀 모델은 다음과 같이 나눌 수 있다.
- y = wx + b : 단순 선형 회귀
- y = w1x1 + w2x2 + ... + b : 다중 선형 회귀
- y = w1x1 + w2x1^2 + ... + b : 다항 회귀 (비선형 회귀의 일종)

비선형 회귀 모델은 다음과 같이 나눌 수 있다.
- 지수 회귀: y = a * exp(bx) 형태로, 데이터가 기하급수적으로 증가하거나 감소하는 경우 사용된다.
- 로그 회귀: y = a * log(bx) 형태로, 데이터가 급격히 증가하다가 어느 시점 이후로 완만해질 때 사용된다.
- 시그모이드 회귀: y = L / (1 + exp(-k(x - x0))) 형태로, S자 곡선을 그리며 데이터가 특정 한계에 수렴할 때 사용된다.
- 다항 회귀: y = w1x + w2x^2 + ... + wn*x^n + b 형태로, 데이터가 비선형적이지만 다항식을 사용해 모델링할 때 사용된다.

회귀 모델의 성능을 평가하는 방법은 다음과 같다.
- MAE (Mean Absolute Error) : 실제 값과 예측 값의 차이를 절대값으로 변환한 후 평균을 계산한다.
- MSE (Mean Squared Error) : 실제 값과 예측 값의 차이를 제곱한 후 평균을 계산한다.
- RMSE (Root Mean Squared Error) : MSE의 제곱근을 계산한다.
- R^2 (R-squared) : 실제 값의 분산 대비 예측 값의 분산 비율을 계산한다.

Regression model에는 아래와 같은 종류가 있다.
- gradient descent
  - linear regression
  - ridge regression
  - lasso regression
  - logistic regression
- tree regression

### 6. demension reduction
개요 : 데이터의 차원을 줄이는 방법으로, 데이터의 특징을 추출하거나 노이즈를 제거하는데 사용된다. 차원을 줄이는 이유는 다음과 같다.
- 차원의 저주를 해결하기 위해
- 데이터 시각화를 위해
- 머신러닝 알고리즘의 성능을 향상시키기 위해

차원을 줄이는 방법은 크게 두 가지로 나눌 수 있다.
- feature selection : 중요한 특징만 선택하고 나머지는 제거하는 방법
- feature extraction : 기존의 특징을 조합하여 새로운 특징을 생성하는 방법

#### PCA
- 데이터의 분산을 최대한 보존하는 새로운 축을 찾아 데이터를 변환하는 방법

##### LDA
- 클래스 간 분산과 클래스 내 분산의 비율을 최대화하는 새로운 축을 찾아 데이터를 변환하는 방법
- PCA와 다르게 LDA는 클래스 정보를 사용하여 데이터를 변환한다.
- LDA는 분류 문제에 사용되는 반면, PCA는 차원 축소에 사용된다.

#### SVD
- 특이값 분해를 이용하여 데이터를 변환하는 방법
- PCA와 유사하게 데이터의 분산을 최대한 보존하는 새로운 축을 찾아 데이터를 변환한다.

#### NMF
- 비음수 행렬 분해를 이용하여 데이터를 변환하는 방법
- NMF는 주로 이미지 처리나 텍스트 마이닝 분야에서 사용된다.

### 7. clustering
개요: 군집화는 비지도 학습의 한 방법으로, 데이터를 여러 그룹으로 나누는 방법이다. 군집화는 데이터의 유사성을 기반으로 데이터를 그룹화하는데 사용된다.

군집화는 다음과 같은 방법으로 나눌 수 있다.
- 계층적 군집화 : 데이터를 계층적으로 그룹화하는 방법
- 비계층적 군집화 : 데이터를 미리 정해진 군집 수에 따라 그룹화하는 방법
- 밀도 기반 군집화 : 데이터의 밀도를 기반으로 그룹화하는 방법
- 확률 기반 군집화 : 데이터의 확률을 기반으로 그룹화하는 방법
- 그래프 기반 군집화 : 데이터의 연결성을 기반으로 그룹화하는 방법


#### K-means
- 데이터를 K개의 그룹으로 나누는 방법
- K-means는 데이터의 분산을 최소화하는 중심점을 찾아 데이터를 그룹화한다.

- K-means는 아래와 같은 순서로 동작한다.
  1. 중심점을 랜덤하게 초기화한다.
  2. 각 데이터 포인트를 가장 가까운 중심점에 할당한다.
  3. 각 그룹의 중심점을 새로운 중심점으로 업데이트한다.
  4. 중심점이 변하지 않을 때까지 1~2를 반복한다.
  5. 중심점이 변하지 않으면 알고리즘이 종료된다.


#### Mean shift
- 데이터의 밀도를 기반으로 그룹화하는 방법
- Mean shift는 데이터의 밀도가 가장 높은 지점을 중심으로 데이터를 그룹화한다.

- Mean shift는 아래와 같은 순서로 동작한다.
  1. 각 데이터 포인트를 중심으로 원을 그린다.
  2. 원 내의 데이터 포인트의 평균을 계산하여 중심점을 업데이트한다.
  3. 중심점이 변하지 않을 때까지 1~2를 반복한다.
  4. 중심점이 변하지 않으면 알고리즘이 종료된다.


#### gaussian mixture model
- 데이터가 여러 개의 가우시안 분포를 가진 데이터의 혼합으로 이루어져 있다고 가정하는 방법
- GMM은 데이터가 여러 개의 가우시안 분포를 가진 데이터의 혼합으로 이루어져 있다고 가정한다.

- GMM은 아래와 같은 순서로 동작한다.
  1. 각 데이터 포인트가 각 가우시안 분포에 속할 확률을 계산한다.
  2. 각 데이터 포인트가 속할 가우시안 분포의 평균과 분산을 업데이트한다.
  3. 중심점이 변하지 않을 때까지 1~2를 반복한다.
  4. 중심점이 변하지 않으면 알고리즘이 종료된다.


#### DBSCAN
- 데이터의 밀도를 기반으로 그룹화하는 방법
- DBSCAN은 데이터의 밀도가 높은 지역을 클러스터링하고, 데이터의 밀도가 낮은 지역을 노이즈로 처리한다.

- DBSCAN은 아래와 같은 순서로 동작한다.
  1. 랜덤한 데이터 포인트를 선택한다.
  2. 선택한 데이터 포인트를 중심으로 반경 epsilon 내에 있는 데이터 포인트의 개수를 계산한다.
  3. epsilon 내에 있는 데이터 포인트의 개수가 min_samples보다 작으면 노이즈로 처리한다.
  4. epsilon 내에 있는 데이터 포인트의 개수가 min_samples보다 크면 새로운 클러스터로 할당한다.
  5. 모든 데이터 포인트에 대해 1~4를 반복한다.
  6. 모든 데이터 포인트를 처리할 때까지 1~5를 반복한다.