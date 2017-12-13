나만의 MarkDown(마크다운) 사용법(ver0.4)
========================================

MarkDown을 처음 사용기
----------------------

MarkDown이라함은 Git을 사용하는 사람들은 누구나 보고있다. 처음 들어가는 화면만 보아도 README라는 파일이름의 .md파일이 존재한다. 그렇다 바로 그것이 MarkDown파일 확장자명이다. 그렇담 우리가 이렇게 보는 MarkDown파일은 어떻게 작성하는 것인가?

마크다운이란?
-------------

1.	마크다운(markdown)은 일반 텍스트 문서의 양식을 편집하는 문법이다[1]. README 파일이나 온새라인 문서, 혹은 일반 텍스트 편집기로 문서 양식을 편집할 때 쓰인다. 마크다운을 이용해 작성된 문서는 쉽게 HTML 등 다른 문서형태로 변환이 가능하다.

2.	존 그루버는 2004년에 문법 면에서 에런 스워츠와 중대한 협업을 통해 마크다운 언어를 만들었으며, 사람들이 읽기 쉽고 쓰기 쉬운 플레인 텍스트 포맷을 사용하여 쓸 수 있으면서 구조적으로 유효한 XHTML(또는 HTML)로 선택적 변환이 가능하게 하는 것이 목표이다.

> [참조 위키피디아 : 마크다운](http://https://ko.wikipedia.org/wiki/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4)

마크다운 사용법(문법)
---------------------

### Headers(헤더)

-	흔히 제목을 적을 때 사용하는 문법이다.
	-	큰제목 : 문서 제목(ex. 나만의 MarkDown(마크다운) 사용법
	-	작은제목 : 문서 부제목 (ex. 마크다운이란?, 마크다운 사용법(문법))
	-	글머리 : 1 ~ 6까지만 지원을 한다. (HTML의 H1~H6와 비슷)

#### 1. 큰제목

-	가장 큰 제목을 쓰는 경우 흔히 1번만 사용한다.<pre><code>나만의 MarkDown(마크다운) 사용법 <br>================================</code></pre>

#### 2. 작은제목

-	큰 제목 다음으로 분류를 할때 사용한다.<pre><code>마크다운이란?<br> -------------</code></pre>

#### 3. 글머리

-	HTML을 공부를 하셨다면 H1 ~ H6이라고 생각하면 쉽습니다.
-	1~6까지만 지원을 합니다.
-	Code가 보이는 곳은 작게 보이지만 실제로 실행해보면 크기가 다릅니다.(#을 적고 한칸 띄어야 합니다.)<pre><code># This is a H1 <br>## This is a H2 <br> ### This is a H3 <br> #### This is a H4 <br> ##### This is a H5 <br> ###### This is a H6 <br></code></pre>

### BlockQuote(인용구)

-	다른 사람이 말한 것을 차용할때 사용합니다.
-	<code>\></code> 를 사용해서 표현합니다.
-	<code>\> ></code> <code>\> > ></code>단계적으로 깊이 사용할 수 있습니다.
-	인용문구 안에서 마크다운 요소를 포함할 수 있습니다.<pre><code> > This is a blockquote</code></pre>

-	예시_스티브잡스 9가지 명언

	> 1.	우주를 놀라게 하자!
	> 2.	해군이 아니라 해적이 되어라!
	> 3.	평생 설탕물만 팔건가요?
	> 4.	나의 비즈니스 모델은 비틀즈다.
	> 5.	창의력은 연결하는 능력이다.
	> 6.	좋아하는 일을 해라!
	> 7.	항상 갈망하라, 무모할 만큼!!
	> 8.	죽음을 상기하라.
	> 9.	여정은 보상이다.

[참조 : 스티브잡스 9가지 명언](http://bonlivre.tistory.com/382)

### 목록

-	순서가 있는 목록(번호)
-	순서가 없는 목록(글머리 기호)

#### 순서가 있는 목록(번호)

-	순서있는 목록은 숫자와 점을 사용합니다.
-	순서를 변경해서 적더라도 자동으로 내림차순으로 만들어 줍니다.

```
1. 첫번째
  3. 두번째
2. 세번째
```

예시

1.	첫번째
	1.	두번째
2.	세번째

#### 순서가 없는 목록(글머리 기호)

-	<code>\*</code>, <code>\+</code>, <code>\-</code> 중에서 어느 것을 사용해도 적용이 됩니다.
-	혼합을 해서 사용해도 적용이 됩니다.

```
* 첫번째
  + 두번째
- 세번째
```

예시

-	첫번째
	-	두번째
-	세번째

### 코드

-	`<pre></pre>` 또는 `<code></code>`를 사용해서 표현합니다.
-	간락하게 <code>\`\`</code>(백틱)을 사용합니다.
-	다수의 줄을 입력할 경우 <code>\`\`\`</code> (코드입력 공간) <code>\`\`\`</code>을 사용합니다.

```
This is a code block.
```

### 수평선

-	아래의 코드들은 수평선을 만듭니다.
-	마크다운 무서를 미리보기로 출력할때 페이지 나누기 용도로 사용됩니다.

```
***
* * *
---
--------------
___
```

### 링크

-	다른 페이지로 이동할 수 있도록 해줍니다.
	-	참조 링크
	-	인라인 링크
	-	자동연결

#### 참조링크

```
[link keyword][id]

Link: [Google][googlelink]
```

#### 인라인 링크(기본 링크)

```
syntax: [Title](link)
```

#### 자동연결

```
<http://example.com/>
<abcd@example.com>
```

### 강조

-	내가 강조하고 싶은 한부분을 진하게, 기울이기, 중간라인 등등을 할 수 있습니다.

```
**rendered as bold text**
_rendered as italicized text_
~~Strike through this text.~~
```

-	**rendered as bold text**
-	*rendered as italicized text*
-	~~Strike through this text.~~

### 이미지

```
![Alt text](/img/test/imgName.jpg)
![Alt text](/img/test/imgName.jpg "Optional title")
```

![testImg](/img/test/imgName.jpg)

참조문서
--------

-	[[공통] 마크다운 markdown 작성법 ](https://gist.github.com/ihoneymon/652be052a0727ad59601)
-	[스티브잡스의 9가지 명언](http://bonlivre.tistory.com/382)
-	[MarkDown Cheatsheet](http://assemble.io/docs/Cheatsheet-Markdown.html)
