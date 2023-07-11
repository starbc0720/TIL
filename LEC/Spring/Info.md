# Spring Framework 사용 시 발생할 수 있는 에러에 대한 조치사항
<br>

## Casue: invalid source release 11 에러
<br>

* 내가 생성한 프로젝트 Java 버전과 내 컴퓨터에 설치/설정된 Java 버전이 일치하지 않기 때문에 발생
  * sol 1) JDK 다운로드/설치 후 환경 변수 편집
    *  syscdm.cpl 명령어 입력, JAVA_HOME 경로를 새로 다운받은 JDK 설치 경로로 편집
    
  * sol 2) IDE에서 Java 버전 재설정
    *  ctrl + shift + alt + s 입력 Project SDK와 Project Lanugauge Level을 프로젝트 버전에 맞춤
    ![image](https://github.com/starbc0720/TIL/assets/57441201/74be3f4a-1f8d-424e-bf26-cb2cc18a02ff)

    *  ctrl + alt + s 입력 Build Tool - Gradle로 이동 Gradle JVM을 새로 설치한 JDK 버전에 맞게 재설정
    ![image](https://github.com/starbc0720/TIL/assets/57441201/9569a423-8d96-4023-8bc7-19d417c4d731)





* [출처] https://charliecharlie.tistory.com/315




> 23.07.12 정리
