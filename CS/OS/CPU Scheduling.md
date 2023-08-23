## CPU Scheduling(CPU 스케줄링)란?

* CPU Scheduling이란, 언제 어떤 프로세스에 CPU를 할당할지 결정하는 작업
<br>

## CPU Scheduler는 언제 Schedule을 결정하는가?

    1)  실행(running) 상테에서 대기(waiting) 상태로 전환(switching) 될 때
    2)  실행(running) 상테에서 준비(ready) 상태로 전환(switching) 될 때
    3)  대기(waiting) 상테에서 준비(ready) 상태로 전환(switching) 될 때
    4)  종료(terminated) 될 때
    
  * 1), 4) 상황에서만 스케줄링 발생하는 것을 비선점형(non-preemptive) 스케줄링, 그 외는 선점형(preemptive) 스케줄링

## 1. 비선점형(non-preemptive) 스케줄링
* 어떤 프로세스가 cpu 점유하고 있을 시 뻇을 수 없도록 하는 방식, 프로세스에 배치에 따라 효율성 차이가 크게 나게 된다.
<br>

### 1-1 비선점형 스케줄링 종류
* FCFS(First Come, First Served)
* 가장 먼저 요청한 프로세스에 CPU 할당해주는 선착순 방식, 몇 개의 시간이 오래 걸리는 프로세스 존재 시 전체 os 느려지는 현상 발생할 수 있다.
<br>

* SJF(Shortest Job First)
* 실행 시간이 가장 짧은 프로세스 먼저 실행하는 알고리즘, 긴 시간 필요로 하는 프로세스 우선순위 밀려 무기한 대기하는 기아 현상 발생할 수 있다.
<br>

## 1. 비선점형(non-preemptive) 스케줄링
* 어떤 프로세스가 cpu 점유하고 있을 시 뻇을 수 없도록 하는 방식, 프로세스에 배치에 따라 효율성 차이가 크게 나게 된다.
<br>

### 1-1 비선점형 스케줄링 종류
* FCFS(First Come, First Served)
* 가장 먼저 요청한 프로세스에 CPU 할당해주는 선착순 방식, 몇 개의 시간이 오래 걸리는 프로세스 존재 시 전체 os 느려지는 현상 발생할 수 있다.
<br>

* SJF(Shortest Job First)
* 실행 시간이 가장 짧은 프로세스 먼저 실행하는 알고리즘, 긴 시간 필요로 하는 프로세스 우선순위 밀려 무기한 대기하는 기아 현상 발생할 수 있다.
<br>



> 23.08.23 정리 중
