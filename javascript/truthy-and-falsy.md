### truthy

-   참 같은 값(true로 평가됨)
-   빈 배열, 빈 객체도 true

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

-   거짓 같은 값(false로 평가됨)
-   0, 빈 문자열, NaN도 false

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

[https://developer.mozilla.org/ko/docs/Glossary/Truthy](https://developer.mozilla.org/ko/docs/Glossary/Truthy)
[https://developer.mozilla.org/ko/docs/Glossary/Falsy](https://developer.mozilla.org/ko/docs/Glossary/Falsy)
