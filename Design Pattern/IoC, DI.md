# IoC, DI

## IoC(Inversion of Control, 제어의 역전)
- 객체의 생명 주기와 같은 프로그램의 제어권을 외부(프레임워크)에 위임하는 개념
- 헐리우드 원칙(Don't call us. We'll call you.)의 프로그래밍 버전
- 개발자가 비즈니스 로직에 더 집중할 수 있다
- 이를 구현한 디자인 패턴으로는 DL, DI가 있다

## DI(Dependency Injection, 의존성 주입)
- IoC를 구현하기 위한 디자인 패턴 중 하나
- 필요한 객체를 직접 생성하지 않고 외부에서 주입받아 사용
- 생성자 주입, Setter 주입, 인터페이스 주입 세 가지 방법이 있다
- 객체 간의 의존성을 줄임으로써 코드 변경에 덜 취약해지고 재사용성을 높일 수 있다
- 단위 테스트에 용이

### IoC Container(DI Container)
- 객체의 생명 주기 및 의존성을 관리하는 컨테이너
- Spring에서는 ApplicationContext(BeanFactory)가 컨테이너의 역할을 한다

#### Reference
* [제어의 역전 (Inversion Of Control, IoC)](https://hudi.blog/inversion-of-control/)
* [제어의 역전(Inversion of Control, IoC) 이란?](https://develogs.tistory.com/19)
* [스프링 - 의존 관계와 DI, Ioc 컨테이너](https://bbeomgeun.tistory.com/141)
* [[Spring DI/IoC] IoC? DI? 그게 뭔데?](https://velog.io/@ohzzi/Spring-DIIoC-IoC-DI-%EA%B7%B8%EA%B2%8C-%EB%AD%94%EB%8D%B0#inversion-of-control)