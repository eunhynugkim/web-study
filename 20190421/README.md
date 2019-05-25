# 20190420 1주차 학습 정리

## 1.git 절차
- working directory -> add -> commit -> local repository -> push -> git의 repository
   
- commit : 수정 내역을 사용자 기준 단위로 기록
- branch : 내 원래 소스코드와 독립된 작업 공간
- checkout : branch간의 이동
- merge: branch와 branch를 병합


## 2.commit을 해서 반영되는 저장소는?
local repository


## 3. md file 이란?
<li> markdown - 텍스트 기반의 마크업 언어로 HTML로 변환이 가능하다.</li>
<br/>
3-1.장점:

-간결하다. <br/>
-별도의 도구없이 작성가능하다. <br/>
-다양한 형태로 변환이 가능하다. <br/>
-텍스트로 저장되기 때문에 용량이 적어 보관이 용이 <br/>
<br/>
3-2.단점:<br/>
-표준이 없다. <br/>
-모든 HTML 마크업을 대신하지 못한다.<br/>

## 4.HTML이란? <br>
- hypertext markup language

<li> link가 가능한 텍스트로 이루어진 markup language </li>

### 4-1. HTML의 작동 절차
1. DOCTYPE읽어들인다.
2. webbrowser에서 실행한다.
3. DOM TREE 생성
4. CSSOM 생성
5. Mixed

## 5. self - closed tag?
```html
<meta />
<hr />
<input />
<link /> 
```
## 7. CSS 적용방법 3가지
<li> in-line stylesheet </li>
<li> internal stylesheet </li>
<li> external stylesheet </li>

## 8. 색상적용 3가지
- 단어로 표현
- rgb
- 16진수 표기 <br>
(#00ff00 -> 00=>0~255가지 ff=>0~255가지 00=>0~255가지)~

## 9. selector란?
- element의 style을 지정할 대상을 선택

## 10. CSS우선순위
1. !important
2. in-line
3. id
4. class
5. tag name

## 11.wild-card 사용방법
ex) h3 * -> h3 하위의 모든 tag 선택

### 12. html과 xhtml 차이점
- XHTML이 XML 문법을 따르므로 HTML과 문법 규칙이 약간 다르다. <br/>
- XHTML을 사용하면 할 수 있으나, HTML로는 불가능한 일이 있다. <br/>
- HTML을 사용하면 할 수 있으나, XHTML로는 불가능한 일이 있다. <br/>
- CSS를 이해하는 방식에 차이가 있다. <br/>
- 클라이언트 쪽의 스크립트(예: 자바 스크립트)를 다루는 방식에 차이가 있다. <br/>


