# TIL

## Git hub



### init & clone

- init & clone은 상위 명령어

- init 은 home-computer 

- clone 은 받아 올 computer2 

- clone 은 init 된 자료를 받아오면 init 된 상태
  (computer2 에서 init 생략가능)  



### push % pull

- init , clone 이 완료된 후
- home-computer 에서 add commit 후 git push origin master
  코드 실행 하면 github에 업데이트 
- computer2 에서 git pull origin master 코드 실행 후 업데이트된 자료 받아옴



## Ignore 

-  <touch .gitignore>

- https://www.toptal.com/developers/gitignore/

  - 여기서 검색해서 이용 가능

- 프라이빗한 정보를 github에서 추적 불가능하게 해줌 

  (ex: API adress, 고유 키 넘버)

  

  


###  Branch

- <git branch 파일 명> 

  -  브랜치 확인 및 생성

    

-  git switch 

  - master 와 branch 를 드나들수 있음

    

- git merge 
  - master 와 branch 를 합침
  
  - git branch 로 현재 master의 위치인지 확인 해야 함
  
    

###  Collison

- commit 내역이 다를 때 충돌이 일어난다

  a 와 b 파일 둘다 커밋이 다를 때 충돌
  
  

###  Pull-request

- hub에서 레지포토리 코드 clone 하기
- vscode 로 연 후 내 브랜치 생성 (git branch -c 브랜치명)
- 내 브랜치로 git switch 하기
- 내용 수정 - 커밋 후 git push origin 브랜치명 해주기
- hub 로 돌아가서 pull-request 버튼 활성화 되어있는지 확인 후
- hub에서 marge 가 완료 되었으면 code에서
- 마스터 브랜치로 git switch 해준 후 
- git push origin master 해주면 완료