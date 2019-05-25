# 20190518 4주차 학습 정리

## 1-1. tr tag
- table row의 약자.
- 가로줄을 만드는 역할을 한다.
- 사용 방법 : `<tr>`내용`</tr>`

## 1-2. th tag
- table head의 약자.
- 글씨체는 bold체로 나온다.
- 표의 제목을 만드는 역할을 한다.
- 사용 방법 : `<th>`내용`<th>`

## 1-3. td tag
- table data의 약자.
- 셀을 만드는 역할을 한다.
- 사용 방법 : `<td>`내용`</td>`

## 1-4. 사용 예시
`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
    `<meta charset="UTF-8">`
`</head>`
`<body>`
`<table border="1">
    <caption>1학년 성적표</caption>
    <colgroup>
        <col/>
        <col/>
        <col span="2"/>
    </colgroup>
    <thead>
    <tr>
        <th rowspan="2" scope="col">이름</th>
        <th rowspan="2" scope="col">학번</th>
        <th colspan="2" scope="colgroup">성적</th>
        <th rowspan="2" scope="col">등수</th>
    </tr>
    <tr>
        <th scope="col">1학기성적</th>
        <th scope="col">2학기성적</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <tr>
        <td>토리</td>
        <td>2020111111</td>
        <td>97</td>
        <td>95</td>
        <td>1</td>
    </tr>
    <tr>
        <td>토리</td>
        <td>2020111111</td>
        <td>97</td>
        <td>95</td>
        <td>1</td>
    </tr>
    <tr>
        <td>토리</td>
        <td>2020111111</td>
        <td>97</td>
        <td>95</td>
        <td>1</td>`
    `</tr>`
    `</tbody>`
    `<tfoot>`
    `<tr>`
        `<th scope="rowgroup" colspan="5">평균</th>`

    </tr>
    <tr>
        <th scope="row">1학기 평균</th>
        <td colspan="4">55</td>
    </tr>

    <tr>
        <th scope="row">2학기 평균</th>
        <td colspan="4">65</td>
    </tr>
    </tfoot>
`</table>`
`</body>`
`</html>`








------------------------------------------------------
![monospace](mono.PNG)

- 맑은고딕과 monospace 폰트를 비교했을때 monospace 폰트가 각 글자마다 일정한 간격을 유지하는것을 볼 수 있다.

## 2. semantic tag란?

- semantic : 의미의, 의미론적이라는 뜻이다.
- ```<div>```와 같은 태그는 non-semantic태그라 할 수 있고 
  ```<aside>, <section>,<header>, <footer>, <nav>, <article>``` 등의 태그는 semantic 태그라고 할 수있다.
- ```<div>``` 태그만 볼때 이 태그 안에 들어간 내용의 의미를 알 수 없지만
  ```<aside>, <article>```과 같은 태그는 안에 들어갈 내용의 의미를 유추할 수 있다.
### 2-1. semantic 태그를 이용하는 이유?
- 검색엔진이 html 파일을 분석할 때 정확하게 컨텐츠를 식별하기 위해 정해진 semantic tag를 사용하기로 규약을 정하였다.
(검색엔진들이 semantic web을 좋아한다.)

![semantic](semantic.PNG)
- 이러한 tag들을 semantic tag라고 한다.
- div와 같은 속성을 지닌다.
- 다 block이다.
- div는 semantic tag로 분류되지 않는 곳에 서 block 처리할 때 사용한다.
- div용도는 container이다. 
- inline끼리 묶여 있는 것을 흩어지지 않게 묶어준다.
## 3. HTML의 형태
- ```<tag name attribute name ="attribute value"> </tag name> ```  
- 예시: ```<h2 style="color:hotpink;background-color:purple;display:inline-block" class="green orange">aaaa</h2>```

## 4. block element, inline element, inline-block element
### 4-1. block element
- block element에는 ```<p>```가 있다. -> paragraph의 약자.
- 한 줄을 다 차지 한다. 
- 기본적으로 가로폭 전체의 넓이를 가지는 직사강형 형태가 되며
  width, height, margin, padding 등을 사용하며 크기를 변형시킬 수 있다.
  그리고 block element 다음에는 줄바꿈이 이루어진다.
  (al, ul, div, h1 태그 등이 있다.)
### 4-2. inline element
- inline element에는 <span>이 있다. -> 한 뼘을 의미함.
- 한 문장 단위를 끊을 때 사용하며 컨텐츠 크기만큼만 차지 한다.</br>
  그래서 임의로 width, height 크기를 변형시킬 수 없다.
- 그리고 inline element 다음에는 줄바꿈이 없고 우측으로 바로 이어서 표시된다.
  (img, var, span, a 태그 등이 있다.)

### 4-3. inline-block element
- inline element와 비슷하지만 width와 height를 지정할 수 있다.

- 예시:

![inline-block-ex](inline block.PNG)
 
 - 예시2:
```css

 .box {
  
	display: inline-block;
    width: 50px;
    height:50px;
	color: pink;
  }
```

## 5. DOM tree 작성 방법
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8"/>
    <title>Title</title>
</head>
<body>
    <p>저는 단락입니다.</p>
    <p>저는 두번째
        <p>저는 안에 있는 단락입니다.</p>
        <p>저는 두번째 안에 있는 두번째 단락입니다.</p>
        단락입니다.
    </p>
    <p>저는 세번째 단락입니다.</p>

</body>
</html>
```

- 결과

![dom-ex2](dom.PNG)

