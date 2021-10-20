# REST API

## REST API 설계 방법
- 동사를 사용하지 않는다.
- Http Method(Request Method)를 사용하여 기능을 구분한다.
	> /movies, GET : 읽기  
	/movies, POST : 생성  
	/movies/abc, PUT : 수정  
	/movies/abc, DELETE : 삭제
- 검색이나 필터 같은 기능을 구현하는 경우 새로운 Url을 만드는 대신 Query String을 사용한다.
	> /movies?created_date=2021

#### Reference
* [5분만에 제대로 설계하는 ⭐️ REST API](https://www.youtube.com/watch?v=4DxHX95Lq2U)
* [RESTful API 설계 가이드](https://sanghaklee.tistory.com/57)