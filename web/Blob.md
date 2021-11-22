### Blob

```javascript
const blob = new Blob(array, options);
```

- Binary Large Object
- 인자 array: ArrayBuffer, ArrayBufferView, DONString ...
- 인자 options: MIME type, endings
- File은 Blob에서 확장됨

```javascript
const url = URL.createObjectURL(blob); // blob:URL
URL.revokeObjectURL(url);
```

- 현재 브라우저에서만 유효한 url이 생성됨
- url 생성후, 꼭 revokeObjectURL로 메모리를 해제해줘야함

---

[https://heropy.blog/2019/02/28/blob/](https://heropy.blog/2019/02/28/blob/)
