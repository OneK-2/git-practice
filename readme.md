# Git Repository 생성 

```shell
cd <path>
git init
.
```

`git init`: 현재 터미널이 있는 위치를 루트로 하는 깃 레포지토리 생성.

# Diff

## Track / Untrack

아무 파일이나 편집/생성 한 후 다음을 터미널에서 실행.

```shell
git status
```

```
On branch master

Initial commit  

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        readme.md

nothing added to commit but untracked files present (use "git add" to track)
```

1. master: 브랜치 이름

제일 먼저 해야할 건, git이 diff를 추적하게 하고자 하는 파일을 track시키는 것.

```shell
git add [file]
```

## Commit

```shell
git commit
```

### git config

커밋을 하기위해선 정보가 필요함

### 커밋의 구성 요소

* title (1줄요약)
    * ex: Create readme.md
    * 명령문 형태로 많이 적음
* description (설명, 필수아님)
* author (email)
* date
* hash (id)
* parent



```shell
git config --global user.email "you@example.com" #  필수 GitHub에서 사용하는 이메일로 할 것
git config --global user.name "Your Name" 
.
```

커밋 제목은 "Create readme.md"로 할 것.

커밋 메시지 작성

```
커밋 제목 (1줄, 필수)
(빈줄)
(커밋 설명)
```


```
[master (root-commit) 5e2610b] Create reademe.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 readme.md
```
