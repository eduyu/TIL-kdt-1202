# git 01

## NEVER

1. `~` 에서 `$ git init` 진행
2. 리포 안에 리포 만들기
3. **`$ git init` 입력 전 확인할 점**
   1. `~` 인지
   2. `(master)` 떠 있는지

## 최초 commit 진행하기

```sh
# pjt 폴더 생성
$ mkdir new_project

# 폴더로 이동
$ cd new_project

# 폴더를 리포로 초기화
$ git init

# README 파일 생성
$ touch README.md

# README 파일 add(tracking)
$ git add README.md

# (계정당 1회) 서명이 등록되지 않았다면, 계정용 서명 등록
$ git config --global user.name '내이름'
$ git config --global user.email 'github에서@쓸메일주소'

# 서명이 정상적으로 등록되었는지 확인
$ cat ~/.gitconfig  

# commit
$ git commit -m 'first commit'
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