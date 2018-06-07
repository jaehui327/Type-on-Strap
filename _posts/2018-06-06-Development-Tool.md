---
layout: post
title: Development Tool
tags: [Seminar, Tool, Github, Dev]
---

어플리케이션 개발자에게 꼭 필요한 개발 툴 사용법 (iOS, Android, Server)

### 1. 서버 기초 지식  
> client(user) <-> web server : 정적인 웹  
> client(user) <-> web server <-> application server : 동적인 웹   
> -> 로그인 후 사용자 정보 변경, 캐싱 등이 필요할 때 사용한다.

* Socket(process), HTTP(web) : 통신  
  * **Socket**  
    양방향 통신이 가능하다.  
    연결 유지, 통신 대기가 가능하다.  
  * **HTTP**  
    일회성 통신만 가능하다.  
    GET, POST 등의 명령을 하면 **Request->, <-response 후 연결이 끊겨** 버리기 때문에 소통이 불가능하다.

### 2. Slack  
1. **업무와 일상 분할** 가능하다. (카톡에서 사진이나 문서를 공유할 때와 다른 장점이다.)  
2. 다양한 생산성 **앱을 지원**해준다. (Github과 연동이 가능하고, 그 이외에도 다양한 앱과도 연동해서 사용할 수 있다.)  
3. 무료로도 꽤 **많은 히스토리 보존** 가능하다.
4. **워크스페이스(단체)** 내의 **채널(공지사항, 일정)** 기능이 있어, 단체를 분류하고 채널 내에서 게시물의 성격에 따라 분류할 수 있다.
5. 웹, 모바일앱, 데스크탑앱 등의 **다양한 플랫폼**을 지원한다.


### 3. Postman (서버 필수 툴)  
1. **HTTP 통신 테스트 가능**하다. HTTP는 단방향 통신이기 때문에 postman을 사용하면 매우 편리해질 수 있다.

2. **HTTP Request와 Response를 저장**해둘 수 있다.     

   결과를 저장해두면 앱 개발자들이 **서버의 기능을 확인**할 수 있다 ! 서버의 기능을 명시할 수 있기 때문에 가능하다.

3. **컬렉션(워크스페이스), 폴더(채널) 기능**이 있다.

4. 컬렉션 공유가 가능하다.

5. **mockup 서버** 구축이 가능하다. mockup 서버란 간단한 작업을 위해 가상의 서버에서 작업하는 것을 말한다.

6. **문서 생성** 기능이 있다. **가독성**이 굉장히 높고 레이아웃이 깔끔하다!

7. 서버 테스트 기능이 있다.


### 4. Github  
1. **버전 관리**가 가능하다. 이로써 우리가 얻을 수 있는 장점은 **버그를 대처**할 수 있다는 것이다. 새로운 버전에서 치명적인 버그가 발생되면 우리는 Github으로 복원할 수 있다.

2. **협업**이 편리하다.

   **Branch**를 이용하면 각자 맡은 부분은 개발하고 합칠 수 있는 **merge**라는 기능이 존재한다. 하지만 같은 파일은 수정했을 경우에는 **conflict**가 발생할 수 있으므로 유의해야 한다.

3. **Issues(버그, 기능, 문의)** 관리를 할 수 있다. 이 장점 또한 협업에서 유리하다.

   * 개발자(dev), 사용자(user) 모두 작성 가능하다.
   * **버그와 함께 commit**을 할 수 있고, 그 issue를 언제까지 마쳐야하는지 일정(기한)도 함께 올릴 수 있다.  
   * 버그, 개발 예정, 추가기능, 건의사항 등을 관리하는 기능으로 아주 유용하다.

4. Milestone : Issues를 결합하여 마감일을 정하는 등의 활용이 가능하다.

5. 터미널에서 commit과 함께 issue 완료 처리를 하려면 다음과 같은 명령어를 입력하면 된다.

   ```css
   git commit -m "fix #1"
   ```

**Github는 Git을 사용할 수 있는 툴** 이다. 따라서 git 명령어를 알아야한다. sourceTree와 같이 관리할 수 있는 툴이 있지만 모든 기능을 포함하고 있진 않기 때문에 Git 명령어를 알아야 한다. 

* Git 명령어  

   * init : git repository 생성    

   * local / remote  : 사용자의 컴퓨터 / git 서버  

   * commit  : 변경된 내용을 comment와 함께 snapshot을 남김  

   * **push** : local의 commits을 remote에 반영  

   * **pull** : remote의 commits을 local에 반영  

   * fetch  : remote의 commits을 local로 그대로 가져옴  

   * branch : 서로 다른 원본을 가지는 commits  

   * clone  : local에 repository 복제  

   * merge   : branch 혹은 commit 간의 내용이 다른 부분을 합침 (하나의 commit)  

   * fork  : github에 다른 사람의 repository를 복사하는 것이다. 해당 repository가 업데이트 되면 바로 반영할 수 있다.

   * stash  : commit으로 만들지 않은 변경 내용을 임시로 저장하는 기능으로, merge를 원하지 않을 때 사용한다. 이 명령어를 이용하면 충돌을 피할 수 있다.

   * **revert** : 삭제하고 싶은 commit의 이전 commit을 불러올 수 있다. 

     ```css
     git revert <commit number>
     ```

      라는 명령어를 입력하면 revert commit message 작성하여 이전의 commit을 새롭게 commit 한다.

   * **reset**  : 이전 commit 상태로 초기화하는 것으로,

     ```css
     git reset --hard <commit number>
     ```

      라는 명령어를 입력하여 해당 commit으로 초기화하는 기능이다. 

   * conflict : merge 시 remote와 local의 commits가 일치하지 않는 경우 conflict가 발생한다. branch 간의 내용이 달라 auto merge가 되지 않는다. 이 경우에는 수동으로 merge 작업을 해줘야한다. 아래와 같이 충돌이 난다.
     ```css
     <<(왼쪽 꺽쇠)...<< HEAD
     aaa 
     =====
     bbb
     (오른쪽 꺽쇠)>>>>
     ```
     aaa 내용과 bbb 내용 둘중에 원하는 내용만 남겨두고 삭제하면 된다.

   * diff  : local의 commit과 다른 파일들을 다 보여줌  

   * status  : 수정된 파일들을 보여줌   

   * rebase  : merge랑 비슷한 개념으로, commit을 병합하고 commit message를 수정할 수 있다.

     ```css
     rebase -i HEAD~4
     ```

      라는 명령어를 사용하여 최근 4개의 commit을 볼 수 있다.

     ```css
     pick
     pick
     pick
     sqush // -> 위의 commit과 병합됨
     ```

     이 때 sqush라는 명령어를 쓰면 바로 위에 있는 commit 과 해당 commit이 병합된다.


#### 직접 해보기  
* 새로운 repository 만들기   
  1. local에 폴더 만들기

  2. teminal에서 해당 폴더로 이동한다.

     ```css
     git init
     ```

  3. 폴더 안의 수정 사항 발생하면 untracked files 이 생겼을 것이다.

     ```css
     git add .
     ```

     ```css
     git commit -m "commit message"
     ```

     ```css
     git remote add origin <repository 주소>
     ```

     ```css
     git push -u origin master
     ```
     하게 되면 origin에 master라는 branch가 생성된다.
* pull
  1. repository에서 수정을 하게 되면 local과 remote의 내용의 차이가 생긴다.
  2. teminal 해당 폴더에서
     ```css
     git pull
     ```
* remote와 local에서 같은 파일 수정한다. 이 때 2가지 경우가 발생한다.
  1. conflict 발생 -> 수정
  2. auto merge

### 5. Waffle (Issues 관리 도구)

1. 여러 프로젝트의 Issues를 한번에 볼 수 있다. github에서는 각각 repository별로만 관리 가능해서 같은 어플리케이션이라도 iOS, Android, Server의 Issues를 한번에 관리할 수 없다. 하지만 Waffle을 사용하면 가능하다.
2. 팀 프로젝트에서 ios, android, server 의 Issues를 한번에 관리할 수 있기 때문에 편리하다.

