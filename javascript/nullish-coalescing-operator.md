```js
// ||
alert(undefined || null || 0);   // 0 
alert(0 || 'hello');    // 'hello'

// ?? 
alert(undefined ?? null ?? 0);   // 0
alert(0 ?? 'hello');    // 0

let height = 0;
alert(height || 100); // 100
alert(height ?? 100); // 0
```

- ||(OR 연산자)
    - 첫 번째 truthy한 값 반환
    - truthy한 값이 없다면 제일 마지막 값 반환
- ??(nullish 병합 연산자)
    - 첫 번째 정의된(defined) 값 반환
    - null, undefined가 아닌 값을 반환
    - (falsy한 값이더라도 null, undefined가 아니라면 반환)
    
