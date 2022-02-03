### KST 시간 변환

```js
const KST_TIME_DIFF = 9 * 60 * 60 * 1000; // 9시간
const date = new Date();
const nowUtc = date.getTime() + date.getTimezoneOffset() * 60 * 1000;
const nowKst = new Date(nowUtc + KST_TIME_DIFF);
```

### getTimezoneOffset

```js
const date = new Date();
date.getTimezoneOffset(); // -540
```

- UTC와 Date 객체에 지정된 Locale 시간과의 차이를 분 단위로 반환
- UTC = KST + timezoneOffset

### Date 생성자로 날짜 객체 생성하기

```jsx
// bad
const date = new Date("2022-01-06 09:00:00");

// good
const date = new Date(Unix 타임스탬프 값);
const date = new Date(년, 월, 일, 시간)
```

특정 일자를 지정해 날짜를 생성할 때 `yyyy-MM-dd HH:mm:ss` 형식의 문자열을 매개변수로 넘기는 식으로 주로 사용했는데, 모바일 브라우저와 사파리에서 Invalid Date가 발생했다.

Date 생성자로 날짜 객체 생성시, 날짜 파싱 동작이 브라우저들 끼리 일관적이지 못하기 때문에 사용하지 않는 편이 좋다.

[https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Date/Date](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Date/Date)

### 달의 마지막 일자 구하기
```js
const date = new Date(2022, 1, 0);      // Mon Jan 31 2022 00:00:00 GMT+0900 (한국 표준시)

new Date(년도, 구하고자 하는 달+1, 0);
```
- 주의, 달의 시작은 0부터(1월이 0, 12월이 11)