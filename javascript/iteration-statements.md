### for/in 문

```js
let obj = {
  name: "kim",
  age: 10,
};
for (let key in obj) {
  console.log(key); // name, age
}
```

- 객체의 열거할 수 있는 프로퍼티의 개수만큼 반복문 실행
- 모든 프로퍼티를 반환하는게 아니고, 오직 열거할 수 있는 프로퍼티만을 반환

### for/of 문

```js
let arr = ["banana", "apple", "orange"];
for (let value of arr) {
  console.log(value); // banana, apple, orange
}
for (let char of "Hello") {
  alert(char); // H,e,l,l,o (char는 순차적으로 H, e, l, l, o가 됩니다.)
}
```

- 반복할 수 있는 객체를 순회
- ex) Array, Map, Set, arguments

---

[https://tcpschool.com/javascript/js_control_loop](https://tcpschool.com/javascript/js_control_loop)
