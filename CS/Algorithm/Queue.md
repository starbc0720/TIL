## Queue란?


* 한쪽 끝에서만 삽입이 이루어지고, 다른 한쪽 끝에서는 삭제 연산만 이루어지는 유한 순서 리스트
<br>

## Stack 2개로 Queue 구현하는 방법
<br>

### Stack이란?
* 한 쪽 끝에서만 자료를 넣고 뺼 수 있는 LIFO(Last In First Out) 형식의 자료 구조
<br>

## 구현 방법

### ex) 1, 2, 3의 3개의 공이 있다고 가정
* 한 개의 스택은 공을 넣기만 하는 용도, 남은 하나는 공을 빼기만 하는 용도로 사용한다고 생각
* 1,2,3 순서대로 넣기만 하는 용도의 스택에 공을 넣고 다 넣은 후 공을 뺀다
* 그렇게 되면 3, 2, 1의 순서대로 공이 나오게 된다
* 이제 뺴기만 하는 용도로 생각했던 스택에 3, 2, 1 순서대로 공을 넣는다.
* 다시 공을 뺴면 1, 2, 3 순서대로 FIFO(First In First Out)구조로 먼저 넣은 것이 먼저 나오는 Queue와 같이 동작함을 알 수 있다.

> 23.08.30 정리
