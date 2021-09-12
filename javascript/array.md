### 배열 메서드

```js
[0, 1].push(2);
[0, 1].pop();
[0, 1].shift();
[0, 1].unshift(-1);
```

- arr.push(...items): 맨 끝에 요소 추가
- arr.pop(): 맨 끝 요소 추출
- arr.shift(): 첫 요소 추출
- arr.unshift(...items): 맨 앞에 요소 추가
- shift, unshift는 배열의 첫 순서에 조작을 가하기 때문에 모든 요소가 이동한다 .

```js
[0, 1, 2].splice(1, 1); // [0,2]
[0, 1, 2].slice(1, 2); // [1]
[0, 1, 2].concat(3, 4); // [0,1,2,3,4]

[1, 2, 15].sort(); // [1,15,2]
[1, 2, 3, 4, 5].reverse(); // [5,4,3,2,1]

"a,b,c".split(","); // [a,b,c]
["a", "b", "c"].join(","); // a,b,c
```

- arr.splice(pos, deleteCount, ...items): pos부터 deleteCount개 요소를 지우고 삭제가 일어난 곳에 items를 추가
- arr.slice(start, end): start부터 end 인덱스 앞 요소까지 새로운 배열 반환
- arr.concat(...items): 배열의 모든 요소 복사하고 items를 추가한 새로운 배열 반환
- arr.sort(): arr을 정렬해 반환
- arr.reverse(): arr을 뒤집어 반환
- splice, sort, reverse는 기존 배열을 변형시킨다.

---

[https://ko.javascript.info/array-methods#ref-345](https://ko.javascript.info/array-methods#ref-345)
