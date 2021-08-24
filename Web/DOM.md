# DOM(Document Object Model, 문서 객체 모델)
- 웹 페이지에 대한 프로그래밍 인터페이스
- 단순한 텍스트로 구성되어 있는 HTML 문서를 트리 형태의 객체 모델로 표현, 해당 DOM에 JavaScript와 같은 언어를 사용해 접근하거나 수정함으로써 웹 페이지를 조작할 수 있게 한다.
- HTML 문서를 통해 생성되지만 내용이 동일하지 않을 수 있음
> HTML 문서가 올바르게 작성되지 않아 내용을 교정한 후 DOM 트리를 생성하는 경우  
JavaScript에 의해 DOM이 수정된 경우
- 브라우저에서 보이는 내용과 다를 수 있음
> display : none과 같은 속성을 가진 요소는 브라우저, 즉 렌더 트리에는 존재하지 않지만 DOM 트리에는 존재함
- 개발자 도구에서 보이는 내용과 다를 수 있음
> before, after와 같은 가상 요소는 CSSOM의 요소이므로 DOM 트리에는 존재하지 않음

#### Reference
* [DOM 소개](https://developer.mozilla.org/ko/docs/Web/API/Document_Object_Model/Introduction)
* [DOM이란 무엇인가?](https://velog.io/@surim014/DOM%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80)
* [DOM은 정확히 무엇일까?](https://wit.nts-corp.com/2019/02/14/5522)