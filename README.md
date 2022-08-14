# 월하합작(MVC)_

# 월하합작: 전국 8도 명주를 찾아서

---

1. 프로젝트 개요
    - 한국 전통주 온라인 판매가 허용됨에 따라 전통주 수요가 증가함
    - 또한, 코로나19 거리두기로 인해 Home술, 혼술은 선택이 아닌 필수가 됨
    - 이에 따라 만 19세 이상 회원에 한해 판매가 이루어지는 온라인 전통주 쇼핑몰 서비스를 기획함
    
2. 설계의 주안점 (프로젝트 결과 탭을 참조해주세요!)
    - Git 커밋메세지 및 Naming 컨벤션을 설정한다.
    - 개발프로세스로는 칸반을 사용한다.
    - 오픈소스를 활용한다.
    - MVC 패턴으로 개발한다.
    - Spring Security로 권한을 관리한다.

1. 프로젝트 진행 기간
    - 2021-1-12 ~ 2021-02-09 : 총 29일

## 1. 기술 스택

---

1. Backend 
    - Tomcat 8.5
    - Spring MVC
    - Spring Security
    - MyBatis
    - Java11

1. Database
    - Oracle - SQLDeveloper
    
2. Server 
    - AWS

1. Frontend
    - Javascript
    - Jquery
    - JSTL
    - Gson

1. Collaboration tool 
    - Git and Github
    - Notion
    - Slack
    - Figma

## 2. ERD 명세서

---

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/dd3798d2-3e57-40ef-83a9-619a898f3310/Untitled.png)

- 상세 보기를 원하시면 아래 Url을 참고해주세요.
    
    [https://www.erdcloud.com/d/wdNtYArwPCWpBgcAj](https://www.erdcloud.com/d/wdNtYArwPCWpBgcAj)
    

## 3. 담당 주요 구현 기능

---

1. 회원가입
- Ajax 통신을 통한 휴대폰 인증 기능
- 휴대폰 인증 기능
    - 오픈소스 문자 전송 API 활용
- 생년월일 정규표현식

1. 문의 기능
- User 권한 사용자
    - 1:1 문의기능 작성 시 본인 작성 게시글만 조회
    - 게시글 상세 조회는 Ajax로 구현
    - 게시글 삭제
- Admin 권한 사용자
    - 전체 문의글 조회
    - 게시글 삭제
    - 답변 작성
    - 답변 삭제

1. 오픈 소스 활용
- 휴대폰 인증 구현 시 문자 전송 API 활용
- 지역별 전통주 종류 개수를 카카오지도 API 를 활용해 클러스터로 나타냄

## 4. 프로젝트 결과

---

1) 월하합작 프로젝트 Overview 

![Honeycam 2022-08-13 07-48-44.gif](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d835a742-52c6-46ba-b477-e15a85757d51/Honeycam_2022-08-13_07-48-44.gif)

- [http://3.37.11.69/](http://3.37.11.69/)

2) Git 커밋메세지와 Naming 컨벤션을 설정한다.  

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/44a1182b-8afb-452b-a453-06608f9d10a7/Untitled.png)

- 컨벤션에 관한 자세한 사항은 아래 Notion 페이지를 참고해주세요!

3) 개발프로세스로는 칸반을 사용한다. 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/36a35ac8-43ec-4585-b803-955d1de4f092/Untitled.png)

- 자세한 사항은 월하합작팀 Notion 을 통해 확인하실 수 있습니다.

4) 오픈소스를 활용한다. 

- 휴대폰 문자 전송 API
    - 회원가입 시 사용자의 휴대폰 번호가 유효한지 검증하는 로직을 구현함
    - 아이디 찾기 시 휴대폰 인증을 통해 본인확인 하는 로직을 구현함
- 카카오결제 API
    - 결제 시 카카오결제와 일반 카드 결제로 구분해서 구현함
- 카카오지도 API
    - 지역별 전통주 입점 수량을 클러스터로 지도에 나타냄
    

## 5. 참고 사항

---

월하합작 팀의 컨벤션 및 회의록 등, 개발 세부 진행사항을 확인하고 싶다면 

아래 Notion 링크를 참조해주세요 ! 

- 월하합작: 전국 8도 명주를 찾아서, Notion 바로가기