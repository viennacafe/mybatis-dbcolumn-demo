# MyBatis DbColumn Demo

한글 필드 변환에 대한 데모 애플리케이션입니다.
`@DbColumn`과 MyBatis 연동은 별도 저장소에서 JitPack으로 배포된
`mybatis-dbcolumn-spring-boot-starter` 라이브러리를 사용합니다.

## 요구 환경

- Java 25
- Gradle Wrapper (Gradle 9.8.0)

## 실행

```bash
./gradlew bootRun
```

Windows:

```bat
gradlew.bat bootRun
```

## 테스트

```bash
./gradlew test
```

## API

```bash
curl http://localhost:8080/customers
curl http://localhost:8080/customers/1001
curl http://localhost:8080/customers/resultmap
curl http://localhost:8080/customers/alias
```

JitPack 의존성 버전은 `build.gradle`의 `dbColumnVersion`에서 변경할 수
있습니다. 현재 값은 `v0.0.2`입니다.