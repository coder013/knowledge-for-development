# HTTP

## HTTP란?
- HTTP(HyperText Transfer Protocol, 하이퍼텍스트 전송 프로토콜)
- 웹 서버와 클라이언트간의 통신을 위한 프로토콜
- TCP/IP를 기반으로 한 응용 계층 프로토콜
- 연결 상태를 유지하지 않는 비연결성 프로토콜

## 동작 방식
- 클라이언트가 요청(Request)을 보내면 서버는 해당 요청에 맞는 응답(Response)을 보냄
- 이 때 보내는 메시지를 HTTP 메시지라고 함
- HTTP 메시지는 시작줄, 헤더, 본문으로 구성되어 있음

## Request

### HTTP 메시지
GET https://www.google.com/ HTTP/3
ACCEPT: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
ACCEPT-Encoding: gzip, deflate, br...

### 시작줄
GET https://www.google.com/ HTTP/3
- **요청 방법**, 주소, HTTP 버전
    - **Request Method(요청 방법)**
		> **GET : 데이터 요청**  
		HEAD  
		**POST : 데이터 생성**  
		**PUT : 데이터 전체 수정**  
		**DELETE : 데이터 삭제**  
		CONNECT  
		OPTIONS  
		TRACE  
		**PATCH : 데이터 부분 수정**

### 헤더
ACCEPT: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
ACCEPT-Encoding: gzip, deflate, br...
- 요청에 대한 정보
- 서버의 도메인 이름(HOST), 클라이언트의 유형(User-Agent), 응답 데이터의 유형(ACCEPT) 등

### 본문
- 요청을 처리하는데 필요한 데이터
- 요청 방법이 POST, PUT, PATCH 등 일 때 있음. 위의 HTTP 메시지는 GET이기 때문에 본문이 없음

## Response

### HTTP 메시지
HTTP/3 200 OK
ALT-SVC: h3=":443"; ma=2592000,h3-29=":443"; ma=2592000,h3-T051=":443"; ma=2592000,h3-Q050=":443"; ma=2592000,h3-Q046=":443"; ma=2592000,h3-Q043=":443"; ma=2592000,quic=":443"; ma=2592000; v="46,43"
BFCACHE-OPT-IN: unload...

<!doctype html><html itemscope="" itemtype="http://schema.org/WebPage" lang="ko"><head><meta charset="UTF-8"><meta content="origin" name="referrer">...

### 시작줄
HTTP/3 200 OK
- HTTP 버전, **상태 코드**, 상태 메시지

### 헤더
ALT-SVC: h3=":443"; ma=2592000,h3-29=":443"; ma=2592000,h3-T051=":443"; ma=2592000,h3-Q050=":443"; ma=2592000,h3-Q046=":443"; ma=2592000,h3-Q043=":443"; ma=2592000,quic=":443"; ma=2592000; v="46,43"
BFCACHE-OPT-IN: unload...
- 응답에 대한 정보
- Access-Control-Allow-Origin 등
	> 요청을 보내는 주소와 응답하는 주소가 다를 경우 CORS 오류 발생  
	요청을 보내는 주소를 Access-Control-Allow-Origin에 추가하여 해당 주소의 접근을 허용

### 본문
<!doctype html><html itemscope="" itemtype="http://schema.org/WebPage" lang="ko"><head><meta charset="UTF-8"><meta content="origin" name="referrer">...
- 요청한 데이터, 해당 본문은 HTML을 보내주고 있음

#### Reference
* [HTTP란 무엇인가](https://www.zerocho.com/category/HTTP/post/5b344f3af94472001b17f2da)
* [HTTP란 무엇인가?](https://velog.io/@surim014/HTTP%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80)
* [HTTP가 어떤 일을 하는지 한번 열어봅시다.](https://brunch.co.kr/@wangho/8)
* [HTTP 요청 메서드](https://developer.mozilla.org/ko/docs/Web/HTTP/Methods)
* [PUT vs PATCH 차이점](https://papababo.tistory.com/entry/HTTP-METHOD-PUT-vs-PATCH-%EC%B0%A8%EC%9D%B4%EC%A0%90)