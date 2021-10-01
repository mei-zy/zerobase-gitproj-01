# direction for git

# 작업 내역 되돌리기

## 파일명 수정 및 이동

단순 mv를 이용해 위치를 옮기거나 이름을 바꿀 경우 git은 기존 파일은 삭제하고 새 파일이 생겼다고 인식 (즉, 파일의 history가 끊어진다)



```
$git mv source destination
```


## 파일 상태 되돌리기 (Unstaged)

```
git checkout -- 파일명
git checkout -- .
```

> git checkout은 브런치 이동하는 switch와 상태를 되돌리는 checkout으로 분리되었음


## 스테이지에 올라간 파일을 언스테이지로 내리기 

```
git reset head 파일명
```

> reset --hard 키워드는 유의할 것 
