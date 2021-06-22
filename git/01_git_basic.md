## Git basic

git 의 기초를 배워요

## WARNING

1. HOME 폴더(`~`)를 리포로 업그레이드 하지 않는다.
2. 리포 안의 폴더에서 `GIT INIT`하지 않는다.
   1. (리포 안에 리포를 두지 않는다.)

## 저장소 초기화 하기

``` 
$ git init
```



## 저장소를 일반 디렉토리로 되돌리기

```
$ rm -rf .git
```



## 업로드

``` 
$ git add 'file name'
```

```
$ git add . (변경된 모든 파일)
```

복수 파일 가능 (분류별 업로드 작업)

## 내리기

```
$ git restore --staged <file>...
```



## 저장

```
$ git commit -m 'massage'
```



## 상태확인

```
$ git status
```

- 빨간색 파일은 commit 에 포함되지 않음
- 초록색 파일은 commit 에 포함됨
- 변경사항이 없는 파일은   표시 되지 않음



## 로그 확인

``` 
$ git log
```

```
$ git log --oneline
```

- 간단하게 보기



## 리모트 연결하기

```
$ git remote add <name> <url>

# 리모트 삭제하기
$ git reomte remove <name>

#리모트 이름 바꾸기
$ git remote rename <old-name> <new-name>
```



## 리모트에 PUSH하기

리모트에 업로드

ex git push origin master

```
$  git push <name> <branch>
```



## 리모트에서 최초 CLONE 받기

리모트 리포 내용을 그대로 복제

```
$ git clone (url.git)
```



##  리모트에서 PULL 하기

```
$ git pull <name> <branch>
```



## 강의장 <=> 집 공부

앉을 때 PULL, 일 어설 때 PUSH

1. 집에서 기상
2. 강의장 도착
   1. `pull`
3. 공부 / TIL 정리
   1. `commit`
4. 강의 종료
   1. `commit`
   2. `push`
5. 집 도착
6. 복습
   1. (처음이라면) `clone`
   2. `pull`
   3. `commit`
7. 복습 끝
   1. `commit`
   2. `push`
8. 잠
9. 1 번으로 이동





## * vim (txt 수정) *

1. `i`수정 모드
2. `esc` 눌러서 나오기
3. `:w`저장
4. `:q`종료
5. `:wg `저장후 종료
6. `:q!` 강제종료







