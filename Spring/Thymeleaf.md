# Thymeleaf


## Thymeleaf
<hr>

## 템플릿 엔진(Template Engine)
### HTML(Markup)과 데이터를 결합한 결과문을 만들어 주는 도구
### Thymeleaf는 템플릿 엔진 중 하나로, Spring Boot에서 JSP가 아닌 Thymeleaf를 사용 권장
### JSP, Freemarked와 같이 서버에서 클라이언트에게 응답할 브라우저 화면을 만들어주는 역할
<br>

## 사용 방법
### Gradle에 dependency 다음과 같이 추가
![image](https://user-images.githubusercontent.com/57441201/173231044-b2d78760-2ff9-4912-9a54-272986351efd.png)

### Gradle에 추가 후 html 태그에 위의 코드를 추가
![image](https://user-images.githubusercontent.com/57441201/173231083-649661c9-8dad-4951-a01b-28a24e1e1dd8.png)

<br>

## 주요 문법
### xmlns:th
  * 타임리프의 th 속성을 사용하기 위해 선언된 네임스페이스
  * 순수 HTML로만 이루어진 페이지의 경우, 선언하지 않아도 무방

### th:text
  * JSP EL 표현식인 ${}와 마찬가지로 타임리프도 ${} 표현식 사용, 컨트롤러에서 전달받은 데이터 접근
  * 일반적인 텍스트 형식으로 화면에 출력

### th:fragment
  *  <head> 태그에 해당 속성 사용하여 fragment 이름 지정
  * fragment는 다른 HTML에서 include 또는 replace 속성 사용하여 적용 가능
  
### th:block
  * layoutL:fragment 속성에 이름을 지정해서 실제 Content 페이지의 내용 채우는 기능
  * 해당 기능은 동적인 처리가 필요할 때 사용
  
### th:replace="~{파일경로 :: 조각이름}"
  * JSP의 <include> 태그와 유사한 속성
  * th:fragment을 통해 설정한 이름을 찾아 해당 코드로 치환
  
### th:href
  * <a> 태그의 href 속성과 동일
  
### xmlns:layout, xmlnslayout:decorator
  * xmlns:layout은 타임리프의 레이아웃 기능을 사용하기 위한 선언
  * xmlnslayout:decorator 레이아웃으로 ~~~.html을 사용하겠다는 의미
  * ::을 기준으로 앞에는 조각이 있는 경로, 뒤에는 조각의 이름
  
### Form 태그 예시
  * ![image](https://user-images.githubusercontent.com/57441201/173233257-05a535f0-fd84-44d7-aa15-db12859c9d20.png)

  
### th:action
  * <form> 태그 사용시 해당 경로로 요청을 보낼 떄 사용
  
### th:object
  * <form> 태그에서 submit 할 때, 데이터가 th:object에 설정해둔 객체로 받아짐
  * 컨트롤러와 뷰 사이의 DTO 클래스 객체
  * ![image](https://user-images.githubusercontent.com/57441201/173232661-49dad68b-edbe-43dd-841d-133443a02ab4.png)

### th:field
  * 위의 th:object 속성을 이용하면, th:field를 이용해서 HTML 태그에 맴버 변수를 매핑 할 수 있음
  * th:field를 이용한 사용자 입력 필드는 id, name, value 속성 값이 자동으로 매핑
  * th:field는 ${} 표현식이 아닌, *{} 표현식 사용
  * th:object와 th:filed는 컨트롤러에서 특정 클래스의 객체를 전달 받은 경우에만 사용 가능

<br>

> 22.06.12 정리
