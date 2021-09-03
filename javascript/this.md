### 함수와 메서드

- 독립성에 차이가 있다.
- 함수? 독립성을 가지고 호출되는 함수
- 메서드? 객체의 프로퍼티에 할당되어 호출된 함수

### this

- 호출한 주체애 대한 정보가 담긴다.
- this는 함수를 호출할 때 결정된다(호출 당시의 주변 스코프에 의해 결정되는게 아니다)

```js
var func = function () {
  console.log(this);
};
func(); // window

var obj = {
  method: func,
};
obj.method(); // obj
```

- 함수로서 호출될 때? this는 전역객체
- 메서드로서 호출될 때? this는 메서드 호출 주체(. 앞의 객체)

```js
var obj = {
  outer: function () {
    console.log(this); // obj
    var innerFunc1 = () => {
      console.log(this); // obj
    };
    var innerFunc2 = function () {
      console.log(this); // winow
    };
    innerFunc1();
    innerFunc2();
  },
};
obj.outer();
```

- 화살표 함수? this 바인딩 과정이 없어서 상위 스코프를 가리킴
- 생성자 함수 내부? this는 새로 만들 인스턴스 자신
- 콜백 함수? 제어권을 넘겨받은 함수가 결정

### 명시적으로 this 바인딩하기

```js
var func = function (a, b, c) {
  console.log(this, a, b, c);
};
func.call({ x: 1 }, 1, 2, 3); // {x:1}, 1, 2, 3
func.apply({ x: 1 }, [1, 2, 3]); // {x:1}, 1, 2, 3

var bindFunc = func.bind({ x: 1 });
bindFunc(1, 2, 3); // {x:1}, 1, 2, 3
```

- Function.prototype.call()? this 바인딩해서 바로 호출
- Function.prototype.apply()? call과 동일, 인자를 배열로 넘김
- Function.prototype.bind()? this 바인딩 후 새로운 함수 리턴

---

책 코어자바스크립트 03 this 참고
