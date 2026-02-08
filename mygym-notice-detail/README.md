# 내 체육관 공지사항 게시판 상세화면 — A → B 변경

## 포함 파일
- freeboard_before_A.css : 변경 전 A 원문
- freeboard_after_B.css  : 변경 후 B 원문

## 변경 요약 (A → B)
### 1) 화면 위치/프레임 배치
- 상세화면 컨테이너 위치가 변경됨
  - A: left 115px / top 24px
  - B: left 126px / top 48px

### 2) Top Navigation 스펙 변경
- A: height 24px, padding 0px 16px, top 64px
- B: height 56px, padding 16px, top 54px
- 타이틀 텍스트 스타일도 변경됨
  - A: Noto Sans / 20px / line-height 110%
  - B: Noto Sans KR / 17px / line-height 24px (Mobile/Heading/17_B)

### 3) 액션(좋아요/더보기) 영역 크기 변경
- Like/More 관련 아이콘 및 컨테이너 크기가 전반적으로 축소됨 (24px → 20px 계열)
- 해당 영역의 전체 높이도 변경됨
  - A: Container height 56px, Like Container height 24px
  - B: Container height 52px, Like Container height 20px

### 4) 하단 입력(탭바) 영역 스펙 변경
- B는 Tab Bar Container height가 69px, Text Field가 48px(+padding 12px 16px)로 커짐
- A는 Tab Bar Container height가 65px, Text Field가 44px(+padding 10px)

### 5) 댓글/헤더 블록 스펙 변화
- top 564px에 위치한 Header 블록의 구성/사이즈가 A와 B에서 다름
  - B: 로고 32px, User Info 폭 325px 기반
  - A: 로고 40px, User Info 폭 311px 기반 등

## 적용 범위
- “내 체육관 공지사항 게시판 상세화면” 화면 1개 (A/B 비교용 CSS)

## 체크포인트 (개발 확인 요청)
- Top Navigation 높이/패딩 변경이 실제 구현에서도 동일하게 반영되는지
- 좋아요/더보기 아이콘 사이즈(20 vs 24) 및 터치 영역이 의도대로인지
- 하단 입력창(Text Field) 높이/패딩 변화로 인해 타이핑 영역이 깨지지 않는지
- 댓글 Header(564px 영역) 레이아웃이 A/B 의도대로 변경되었는지
