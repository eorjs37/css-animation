# css animation

## * 애니메이션 속성 정의

### animation-delay
> 애니메이션을 시작할 시점 (몇초후에 시작할지)
```css
animation-delay: 250ms;
```
### animation-direction
> 애니메이션이 종료되고 다시 정방향으로 할지 역방향으로 할지 설정

```css
animation-direction: normal;
```

### animation-duration
> 애니메이션이 한 사이클 완료하는데 걸리는 시간
```css
animation-duration: 3s;
```

### animation-iteration-count
> 애니메이션 반복 횟수 infinite도 가능
```css
animation-iteration-count: infinite;
```

### animation-name
> 애니메이션의 중간상태를 지정
```css
animation-name: slide;

@keyframes slide {
    from {
        margin: 0;
    }

    to {
        margin-left: 250px;
    }
}
```

### animation-timing-function
> 애니메이션 중간 중간 속도의 조절
```css
animation-timing-function: ease-out;
```

## 웹 브라우저 UI 방식

### 1.Recalculate Style
> 요소에 적용할 스타일 계산
### 2.Layout
> 요소에 레이아웃 생성 및 화면에 배치
### 3.Paint
> 생성된 레이아웃에 픽셀 추가
### 4.Composite Layers
> 생성한 레이어 계층을 합성


### top을 썼을 때와 transform 썼을때 차이
> top을 사용해서 애니메이션을 구현할 경우 Schedule Style Recalculation,Recalculate Style,Layout 이 반복중이지만, transform을 사용했을 때는 Schedule Style Recalculation,Recalculate Style,Layout 을 반복하지 않는다.
