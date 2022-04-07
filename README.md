# 🔴깃 명령어 정리

#### Branch Remote Local 기본 과정

---

- git init (현재 디렉토리에 git 적용)
- git add README.md (readme 추가)
- git commit -m "" (하나의 버전을 히스토리에 저장)
- git status (현재 local 적용상태 확인)
- git push (local을 remote로 저장)
- git pull (remote를 local로 저장)

#### Branch 명령어 ( Local Repository )
---
- git branch (로컬 브랜치 목록 조회)
- git branch -r (원격 브랜치 목록 조회)
- git branch -a (모든 브랜치 목록 조회)
- git branch {브랜치명} ( local 브랜치 생성)
- git checkout -b {브랜치명} (명령어를 통해 신규 브랜치 생성과 동시에 체크아웃)
- git checkout {브랜치명} (브랜치 변경)
- git branch -d {브랜치명} ( 브랜치 삭제 )

#### 원격 저장소( remote repository )

---

- git push origin -u <new_name_branch> (Remote Branch(원격 브랜치) 이름 변경 방법)
- git remote -v (현재 연결되어 있는 원격 레파지토리를 확인)
- git remote add <name> <url> (원격저장소와 연결하고 싶으실 경우엔)
- git clone [저장소 주소] ( 저장소 복제 )
- git fetch (remote를 local로 저장, 직접 비교대조 후에 수동 merge)
- git pull (remote를 local로 저장, 자동 merge)

                                              
# 🟠깃 기본사용
#### 1. 디렉토리 들어가기

###### git bash
- $ cd "C:\Users\gittest\Desktop\git_practice"  <- " "를 붙여줘야한다.                                                 
                                                 
                                                 
#### 2. 사용자등록

- git config --global user.email "[이메일주소]"
- git config --global user.name "[이메일주소]"                                                 
#### 3. 저장소생성

- git init
  + master branch 생성, git bash 폴더명에 (master)추가됌, .git이라는 숨김폴더 추가                                       
#### 4. 스테이지에 올리기

- git add .(전체폴더 >> 특정폴더명 지정가능)
- git status
#### 5. 로컬에 세이브

- git commit -m "커밋메세지"
- git log 
  + commit된 리스트를 보여줌
#### 6. 원격저장소 연동

- git remote add origin https://github.com/myungyi0314/githubTest.git
- git remote -v
#### 7. 원격저장소에 올리기

- git push origin master 

# 🟢깃 fork와 clone 비교
#### fork
---
#### clone
---
                                                 🔴🟠🟡🟢🔵🟣🟤⚫⚪                                                 
                                                 
