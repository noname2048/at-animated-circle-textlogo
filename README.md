# at-animated-circle-textlogo

* [online tutorials - Animated Circle Text Logo Effects using CSS & Javascript](https://www.youtube.com/watch?v=zwl3kZPZ8H8) 의 클론 코딩
* 포트폴리오에 넣어 볼까 생각했었다.

## 결과물
![result](circle-logo.gif)

## 노트

* querySelector에 선택자로 한가지만 쓰는 예제를 봤는데 두가지 이상 가능하다.
  * `document.querySelector(".text p")`라고 검색하면
  * 자손선택자로써 `.text` 클래스를 가진 태그 자손에 `p`를 선택한다
* `innerHTML`은 `<a class="...>`와 같이 서술된다.
* `innerTEXT`는 말 그대로 태그 사이의 값
* `innerTEXT`를 기준으로 split 한뒤 map을 쓰는 예제
  * `textP.innerHTML = textP.innerTEXT.split("").map((char, i) => <span>...</span>).join()`
  * text는 p 태그이다. p 태그 안에는 글자가 써져 있다.
  * 순식간에 span 태그가 글자수대로 증식한다.
  * 그런데 join은 왜 하는 걸까
  * map의 반환값은 리스트이다.
  * json 표기 방식에 의하면 리스트는 , 로 구분된다.
  * join을 쓰지 않으면 ,로 이어져버린다.
* html filter 속성에 brightness() contrast() 같은 함수가 사용 가능하다.
* transform-origin 속성이 있다.
