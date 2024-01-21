# 1. 프로젝트 기본 세팅

## 1.1. 스프링 프로젝트 구성
* [Spring 공식 웹사이트](https://start.spring.io/)에서 기본적인 세팅을 넣어주면 프로젝트를 자동으로 생성해줌. 해당 서비스를 이용하자.
> Spring web을 dependency로 추가

## 1.2. JDK 세팅
* `build.gradle` 에 정의된 `java.sourceCompatibility` 가 `21`로 설정되었기 때문에 해당 버전에 맞는 JDK 다운로드 필요
* 다음과 같이 openjdk 설치 
```
brew install temurin21
```

# 2. 프로젝트 구조
* 가장 많이 본 Spring Controller - Service - Dao 구조로 구성해보자
* 추후 `@RestController`로 교체해도 되니 일단은 `@Controller`로 생각없이 작성해보자
> 중단점: 기존에 vscode에 세팅해놓은 플러그인들이 adoptopenjdk11로 설정되어있어서 현재 설정해놓은 프로젝트와 호환이 잘 안되는 것 같음. 자동완성도 안되고...

> 시도중: 이유를 찾아보자...