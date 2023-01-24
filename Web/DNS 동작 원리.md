# DNS(Domain Name System)란?
- 인터넷의 전화번호부
- 우리는 일반적으로 웹 사이트에 접속할 때 외우기 어려운 IP 주소 대신 도메인 이름을 입력한다
- 입력한 도메인 이름과 매칭되는 IP 주소를 찾아 접속시켜주는 역할을 하는 것이 DNS이다

## DNS 서버의 종류
- Recursive DNS 서버
- Root DNS Server
- TLD DNS 서버
- Authoritative DNS 서버

## DNS의 동작 방식
1. 사용자가 Recursive DNS 서버에게 도메인 이름(www.google.com)을 주며 IP 주소 요청
2. Recursive DNS 서버가 Root DNS 서버에게 안내 요청
3. Root DNS 서버는 .com을 보고 com 도메인을 관리하는 TLD DNS 서버에게 안내
4. Recursive DNS 서버가 TLD DNS 서버에게 안내 요청
5. TLD DNS 서버는 google.com를 보고 google.com 도메인을 관리하는 Authoritative DNS 서버에게 안내
6. Recursive DNS 서버가 Authoritative DNS 서버에게 안내 요청
7. Authoritative DNS 서버는 www.google.com의 IP 주소를 찾아서 알려줌
8. 마지막으로 Recursive DNS 서버가 사용자에게 IP 주소를 알려주고 웹 사이트에 접속

- ##### 사용자 -> Recursive DNS 서버 -> Root DNS 서버 -> TLD DNS 서버 -> Authoritative DNS 서버 -> 웹 사이트

#### Reference
* [DNS란? (도메인 네임 시스템 개념부터 작동 방식까지)](https://hanamon.kr/dns%EB%9E%80-%EB%8F%84%EB%A9%94%EC%9D%B8-%EB%84%A4%EC%9E%84-%EC%8B%9C%EC%8A%A4%ED%85%9C-%EA%B0%9C%EB%85%90%EB%B6%80%ED%84%B0-%EC%9E%91%EB%8F%99-%EB%B0%A9%EC%8B%9D%EA%B9%8C%EC%A7%80/)
* [DNS란 뭐고, 네임서버란 뭔지 개념정리](https://gentlysallim.com/dns%EB%9E%80-%EB%AD%90%EA%B3%A0-%EB%84%A4%EC%9E%84%EC%84%9C%EB%B2%84%EB%9E%80-%EB%AD%94%EC%A7%80-%EA%B0%9C%EB%85%90%EC%A0%95%EB%A6%AC/)
* [DNS란 무엇입니까? | DNS 작동 원리](https://www.cloudflare.com/ko-kr/learning/dns/what-is-dns/)