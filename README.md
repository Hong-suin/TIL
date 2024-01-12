# StartCamp 3일차

### 원격 저장소

: 코드와 버전 관리 이력을 온라인 상의 특정 위치에 저장하여 여러 개발자가 협업하고 코드를 공유할 수 있는 저장 공간.

: gitlab, github, bitbucket

### 로컬 & 원격 저장소

- 공용 문서 안내에 따라 github 가입 및 설정 진행
- github repository 생성.

`git remote add origin remote_repo_url` : 로컬 저장소에 원격 저장소 주소 추가

*origin : 푸가하는 원격 저장소에 대한 이름

```jsx
push : 로컬 → 원격 전송 / 원격 저장소에 commit이 올라가는 것.
(commit 이력이 없다면 push 불가)
pull : 원격 → 로컬

(+clone : 로컬에는 데이터가 없을 때 그대로 가져옴. clone을 하게되면 git init 할 필요 x )```
```

* -u옵션 : 처음 push 할 때의 origin master로 하면 이후에 git push 만 써도됨

*master : branch 이름 

`git push -u origin master` : 원격 저장소에 commit 목록 업로드 

`git pull -u origin master`  : 원격 저장소의 변경 사항만을 받아옴

비어있는 원격 저장소에 local의 내용 동기화하는 법

1. Local을 먼저 생성 (local에 commit이 있음.)
2. 원격 저장소 생성 (빈 저장소여야 함 (commit이 없는 것.))

`clone` : local은 비어있고 원격에 기존의 commit이 있을 때 동기화 하는 방법

### Git New Repository 생성

[README.](http://README.MD)md check box 선택하여 생성하면 첫번째 커밋을 자동으로 생성시킴ㅂ.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/a3626c85-51b5-40ae-a258-a58d96acadcb/573281fb-755b-40e7-b153-79f8b9f4dd10/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/a3626c85-51b5-40ae-a258-a58d96acadcb/b9d8d898-22cb-4a21-a481-b2ab8b2cf360/Untitled.png)

### pc 이동 시 기존 저장된 계정 삭제

- window 자격 증명 관리자 → 편집 or 삭제

.gitignore 습관적으로 만들기 . 올릴필요 없는 파일들 등록하기

`.gitignore` : git 에서 특정 파일이나 디렉토리를 추적하지 않도록 설정하는 데 사용되는 텍스트 파일 

이미 커밋한 것들은 gitignore 소용x 계속 추적함

add, 커밋 전에 ignore ㅐㅎ야함.

예시 : 

1. .gitignore 파일생성
2. a와 b 이름을 가진 텍스트파일 생성
3. gitignore에txt 파일 생성
4. ???

### README.md file

- 프로젝트에 대한 설명, 사용법, 문서화된 정보 등을 포함하는 역할
- Markdown 형식으로 작성되며, 프로젝트의 사용자, 개발자, 기여자에게 프로젝트에 대한 전반적인 이해와 활용ㅇ방법을 제공하는데 사용
- 주로 프로젝트 소개, 설치 및 설정 방법, 사용 예시, 라이선스 정보, 기여방법 등을 포함
- 반드시 저장소 최상단에 위치해야하며 원격 저장소에서 올바르게 출력됨

---

### git push하는 과정

git init

touch README.md

git add .

git commit -m ‘ ‘

git remote add origin 원격 저장소 link

git push origin master

---

### clone하는 과정

pull

add

commit

git push

---

문서화 연습의 중요성

https://d2.naver.com/news/3435170