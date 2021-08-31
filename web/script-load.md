![img](https://uploads.disquscdn.com/images/4303414a00e244a653fc9a4894719b730caae6d4c647b97966b1061ae16fec48.png)
![img](https://uploads.disquscdn.com/images/84255af6a3268816f146e255c48db97c670931c351d640f844ecd78f591077a2.png)

### defar

- 스크립트 실행 순서를 보장한다.
- DOM 로드가 끝난 후 스크립트가 실행된다.
- DOMContentLoaded 이벤트 발생 전에 실행된다.
- 외부 스크립트에만 유효하다.

### async

- DOM 로드와는 상관 없이 스크립트 다운로드가 완료되면 실행된다.
- 스크립트 실행 순서가 보장되지 않는다.
- DOM에 의존적이지 않거나, 페이지와 연관이 없는 서드 파티 스크립트의 경우 유용하다.

---

[https://ko.javascript.info/script-async-defer](https://ko.javascript.info/script-async-defer)
