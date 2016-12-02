
## 기말 프로젝트 평가

### 준비사항

git project 내에 설명 문서('프로젝트결과보고서.md') 준비할 것

**내용**

- 프로그램 설명
- 패키지 구조
    - 패키지의 역할 등을 설명
    - 패키지 간의 의존성
- 주요 클래스 및 인터페이스 설명
    - 구현 코드가 아니라 **역할과 책임**이 중요.
    - 다른 클래스와의 의존관계
    - 해당 클래스에 대한 테스트코드 (링크)
- 회고
    - 느낀점
    - 잘한점
    - 못한점

### 평가 기준

1. Naming (3pt)
    - *"Class, Object, Method 등이 적절한 이름을 가지고 있는가?"*
    - **클래스 이름**과 **public method**이 그 클래스의 *정체성*을 잘 드러낼 수 있어야 한다.
    - metaphore
        - `noun - verb`
        - `message - receiver`
    - Coding convension을 준수할 것
        - [java-coding-convension]
        - [자바코딩컨벤션][codeconvension-kr]
2. Dependency Control (5pt)
    - _"각 객체간의 의존성이 명확하게 제어되고 있는가?"_
    - 생성의존성이 있으면 안됨!
    - Spring DI 혹은 weaving code가 명시적으로 존재할 것
    - package 간 의존 cycle이 없을 것
3. Design Principal (10pt)
    - _"SOLID 원칙을 잘 준수하고 있는가?"_
        - 특히 SRP, OCP
    - UserInterface(e.g. GUI)와 Domain Logic은 완전히 분리되어 있을것
4. Unit Test (5pt)
    - _"주요 클래스에 대한 단위 테스트가 잘 작성되어 있는가?"_
    - 단위 테스트를 쓸 수 없다면 좋은 설계가 아니다!
    - 단위 테스트 자체가 해당 클래스의 행동을 잘 설명할 수 있도록...
        - e.g. test method 이름을 문장으로.. (e.g. `~하면~해야한다`)
    - SystemUnderTest가 되는 클래스를 격리시켜서 테스트 (mocking)
5. 기타 (7pt)
    - 실습과정 및 발표 태도
    - 기본 가이드에 대한 준수
        - anti-pattern
        - readability
        - complexity
        - testability


[java-coding-convension]:http://www.oracle.com/technetwork/java/codeconvtoc-136057.html
[codeconvension-kr]:http://blog.naver.com/jeany4u/20003876157
