# 테스트

개인 실습용 프로젝트로, Spring boot, netflix Eureka, zuul 등 api를 활용해보며
MSA 아키텍쳐로 도메인모델링 및 서비스 구현까지 해볼 예정

## 요구사항

### 기능 요구사항

- 회원 관리
  - 셀러/일반사용자 등록수정삭제
  - 로그인/로그아웃
- 상품 관리
  - 상품 등록수정삭제
  - 찜(즐겨찾기)
  - 장바구니
- 게시물 관리
  - 리뷰
  - 공지
  - QNA
- 매출 관리
  - 오늘/한달/일년 정산
- 쿠폰 관리
  - 쿠폰발급 
  - 유효일지정

### 비기능 요구사항

- API GATEWAY
- EUREKA
- 캐싱
- JPA
- Kafka, kafdrop
- ELK

### 구조
REGISTRY : 어플리케이션 구동에 필요한 configuration 정보와 service discovery를 담당하는 서비스

UAA : 사용자/인증/인가 서비스

PRODUCT : 상품 서비스

INSIGHT : 매출 관리 서비스

COUPON : 쿠폰 서비스

