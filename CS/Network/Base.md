## 네트워크에 대한 기본적인 지식에 대한 것을 정리하는 공간


* URL과 URI의 차이점
<br>

## URL이란?
<br>

### URL(Uniform Resource Locator)
* 웹주소, 컴퓨터 네트워크상에서 리소스가 어디에 위치하는지 알려주기 위한 규약
* 식별자 + 위치
* https://elancer.co.kr -> 프로토콜 + URI 형태
<br>

## URI이란?
<br>

### URI(Uniform Resource Identifier)
* 네트워크 통합자원의 위치를 나타내기 위한 규약
* 식별자
* URL 보다 더 포괄적 개념
* ex) elancer.co.kr
<br>

## Proxy란?
<br>

### Proxy
* '대리', '대신'이라는 뜻을 가지며, 프로토콜에 있어서 대리 응답 등에서 사용하는 개념
* 클라이언트와 서버 사이에 존재, 중계기로서 대리로 통신 수행하는 것을 Proxy라고 함, 이때 중계 기능을 하는 주체를 Proxy Server라고 함
<br>

### Proxy Server 종류
* Forward Proxy(포워드 프록시)
  <br>
  -> 통상적인 Proxy 의미
  <br>
  -> Client와 Server 사이에 위치하여 요청 중계, 요청과 응답은 Proxy Server 거침  
  -> Client 감추는 효과 존재
  <br>
  <br>
* Reverse Proxy(리버스 프록시)
  <br>
  -> 요청과 응답이 Proxy Server로 이동, 포워드 프록시와 다르게 Server들이 주로 내부망으로 구성되며 프록시에게만 연결 허용
  <br>
  -> 서비스를 위한 보안 채널 구축
  <br>
  -> Client가 Server에 직접 접근 불가능
  <br>
  -> Reverse Proxy에서 요청을 적극적 중계하는 Load Balancing 역할 수행
  <br>
  -> Server 감추는 효과 존재
  <br>
<br>

### Proxy Server 사용 이유
* 개인정보 보호 가능
  <br>
  -> 서버측에서 나의 ip가 아닌 Proxy Server ip 보게됨
  <br>
  -> ip 숨기기 가능
  <br>
* 캐시 사용으로 인한 속도 향상
  <br>
  -> 같은 요청 들어올 경우 cache 자원 반환, 서비스 속도 높이고 대역폭 줄이기 가능
  <br>
* 로그 기록, 관리 가능
  <br>
  -> Proxy Server에 클라이언트 기록 존재
  <br>
  -> 어떤 ip에서 어떤 ip로 얼마나 접속해있는지 확인 가능
  <br>
  -> 특정 ip가 방문할 수 있는 웹사이트 제한도 가능
  <br>
* 접속 우회 가능
  <br>
  -> 다른 나라에서 접속한 것처럼 우회 가능
  <br>

  
> 23.09.20 정리
