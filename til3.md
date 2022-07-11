# Jupyter

## Pandas & Numpy

### Series

- pd.Series() 이용

- 1차원 배열을 나타낸다
- index를 따로 지정 안하면 0-base 인덱스
- 튜플, 딕셔너리, 리스트로 생성 가능
- 함수
  - size(속성) : 개수 반환
  - shape(속성) : 튜플형태로 shape반환
  - unique: 유일한 값만 ndarray로 반환
  - count : NaN을 제외한 개수를 반환
  - mean: NaN을 제외한 평균
  - value_counts: NaN을 제외하고 각 값들의 빈도를 반환

## DataFrame

- pd.DataFrame() 이용
- 2차원 배열을 나타낸다
- 행과 열로 만들어진다
- 시리즈, 딕셔너리, 리스트로 생성가능
- read_csv 함수를 사용하여 DF생성가능