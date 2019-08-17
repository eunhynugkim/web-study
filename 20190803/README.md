#20190810 정리
## positioncss posistion
- 태그들의 위치를 결정하는 css
        
## static
- 기본 값으로 static으로 지정되어 있음
순서는 차례로 왼쪽에서 오른쪽, 위에서 아래쪽으로 쌓인다.
        
## relative
 - 태그가 기존 static이었을 때의 위치를 기준으로 top, right, bottom, left 속성을 사용하여 위치 조절이 가능하다.
        
## absolute
- position:static 속성을 가지고 있지 않은 부모를 기준으로 움직인다.
- 부모 중에서 relative, absolute, fixed 태그가 존재하지 않다면 가장 위의 태그(body)가 기준이 된다.
        
## fixed
- 특정 위치에 고정되어 있으며 스크롤을 내려도 그 자리에 계속 위치한다.
        
        
## css hover  ==js의 mouseover + mouseout
        
- hover는 마우스를 올려놓았을 때 해당 속성들을 적용하고 마우스를 적용범위에서 벗어났을 때 해당속성들을 제외시킴      
- js는 mouseover를 했을 때 해당속성들을 적용하지만 마우스 적용범위를 벗어났을 때 해당 속성들을 제외시키지 않기 때문에 mouseout envent에서 해당 속성들을 제외하는 로직을 직접 작성해야한다.

  ->가급적이면 js를 사용하지 않고 hover를 구현하는 방법이 좋다.
