## dependencies 종류

### dependencies

- 운영 환경에서 필요한 패키지
- 런타임에 필요한 패키지

### devDependencies

- 개발 환경에서 필요한 패키지
- ex) babel

### peerDependencies

- 내 모듈이 동작할 수 있는 다른 모듈의 호환성 정보

### optionalDependencies

- 설치가 실패해도 문제가 없는 패키지
- 설치에 실패해도 패키지 설치 과정이 중단되지 않는다

### bundledDependencies

- 퍼블리싱 할 때 번들되는 패키지 이름들의 목록



## yarn.lock
- 패키지 잠금 파일
- package.json에는 패키지의 특정한 버전이 적혀져있지 않고 version range로 적혀있음
- 그럼 해당 프로젝트를 설치하는 개발자마다 패키지 버전이 달라질 수 있음
- 패키지 잠금 파일에 package.json에 명시된 패키지의 버전을 정확하게 명시해서 위와 같은 불상사를 없앰
- npm에서는 package-lock.json, yarn에서는 yarn.lock
---

[https://classic.yarnpkg.com/en/docs/dependency-types#toc-dev-dependencies](https://classic.yarnpkg.com/en/docs/dependency-types#toc-dev-dependencies)
[https://www.daleseo.com/js-package-locks/](https://www.daleseo.com/js-package-locks/)