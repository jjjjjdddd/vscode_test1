# Calculator with JUnit4 (calc-junit4)

정수 사칙연산 `Calculator` 컴포넌트와 JUnit4 기반 테스트 프로젝트입니다.  
(과제 제출용 – VS Code, JDK17, Maven 환경)

---

## 기능 요구사항
- `Calculator` 클래스
  - `int add(int a, int b)`
  - `int subtract(int a, int b)`
  - `int multiply(int a, int b)`
  - `int divide(int a, int b)` → `b == 0`이면 `IllegalArgumentException` 발생

---

## 테스트 요구사항
- JUnit4 (`junit 4.13.2`)
- 정상 케이스 + 경계/특수 케이스(0, 음수 조합) 포함
- 예외 테스트: `divide(?, 0)` → `IllegalArgumentException`
- 테스트 메서드 수: 13개 작성 (`add_twoPositives_returnsSum`, `divide_zeroDivisor_throwsIAE` 등)

---

## 실행 환경
- JDK 17
- VS Code + Test Runner for Java
- Maven (빌드 도구 권장)

---

## 실행/테스트 방법

### 1) Maven CLI
```bash
# 프로젝트 루트(calc-junit4)에서 실행
mvn -v      # Maven/Java 버전 확인
mvn test    # JUnit4 테스트 실행
