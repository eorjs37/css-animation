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