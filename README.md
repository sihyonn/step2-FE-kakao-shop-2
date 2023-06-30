# Step-2.-Week-1

## 과제 1

`쇼핑몰 웹사이트를 탐색해 어떠한 페이지 구성을 가지고 있는지 체크`

### 웹사이트 전체 페이지 구성

- 메인 페이지
- 회원가입 페이지
- 로그인 페이지
- 상품 검색 결과 페이지
- 개별 상품 상세 페이지
- 리뷰 페이지
- 문의 페이지
- 장바구니 페이지
- 결제 페이지
- 결제 완료 페이지
- 마이페이지
- ...

### 페이지별 구성

1. 메인 페이지

- 핵심 기능: (접속시 바로 보이는 화면) 전체 상품 조회 및 배너, 네비게이션바
- 기능 상세 설명
  1. 상단 - 네비게이션바 고정(홈, 카테고리, 검색, 장바구니, 로그인으로 구성).
  2. 네비게이션 바 아래 Carousel을 통해 특가, 소식, 광고 보여준다.
  3. 캐러셀 아래 전체 상품 목록을 조회할 수 있도록 품목별 카테고리와 톡딜가 상품들의 사진, 상품명, 가격등을 보여준다.
- 인터페이스 요구사항
  1. 장바구니, 배송버튼, 상품하단 하트 클릭시 로그인 필요
  2. 상품하단 공유버튼을 통해 sns로 상품 페이지 공유

2. 회원가입 페이지

- 핵심 기능: 사이트 이용을 위한 계정 생성
- 기능 상세 설명:
  1. 가입을 위한 성명 아이디, 비밀번호, 이메일 등을 받는다.
  2. 아이디 비밀번호 유효성 검사(공백x, 영문, 특수기호 조건 명시)
- 인터페이스 요구사항: 아이디 확인시 중복검사필요. 비밀번호 보안처리, 가입 완료 시 성공적으로 가입 되었음을 알린다.

3. 로그인 페이지

- 핵심 기능: 로그인 요청 및 사용자 로그인 정보 저장
- 기능 상세 설명: 이메일과 비밀번호를 이용해 로그인진행, 이에 대한 상태 처리
- 인터페이스 요구사항: 이메일 또는 비밀번호에 들어온 값이 적합하지 않은 경우 적절한 알림을 보낸다.

4. 상품 검색 결과 페이지

- 핵심 기능: 상품 검색 및 검색 결과 연관된 상품 결과 보여줌
- 기능 상세 설명
  1.  검색 버튼 클릭시 입력창이 뜨고 원하는 키워드 입력 가능
  2.  검색어 입력 시 해당 글자로 시작되는 연관 상품 자동완성으로 보여준다.
  3.  검색어 입력창 하단 최근 검색결과 인기 키워드 등 제시
  4.  상품 검색 시 해당 단어가 포함된 모든 상품 조회 결과를 제시한다.
  5.  검색 결과에 대한 필터 제공(톡딜상품, 무료배송, 가격, 상품유형 등)
  6.  검색 결과 정렬기능(추천순, 인기순, 낮은가격순, 높은가격순)
- 인터페이스 요구사항
  1.  검색 결과 상품들 중 클릭시 해당 상품에 대한 상세 페이지로 넘어감
  2.  찜 버튼을 누르면 비회원의 경우 로그인페이지로, 회원의경우 해당 상품 저장 및 카톡으로 전송

5. 개별 상품 상세 페이지

- 핵심 기능 : 해당 상품명, 이미지, 가격 등 상세정보 제공 및 구매하기
- 기능 상세 설명
  1.  상품에 대한 이미지와 상품명, 가격, 할인정보 등을보여주고 하단에서 더 상세한 정보 보여준다.
  2.  리뷰 및 QnA를 확인할 수 있다.
  3.  하단에서 해당 상품과 비슷한 혹은 옵션만 다른 제품을 볼 수 있다.
- 인터페이스 요구사항
  1. 상품 수량 및 옵션 선택 후 구매하기버튼을 누르면 결제 페이지로 이동
  2. 리뷰 누르면 다른 사용자가 남긴 리뷰를 볼 수 있는 페이지로 이동
  3. QnA 누르면 다른 사용자가 남긴 문의와 답변 볼 수 있는 페이지로 이동

6. 문의 페이지

- 핵심 기능 : 궁금한 사항에 대한 문의 및 답변 열람
- 기능 상세 설명
  1. 문의하기를 통해 문의 작성을 할 수 있다.
  2. 다른 사용자들의 공개된 문의를 확인할 수 있다.(비밀문의 경우 불가능)
  3. 답변대기, 답변완료 등 답변여부를 확인할 수 있다.
  4. 내 문의만 확인가능 하며 상품, 배송, 반품및교환, 취소환불, 기타 등으로 필터 가능하다.
- 인터페이스 요구사항 : 문의하기를 누르면 문의유형, 사진등록, 문의내용, 비밀글 설정 등을 기재하여 문의 등록

7. 리뷰 페이지

- 핵심 기능: 다른 사용자가 남긴 텍스트리뷰, 이미지첨부리뷰를 확인 할 수 있다.
- 기능 상세 설명

  1. 해당 상품에 대한 전체 리뷰를 확인 할 수 있다.(옵션, 배송만족여부 확인가능)
  2. 사진/동영상 리뷰만 따로 확인 할 수 있다.
  3. 리뷰 정렬가능(추천순, 최신순, 오래된순 등)

- 인터페이스 요구사항
  1. 공유버튼 클릭시 sns 계정을 통한 공유 가능
  2. 추천, 도움돼요 등의 버튼을 누르면 1씩 숫자 증가

8. 장바구니 페이지

- 핵심 기능: 구매하고자 하는 상품을 모아서 보고 결제할 수 있다.
- 기능 상세 설명
  1. 장바구니에 담은 각 상품에 대한 이미지, 옵션, 금액등을 확인할 수 있다.
  2. 전체를 선택하거나 부분적으로 선택해서 주문예상금액을 확인하고 주문할 수 있다.
- 인터페이스 요구사항: 주문하기 버튼을 누르면 결제 페이지로 넘어간다.

9. 결제 페이지

- 핵심 기능: 배송지 정보, 주문상품 정보, 결제금액 확인 후 결제수단을 선택해 결제진행
- 기능 상세 설명
  1. 배송지정보 및 요청사항을 입력받는다.
  2. 포인트 사용여부, 사용할 포인트를 입력받는다.
  3. 결제 수단 선택, 현금영수증 발급신청 여부를 확인한다.
  4. 결제 진행
- 인터페이스 요구사항: 결제를 누르면 선택한 결제수단으로 넘어간다.

10. 결제완료 페이지

- 핵심 기능: 결제 완료 알림 및 최종 결제한 상품 정보 제공
- 기능 상세설명
  1. 결제 및 구매가 완료되었음을 알린다.
  2. 동시에 사용자가 구매한 목록 제시한다.
- 인터페이스 요구사항: 구매 목록을 클릭하면 배송정보, 교환/환불 정보 등 주문상세내용을 보여 준다.

11. 마이페이지

- 핵심 기능: 내 정보 확인 및 수정, 주문/배송내역, 장바구니, 찜한 상품 정보, 쿠폰 등 확인
- 기능상세설명
  1.  나의 계정정보(이름 or 아이디, 등급, 핸드폰번호, 주소 등)를 확인하고 수정할 수 있다.
  2.  주문하거나 했던 내역을 확인할 수 있고 배송여부를 확인할 수 있다.
  3.  찜한 상품 정보를 간략히 보여준다.
  4.  쿠폰이나 포인트 내역을 확인 할 수 있다.
- 인터페이스요구사항: 내 정보 수정 시 본인인증 절차로 넘어간다.

### 디렉터리 구조

```
    -/public
        - index.html
        - ...
    -/src
        -/components
            -Header.jsx
            -ProductCard.jsx
            - ...
        -/pages
            -Main.js
            -Cart.js
            -Payment.js
            -Search.js
            - ...
        -/assets
        -/hooks
        -/styles
        -/services
        -/utils
        -/apis
        -App.js
        -index.js
```
