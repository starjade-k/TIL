# 데이터 프레임 카테고리 값 세기

- value_counts() 메서드를 사용해서 각각 횟수를 셀수있음
- normalize=True 사용 시 범주형 데이터의 비율계산
- Series.value_counts(normalize=True)
- df에 사용시 series 로 반환



## 데이터 정렬

- sort_index() : 인덱스를 기준으로 정렬
- sort_value() : 데이터 값을 기준으로 정렬



## 데이터 프레임 정렬

- df.sort_values() : 특정열 값 기준 정렬
  - 데이터프레임은 2차원 이므로 정렬시 기준열을 줘야 한다.
  -  by 인수 사용 : 생략 불가
  - by = 기준열, by=[기준열1,기준열2]
  - 오름차순/내림차순 : ascending = True/False (생략하면 오름차순)
- df.sort_index() : DF의 INDEX 기준 정렬
  - 오름차순/내림차순 : ascending = True/False (생략하면 오름차순)





### 행/열 합계

- df.sum() 함수 사용
- 행과 열의 합계를 구할때는 sum(axis=0/1) - axis는 0이 기본

- 각 열의 합계를 구할때는 sum(axis=0)

- 각 행의 합계를 구할때는 sum(axis=1)\

- df의 함수로는 

  ​      mean(axis=0/1)

  ​      min(axis=0/1)

  ​      max(axis=0/1)