<a href="./attribute1.md">이전 파일</a>

## background

`background` 속성은 태그의 배경을 지정하는 속성으로, `font `속성과 비슷하게 세부적인 속성들을 한번에 쓸 수 있는 속성이다.

- `background-color`: 배경 색
- `background-image`: 배경 이미지
- `background-repeat`: 배경 이미지 반복 여부
- `background-position`: 배경 이미지 위치

### background-color
배경색을 의미하며, 값은 `color` 속성의 포맷을 사용한다.
>태그의 크기가 없을 경우 배경색은 표기되지 않는다.

예시 코드
``` html
<style>
	#box1{
         background-color: green; 
    }
	#box2{ 
        background-color: #FF00CC; 
        width: 200px ;
    }
</style>
<div id="box1">
    상자1
</div>
<div id="box2">
    상자2
    <br>
    상자2
</div>
```

출력 결과
<img src="../../img/background_color.png">

### background-image
배경 이미지를 설정하며, 주로 이미지 경로를 지정하는 방식으로 사용합니다.
경로는 `background-image: url("이미지 경로")` 처럼 작성합니다.

>컨테이너의 크기와 상관없이 삽입된 `background-image`의 크기는 컨테이너에 맞춰 늘어나거나 줄어들지 않고 그대로 표시되며, 이미지 보다 컨테이너가 더 크다면 이미지는 반복되어 표시되게 된다.

예시 코드
```html
<style>
	#box1 {
		width: 100px;
		height: 100px;
		background-image: url("/images/attach/earth.jpg");
	}
	#box2{
		width: 300px;
		height: 150px;
		margin-top: 30px;
		background-image: url("/images/attach/earth.jpg");
	}
</style>
<div id="box1"></div>
<div id="box2"></div>
```

출력 결과
<img src="../../img/background_img.png">

### background-repeat
`background-image`로 컨테이너보다 작은 이미지를 적용하면 이미지가 반복되어 출력된다. 이때 `background-repeat` 속성을 사용하면 반복여부를 지정 할 수 있다.

예시코드
```html
<style>
	.abox{
		width: 500px;
		height: 100px;
		margin-bottom: 15px;
		background-image: url("./안드로이드 이미지");
		border: 1px solid #AAA;
	}
	#box1{ 
        background-repeat: no-repeat;
    }
	#box2{ 
        background-repeat: repeat-x; 
    }
	#box3{ 
        background-repeat: repeat-y; 
    }
	#box4{ 
        background-repeat: repeat; 
    }
</style>

<div id="box1" class="abox"></div>
<div id="box2" class="abox"></div>
<div id="box3" class="abox"></div>
<div id="box4" class="abox"></div>
```

출력 결과
<img src="../../img/background_repeat.png">

### background-position
일반적으로 `background-image` 는 왼쪽 위부터 이미지를 출력한다. `background-position` 속성을 사용하면 이미지의 좌표를 수정 할 수 있게 된다.

`margin`, `padding` 속성에서 지정했던 것과 비슷하게 띄어쓰기를 기준으로 `x좌표`, `y좌표`를 지정한다. 픽셀 뿐만 아니라 `left`, `top`, `center`, `bottom`, `right` 등의 상수도 쓸 수 있다.

```html
<style>
	.abox{
		width: 500px;
		height: 100px;
		margin-bottom: 15px;
		background-image: url("./안드로이드 이미지");
		border: 1px solid #AAA;
	}
	#box1{ 
        background-position:center center; background-repeat: no-repeat;
    }
	#box2{ 
        background-position:30px right; 
        background-repeat: repeat; 
    }
	#box3{ 
        background-position:-100px -60px; 
        background-repeat: repeat-x;
    }
	#box4{ 
        background-position:40px -90px; 
        background-repeat: repeat-y; 
    }
</style>

<div id="box1" class="abox"></div>
<div id="box2" class="abox"></div>
<div id="box3" class="abox"></div>
<div id="box4" class="abox"></div>
```

출력 결과
<img src="../../img/background_position.png">


