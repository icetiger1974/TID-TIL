# CSS 속성
1. [width, height](#width,-height)
2. [margin, padding ](#margin,-padding )

<hr>

## width, height
`width`와 `height` 속성은 각각 가로 길이, 세로 길이를 의미한다.

값을 정의 할때는 `100px` 처럼 숫자 뒤에 단위를 표시하여 작성한다.

예시 코드

```css
div { 
    width: 100px; height: 60px 
}
```

## margin, padding 

`margin`과 `padding` 속성은 각각 바깥쪽 여백, 안쪽 여백을 의미한다.
`width`, `height` 속성과 마찬가지로 숫자 뒤에 단위를 표시하여 적는다.

`margin`과 `padding`는 `border` 을 경계로 나뉜다.

#### 방향
방향마다 여백을 다르게 설정할 수 있습니다.

- margin: 20px 같은 표현은 상하좌우 모두 20px을 의미한다.
- margin: 30px 10px은 상하 30px, 좌우 10px을 의미한다.
- margin: 30px 10px 20px 50px은 위 30px, 오른쪽 10px, 아래 20px, 왼쪽 50px을 의미한다.
- margin: 30px 10px 40px은 위 30px, 좌우 10px, 아래 40px을 의미한다.
즉 방향의 위부터 시계방향으로 회전하여 위 오른쪽 아래 왼쪽 순서로 설정한다.

> margin과 padding은 top, bottom, left, right 로 상 하 좌 우를 각각 지정할 수 있다.

예시 코드
```css
#box{ 
    margin: 10px;
    padding: 20px ;
}
.Container{ 
    margin-top: 15px;
    padding-left: 50px;
    padding-right: 40px;
}
```