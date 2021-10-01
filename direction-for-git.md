# direction for git

# 작업 내역 되돌리기

## 파일명 수정 및 이동

단순 mv를 이용해 위치를 옮기거나 이름을 바꿀 경우 git은 기존 파일은 삭제하고 새 파일이 생겼다고 인식 (즉, 파일의 history가 끊어진다)



```
$git mv source destination
```


