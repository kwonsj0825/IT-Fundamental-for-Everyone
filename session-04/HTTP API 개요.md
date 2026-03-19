## HTTP API

**HTTP API란?**

HTTP 프로토콜을 이용하여 클라이언트가 서버와 데이터를 주고받는 방식이다. 

<aside>
🧑‍💻

    GET /users/1 HTTP 1.1

    Host : example.com

</aside>

이렇게 http API 요청은 기본적으로 **URI와 HTTP 메서드**로 구성된다.

URI 자원을 HTTP 메세지는 동작을 의미하는데

하나의 자원에 어떤 HTTP 메세지를 붙이느냐에 따라 결과가 달라진다.

ex) URI와 HTTP 메서드의 조합

| URI | HTTP 메서드 | 기능 |
| --- | --- | --- |
| /users | GET | 사용자 조회 |
|  | POST | 사용자 추가 |
| /users/1 | GET | 1번 사용자 조회 |
|  | PUT | 1번 사용자 수정 |
|  | DELETE | 1번 사용자 삭제 |

### 왜 이렇게 구분할까?

URI와 HTTP 메서드를 구분하면 더 단순하고, 일관되고, 확장하기 쉬워진다.

같은 자원을 다른 여러가지 방식으로 표현한다면 혼란스럽다.
