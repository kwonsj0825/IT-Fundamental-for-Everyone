# HTTP(HyperText Transfer Protocol) 메시지
- HTTP 메시지는 클라이언트와 서버 간에 데이터가 교환되는 방식이다.
- 크게 요청(Request)과 응답(Response)으로 구분된다.
- 요청은 메서드와 경로, 응답은 상태 코드를 핵심으로 하며, 헤더와 바디를 통해 부가 정보와 데이터를 전달한다.

## 1. 공통 구조
모든 HTTP 메시지는 다음과 같은 논리적 구조를 가진다.
- 시작 줄(Start Line): 실행될 요청이나 요청의 상태를 나타냄. ex) POST /login HTTP/1.1
- HTTP 헤더(Message Headers): 요청/응답에 대한 추가 정보(메타데이터). ex) Host:localhost:8000 Connection:keep-alive
- 빈 줄(CRLF): 헤더의 끝을 알리는 필수 공백 라인. ex) CRLF(개행)
- 본문(Message Body): 실제 전송할 데이터 (선택 사항). ex) username=min&password=1234

## 2. HTTP 요청 메시지 (HTTP Request)
클라이언트가 서버에 특정 액션을 요구할 때 보내는 메시지이다.
### 구성 요소
- Request Line : 요청 메소드(Method), 요청 대상(Target), HTTP버전
  -Method (메서드): 수행할 작업의 종류 (GET, POST, PUT, DELETE 등).
    - GET : 존재하는 자원에 대한 요청
    - POST : 새로운 자원을 생성
    - PUT: 존재하는 자원에 대한 변경
    - DELETE : 존재하는 자원에 대한 삭제
  - Path (대상 경로): 리소스의 URL 경로 (예: /index.html).
  - HTTP Version: 사용 중인 HTTP 버전 (예: HTTP/1.1).

- Headers: 호스트 정보, 브라우저 정보, 인증 토큰 등을 포함.
- Body : 주로 POST 메서드를 사용할 때 데이터를 보낼 때 사용되고, GET 요청에서는 일반적으로 본문이 없다.
- 본문의 형식은 Content-Type 헤더에 따라 다르며, 텍스트, JSON, XML, 바이너리 등의 형식이 될 수 있다.
- 요청 메시지의 본문은 클라이언트가 서버로 전송하는 데이터를 포함한다.


## 3. HTTP 응답 메시지 (HTTP Response)
서버가 클라이언트의 요청에 대해 답변하는 메시지이다.
### 구성 요소
- Status Code (상태 코드): 요청의 성공/실패 여부를 나타내는 3자리 숫자 (ex : HTTP/1.1 200 OK).
- Headers: 서버 정보, 콘텐츠 타입, 데이터 길이 등을 포함.(ex: Content-Type, Content-Length, Server 등)
- Body: 클라이언트가 요청한 데이터 (HTML, JSON, 이미지 등).
- 응답 메시지의 본문은 일반적으로 서버의 응답 데이터를 포함한다.



