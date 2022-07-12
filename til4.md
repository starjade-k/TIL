# 데이터 프레임생성

## 리스트로 데이터 프레임 생성

- df = pd.DataFrame([['a','b','c'],['a','n','g'],['a','a']])





## 딕셔너리로 데이터프레임 생성

- 

df1 = pd.DataFrame(
{
    'A':[90,80,70],
    'B':[85,98,75],
    'C':[88,99,77],
    'D':[87,89,86]
},index = [1,2,3]# 행 인덱스
)
df1





## 시리즈로 데이터프레임 생성

- a = pd.Series([1, 2, 3], ['a', 'b', 'd'])
  b = pd.Series([11, 21, 31], ['a', 'b', 'k'])
  c = pd.Series([12, 13, 14], ['a', 'b', 'c'])

- pd.DataFrame([a,b,c],index=[11,14,3])



# 행, 열 이름 설정

- df.index.name='이름'
- df.columns.name='이름'



# 데이터프레임 내용 변경

- 열추가 : df[열이름(key)]=values

- 열 내용 갱신 : df[열이름(key)]=values

- 열 삭제 : del df['삭제 열'] -원본반영 삭제 /              

  ​                drop(index=['삭제명']) - 원본 비반영 삭제 반영시 inplace= True 이용

  



# loc, iloc

- loc : 라벨값 기반의 2차원 인덱싱
- iloc : 순서를 나타내는 정수 기반의 2차원 인덱싱

##### loc 인덱서 : 행 우선 인덱서

- df.loc[''행'']  행우선 인덱서

- df.loc[''행'','열']

- df['열'] 열 우선 인덱서

  #### 인덱싱 값

  - 인덱스 데이터(index, column)

  - 인덱스슬라이싱

  - 같은 행 인덱스를 갖는 불린 시리즈(행 인덱싱)

  - 위 값을 반환하는 함수



# 

## 데이터 개수 세기

- count() 함수 사용
  - NAN 값은 세지않음



## 난수를 발생시켜 df 생성

-  seed(값) 사용 시  동일한 난수가 발생
- seed함수 사용할때마다 매번 코드를 실행시켜줘야 적용
- ex)  np.random.seed(값)
         np.random.randint(n (0~n 사이의 수에서 난수 발생,size=4(난수를 4개 생성)) 





## 카테고리 값 세기



- 시리즈.value_counts()메서드를 사용해 각각의 값이 나온 횟수를 셀 수 있음
- 파라미터 normalize=True 를 사용 (범주형 데이터)
  - 시리즈.value_counts(normalize=True)

- s2.tail() 공란일 시 5개를 추출
- s2.head() 공란 일 시 5개를 추출
- s2.head(값) # 값 개수 만큼의 데이터를 추출