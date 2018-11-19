---
layout: post
title: Development Tool
tags: [Seminar, Tool, Github, Dev]
---

어플리케이션 개발자에게 꼭 필요한 개발 툴 사용법 (iOS, Android, Server)

<p>
앱센터 민재님께서 개발자 필수 툴에 대한 세미나를 해 주셨다. <br>
개발자에겐 역시 협업은 뗄레야 뗄 수 없는 존재! <br>
협업에 도움이 되는 툴 위주로 설명해주셨으니, 참고하면 좋을 것 같다.<br></p>

<p></p>
<p></p>

<p>
<h3> 1. 서버 기초 지식  </h3> <br>
<img src="https://s3.ap-northeast-2.amazonaws.com/jaehui-blog/img180606/server.png"><br><br>
<h4>정적인 웹과 동적인 웹</h4>
<ul>
  <li><strong>정적</strong>인 웹</li>
  <strong>client</strong>(user) <-> <strong>web server</strong> <br>
  서버에 <strong>미리 저장</strong>된 파일이 <strong>그대로</strong> 전달된다. <br><br>
  사용자는 서버에 저장된 데이터가 변경되지 않는 한 고정된 페이지를 보게 된다. <br><br>
  <li><strong>동적</strong>인 웹 </li>
  <strong>client</strong>(user) <-> <strong>web server</strong> <-> <strong>application server</strong> <br>
  서버는 사용자의 요청을 해석하여 데이터를 가공한 후 생성되는 웹페이지를 보여준다. <br><br>
  사용자는 <strong>상황, 시간, 요청 등에 따라 달라</strong>지는 웹페이지를 보게 된다. <br>
  로그인 후 사용자 정보 변경, 캐싱 등이 필요할 때 사용한다. 
</ul><br></p>

<p>
<h4>Socket(process)과 HTTP(web)</h4>
통신 방식을 두 분류로 구분할 수 있는데, 가장 큰 차이점은 <strong>접속</strong>을 유지하는지의 여부이다. <br>
<ul>
  <li><strong>Socket</strong></li>
  <strong>양방향</strong> 통신이 가능하다. 즉, 주고 받는 것이 가능! <br>
  연결 유지, 통신 대기가 가능하다. <br><br>
  <li> <strong> HTTP </strong></li>
  <strong>일회성</strong> 통신만 가능하다. 보내거나, 받거나, 일회성으로 통신을 한다. <br>
  GET, POST 등의 명령을 하면 <strong>Request->, <-response 후 연결이 끊겨</strong> 버리기 때문에 <strong>소통이 불가능</strong>하다.
</ul><br><br>
</p>

<p>
<h3>2. Slack  </h3><br>
<img src="https://s3.ap-northeast-2.amazonaws.com/jaehui-blog/img180606/slack.png"><br><br>
<ol>
  <li><strong>업무와 일상 분할</strong>이 가능하다.</li>
  퇴근 후 또는 여가 생활 중 카톡으로 일적인 사진이나 문서를 받을 때의, 그 말로 형용할 수 없는 기분에서 조금이나마 벗어날 수 있게 해주는 것 같다.<br><br>
  <li>다양한 생산성 <strong>앱을 지원</strong>해준다.</li>
  Github과 연동이 가능하고, 그 이외에도 다양한 앱과도 연동해서 사용할 수 있다. <br><br>
  <li>무료로도 꽤 <strong>많은 히스토리 보존</strong> 가능하다. </li>
  민재님께서는 이 점이 가장 좋다고 하셨다. <br><br>
  학생이라면 무료를 찾기 마련인데, 무료임에도 많은 이전 대화와 자료들을 확인할 수 있다! <br>
  <li><strong>워크스페이스(단체)</strong> 내의 <strong>채널(공지사항, 일정)</strong> 기능이 있어, 단체를 분류하고 채널 내에서 게시물의 성격에 따라 분류할 수 있다. </li><br>
  <li>웹, 모바일앱, 데스크탑앱 등의 <strong>다양한 플랫폼</strong>을 지원한다. </li><br> 
</ol>
</p>

<p>
<h3>3. Postman (서버 필수 툴)  </h3><br>
<img src="https://s3.ap-northeast-2.amazonaws.com/jaehui-blog/img180606/postman.png"><br><br>
<ol>
  <li><strong>HTTP 통신 테스트</strong> 가능하다. </li>
  HTTP는 단방향 통신이기 때문에 postman을 사용하면 매우 편리해질 수 있다.<br><br>
  <li><strong>HTTP Request와 Response를 저장</strong>해둘 수 있다. </li>
  결과를 저장해두면 앱 개발자들이 <strong>서버의 기능을 확인</strong>할 수 있다 ! <br>
  서버의 기능을 명시할 수 있기 때문에 가능하다.<br><br>
  <li><strong>컬렉션(워크스페이스), 폴더(채널) 기능</strong>이 있다. </li><br>
  <li> 컬렉션 공유가 가능하다. </li> <br>
  <li><strong>mockup 서버</strong> 구축이 가능하다. </li>
  mockup 서버란 간단한 작업을 위해 가상의 서버에서 작업하는 것을 말한다. <br><br>
  <li><strong>문서 생성</strong> 기능이 있다. </li>
  <strong>가독성</strong>이 굉장히 높고 레이아웃이 깔끔하다! <br><br>
  <li>서버 테스트 기능이 있다. </li><br>
</p>

<p>
<h3>4. Github  </h3><br>
<img src="https://s3.ap-northeast-2.amazonaws.com/jaehui-blog/img180606/github.png"><br><br>
<ol>
  <li><strong>버전 관리</strong>가 가능하다.</li>
  이로써 우리가 얻을 수 있는 장점은 <strong>버그를 대처</strong>할 수 있다는 것이다. <br>
  새로운 버전에서 치명적인 버그가 발생되면 우리는 Github으로 복원할 수 있다.<br><br>
  <li><strong>협업</strong>이 편리하다. </li>
  <strong>Branch</strong>를 이용하면 각자 맡은 부분은 개발하고 합칠 수 있는 <strong>merge</strong>라는 기능이 존재한다. 
  하지만 같은 파일은 수정했을 경우에는 <strong>conflict</strong>가 발생할 수 있으므로 유의해야 한다. <br><br>
  <li><strong>Issues(버그, 기능, 문의)</strong>관리를 할 수 있다. </li>
  이 장점 또한 협업에서 유리하다.<br>
  <ul>
    <li> 개발자(dev), 사용자(user) 모두 작성 가능하다.</li>
    <li> <strong>버그와 함께 commit</strong>을 할 수 있고, 그 issue를 언제까지 마쳐야하는지 일정(기한)도 함께 올릴 수 있다. </li>
    <li> 버그, 개발 예정, 추가기능, 건의사항 등을 관리하는 기능으로 아주 유용하다.</li>
  </ul>
  <li>Milestone로 Issues를 결합하여 마감일을 정하는 등의 활용이 가능하다. </li><br>
  <li>터미널에서 commit과 함께 issue 완료 처리를 하려면 다음과 같은 명령어를 입력하면 된다. </li>
</ol>
</p>

```css
   git commit -m "fix #1"
```

<p>
Github는 Git을 사용할 수 있는 툴이다. <br>
따라서 <strong>Git 명령어</strong>를 알아야한다. <br><br>
<a href="https://www.sourcetreeapp.com" target="_blank" title="SourceTree">SourceTree</a>와 같이 관리할 수 있는 툴이 있지만 모든 기능을 포함하고 있진 않기 때문에 Git 명령어를 알아두면 좋다! <br>
<ul> 
  <li> init </li>
  git repository 생성 <br><br>
  <li> local / remote </li>
  사용자의 컴퓨터 / git 서버  <br><br>
  <li> commit  </li>
  변경된 내용을 comment와 함께 snapshot을 남김  <br><br>
  <li><strong>push</strong></li>
  local의 commits을 remote에 반영  <br><br>
  <li><strong>pull</strong></li>
  remote의 commits을 local에 반영<br><br>
  <li>fetch</li>  
  remote의 commits을 local로 그대로 가져옴 <br><br>
  <li>branch </li>
  서로 다른 원본을 가지는 commits <br><br>
  <li>clone </li>
  local에 repository 복제  <br><br>
  <li>merge   </li>
  branch 혹은 commit 간의 내용이 다른 부분을 합침 (하나의 commit)  <br><br>
  <li>fork </li>
  github에 다른 사람의 repository를 복사하는 것이다. 해당 repository가 업데이트 되면 바로 반영할 수 있다.<br><br>
  <li>stash  </li>
  commit으로 만들지 않은 변경 내용을 임시로 저장하는 기능으로, merge를 원하지 않을 때 사용한다. <br>
  이 명령어를 이용하면 충돌을 피할 수 있다.<br><br>
  <li><strong>revert</strong></li> 
  삭제하고 싶은 commit의 이전 commit을 불러올 수 있다. 
</ul></p>

```css
git revert <commit number>
```

<p>
위 명령어를 입력하면 revert commit message 작성하여 이전의 commit을 새롭게 commit 한다.<br>
<ul>
  <li><strong>reset</strong></li> 
  이전 commit 상태로 초기화하는 것이다.<br>
</ul></p>

```css
git reset --hard <commit number>
```

<p>
라는 명령어를 입력하여 해당 commit으로 초기화하는 기능이다. <br>
<ul>
  <li>conflict </li>
  merge 시 remote와 local의 commits가 일치하지 않는 경우 conflict가 발생한다. <br>
  branch 간의 내용이 달라 auto merge가 되지 않는다. <br>
  이 경우에는 수동으로 merge 작업을 해줘야한다. 아래와 같이 충돌이 난다.<br>
</ul></p>

```css
<<(왼쪽 꺽쇠)...<< HEAD
aaa 
=====
bbb
(오른쪽 꺽쇠)>>>>
```

<p>
  aaa 내용과 bbb 내용 둘중에 원하는 내용만 남겨두고 삭제하면 된다.<br>
<ul>
  <ul>
  <li>diff  </li>
  local의 commit과 다른 파일들을 다 보여줌  <br>
  <li>status </li>
  수정된 파일들을 보여줌  <br>
  <li>rebase  </li>
  merge랑 비슷한 개념으로, commit을 병합하고 commit message를 수정할 수 있다.<br>
  </ul>
</ul>
</p>

```css
rebase -i HEAD~4
```

<p>
  라는 명령어를 사용하여 최근 4개의 commit을 볼 수 있다.
</p>

```css
pick
pick
pick
sqush // -> 위의 commit과 병합됨
```

<p>
  이 때 sqush라는 명령어를 쓰면 바로 위에 있는 commit 과 해당 commit이 병합된다.
</p>

<p>
<h4>직접 해보기</h4> <br>
<img src="https://s3.ap-northeast-2.amazonaws.com/jaehui-blog/img180606/terminal.jpeg"><br><br>
<ul>
  <li>새로운 repository 만들기  </li>
  <ol>
    <li>local에 폴더 만들기</li>
    <li>teminal에서 해당 폴더로 이동한다.</li>
  </ol>
</ul>
</p>

```css
git init
```

<p>
  폴더 안의 수정 사항 발생하면 untracked files 이 생겼을 것이다.<br>
</p>


```css
git add .
git commit -m "commit message"
git remote add origin <repository 주소>
git push -u origin master
```

<p>
이처럼 하게 되면 origin에 master라는 branch가 생성된다.
</p>


<p>
<ul>
  <li>pull</li>
  <ol>
    <li>repository에서 수정을 하게 되면 local과 remote의 내용의 차이가 생긴다.</li>
    <li>teminal 해당 폴더에서</li>
  </ol>
</ul>
</p>

```css
git pull
```

<p>
<ul>
  <li>remote와 local에서 같은 파일 수정한다. 이 때 2가지 경우가 발생한다.</li>
  <ol>
    <li>conflict 발생 -> 수정</li>
    <li>auto merge</li>
  </ol>
</ul>
</p>

<p>
<h3>5. Waffle (Issues 관리 도구)</h3>
<ol>
  <li>여러 프로젝트의 Issues를 한번에 볼 수 있다. </li>
  github에서는 각각 repository별로만 관리 가능해서 같은 어플리케이션이라도 iOS, Android, Server의 Issues를 한번에 관리할 수 없는데, Waffle을 사용하면 가능하다.<br><br>
  <li>팀 프로젝트에서 ios, android, server 의 Issues를 한번에 관리할 수 있기 때문에 편리하다.</li>
</ol></p>


