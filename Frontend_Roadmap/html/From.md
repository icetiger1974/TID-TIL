## Form?
HTML 에서 `<form>`이라는 요소는 사용자에게서 얻은 정보를 모으기 위해서 사용된다. 예를 들어서 네이버에 접속을 하시게 되면 아이디와 비밀번호를 입력하는 창이 있다. 사용자한테서 입력하는 그 공간이 `<form>`으로 이루어져있다고 생각하시면 된다.
<img src="../../img/form.png">
>폼, 입력 폼은 웹 프로그래밍의 기술의 하나이다. 클라이언트가 정보를 입력 · 선택하고, 웹 서버 등의 폼을 처리하는 에이전트로 제출하기 위한 기구이다.

```html 
<body>
    <form action="" method="" enctype="">
        <input type="id" name="id" />
        <input type="submit" />
    </form>
</body>
```
HTML의 form은 위의 코드와 같이 클라이언트에게 보낼 `<input/>`를 감싸는 형태로 작성된다.

form 태그에는 `action`,`method`,`enctype` 속성이 있다.
- `action` 은 데이터를 보낼 url 주소를 정한다.
- `method` 는 GET,POST,PUT 등 어떤 방식으로 데이터를 보낼지 정한다.
- `enctype` 은 데이터의 인코딩 방식을 정한다.


이렇게 form은 자신의 태그 안에 있는 input 태그들의 정보들을 모아 action에 설정된 url로 method에 정의된 방식으로 데이터를 enctype에 따라 보내게 된다.
위 코드는 첫번째 input인 id에 적은 값을 url로 보낸다. 하지만 action에 url을 지정하지 않았기에 아무일도 일어나지 않는다.
