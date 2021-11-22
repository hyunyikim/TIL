### FormData

```javascript
const formData = new FormData();
formData.append("key", "value");
formData.set("key", "value");

for (let entry of formData.entries()) {
  console.log(entry[0], entry[1]);
}
```

- body에 formData를 넣어 요청하면, 자동으로 request header가 `Content-Type: multipart/form-data`로 설정됨
- append? 동일한 키가 존재하더라도 값이 추가됨
  - (FormData가 object 형태라서 동일한 키가 존재하지 않을거라고 생각했는데, append로 동일한 키로 값이 추가된다)
- set? 동일한 키가 존재한다면, 값을 교체

---

[https://ko.javascript.info/formdata](https://ko.javascript.info/formdata)
