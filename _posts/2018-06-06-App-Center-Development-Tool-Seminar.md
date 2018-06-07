---
layout: post
title: App Center Development Tool Seminar
tags: [Seminar, Tool, Github, Dev]
---

어플리케이션 개발자에게 꼭 필요한 개발 툴 사용법 (iOS, Android, Server)

## 1. 서버 기초 지식

클라이언트(사용자) <-> 웹 서버 : 정적인 웹
클라이언트(사용자) <-> 웹 서버 <-> 어플리케이션 서버 : 동적인 웹
: 로그인 후 사용자 정보 변경, 캐싱 등

* Socket(프로세스), HTTP(웹) : 통신
  * **Socket**
    : 양방향 통신
    : 연결 유지, 통신 대기 가능

  * **HTTP**
    : 일회성 통신
    GET, POST 등의 명령을 하면 **Request->, <-response 후 연결이 끊김**

    

## 2. Slack

: 업무와 일상 분할 가능 (카톡과 다른 점)
: 다양한 생산성 앱을 지원해줌 (Github과 연동 가능 등)
: 무료로도 꽤 많은 히스토리 보존 가능
: 워크스페이스(단체) 내의 채널(공지사항, 일정) 기능
: 다양한 플랫폼 지원



## 3. Postman (서버 필수 툴)

: HTTP 통신 테스트 가능
: **HTTP Request와 Response를 저장**해둘 수 있음 
  -> 앱 개발자들이 **서버의 기능을 확인**할 수 있다 ! (서버 기능 명시 가능)
: 컬렉션(워크스페이스), 폴더(채널) 기능
: 컬렉션 공유
: 목업 서버
: 문서 생성 기능
: 서버 테스트 기능



## 4. Github

: 버전 관리 (버그 대처)
: 협업이 편리함
  -> **Branch**를 이용하면 각자 개발한 후 병합 가능
*  **Issues(버그, 기능, 문의)** 관리
    -> dev, user 모두 작성 가능
    -> 버그와 함께 commit 가능 + 일정(기한)
    : 버그, 개발 예정, 추가기능, 건의사항 등을 관리하는 기능
  * Milestone : 마감일 설정 등
  * ```git commit -m "fix #1"``` : issue 완료 처리 (commit과 연결 가능)

** Github는 Git을 사용할 수 있는 툴

* Git 명령어
  * init : git repository 생성
  * local / remote : 사용자의 컴퓨터 / git 서버
  * commit : 변경된 내용을 comment와 함께 snapshot을 남김
  * push : local의 commits을 remote에 반영
  * **pull** : remote의 commits을 local에 반영
  * **fetch** : remote의 commits을 local로 그대로 가져옴
  * branch : 서로 다른 원본을 가지는 commits
  * clone : local에 repository 복제
  * merge : branch 혹은 commit 간의 내용이 다른 부분을 합침 (하나의 commit)
  * fork : github에 repository를 복사
    -> 다른 사람의 업데이트도 가져올 수 있음
  * stash 
    : commit으로 만들지 않은 변경 내용을 임시로 저장
    : merge를 원하지 않을 때 사용
    : 충돌을 피할 수 있음
  * **revert** 
    : 삭제하고 싶은 commit의 이전 commit을 불러올 수 있음
    ```git revert <commit number>``` -> revert commit message 작성
  * **reset** 
    : 이전 commit 상태로 초기화
    ```git reset --hard <commit number>``` -> 해당 commit으로 초기화
  * conflict 
    : merge 시 remote와 local의 commits가 일치하지 않는 경우
    : branch 간의 내용이 달라 auto merge가 되지 않음
    ```css
    <<(왼쪽 꺽쇠)...<< HEAD
    aaa 
    =====
    bbb
    (오른쪽 꺽쇠)>>>>
    ```
  * diff : local의 commit과 다른 파일들을 다 보여줌
  * status : 수정된 파일들을 보여줌
  * rebase 
    : merge랑 비슷한 개념으로, commit을 병합하고 commit message를 수정할 수 있음
    ```rebase -i HEAD~4``` : 최근 4개의 commit을 보여줌
    ```css
    pick
    pick
    pick
    sqush // -> 위의 commit과 병합됨
    ```
    
  ** 학생 정보 등의 github에 업로드하면 안되는 정보 지우는 법

* 새로운 repository 만들기
  1. local에 폴더 만들기
  2. teminal에서 해당 폴더로 이동
  3.  ```git init```
  4. 폴더 안의 수정 사항 발생하면 untracked files 이 생김
  5. ```git add .```
  6. ```git commit -m "commit message"```
  7. ```git remote add origin <repository 주소>```
  8. ```git push -u origin master``` -> origin에 master라는 branch가 생성됨
* pull
  1. repository에서 수정
  2. teminal 해당 폴더에서 ```git pull```
* remote와 local에서 같은 파일 수정
  1. conflict 발생 -> 수정 or auto merge

     


## 5. Waffle (Issues 관리 도구)

: 여러 프로젝트의 Issues를 한번에 볼 수 있음 
  -> github에서는 각각 repository별로만 관리 가능
  -> 팀 프로젝트에서 ios, android, server 의 Issues를 한번에 관리할 수 있음
