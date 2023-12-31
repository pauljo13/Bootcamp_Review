# Section1 : Introduction to Data Science
## EDA
### 정의
EDA(Exploratory Data Analysis)는 데이터 분석의 초기 단계로, 데이터를 다각도로 관찰하고 이해하기 위한 과정입니다. 이 과정은 데이터의 정제 및 전처리를 포함하며, 추가적으로 통계치와 시각화를 통해 데이터를 분석합니다.

### 중요성
원본 데이터(Raw Data)만으로는 인사이트를 얻기 어렵습니다. Raw 데이터에는 종종 불필요하거나 잘못된 데이터가 포함되어 있어, 이를 정제하고 전처리하는 과정이 필수적입니다. 이러한 작업을 통해 데이터 분석 과정에서 오류를 최소화할 수 있습니다.

### EDA 과정
1. **라이브러리 모듈 호출**
   - 데이터 분석에 필요한 라이브러리 모듈을 불러옵니다.
   ```python
   import numpy as np
   import pandas as pd
   ```

2. **데이터 업로드**
   - 분석할 데이터를 업로드합니다. 대부분의 데이터는 `.csv` 또는 `.excel` 형태의 파일입니다.
   ```python
   df = pd.read_csv('파일.csv')
   df = pd.read_excel('파일.xlsx')
   ```

3. **데이터 확인**
   - 데이터의 상태를 확인하고, pandas의 메서드를 사용해 문제가 있는지 탐색합니다.
   ```python
   df.head()
   df.shape
   df.info()
   df.describe()
   df.isnull().sum()
   df.duplicated().sum()
   ```

4. **데이터 정리**
   - 문제가 되는 데이터를 정리합니다.
     - 결측치 처리: 데이터 삭제 또는 채우기
     - 중복값 처리: 중복값 제거
     - 데이터 타입 변경: 적절한 데이터 타입으로 변경
     - 인덱스 재정렬: `df.reset_index(drop=True)`

### 추가 정보
- 데이터의 시각화: 데이터의 이해를 돕기 위해 matplotlib, seaborn 등의 라이브러리를 사용하여 데이터를 시각화합니다.
- 데이터의 상관관계 분석: 변수 간의 관계를 파악하기 위해 상관계수를 계산하고, 이를 시각화합니다.
- 피처 엔지니어링: 모델의 성능을 높이기 위해 적절한 피처를 선택하거나 생성합니다.

## Data Wrangling

## Bayesian Theorem

## Central Limit Theorem

## Hypothesis Test

## AB test

## Linear Algebra

## PCA

## Clustering

## Gradient Descent