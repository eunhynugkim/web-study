# 20190616 6주차 학습 정리
## dom-tree
```
var span = document.createElement("span");
span.appendChild(document.createTextNode("저는 text-container입니다."));
span.appendChild(document.createElement("p"));
document.createTextNode("저는 text-container입니다.");
```
## 결과 
![dom](dom.PNG)