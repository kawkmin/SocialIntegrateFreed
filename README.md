# 소셜 미디어 통합 feed 서비스

![image](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/assets/86940335/9b560f6e-8a9d-4398-98dd-e24ac97ac7e4)
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Spring Boot 3.1.5-6DB33F?style=for-the-badge&logo=spring&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Spring Security-6DB33F?style=for-the-badge&logo=spring-security&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Spring rest docs-6DB33F?style=for-the-badge"/></a>
<img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Spring Data JPA-gray?style=for-the-badge&logoColor=white"/></a>
<img src="https://img.shields.io/badge/QueryDSL-0078D4?style=for-the-badge&logo=Spring Data JPA&logoColor=white"/></a>
<img src="https://img.shields.io/badge/MySQL 8-4479A1?style=for-the-badge&logo=MySQL&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Junit-25A162?style=for-the-badge&logo=JUnit5&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Mockito-6DB33F?style=for-the-badge"/></a>

## 목차

1. [개발 기간](#개발-기간)
2. [프로젝트 개요](#프로젝트-개요)
3. [프로젝트 일정관리](#프로젝트-일정관리)
4. [구현 기능 목록](#구현-기능-목록)
5. [ERD](#erd)
6. [구현 과정](#구현-과정)
7. [담당한 역할](#담당한-역할)
8. [API 명세](#api-명세)
9. [테스트](#테스트)

## 개발 기간

2023-10-25 ~ 2023-10-30 (6일)

## 코드 컨벤션

코드 컨벤션 관한 노션 정리

https://mizuirohoshi7.notion.site/b298797bef954741bd7ab33a047ba01a

## 프로젝트 개요

여러 SNS의 게시물들을 한번에 관리하는 서비스입니다.

검색한 해시태그가 포함된 게시물들을 하나의 서비스에서 확인할 수 있습니다.

이를 통해 본 서비스의 고객은 하나의 채널로 유저, 브랜드 등 SNS 노출 게시물 및 통계를 확인할 수 있습니다.

좋아요, 공유 기능도 SNS를 각각 이용하지 않고 한번에 수행할 수 있습니다.

## 프로젝트 일정관리

**Git Projects 사용**

<details>
    <summary>자세히 (클릭)</summary>

[Git Projects 링크 (클릭)](https://github.com/orgs/wanted-preonboarding-team-m/projects/1/views/5)
![image](https://github.com/kawkmin/smart_budget_craft/assets/86940335/a0d7f93b-e160-4a9d-a62d-e3c2ffabd36e)

</details>


## 구현 기능 목록

<details>
    <summary>자세히 (클릭)</summary>

- 유저

  - 회원가입
  - 가입승인
  - 로그인

- 피드

  - 피드 목록
  - 피드 상세
  - 피드 좋아요 (실제 연동은 구현되지 않았습니다.)
  - 피드 공유 (실제 연동은 구현되지 않았습니다.)

- 통계
  - 해시태그를 날짜 혹은 시간으로 조회

</details>

## ERD

**Erd Cloud**

<details>
    <summary>자세히 (클릭)</summary>

![erd](https://github.com/wanted-preonboarding-team-m/.github/assets/142835195/656e203d-677d-41a6-8109-b12db38047f9)

</details>

## 구현 과정

1. [프로젝트 환경 설정](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/issues/1)

   - application.yml 설정
   - P6Spy 설정
   - RestDocs 설정
   - Response Api Format 설정
   - [공통 예외 처리](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/issues/5)

2. 유저 기능 구현

   - [유저 엔티티 생성](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/issues/2)
   - [유저 등록 구현](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/issues/6)

3. 게시물 기능 구현

   - [게시물 엔티티 생성](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/issues/7)
   - [게시물 CRUD 구현](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/issues/11)
   - [좋아요 및 공유 기능](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/issues/33)

4. 통계 기능 구현
   - [쿼리 파라미터로 검색하여 통계 결과 생성](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/issues/22)

## 담당한 역할

- [김정훈](https://github.com/jhva): 유저 인증/인가
- [곽민성](https://github.com/kawkmin): 프로젝트 환경 설정
- [김선재](https://github.com/mizuirohoshi7): 통계, 좋아요 및 공유 기능
- [최소영](https://github.com/soyeong125): 게시물 CRUD

- 코드 리뷰 및 리팩토링은 조원 모두가 함께 했습니다.

## API 명세

**Spring Rest Docs 기반 API 명세서**


<details>
    <summary>자세히 (클릭)</summary>


[API 명세서 보기 (클릭)](https://wanted-preonboarding-team-m.github.io/01_SocialIntegrateFreed/src/main/resources/static/index.html)
![image](https://github.com/kawkmin/smart_budget_craft/assets/86940335/bdaf41ab-9ad4-43a7-894d-7c940986cce3)


</details>

## 테스트

### ✅ 43/43 (2초 278ms)

![테스트 결과](https://github.com/wanted-preonboarding-team-m/01_SocialIntegrateFreed/assets/86940335/de460e75-9c09-407c-84a3-d3b681f19f96)

단위 테스트로 각 계층을 분리했습니다.
