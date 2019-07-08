# 20190707 8주차 학습정리

##javascript 변수, 자료type

### 변수란?

- 변수의 종류

### 자료 type 

- type 종류

- 사용법 :typeof

```javascript
<script>
    var a = 10;
    console.log(a, typeof (a));

    a = '';
    console.log(a, typeof (a));

    a =" ";
    console.log(a, typeof(a));

    a= undefined;
    console.log(a, typeof(a));

    a= null;
    console.log(a, typeof(a));

    a = false;
    console.log(a, typeof(a));

    a= Infinity;
    console.log(a, typeof(a));

    a=3.141592;
    console.log(a, typeof(a));

    a = NaN;
    console.log(a, typeof(a));

    a={ };
    console.log(a, typeof(a));

    a = [];
    console.log(a, typeof(a));

    console.log('10+20',10+20,typeof(10+20));

    console.log('10+20','10'+20,typeof('10'+20));

    console.log('10+20',parseInt('10')+20,typeof(parseInt('10')+20));

    console.log('10*20',10*20,typeof(10*20));

    console.log('10*20','10'*20,typeof('10'*20));

    console.log('10*20',10*'20',typeof(10*'20'));

    console.log('10*20','10'*'20',typeof('10'*'20'));

    console.log('10/20',10/20,typeof(10/20));

    console.log('10/20','10'/20,typeof('10'/20));

    console.log('false+1',false+1,typeof(false+1));

    console.log('true+1',true+1,typeof(true+1));

    console.log('false*12',false*12,typeof(false*12));

    console.log('true*12',true*12,typeof(true*12));

    console.log('false/12',false/12,typeof(false/12));

    console.log('12/false',12/false,typeof(12/false));

    console.log('true/12',true/12,typeof(true/12));

    console.log('NaN+17',NaN+17,typeof(NaN+17));

    console.log('NaN-17',NaN-17,typeof(NaN-17));

    console.log('null+17',null+17,typeof(null+17));

    console.log('null-17',null-17,typeof(null-17));

    console.log('[]+17',[]+17,typeof([]+17));

    console.log('[]*17',[]*17,typeof([]*17));

    console.log('[]/17',[]/17,typeof([]/17));

    console.log('[]-17',[]-17,typeof([]-17));

    console.log('{}+17',{}+17,typeof({}+17));

    console.log('{}*17',{}*17,typeof({}*17));

    console.log('{}-17',{}-17,typeof({}-17));

    console.log('{}/17',{}/17,typeof({}/17));

    console.log("10=='10'",10=='10',typeof(10=='10'));

    console.log("10==='10'",10==='10',typeof(10==='10'));

    console.log('null==0',null==0,typeof(null==0));

    console.log('null===0',null===0,typeof(null===0));

    console.log('false==0',false==0,typeof(false==0));

    console.log('false===0',false===0,typeof(false===0));

    console.log('[]==0',[]==0,typeof([]==0));

    console.log('[]===0',[]===0,typeof([]===0));

    console.log('[]==[]',[]==[],typeof([]==[]));

    console.log('[]===[]',[]===[],typeof([]===[]));
    ```