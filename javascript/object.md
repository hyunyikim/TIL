### 객체

- 프로퍼티를 저장하는 key-value 형식의 데이터 타입
- 키는 문자열이나 심볼, 값은 어떤 자료형도 가능
- Array, Date, Error도 객체이다

### 프로퍼티 접근 방법

- 점 표기법
  - obj.property
  - 일반적으로 사용
- 대괄호 표기법
  - obj["property"]
  - 프로퍼티가 변수이거나, 유효한 변수 식별자가 아닐 경우 사용

### 객체 추가 연산자

```js
// 프로퍼티 삭제
delete obj.property

// 해당 key를 가진 프로퍼티가 객체 내에 있는지 확인
// return true or false
"key" in obj

// 프로퍼티 나열
for(let key in obj)
```

---

[https://ko.javascript.info/object](https://ko.javascript.info/object)
