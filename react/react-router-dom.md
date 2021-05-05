### window History API

-   브라우저의 세션 기록을 조작할 수 있다

```jsx
history.back();
history.forward();
history.pushState(데이터, 주소, 타이틀); // 페이지는 갱신되지 않고 주소만 변경됨, 데이터 함께 전달 가능
history.replaceState(데이터, 주소, 타이틀); // 현재 히스토리를 변경
```

-   popstate 이벤트
    -   히스토리 엔트리에 변화가 일어날 때 발생한다
    -   브라우저 뒤로가기나 history.back() 호출시 발생한다
    -   history.pushState(), history.replaceState() 호출시에는 발생하지 않는다

```jsx
window.onpopstate = (event) => {};
```

### react-router-dom

react-router로 라우팅 되면, props에 history, location, match 정보가 넘어온다.

-   history? window.history 객체와 유사, 주소 변경을 할 수 있다
-   location? window.location 객체와 유사, 현재 페이지 정보를 지니고 있다
-   match? Route의 path에서 정의된 정보를 갖고 있다

[https://developer.mozilla.org/ko/docs/Web/API/History](https://developer.mozilla.org/ko/docs/Web/API/History)

[React Router: Declarative Routing for React](https://reactrouter.com/web/api/history)

[React Router V4 정리](https://medium.com/@han7096/react-router-v4-%EC%A0%95%EB%A6%AC-e9931b63dcae)
