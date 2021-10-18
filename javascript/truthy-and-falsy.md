### truthy

- 참 같은 값(true로 평가됨)
- 빈 배열, 빈 객체도 true

```js
if (true)
if ({})
if ([])
if (42)
if ("0")
if ("false")
if (new Date())
if (-42)
if (12n)            // BigInt
if (3.14)
if (-3.14)
if (Infinity)
if (-Infinity)
```

### falsy

- 거짓 같은 값(false로 평가됨)
- 0, 빈 문자열, NaN도 false

```js
if (false)
if (null)
if (undefined)
if (0)
if (-0)
if (0n)
if (NaN)
if ("")
```

### 논리연산자

#### OR (||)

- 첫 번째 truthy를 찾는다.
- truthy 값이 없으면, 마지막 값을 리턴

```js
alert(1 || 0); // 1
alert(null || 1); // 1
alert(undefined || null || 0); // 0
```

#### AND (&&)

- 첫 번째 falsy를 찾는다.
- falsy 값이 없으면, 마지막 값을 리턴

```js
alert(1 && 0); // 0
alert(1 && 5); // 5
alert(null && 5); // null
alert(0 && "a"); // 0
```

- ***

[https://developer.mozilla.org/ko/docs/Glossary/Truthy](https://developer.mozilla.org/ko/docs/Glossary/Truthy)
[https://developer.mozilla.org/ko/docs/Glossary/Falsy](https://developer.mozilla.org/ko/docs/Glossary/Falsy)
[https://ko.javascript.info/logical-operators](https://ko.javascript.info/logical-operators)
