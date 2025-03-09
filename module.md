# 모듈 (Module)

새로운 기능을 만들 때 마다 새로운 모듈을 생성하기에,
Nest.js에서 모듈은 특정 기능의 패키지이다.

즉, 모듈은 애플리케이션의 한 측면 또는 기능과 관련된 모든 파일을 포함한다.

```md
- USER MODULE (users.module.ts) <!-- 진입점 -->
  - users.controller.ts <!-- 모듈과 관련된 API엔드포인트에 대한 라우팅 로직 -->
  - users.service.ts <!-- 비지니스 로직 및  -->
  - users.entity.ts <!-- DB 상호작용 (ORM)-->
  - users.controller.spec.ts <!-- 컨트롤러 테스트 파일 -->
```

- APP MODULE (app.module.ts)는 Nest.js 애플리케이션의 주요 모듈이다.
- Nest.js는 다른 모듈을 식별할 수 있다.
- 의존성 주입을 사용해, 모듈을 연결할 수 있다.
