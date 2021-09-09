### 부분 문자열 추출하기

```js
let str = "012345";
console.log(str.slice(0, 3)); // 012
console.log(str.slice(-4, -1)); // 234
console.log(str.substring(0, 3)); // 012
console.log(str.substr(0, 3)); // 012
```

- slice(start, end)
  - start부터 end까지(end 미포함)
  - 음수 허용
- substring(start, end)
  - start부터 end 사이
  - 음수 0으로 취급
- substr(start, length)
  - start부터 length개의 글자
  - 음수 허용
  - 구식 스크립트 대응 위해 남겨놓음
    음수까지 허용되는 slice를 되도록 사용한다.

---

[https://ko.javascript.info/string](https://ko.javascript.info/string)
