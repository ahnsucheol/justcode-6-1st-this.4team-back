
<div align="center">
  <img src="https://user-images.githubusercontent.com/110225060/197337903-82af5ddd-444f-443b-a16a-b48b56ef2bf1.png" width=200/>

  ### 👉 이거사조팀의 **[Hola!](https://holaworld.io/)** 클론 코딩 프로젝트
</div>

---
<br>

## **프로젝트 소개**
```
개발 관련 스터디, 프로젝트 동료 구하는 사이트로 기술 스택 별로 게시글을 보여주며, 사용자가 글
을 작성 및 댓글을 남겨 원하는 팀원을 구할 수 있습니다.
```

<br>

### **개발 인원 및 기간**

- 개발기간 : 2022/8/29 ~ 2022/9/8
- 개발 인원 : 6명
- 프론트 엔드 : 이혜림, 안승섭, 박유빈, 이고운
- 백 엔드 : 김현정, 안수철

<br>

## 역할 분담

- 이혜림
    - header nav
    - footer
    - 새글 작성 UI 및 api 연동
    - 사용자 수정 UI 및 api 연동
- 안승섭
    - 메인 화면 UI, 내 글 목록 화면 UI
    - 무한 스크롤, API 연동
    - 각종 버그 수정
- 박유빈
    - 게시글 상세페이지 UI
    - 게시글 삭제 및 뒤로가기
    - 댓글 리스트 UI
    - 댓글 작성, 수정 , 삭제
- 이고운
    - 로그인
    - 이용약관
    - 회원가입
- 김현정
    - 회원가입 및 로그인
    - 사용자 정보 가져오기 및 정보 수정
    - 게시글 목록 가져오기
    - 게시글 선택 내용 읽기
    - 기술 스택 목록 읽어오기
- 안수철
   - 게시글 작성, 수정, 삭제
   - 댓글 불러오기, 작성, 수정, 삭제

<br>

### **프로젝트 선정이유**
-  Hola Word는 겉보기에는 간단한 사이트처럼 보이지만, 게시글과 댓글의 작성, 읽기, 수정, 삭제 등 웹 개발의 기본적인 기능을 경험해 볼 수 있는 사이트입니다. 이 프로젝트는 부트 캠프에서 처음 시작하는 프로젝트인 만큼 현업에서 사용되는 기술과 기능을 최대한 반영하여 웹 개발의 기본적인 기능을 경험해 볼 수 있도록 구현하였습니다.
-  e-commerce 사이트의 경우 조회에 관련된 기능들이 메인으로 조회 기능에 치우쳐서 프로젝트를 진행하기 보다는 밸런스있게 CRUD를 경험하고자 선정하였습니다.
-  이미지 저작권 문제 해소

### **사용 스택**
#### FE
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=React&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=Sass&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/Slick-FF880F?style=for-the-badge&logo=SlickPic&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/React modal-0088CC?style=for-the-badge&logo=React&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/Create portal-09D3AC?style=for-the-badge&logo=Create React App&logoColor=white"/>&nbsp; <br>
#### BE
<img src="https://img.shields.io/badge/Node.js-39933?style=for-the-badge&logo=Node.js&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/TypeORM-262627?style=for-the-badge&logo=TypeORM&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/Bcrypt-003A70?style=for-the-badge&logo=Bcrypt&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/JWT-FBBA00?style=for-the-badge&logo=JWT&logoColor=white"/>&nbsp;
<img src="https://img.shields.io/badge/RESTful API-2478CC?style=for-the-badge&logo=RESTful API&logoColor=white"/>&nbsp;

<br>


# _✨프로젝트 구조_
```
📦/
 ┣ 📂controllers
 ┣ 📂db
 ┣ 📂middleware
 ┣ 📂models
 ┣ 📂routes
 ┣ 📂services
 ┣ 📜app.js.js
 ┣ 📜package-lock.json
 ┣ 📜package.json
 ┗ 📜server.js
```
<br>

# _✨DB 모델링_
![](https://user-images.githubusercontent.com/110225060/197342659-41c8fe87-7d62-4e41-a043-8bddd7b9c064.png)

<br>

### **구현 기능**
📌[API 명세서 ](https://documenter.getpostman.com/view/22723177/VUxNR7mw#dd4ed3cb-7fdc-4575-8732-19c22d916e9b)


**회원가입**
- 아이디와 비밀번호를 입력 받아 가입할 수 있는 간단한 회원 가입 API.
- 아이디의 중복 여부 체크, 그리고 비밀번호를 해시 함수로 암호화하는 기능이 포함되어 있습니다.

**로그인**
- 입력 받은 아이디와 비밀번호를 받아와 로그인할 수 있는 API
- 사용자는 로그인을 성공적으로 마쳤을 경우 토큰을 발급 받을 수 있습니다.

**사용자 정보**
- 로그인한 사용자에게 발급 된 토큰으로 아이디를 확인하여 정보를 가지고와 수정하는 API
- 발급 된 토큰으로 알맞은 사용자가 요청하였는지 확인 후 수정이 진행됩니다.

**기술 스택 리스트**
- 기술 스택의 목록을 읽어오는 API
- 각 기술 스택의 카테고리에 알맞는 것을 보여주는 필터링 기능과 인기 목록의 경우 자주 작성된 기술 스택 중 상위 10개를 보여주도록 하였습니다.

**게시글 목록 읽어오기**
- 작성된 게시글 목록을 읽어오는 API
- 게시글에 선택된 기술 스택으로 검색할 수 있는 필터링 기능과, 한 화면에 보여지는 게시글 수를 조정할 수 있는 페이징 기능이 포함되어 있습니다.

**게시글 내용 읽어오기**
- 목록에서 선택된 게시글의 내용을 보여주는 API

**게시글 작성**
- 게시글을 작성하는 API
- 발급 된 토큰으로 어떤 사용자가 작성하였는지 구분하여 데이터베이스 테이블에 데이터가 삽입됩니다.

**게시글 수정&삭제**
- 게시글을 수정&삭제하는 API
- 발급 된 토큰으로 구분하여 게시글 작성자와 로그인 한 유저가 같아야 수정 혹은 삭제가 가능하게 구현하였습니다.

**댓글 읽어오기**
- 게시글에 작성된 댓글을 읽어오는 API

**댓글 작성**
- 댓글을 작성하는 API
- 발급 된 토큰으로 어떤 사용자가 작성하였는지 구분하여 데이터베이스 테이블에 데이터가 삽입됩니다.

**댓글 수정&삭제**
- 댓글을 수정&삭제하는 API
- 발급 된 토큰으로 구분하여 댓글 작성자와 로그인 한 유저가 같아야 수정 혹은 삭제가 가능하게 구현하였습니다.


<br>

# _✨프로젝트 실행 방법_
### 1. 레포지토리 clone

```
git clone https://github.com/ahnsucheol/justcode-6-1st-this.4team-back.git
```

### 2. 프로젝트 폴더 선택 후 아래의 명령어 실행
```
npm i
```

### 3. 데이터베이스 스키마 설정
dbmate 설치 관련은 [참조](https://github.com/amacneil/dbmate)
```
dbmate up
```

### 4. .env 환경변수 설정
```
DATABASE_URL={dbmate 연동 URL} 
ex) mysql://{user}:{password}@{host}:{port}/{dbname}
TYPEORM_CONNECTION = 사용할 데이터베이스 종류
TYPEORM_HOST = host              
TYPEORM_PORT = port                   
TYPEORM_USERNAME = user               
TYPEORM_PASSWORD = password         
TYPEORM_DATABASE = dbname
```

### 5. 프로젝트 실행
```
npm start
```

<br>

# _📹프로젝트 시연 영상_
[![프로젝트 시연 영상](http://img.youtube.com/vi/xo1gqoUQRx0/0.jpg)](https://youtu.be/xo1gqoUQRx0?t=0s) 

<br>

# *✨링크*
### 👉[API 명세서 ](https://documenter.getpostman.com/view/22723177/2s847Ftsdk)  
### 👉[프론트엔드 Github 링크](https://github.com/wecode-bootcamp-korea/justcode-6-1st-this.4team-front) 
