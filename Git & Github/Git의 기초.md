## git init과 git status
 

git init : 명령어를 실행하는 터미널에서 새로운 깃 저장소를 생성함

git status : git 프로젝트의 상태를 확인할 수 있는 명령어

git init을 하기 전에 git status를 하면 ‘not a git repository’라는 문구가 뜬다

</br>

## Git 초심자가 흔히 저지르는 실수

Do not init a repo inside of a repo

before running git init, use git status to verify that you are not currently inside of a repo

만약 존재하는 저장소 안에 새 저장소를 초기화하고 싶다면 상응하는 .git 폴더를 지워서 저장소를 삭제

</br>

## git add와 git commit

git add로 변경사항 스테이징한 후 git commit

 </br>
 
**(+) 추가로 알아두면 좋은 것**

git log : 깃 저장소에 대한 커밋 정보들을 검색

git log —oneline : 커밋을 한 줄로 요약해서 보여줌

git add . : 이 시점에 변경된 모든 파일 add

git commit —amend : commit 실수 수정

 </br>

**(+) atomic commit**

'atomic commit' 이라는 말이 있던데 기능 단위로 쪼개서 커밋하라는 거였다

최근에 git add *를 남발했는데 반성하고 중간 중간 커밋하는 거 잊지 말아야겠다

 </br>

 

## .gitignore
: git으로 관리할 필요가 없는 경우 제외시킬 파일이나 폴더 등을 지정한다

  예를 들면 npm module이나 AWS 비밀키, JWT 비밀키 처럼 용량이 크거나 보안상 문제가 되는 것들을 제외시켜 준다
  
</br>

**.gitignore 사용하는 규직**

.파일이름

폴더이름 /

*.log 의 경우 확장자
 

 

 
