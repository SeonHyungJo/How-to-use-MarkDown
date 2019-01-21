# How to use Markdown(ver 1.0) :pencil2:

<div align=center>

![Main_image](./asset/images/Markdown.png)

</div>

<br/>

## MarkDown 처음 사용기

MarkDown이라함은 Git을 사용하는 사람들은 누구나 보고있다. 현재 지금 이 글을 읽고 있는 당신도 이미 경험을 하고 있다.
<br/>
현재 파일명만 보아도 간단하게 알 수있다. `README`라는 파일이름의 `.md` 확장자를 가진 파일이 존재한다. `README`라는 파일이름은 GitHub에서 기본으로 보여줄 MarkDown의 파일이름이다.
<br/>
그렇다면 우리가 이렇게 보는 MarkDown파일은 어떻게 작성하는 것인가?
<br/>

## 마크다운이란

1. 마크다운(Markdown)은 일반 텍스트 문서의 양식을 편집하는 문법이다. README 파일이나 온새라인 문서, 혹은 일반 텍스트 편집기로 문서 양식을 편집할 때 쓰인다. 마크다운을 이용해 작성된 문서는 쉽게 HTML 등 다른 문서형태로 변환이 가능하다.
2. 존 그루버는 2004년에 문법 면에서 에런 스워츠와 중대한 협업을 통해 마크다운 언어를 만들었으며, 사람들이 읽기 쉽고 쓰기 쉬운 플레인 텍스트 포맷을 사용하여 쓸 수 있으면서 구조적으로 유효한 XHTML(또는 HTML)로 선택적 변환이 가능하게 하는 것이 목표였다고 한다.

<br/>

> [참조 위키피디아 : Markdown](http://https://ko.wikipedia.org/wiki/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4)

<br/>

## 마크다운 사용법(문법)

### Contents

- [Headers](#headers)
- [글머리](#글머리)
- [BlockQuote(인용구)](#BlockQuote)
- [목록(List)](#목록)
- [코드(Code)](#코드)
- [수평선](#수평선)
- [링크(Link)](#링크)
- [강조](#강조)
- [이미지](#이미지)
- [테이블](#테이블)
- [숨김, 열림](#숨김-열림)


## Headers

- 흔히 **제목을 적을 때 사용하는 문법** 이다.
- 큰제목 : 문서 제목(ex. How to use Markdown)
- 작은제목 : 문서 부제목 (ex. 마크다운이란?, 마크다운 사용법(문법)등등)
- 글머리 : 1 ~ 6까지만 지원을 한다. (HTML의 H1~H6와 비슷)

<br/>

### 큰제목

- 가장 큰 제목을 쓰는 경우 흔히 한 번만 사용한다.

```md
  // Version 0.70이상에서는 이 페이지에서 사용하지 않음
  나만의 MarkDown(마크다운) 사용법
  ===============================
```

하지만 이 방법보다는 `#` 하나를 사용하는 방법을 추천하고 싶다.

:point_right: **Example**

나만의 MarkDown(마크다운) 사용법
===============================

---

### 작은제목

- 큰 제목 다음으로 분류를 할때 사용한다.

```md
  // Version 0.70이상에서는 이 페이지에서 사용하지 않음
  마크다운이란?
  -------------
```

하지만 이 방법보다는 `#` 두 개 사용하는 방법을 추천하고 싶다.

:point_right: **Example**

마크다운이란?
-------------

---

### 글머리

- HTML을 공부를 하셨다면 **H1 ~ H6**이라고 생각하면 쉽습니다.
- 1 ~ 6까지만 지원을 합니다.
- Code가 보이는 곳은 작게 보이지만 실제로 실행해보면 크기가 다릅니다.( `#` 을 적고 한칸 띄어야 합니다.)

```md
  # This is a H1
  ## This is a H2
  ### This is a H3
  #### This is a H4
  ##### This is a H5
  ###### This is a H6
```

:point_right: **Example**

# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6

<br/>

---

## BlockQuote

- 다른 사람이 말한 것을 차용할때 사용합니다.
- `>` 를 사용해서 표현합니다.
- `>` `>>` `>>>` 단계적으로 깊이 사용할 수 있습니다.
- 인용문구 안에서 마크다운 요소를 포함할 수 있습니다.

```md
  > 1. 우주를 놀라게 하자!
  > 2. 해군이 아니라 해적이 되어라!
  > 3. 평생 설탕물만 팔건가요?
  > 4. 나의 비즈니스 모델은 비틀즈다.
  > 5. 창의력은 연결하는 능력이다.
  > 6. 좋아하는 일을 해라!
  > 7. 항상 갈망하라, 무모할 만큼!!
  > 8. 죽음을 상기하라.
  > 9. 여정은 보상이다.
```

:point_right: **Example**

> 1. 우주를 놀라게 하자!
>> 2. 해군이 아니라 해적이 되어라!
>>> 3. 평생 설탕물만 팔건가요?
> 4. 나의 비즈니스 모델은 비틀즈다.
> 5. 창의력은 연결하는 능력이다.
> 6. 좋아하는 일을 해라!
> 7. 항상 갈망하라, 무모할 만큼!!
> 8. 죽음을 상기하라.
> 9. 여정은 보상이다.

[참조 : 스티브잡스 9가지 명언](http://bonlivre.tistory.com/382)
<br/>

---

## 목록

- 순서가 있는 목록(번호)
- 순서가 없는 목록(글머리 기호)

<br/>

### 1. 순서가 있는 목록(번호)

- 순서있는 목록은 숫자와 점을 사용합니다.
- 순서를 변경해서 적더라도 자동으로 내림차순으로 만들어 줍니다.

```
1. 첫번째
  1. 첫번째 안에 첫번째
2. 세번째
```

:point_right: **Example**

1. 첫번째
	1. 첫번째 안에 첫번째
2. 세번째

<br/>

---

### 2. 순서가 없는 목록(글머리 기호)

- `*`, `+`, `-` 중에서 어느 것을 사용해도 적용이 됩니다.
- 혼합을 해서 사용해도 적용이 됩니다.

```

* 첫번째
  + 첫번째 안에 첫번째
- 세번째

```

:point_right: **Example**

* 첫번째
	+ 첫번째 안에 첫번째
- 세번째

<br/>

## 코드

- `<pre></pre>` 또는 `<code></code>`를 사용해서 표현합니다.
- 간락하게 <code>\`\`</code>(백틱)을 사용합니다.
- 다수의 줄을 입력할 경우 <code>\`\`\`</code> (코드입력 공간) <code>\`\`\`</code>을 사용합니다.

```md
  \```
    This is a code block.
  \```
```

:point_right: **Example**

```
  This is a code block.
```

---

## 수평선

- 아래의 코드들은 **수평선**을 만듭니다.
- 마크다운 문서를 미리보기로 출력할때 페이지 나누기 용도로 사용됩니다.

```md
  ***
  * * *
  ---
  --------------
  ___
```

:point_right: **Example**

***
* * *
---
--------------
___

<br/>

---

## 링크

- 다른 페이지로 이동할 수 있도록 해줍니다.
- 참조 링크
- 인라인 링크
- 자동연결

### 1. 참조링크

```md
  [link keyword][id]
  Link: [Google][googlelink]
```

### 2. 인라인 링크

```md
  syntax: [Title](link)
```

:point_right: **Example**

[Google](https://www.google.com/)

### 3. 자동연결

```md
  <http://example.com/>
  <abcd@example.com>
```

:point_right: **Example**

<https://www.google.com/>

### 목차 만들기(링크 활용)

링크를 응용해서 한페이지 내에서 이동하는 목차를 만들겠습니다.

- [MarkDown 처음 사용기](#MarkDown-처음-사용기)
- [참조링크](#1.-참조링크)
- [인라인 링크](#2.-인라인-링크)
- [자동연결](#3.-자동연결)

만들때 주의할 점은 띄어쓰기는 `-`로 대체합니다.

---

## 강조

- 내가 강조하고 싶은 한부분을 진하게, 기울이기, 중간라인 등등을 할 수 있습니다.

```md
  **rendered as bold text**
  _rendered as italicized text_
  ~~Strike through this text.~~
```

:point_right: **Example**

- **rendered as bold text**
- *rendered as italicized text*
- ~~Strike through this text.~~

---

## 이미지

```md
![Alt text](/asset/images/imgName.jpg)
![Alt text](/asset/images/imgName.jpg "Optional title")
```

:point_right: **Example**

![테스트 이미지](https://github.com/SeonHyungJo/How_to_use_MarkDown/blob/master/asset/images/testName.jpg?raw=true "Optional title")

---

## 테이블

- 테이블은 필요하더라...
- 테이블을 그리는 방법
- header 그리는 방법
- 왼쪽 정렬, 오른쪽 정렬, 가운데 정렬을 하는 방법

### 1. 테이블 그리기

- 기본적으로 열을 나누는 방법은 `|`을 사용하는 방법이다.(`\`\_역슬레쉬 위에 있는 문자)

```

|기본적으로|역슬래쉬로|구간나누기|

```

:point_right: **Example**

| 기본적으로 |역슬래쉬로|구간나누기|

- 그러나 그냥 한 줄만 작성할 경우 테이블이 생기지 않는다.

```

|기본적으로|역슬래쉬로|구간나누기|
|-|-|-|

```

:point_right: **Example**

| 기본적으로 | 역슬래쉬로 | 구간나누기 |
|-|-|-|

<br/>

- 위의 내용처럼 하단에 행 수만큼의 `-`를 적어주게 되면 그때부터 테이블이 생성되기 시작한다.
- `-`을 기준으로 위에는 **header가** 되며 아래는 내용들이 된다.

:point_right: **Example**

```

| 기본적으로 | 역슬래쉬로 | 구간나누기 |
|-|-|-|
|왼쪽|가운데|오른쪽|
|왼쪽2|가운데2|오른쪽2|

```

:point_right: **Example**

| 기본적으로 | 역슬래쉬로 | 구간나누기 |
|-|-|-|
|왼쪽|가운데|오른쪽|
|왼쪽2|가운데2|오른쪽2|

<br/>

### 2. 정렬하기

- 테이블에서 잘 쓰이는 것이 정렬이다.
- 정렬의 종류는 3가지로 왼쪽, 가운데, 오른쪽 정렬이 있다.
- 정렬의 구분은 `:`를 사용해서 구분한다.
- 왼쪽 정렬 `:-`, 가운데 정렬 `:-:`, 오른쪽 정렬 `-:`이다.

```md
| 기본적으로 | 역슬래쉬로 | 구간나누기 |
|:-|:-:|-:|
|왼쪽|가운데|오른쪽|
|왼쪽2|가운데2|오른쪽2|
```

:point_right: **Example**

| 기본적으로 | 역슬래쉬로 | 구간나누기 |
| :-------- | :-------: | ---------:|
|왼쪽|가운데|오른쪽|
|왼쪽2|가운데2|오른쪽2|

<br/>

---

## 숨김, 열림

```md
<details>
<summary> 열기 </summary>

- [Memoization](https://github.com/Im-D/Dev-Docs/blob/master/Design_Pattern/Memoization.md)
- [쓰로틀링과 디바운싱](https://github.com/Im-D/Dev-Docs/blob/master/Design_Pattern/Throttle%20and%20Debounce.md)

</details>
```

:point_right: **Example**

<details>
<summary> 열기 </summary>

- [Memoization](https://github.com/Im-D/Dev-Docs/blob/master/Design_Pattern/Memoization.md)
- [쓰로틀링과 디바운싱](https://github.com/Im-D/Dev-Docs/blob/master/Design_Pattern/Throttle%20and%20Debounce.md)

</details>

<br/>

---

## YouTube

```md
  [![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/BVRcKLOEmF8/0.jpg)](http://www.youtube.com/watch?v=BVRcKLOEmF8)
```

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/BVRcKLOEmF8/0.jpg)](http://www.youtube.com/watch?v=BVRcKLOEmF8)

---

####  Reference

- [[공통] 마크다운 markdown 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601)
- [스티브잡스의 9가지 명언](http://bonlivre.tistory.com/382)
- [MarkDown Cheatsheet](http://assemble.io/docs/Cheatsheet-Markdown.html)
