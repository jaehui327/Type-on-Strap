---
layout: post
title: WEB1- HTML & Internet
tags: [Dev, WEB, HTML]
---

생활코딩 - WEBn  

[생활코딩 바로가기](https://opentutorials.org/course/3083)  

### 1. HTML란  
**1. 쉽다**  
**2. 중요하다**  
쉽다고 사소하고 하찮다고 생각하지 마세요. 쉬운 것이 가장 중요하고 기본적인 것입니다.  

- search `html editor`  
  [atom 설치하기](https://atom.io/)  
  
### 2. 태그  
1. 강조하기
```html
Hypertext Markup Language (HTML) is the standard markup language for <strong>creating web pages</strong> and web applications.
```
2. 밑줄(언더라인)
```html
Hypertext Markup Language (HTML) is the standard markup language for <strong>creating <u>web</u> pages</strong> and web applications.
```

### 3. 태그 추측해보기   
```html
<h1>W3C</h1>
```
* search `HTML h1 tag`   
[검색 결과 보기](https://www.w3schools.com/tags/tag_hn.asp)  
* heading 은 `제목` !  
* 검색을 통해 빠르게 정보를 알아낼 수 있다면 이미 알고 있는 정보나 다름없습니다. 검색을 두려워 하지 마세요.  

### 4. 통계에 기반한 학습  
* HTML tag는 약 150개, *다 외워야 할까요?*  
  [구글에서 웹페이지를 분석한 결과](https://advancedwebranking.com/html/)  
  통계에 따르면 26개 정도의 태그를 사용하는 웹 사이트가 가장 많습니다.  
  150개를 전부 다 외우려고 할 필요가 없습니다.  
* 중국어 공부를 하려고 할 때, *그 많은 한자를 다 외워야 할까요?*  
  * search `frequency of chinese words`  
    [검색 결과](http://lingua.mtsu.edu/chinese-computing/statistics/char/list.php?Which=MO)  
  1등은 的자입니다.  
  1000번째 단어가 2미터 키를 가진 사람이라면 적자는 세계에서 10번째로 높은 빌딩의 높이와 비슷합니다.  
  8000번째 단어가 2미터 키를 가진 사람이라면 적자는 지구의 지름보다 3000km 더 깁니다.  
* 공부를 할 때, 통계를 기반으로 공부방향을 스스로 설정해보는건 어떨까요?  

### 5. 줄바꿈  
1. `<br>`   
   무엇인가를 설명하지 않는 태그들은 감싸야하는 컨텐츠가 없기 때문에 태그를 닫지 않는다는 규칙이 있습니다.  
2. `<p></p>`  
   단락(paragraph)을 표현하는 태그입니다.  
   하나의 단락을 그룹핑할 수 있도록 열고, 닫는 태그가 존재합니다.  
   * 단락을 사용할 때 p 태그가더 좋은 선택입니다. 단락에 단락 태그를 사용하는 것이 웹페이지를 정보로서 보다 가치있게 해 주기 때문입니다.  
   * CSS를 이용하면 p태그의 한계를 극복할 수 있습니다.  
```html
<p style="margin-top:45px;">
```

### 6. 부모자식과 목록  
* `<ul>` (unordered list)  
  다른 목록과 구분할 수 있도록 경계가 필요할 때 사용합니다.  
```html
<ul>
  <li>1. HTML</li>
  <li>2. CSS</li>
  <li>3. JavaScript</li>
</ul>
<ul>
  <li>egoing</li>
  <li>k8805</li>
  <li>sorialgi</li>
</ul>
```

li 태그는 ul 태그를 꼭 필요로 합니다. ul 태그 역시 li 태그가 없다면 존재 가치가 없습니다. 이 둘은 서로 아주 밀접한 관계입니다.  
* `<ol>` (ordered list)
```html
<ol>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ol>
```

### 7. 문서의 구조와 슈퍼스타들  
```html
<title>WEB1 - html</title>
<meta charset="utf-8">
```
제목을 나타내주는 <title> 태그와 한글이 깨지지 않도록 웹페이지를 UTF-8 방식으로 열도록 하는 <meta charset> 태그입니다.
이 코드들은 본문이 아니고, 본문을 설명합니다.  
본문과 본문을 설명하는 코드를 분리하기 위해 본문은 body 태그로, 본문을 설명하는 태그는 head 태그를 사용합니다.  
또 body 태그와 head 태그를 감싸는 하나의 태그, html 태그로 전체를 감싸줍니다.  
또 이 웹페이지가 HTML로서 만들어졌다는 것을 표현하기 위해서  문서의 시작에 <!doctype html>를 추가합니다. 

```html
<!doctype html>
<html>
<head>
  <title>WEB1 - html</title>
  <meta charset="utf-8">
</head>
<body>
  <ol>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
  </ol>
  <h1>HTML</h1>
  <p>Hypertext Markup Language (HTML) is the standard markup language for <strong>creating <u>web</u> pages</strong> and web applications.Web browsers receive HTML documents from a web server or from local storage and render them into multimedia web pages. HTML describes the structure of a web page semantically and originally included cues for the appearance of the document.
  <img src="coding.jpg" width="100%">
  </p><p style="margin-top:45px;">HTML elements are the building blocks of HTML pages. With HTML constructs, images and other objects, such as interactive forms, may be embedded into the rendered page. It provides a means to create structured documents by denoting structural semantics for text such as headings, paragraphs, lists, links, quotes and other items. HTML elements are delineated by tags, written using angle brackets.
  </p>
</body>
</html>
```

* 공부를 하면 이렇게 눈이 밝아지고 시력이 좋아집니다. 예전에는 보이지 않았던 것이 보입니다.  

### 8. 링크  
```html
<a href="https://www.w3.org/TR/html5/" target="_blank" title="html5 specification">Hypertext Markup Language (HTML)</a>
```
### 9. 원시웹  
[세계 최초의 웹페이지](http://info.cern.ch)  

