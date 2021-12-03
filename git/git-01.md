# git 01

## NEVER

1. `~` 에서 `$ git init` 진행
2. 리포 안에 리포 만들기
3. **`$ git init` 입력 전 확인할 점**
   1. `~` 인지
   2. `(master)` 떠 있는지

## 프로젝트 초기화 진행

```sh
# pjt 폴더 생성
$ mkdir new_project

# 폴더로 이동
$ cd new_project

# README 파일 & .gitignore 생성
$ touch README.md .gitignore
# gitignore.io 에 접속하여 필요한 내용 복-붙

# 폴더를 리포로 초기화
$ git init

# README & .gitignore 파일 add(tracking)
$ git add .

# commit
$ git commit -m 'first commit'

# 원격 저장소 생성 @ github.com
# 생성한 원격 저장소 등록
$ git remote add origin <URL>

# 등록된 저장소 확인
$ git remote -v

# 지금까지의 commit push
$ git push origin master
```

### 계정 세팅

```sh
# (계정당 1회) 서명이 등록되지 않았다면, 계정용 서명 등록
$ git config --global user.name '내이름'
$ git config --global user.email 'github에서@쓸메일주소'
# 서명이 정상적으로 등록되었는지 확인
$ cat ~/.gitconfig  
```



## 명령어 정리

- 초기화 시점에 1회 입력

```sh
$ git init 
```

- 작업중

```sh
$ git add <filename>
$ git commit -m 'MESSAGE'
```

- 모니터링 명령어

```sh
$ git status  # 현재 상황
$ git log     # commit 로그 
```

- github 에 원격 저장소 생성하기
- 원격 저장소(remote repo) 추가하기

```sh
$ git remote add origin <URL>
```

- 원격 저장소 확인하기

```sh
$ git remote -v
```

- 원격 저장소에 지금까지의 commit 들 PUSH 하기

```sh
$ git push origin master
```

- 새로운 컴퓨터에서 기존 원격 저장소 복제하기
```sh
$ git clone <URL>
```

- 원격 저장소의 내용 받아오기
```sh
$ git pull origin master
```