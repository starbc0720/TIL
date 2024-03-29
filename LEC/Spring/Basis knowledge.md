# 자바 공부하기 전 알아두면 좋을 기초 상식
<br>

## 기초 상식
<br>

* 컴파일
  * 인간이 이해하기 쉬운 언어를 기계어로 번역하는 과정
 
* 컴파일러
  * 컴파일을 하는 프로그램
  * ex) JVM (Java에서 사용하는 컴파일러, Java 바이트 코드를 OS마다 다르게 해석)

* 바이트 코드
  * 0과 1로 이루어진 코드, 컴퓨터가 이해 가능

![image](https://github.com/starbc0720/TIL/assets/57441201/851de2b9-87e8-4d3d-bb89-88886cbeca37)

<br>

* JVM(Java Virtual Machine)
  * 자바 가상 머신 
  * OS 별로 존재
  * 바이너리 코드를 읽고 검증
 
* JRE(Java Runtime Environment)
  * 자바 실행 환경
  * JVM + 자바 프로그램 실행에 필요한 라이브러리 파일 등
  * JVM의 실행환경 구현
 
* JDK(Java Development Kit)
  * 자바 개발 도구
  * JRE + 개발을 위한 도구
  * 컴파일러, 디버그 도구 등이 포

![image](https://github.com/starbc0720/TIL/assets/57441201/892a99f3-a962-4a22-8d34-5ef0f038c1ba)

<br>

* 빌드(build)
  * 소스 코드 파일을 컴퓨터에서 실행할 수 있는 독립 SW 가공물로 변환시키는 과정 
  * JRE + 개발을 위한 도구
  * 컴파일러, 디버그 도구 등이 포함

 
* 실행(run)
  * 내가 작성한 코드를 컴파일하여 작동시켜 보는 것
  * JRE + 개발을 위한 도구
  * 컴파일러, 디버그 도구 등이 포함

 
* 빌드 툴(build tool)
  * 소스코드의 빌드 과정을 자동으로 처리 해주는 프로그램
  * 외부 소스 코드 (외부 라이브러리) 자동 추가, 관리
  * ex) APACHE ANT, MAVEN, GRADLE

 
* Apach Ant
  * 설정 위해 xml 사용
  * 간단하고 사용하기 쉬움
  * 복잡한 처리 -> 빌드 스크립트 장황 -> 관리 어렵
  * 외부 라이브러리 관리하는 구조 미존재


* Maven
  * 설정 위해 xml 사용
  * 외부 라이브러리 관리 가능
  * 장황한 빌드 스크립트 문제 해결
  * 특정 경우 xml 복잡해질 수 있음
  * xml 자체 한계 존재

 
* Gradle
  * 설정을 위해 groovy 언어 사용
  * 외부 라이브러리 관리
  * 유연하게 빌드 스크립트 작성 가능
  * 성능 뛰어남

 
* HTTP
  * HTTP(HyperText Transfer Protocol)
  * Protocol : 표준, 약속
  * ex) HTTP Method
    * GET -> 데이터를 달라 요청, 쿼리 
    * POST -> 데이터를 저장하라 요청, 바디
    * PUT -> 데이터를 수정하라, 바디
    * DELETE -> 데이터를 삭제하라 쿼리 


* API(Application Programming Interface)
  * 정해진 약속을 하여, 특정 기능을 수행하는 것 


* URL(Uniform Resource Locator)
  * 주소창
  * http://spring.com:3000/portion?color=red&count=2
  * http -> 사용하고 있는 프로토콜 종류
  * // -> 구분기호
  * spring.com:3000 -> 도메인 이름, ip로 대체 가능
  * portion -> path(자원의 경로)
  * color=red&count=2 -> 쿼리(추가 정보)


* HTTP 응답 종류
  * 200 : 정상적으로 응답
  * 300 : 다른곳으로 요청해야하는 상태
  * 404 : 요청하는 곳을 못찾음
  * 500 : 내부 오류


* HTTP 응답 종류
  * 200 : 정상적으로 응답
 

* JSON(JavaScript Object Notation)
  * 객체 표기법
  * 중괄호({. }) 무조건 양 끝에 존재
  * 중괄호 안에 "key" : value로 표기
  * ex)
   * {"name" : "최태현", "age" : 99}
  * 속성은 각각 쉼표로 구분





* [출처] https://www.youtube.com/watch?v=f0cAmTYo4tQ


> 23.07.18 수정 
