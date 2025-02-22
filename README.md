# Zenith 코드 에디터 사이트

**웹 기반 실시간 코드 편집 및 협업 플랫폼**

Monaco Editor와 WebSocket을 활용하여 실시간 코드 작성과 다중 사용자 동기화를 지원하는 코드 에디터 프로젝트입니다. 
사용자 맞춤형 설정(테마, 폰트, 템플릿) 관리 기능을 제공하며, 
Spring MVC와 MyBatis를 기반으로 확장성과 유지보수성을 고려해 설계되었습니다.

<br> 

## 목표

개발자들이 별도의 설치 없이 동일한 환경에서 실시간으로 협업하며 효율적으로 코드 작업을 수행할 수 있도록 **Monaco Editor**와 **WebSocket**을 활용한 동기화된 코드 편집 환경을 구축합니다. 
이를 통해 예비 개발자들이 실제 협업 환경을 경험하고, 다양한 요구를 충족하는 실용적인 플랫폼을 제공합니다.

<br> 

## 핵심 기능

- **실시간 코드 편집 및 실행**: Monaco Editor와 WebSocket을 통해 코드 작성과 실행을 실시간으로 동기화.
- **사용자 맞춤형 설정 관리**: 테마, 폰트, 색상, 템플릿 등의 설정을 저장하고 실시간으로 반영.
- **다중 사용자 동기화**: WebSocket을 통한 다중 사용자 협업 및 실시간 동기화 지원.
- **협업 채팅 및 챗봇**: 팀원들과의 실시간 채팅 및 코드 작성 지원을 위한 챗봇 기능 제공.

<br> 

## 개발 환경

-   **운영체제**: Windows 11, macOS, Linux(Ubuntu)
-   **서버**: Apache Tomcat, AWS EC2, Oracle
-   **개발 툴**: STS 3, Visual Studio Code, SQL Developer
-   **협업 툴**: GitHub, Notion, Discord, ERD Cloud, Draw\.io, Figma, Google Drive, MiriCanvas

<br> 

## 사용 기술

-   **프로그래밍 언어**: Java 11, HTML, CSS, JavaScript (ES6), ANSI-SQL, PL/SQL
-   **프레임워크 및 라이브러리**:
    -   Spring, Maven, Spring Security, Lombok, HikariCP, MyBatis, Tiles, Jackson
    -   jQuery, jQuery UI, Ajax, RESTful API
    -   Monaco Editor, OpenAI API, FullCalendar Library
-   **데이터베이스**: Oracle 11g EX

<br>

## 사용 기술

- **Spring MVC**: MVC 구조를 기반으로 한 웹 애플리케이션 개발.
- **MyBatis**: 데이터베이스 연동을 위한 ORM 프레임워크.
- **WebSocket**: 실시간 양방향 통신을 통한 코드 편집 동기화.
- **Monaco Editor**: 고성능 코드 에디터를 이용한 실시간 코드 편집 환경.
- **AJAX**: 비동기 처리를 통해 빠른 응답 속도 제공.

<br> 

## 성과

- Monaco Editor와 WebSocket을 이용한 실시간 코드 편집 및 실행 기능 구현.
- 사용자가 선택한 설정(테마, 폰트, 색상 등)을 저장하고 실시간으로 반영.
- 다중 사용자가 동시에 작업할 수 있는 동기화된 협업 환경 구축.
- Spring MVC와 MyBatis를 활용하여 데이터베이스 최적화 및 안정적 연동.
- OpenAI API 연동을 통한 코드 작성 및 학습 지원 기능 구현.

<br> 

## 트러블 슈팅 및 성능 최적화 경험

**1. Lazy Loading 활용 및 성능 최적화 경험**

연관 데이터 조회 시 불필요한 데이터 로딩을 방지하기 위해, `MyBatis`에서 **Lazy Loading**을 적용하여 성능을 최적화하였습니다. 
이로 인해 데이터 조회 시 불필요한 쿼리 실행을 줄여, **응답 속도**와 **서버 부하**를 크게 개선할 수 있었습니다.

<br> 

**2. 모듈화된 데이터 삽입 프로시저 사용**

코드 유지보수성을 높이기 위해 **프로시저**를 활용하여 데이터 삽입 작업을 모듈화하고, 중복된 작업을 최소화했습니다.

- 리팩토링 전: 각 회원별 기본 설정값 삽입을 코드로 반복 작성
- 리팩토링 후: 프로시저 호출로 **코드 간소화 및 관리 용이성 증가**

<br> 

**3. HikariCP로 데이터베이스 커넥션 풀 성능 개선**

기본 JDBC 커넥션 풀 대신 HikariCP를 사용하여 데이터베이스 연결 성능을 최적화하였습니다. 
HikariCP는 빠르고 효율적인 커넥션 풀 관리 기능을 제공하여 데이터베이스 연결을 보다 빠르게 처리하고, **서버의 부하**를 줄이며, **응답 속도**를 개선할 수 있었습니다.

<br> 

**4. Ajax 비동기 처리로 사용자 경험 개선**

`Ajax`를 활용하여 비동기 방식으로 데이터를 처리함으로써, 페이지 새로 고침 없이 빠른 응답을 제공하고 사용자 경험을 개선했습니다.

- 리팩토링 전: 페이지 리로드로 데이터 처리 및 응답 시간 증가
- 리팩토링 후: 비동기 처리로 페이지 리로드 없이 빠른 데이터 처리 및 응답 속도 개선

<br> 

## 프로젝트 링크

- 원본 레포지토리: https://github.com/chimy2/code-editor
