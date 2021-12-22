# 스프링 입문 - 코드로 배우는 스프링 부트, 웹 MVC, DB 접근 기술
> 인프런의 김영한님 강의를 들으며 공부하고 실습한 내용을 정리한 repo


## Project 구성
+ Project : Gradle Project 
+ Spring Boot : 2.3.x 
+ Language : Java 
+ Packaging : Jar
+ Java : 11
+ Dependencies : Spring Web, Thymeleaf, spring-boot-devtools

## Library 살펴보기
+ Gradle은 의존관계가 있는 라이브러리를 함께 다운로드 한다.
+ 스프링 부트 라이브러리
  + spring-boot-starter-web 
    + spring-boot-starter-tomcat : 톰캣 (웹서버) 
    + spring-webmvc : 스프링 웹 MVC
  + spring-boot-starter-thymeleaf : 타임리프 템플릿 엔진(View) 
  + spring-boot-starter(공통) : 스프링 부트 + 스프링 코어 + 로깅
    + spring-boot 
      + spring-core
  + spring-boot-starter-logging 
    + logback, slf4j
+ 테스트 라이브러리
  + spring-boot-starter-test
    + junit : 테스트 프레임워크
    + mockito : 목 라이브러리
    + assertj: 테스트 코드를 좀 더 편하게 작성하게 도와주는 라이브러리 
    + spring-test: 스프링 통합 테스트 지원
    
## Build & Run
+ For MacOS
  1. 터미널 -> ./gradlew build
  2. cd build/libs
  3. java -jar hello-spring-0.0.1-SNAPSHOT.jar
+ For Windows
  1. 명령 프롬프트(cmd) or git bash -> ./gradlew 
  2. gradlew.bat 를 실행(명령 프롬프트에서는 gradlew 하고 엔터)
  3. gradlew build

## Welcome Page
+ [스프링 부트가 제공하는 Welcome Page 기능](https://docs.spring.io/spring-boot/docs/2.3.1.RELEASE/reference/html/spring-boot-%20features.html#boot-features-spring-mvc-welcome-page)
+ static/index.html 을 올려두면 Welcome page 기능을 제공