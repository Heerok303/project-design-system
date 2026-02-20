# 설정 (Before A → After B)

## 파일 구성
- `before_A.css`: 변경 전 A 원문
- `after_B.css`: 변경 후 B 원문
- `README.md`: 변경점 요약

## 변경 요약 (A → B)

### 1) Top Navigation 구조 변경
- **A**: `position: absolute`, height 42px, padding `10px 16px`, 단독 배치
- **B**: Fixed Top 컨테이너(height 110px) 안에 포함, height **56px**, padding **16px**
- **Title 폰트 변경**:
  - A: `Noto Sans` (20px, Bold)
  - B: `Noto Sans KR` (17px, Bold) - "Mobile/Heading/17_B" 토큰 적용
- B에서 Back Icon은 `display: none`으로 숨김 (설정 화면은 최상위이므로 뒤로가기 불필요)

### 2) Fixed Top 도입 (B 전용)
- Status Bar + Top Navigation을 **Fixed Top** 컨테이너로 묶어 상단 고정
- Status Bar의 Battery 아이콘 색상: A에서는 일부 `#000000` → B에서 모두 `#FFFFFF`로 통일

### 3) Settings Container 레이아웃 변경
- **A**: padding `0px 16px`, height 200px, top 116px
- **B**: padding **16px**, height **232px**, top **110px**
- A에서는 List 안에 별도 **Navigation** 래퍼가 있었으나, B에서는 제거되고 텍스트가 List 직속 자식으로 배치

### 4) Typography & Token 적용
- 리스트 항목 텍스트: `Noto Sans` → `Noto Sans KR`, "Mobile/Body/15" 토큰 적용
- `line-height`: 110% → **22px** 고정, `letter-spacing: 0.005em` 추가

### 5) Touch Box 크기 변경
- A: padding `10px`, width/height **44px**
- B: padding **8px**, width/height **40px**

### 6) Tab Bar 변경
- **Tab Bar Container 높이**: A 65px → B **69px**
- **Tab Bar 높이**: A 44px → B **48px**
- **Nav Menu 높이**: A 44px → B **48px**
- **Label 폰트**: A `Pretendard` → B `Noto Sans KR`, "Mobile/Label/11" 토큰 적용
- **활성(설정) Label weight**: A `700`(Bold) → B `500`(Medium)
