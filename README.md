# 소프트웨어 테스팅 실습 — Java와 Python

은행 계좌를 예제로 **단위 테스트(Unit)** 와 **통합 테스트(Integration)** 의 검증 범위를 비교합니다.

|언어|1단계: 단위 테스트|2단계: 통합 테스트|
|---|---|---|
|Java 25 / Gradle 9.7.1 / JUnit Jupiter|[java/01-unit](java/01-unit)|[java/02-integration](java/02-integration)|
|Python 3.12+ / pytest|[python/01-unit](python/01-unit)|[python/02-integration](python/02-integration)|

각 단계는 독립된 실습 프로젝트이며 해당 디렉터리의 **README.md**에 요구사항, 테스트 케이스, 구현-테스트 대응, 실행 방법, 보고서 확인, 실패 실습을 설명합니다.

학습 순서: 단일 Account 객체의 정상/경계/예외 검증 → 의도적 결함 삽입 → Service와 Repository 연동 검증 → HTML/터미널 테스트 결과 분석.

Java: 각 단계에서 설치된 Gradle로 `gradle wrapper --gradle-version 9.7.1`을 1회 실행한 뒤 `./gradlew clean test`를 실행합니다. Java 25 JDK가 필요합니다.
Python: 각 단계에서 `python -m pip install -r requirements.txt`, `python -m pytest -v`를 실행합니다.

**참고:** 배포 자료에 Gradle Wrapper 바이너리 파일은 포함되지 않습니다. Java 예제는 JUnit 실행까지 CI에서 별도 확인이 필요합니다.
