## 시멘틱 버저닝(Semantic Versioning, SemVer)

- major.minor.patch
    - major- 하위 버전과 호환되지 않는 변화가 생겼을 때
    - minor- 하위 버전과 호환이 되는 기능 업데이트 시
    - patch- 버그 수정, 하위 호환 가능할 때
- 틸드(~)
    - 현재 지정한 버전의 마지막 자리 내의 범위에서만 허용
    - ~0.0.1: ≥0.0.1, <0.1.0
    - ~0.1: ≥0.1.0, <0.2
- 캐럿(^)
    - 가장 왼쪽에 있는 0이 아닌 요소를 수정하지 않는 변경 허용
    - ^1.0.0: minor, patch 업데이트 허용
    - ^0.2.3: patch 업데이트 허용
    - ^0.0.3: 업데이트 허용하지 않음

---
[https://velog.io/@slaslaya/npm-semver-틸트-범위와-캐럿-범위](https://velog.io/@slaslaya/npm-semver-%ED%8B%B8%ED%8A%B8-%EB%B2%94%EC%9C%84%EC%99%80-%EC%BA%90%EB%9F%BF-%EB%B2%94%EC%9C%84)