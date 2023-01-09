# equals, hashCode
- Object 클래스에 정의된 메소드

## equals
- 두 객체가 동일한지 판단하는 메소드
- 주솟값을 비교하여 동일한 객체인지 판단
- 객체의 내용이 동일한 경우에도 동일한 객체로 판단할 수 있도록 메소드를 오버라이딩해야 한다

## hashCode
- 객체의 고유한 값을 출력하는 메소드
- 객체 생성 시 임의로 정해진 정수를 출력
- HashMap, HashSet 등과 같은 자료구조는 내부적으로 hashCode를 사용하여 데이터를 저장한다
- 중복된 데이터의 저장을 막기 위해 객체의 내용이 동일한 경우 hasCode 값도 동일하도록 메소드를 오버라이딩해야 한다

#### Reference
* [[Java] equals와 hashCode 함수](https://mangkyu.tistory.com/101)
* [자바 hashCode()](https://brunch.co.kr/@mystoryg/133)
* [hashCode는 정말 메모리주소와 관련이 있을까?](https://velog.io/@cieroyou/hashCode%EB%8A%94-%EC%A0%95%EB%A7%90-%EB%A9%94%EB%AA%A8%EB%A6%AC%EC%A3%BC%EC%86%8C%EC%99%80-%EA%B4%80%EB%A0%A8%EC%9D%B4-%EC%9E%88%EC%9D%84%EA%B9%8C)
* [java.lang.Object.hashcode() 값은 실제 메모리 주소와 어떤 연관이 있나요?](https://okky.kr/articles/1381057)