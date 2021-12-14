## useState

### useState 기본값으로 props를 사용하면 안된다

```javascript
import React from "react";

const Box = ({ num }) => {
  const [state, setState] = React.useState(num);

  // TODO
  useEffect(() => {
    setState(num);
  }, [num]);

  return <div>child state ${state}</div>;
};

const App = () => {
  const [state, setState] = React.useState();
  return (
    <div className="App">
      <button onClick={() => setState(Math.random(10))}>Click Me</button>
      <Box num={state} />
    </div>
  );
};
export default App;
```

- 자식 컴포넌트에서 props가 바뀌어도 리렌더링이 안되는 문제가 발생
- 원인은 props를 useState의 기본값으로 사용한 것이 원인
- useState는 처음 렌더링 시에만 호출되고, 그 이후에는 props가 변경되더라도 바뀌지 않음
- useEffect로 props가 변경되었을 때, state를 변경해준다.

[https://medium.com/@digruby/do-not-use-props-as-default-value-of-react-usestate-directly-818ee192f454](https://medium.com/@digruby/do-not-use-props-as-default-value-of-react-usestate-directly-818ee192f454)

### 지연 초기 state

```javascript
const [count, setCount] = useState(window.localStorage.getItem(key));

// 지연 초기 적용
const [count, setCount] = useState(() => window.localStorage.getItem(key));
```

- 지연 초기? 값 대신 함수를 useState 인자로 넘김
- 상태가 최초로 생성될 때만 실행되고, 이후 리렌더링 시에는 실행하지 않는다.
- 초기값의 계산 비용이 클 때 사용

[https://ui.toast.com/weekly-pick/ko_20201022](https://ui.toast.com/weekly-pick/ko_20201022)
