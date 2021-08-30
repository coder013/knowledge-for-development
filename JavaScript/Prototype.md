# Prototype
 - 자바스크립트는 프로토타입 기반 언어
 - number, string, boolean과 null, undefined를 제외한 모든 것들은 객체이다.
 - 프로토타입 객체(prototype object)는 객체의 원본에 해당하는 객체이다.
 - 프로토타입 객체 또한 상위 프로토타입 객체를 가질 수 있으며 모든 객체의 최상위 프로토타입 객체는 Object.prototype이다.
 - 모든 객체는 프로토타입 객체에 대한 링크인 proto 속성을 가지고 있다.
 - 함수 선언 시 새로운 프로토타입 객체가 생성되며 해당 함수의 prototype 속성을 통해 접근할 수 있다.  
 해당 프로토타입 객체는 생성자 함수를 참조하는 constructor 속성을 가지고 있다.
 - 객체의 특정 속성에 접근하고자 할 때 그 속성이 없을 경우 프로토타입 객체를 확인한다. 프로토타입 객체에도 없을 경우 상위 프로토타입 객체를 확인하고 속성이 있을 경우 값을 반환한다. 이 과정을 최상위 프로토타입 객체까지 반복한다.  
 이처럼 프로토타입 객체부터 최상위 프로토타입 객체까지 연결되어 있는 구조를 프로토타입 체인(prototype chain)이라고 한다.
 - 프로토타입 객체는 해당 프로토타입 객체를 원본으로 가지고 있는 모든 객체가 공유하기 때문에 변수나 함수를 한 번만 선언해도 모든 객체에서 사용 가능하다. 그 덕분에 불필요한 메모리 사용을 줄일 수 있다.
 
 #### Reference
 * [Object Prototype](https://gyoogle.dev/blog/computer-language/Javascript/Object%20Prototype.html)
 * [Object prototypes](https://developer.mozilla.org/ko/docs/Learn/JavaScript/Objects/Object_prototypes)
 * [JavaScript : 프로토타입(prototype) 이해](https://www.nextree.co.kr/p7323/)
 * [자바스크립트 Prototype 완벽 정리](https://velog.io/@adam2/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-Prototype-%EC%99%84%EB%B2%BD-%EC%A0%95%EB%A6%AC)