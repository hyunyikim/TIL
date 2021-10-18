### falsy 값 렌더링

```jsx
render () {
    const count = 0;
    return (
        <div>
            {count && <h1>{count}</h1>}
        </div>
    )
}
```

- `<div>0</div>`이 렌더링 됨
- && 연산자로 falsy한 값인 count가 리턴 되면서 렌더링이 된다.
- `false, null, undefined, true`가 렌더링 되지 않음
- <b>그 외 `falsy` 값들은 리액트가 렌더링 한다!</b>
- 렌더링을 막기 위해서는 `null` 리턴하기

---

[https://ko.reactjs.org/docs/jsx-in-depth.html#booleans-null-and-undefined-are-ignored](https://ko.reactjs.org/docs/jsx-in-depth.html#booleans-null-and-undefined-are-ignored)
[https://yceffort.kr/2020/10/use-ternaries-not-and-and-in-jsx](https://yceffort.kr/2020/10/use-ternaries-not-and-and-in-jsx)
