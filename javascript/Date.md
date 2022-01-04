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
