# git 01



```

$ git init
$ touch README.md
$ git add README.md
$ git config --global user.name '내이름'
$ git config --global user.email 'github에서@쓸메일주소'
$ cat ~/.gitconfig  # => 입력한 대로 잘 나오는지 확인!
$ git commit -m 'first commit'
```



**NEVER**

1. `~` 에서 `$ git init` 진행
2. 리포 안에 리포 만들기
3. **`$ git init` 입력 전 확인할 점**
   1. `~` 인지
   2. `(master)` 떠 있는지



초기화 시점에 1회 입력

```
$ git init 
```

작업하며 계속 입력

```
$ git add <filename>
$ git commit -m 'MESSAGE'
```

모니터링 명령어

```
$ git status  # 현재 상황
$ git log     # commit 로그 
```

