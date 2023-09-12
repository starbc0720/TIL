## Hash

* Hash란 단방향 암호화 기법인 해시함수을 이용하여 생성도니 고정 길이의 비트열 의미
* 해시함수는 입력된 임의의 데이터를 고정된 길이의 데이터로 변경하여 출력
* 변경 전 원래 데이터 값을 키, 변경 후 데이터 값을 해시값이라고 하며 변환되는 과정을 Hashing 이라고 함
* 변환된 값이 중복되는 경우 발생할 수 있는데 이를 Hash Collision(해시충돌)이라고 함
<br>

## HashTable

* 해시함수 사용 키를 해시 값으로 매핑, 이 해시값을 Index(색인) 혹은 주소 삼아 데이터의 값을 키와 함께 저장하는 자료구조
<br>

## HashMap, HashTable
<br>

### 공통점

* 해시함수 사용 키를 해시 값으로 매핑, 이 해시값을 Index(색인) 혹은 주소 삼아 데이터의 값을 키와 함께 저장하는 자료구조
<br>

### 차이점
* HashTable은 Thread Safe하고 HasMap은 Thread Safe하지 않음
  <br>
  -> Thread Safe란? 어떤 함수나 변수, 혹은 객체가 여러 스레드로부터 동시에 접근이 이루어도 프로그램 실행에 문제가 없음
  <br>
  -> HashMap 성능이 더 뛰어남
  <br>
  <br>
* HashTable은 key에 null 허용 x, HashMap은 key에 null 허용 
  <br>
  <br>
* HashTable은 Enumertaion 제공, HashMap은 Enumeration 미제공
  <br>
  <br>



> 23.09.12 정리
