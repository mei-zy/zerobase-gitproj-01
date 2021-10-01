# direction for git

## 1.혼자하는 git flow process

1) git flow 초기화
`git flow init` 을 해준다.
`git branch` 명령어를 입력하면 develop이라는branch 생성

2) feature start & finish
 `git flow feature start (feature name)`을 해주면 새로운 feature 생성완료

+ git add, commit 진행

`git flow feature finish (feature name)`을 진행해서 기능을 완료한다.

3) release and push
+ release 시작

`git flow release start (version)`해서 release 해준다.

`git push -u origin develop` : 처음 push 할 때
`git push --tags`




2. 작업 내역 되돌리기

1) 파일명 수정 및 이동

단순 mv를 이용해 위치를 옮기거나 이름을 바꿀 경우 git은 기존 파일은 삭제하고 새 파일이 생겼다고 인식 (즉, 파일의 history가 끊어진다)



```
$git mv source destination
```


2) 파일 상태 되돌리기 (Unstaged)

```
git checkout -- 파일명
git checkout -- .
```

> git checkout은 브런치 이동하는 switch와 상태를 되돌리는 checkout으로 분리되었음


3) 스테이지에 올라간 파일을 언스테이지로 내리기 

```
git reset head 파일명
```

> reset --hard 키워드는 유의할 것


4) 메시지 되돌리기


```
git commit --amend /* 최근 커밋메시지 수정 */
```


5) 커밋 되돌리기

```
git revert --no-commit HEAD~3.. /* 최근 커밋 3개 전으로 */
git commit
```

