# 홈스타그램 프로젝트 소개

인테리어 커머스 사이트 프로젝트<br/>
프로젝트 기간이 길지 않아 전체가 아닌 일부 기능에 집중해 기획했습니다.<br/>
개발은 초기 세팅부터 전부 직접 구현했으며, 아래 데모 영상에서 보이는 부분은 실제 사용할 수 있는 서비스 수준으로 개발한 것입니다.

### 개발 인원 및 기간<br/>
개발기간 : 2021/8/17 ~ 2021/8/27<br/>
프론트엔드 : 이지선, 최정민, 남재현<br/>
백엔드 : 장호준, 송진수<br/>
백엔드 깃헙 주소 : https://github.com/bigfanoftim/23-2nd-Homestagram-backend

### 프로젝트 선정이유<br/>
게시글 속 태그를 통하여 커뮤니티와 커머스 기능을 결합한 점에 매력을 느끼고, 이에 모티브를 얻어 OpenMarket은 존재한다는 가정하에 SNS기능에 집중하여 프로젝트를 진행하였습니다.

### 데모 영상<br/>
https://youtube.com/watch?v=ZxATcPFrrqg

### 사이트 이미지<br/>
#### Main Feed
<img width="803" alt="main" src="https://user-images.githubusercontent.com/4047515/131617686-abeeccd1-cf7f-44ef-9b6f-65083e91e2cc.png">

#### Product Page
<img width="829" alt="detail page" src="https://user-images.githubusercontent.com/4047515/131617802-9680cf05-192c-4094-b93b-d2f63268ec9f.png">

#### Order Page
<img width="708" alt="order page" src="https://user-images.githubusercontent.com/4047515/131617834-968daeec-d882-450e-8dc5-2c6ebc5764ec.png">

#### Paypal
<img width="958" alt="paypal" src="https://user-images.githubusercontent.com/4047515/131617858-1aeaf7e2-17b7-4036-ac18-e5b5d971ff65.png">

#### My Info
<img width="823" alt="my info" src="https://user-images.githubusercontent.com/4047515/131617873-b0d2d9ce-8408-4dd6-be7a-2b7888174454.png">

#### Write Feed
<img width="879" alt="KakaoTalk_Photo_2021-08-30-21-18-10" src="https://user-images.githubusercontent.com/4047515/131617912-836f4f15-9691-4e17-8352-67d82c0298af.png">

#### Image Tag
<img width="892" alt="image tag1" src="https://user-images.githubusercontent.com/4047515/131617925-bd20f152-ee85-41ef-a5ee-3bc0cf242223.png">
<img width="763" alt="image tag2" src="https://user-images.githubusercontent.com/4047515/131617934-a9b4673e-6329-4ca7-ad55-505f25edb97e.png">

**적용 기술 및 구현 기능** <br/>
Front-End : HTML5, React, JavaScript <br/>
Back-End : Python, Django web framework, Bcrypt, PyJWT, MySQL <br/>
Common : AWS(RDS/EC2/S3), KAKAO social login, PayPal API, RESTful API <br/>
Communication: Slack, Trello, Goolge Docs <br/>


#메인 서비스
**구현 기능 상세**
---------------------
### 공통
 - CRA를 이용한 초기셋팅
 - Footer

### 소셜로그인 (최정민)
- 모달 창을 이용한 회원추가 정보 가입
- Kakao Api를 사용하여 로그인
- 카카오 소셜 로그인 API를 통한 유효성 검사
- JWT 토큰 발행 후 닉네임 설정, 사이트 내 로그인 수행

### 피드 업로드 기능 (최정민)
- 모달창을 통해 피드 작성
- 이미지 업로드 및 description 입력 
- 이미지 속 원하는 위치에 태그를 추가하여 구매한 목록을 중 해당되는 상품을 선택하여 매치할 수 있는 기능

### 피드 페이지 (최정민)
- 업로드 한 피드들이 보여짐
- 피드 사진에 마우스 호버시 추가되어있는 태그들이 나타남
- 태그 클릭 시 매치되어있는 상품정보가 뜨는 기능

### 유저 팔로우 기능 (최정민)
- 유저간 팔로우 기능 구현

### 상품 상세 페이지 (이지선)
- 피드 페이지의 피드 사진에 태그에 매치되어있는 상품을 클릭하면 상세페이지로 이동
- 제품의 옵션 선택 기능 구현
- 가격을 계산하여 구매 페이지로 보냄

### 결제 페이지 (이지선)
- 다음 우편번호 Api를 사용하여 주소 검색
- 최종 결제 금액 계산

### 북마크 (이지선)
- 마음에 드는 피드를 북마크하여 내 정보에 보관

### 페이팔 결제 (남재현)
- 페이팔 Api를 사용하여 결제 시스템 구현
- 구매 영수증을 검증하여 구매목록(히스토리)에 보관

