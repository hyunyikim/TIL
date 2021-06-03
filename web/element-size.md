### offset

- offsetTop, offsetLeft,
  - 부모 요소(offsetParent)를 기준으로 얼만큼 떨어져 있나
- offsetWidth, offsetHeight
  - 테두리를 포함한 요소 전체의 사이즈
  - margin은 제외

### client

- clientTop, clientLeft
  - 요소 시작점으로부터 컨텐츠까지의 높이, 너비
  - 즉, 테두리
  - 스크롤 너비까지도 잡힌다
- clientWidth, clientHeight

  - 테투리 안 영역의 사이즈
  - padding + content size
  - 스크롤 영역은 제외된다
  - 스크롤은 컨텐츠의 영역을 빌려 위치한다

    ex) content width가 300인데, 스크롤이 발생한다면? 스크롤에 16px을 주어 content width가 284px이 된다

### Scroll

- scrollWidth, scrollHeight
  - 스크롤바에 감춰진 영역 전체
- scrollLeft, scrollTop
  - 스크롤이 얼마나 움직였나
  - 수정 가능한 프로퍼티이다.

---

[https://ko.javascript.info/size-and-scroll](https://ko.javascript.info/size-and-scroll)
