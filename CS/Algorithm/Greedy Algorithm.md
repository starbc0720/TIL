## Greedy Algorithm(탐욕법 알고리즘)란?


* Greedy Algorithm이란 매 순간 가장 좋아 보이는 것만 선택하고 나중에 미칠 영향은 고려하지 않는 방식
<br>

## Greedy Algorithm의 단점
<br>

### 1. 최적의 해를 찾는 방법이 아님
* 항상 상황에 만족하는 최선의 해를 찾는 방법일 뿐, 최적의 해를 찾는 방법이 아님
<br>

## Greedy Algorithm 문제 해결 방법

### 1. Selection Procedure(선택 절차)
* 현재 상태에서의 최적의 해답을 선택
<br>

### 2. Feasibility Check(적절성 검사)
* 선택된 해가 문제의 조건을 만족하는지 검사
<br>

### 3. Solution Check(해답 검사)
* 원래의 문제가 해결되었는지 검사하고, 해결되지 않았다면 선택 절차로 돌아가 위의 과정 반복
<br>

## Greedy Algorithm 적용하려면 성립해야 하는 조건 2가지
<br>

### 1. Greedy Choice Property(탐욕적 선택 속성)
* 앞의 선택이 이후의 선택에 영향을 주지 않아야 함
<br>

### 2. Optimal Substructure(최적 부분 구조)
* 문제에 대한 최종 해결 방법은 부분 문제에 대한 최적 문제 해결 방법으로 구성되어야 함
<br>

## Greedy Algorithm 예시
<hr>

### 1. 거스름돈
* 당신은 음식점의 계산을 도와주는 점원이다. 카운터에는 거스름돈으로 사용할 500원, 100원, 50원, 10원짜리 동전히 무한히 존재한다고 가정한다. 손님에게 거슬러 줘야 할 돈이 N원일 때 거슬러 줘야할 동전의 최소 개수를 구하라. 단 거슬러 줘야 할 돈 N은 항상 10의 배수이다.
<br>

 

### 풀이
 

* 그리디 알고리즘의 대표적인 유형인 거스름돈 문제다.

* 이 문제는 ‘가장 큰 화폐 단위부터’ 돈을 거슬러 주는 아이디어로 풀 수 있다.

* N원을 거슬러 줘야 할 때, 가장 먼저 500원으로 거슬러 줄 수 있을 만큼 거슬러 준다.

* 이후 100원, 50원, 10원짜리 동전을 차례대로 거슬러 줄 수 있을 만큼 거슬러 주면 최소의 동전 개수로 모두 거슬러 줄 수 있다.

 

* N = 1,260 이라고 가정하자.

 

  * 1.  500원짜리로 거슬러 줄 수 있는 돈은 1,000원, 즉 500원 2개이고 남은 돈은 260원이다.

  * 2. 100원짜리로 거슬러 줄 수 있는 돈은 200원, 즉 100원 2개이고 남은 돈은 60원이다.

  * 3. 50원짜리로 거슬러 줄 수 있는 돈은 50원, 즉 50원 1개이고 남은 돈은 10원이다.

  * 4. 10원짜리로 거슬러 줄 수 있는 돈은 10원, 즉 10원 1개이고 거스름돈 계산을 모두 마쳤다.

 

* 따라서 N = 1,260 일때 손님이 받은 동전의 최소 개수는 6개이다.
<br>


> 22.10.31 정리
