# 내체육관 일정(캘린더) 전체보기 (Before A → After B)

## 파일 구성
- `before_A.css`: 변경 전 A 원문
- `after_B.css`: 변경 후 B 원문
- `README.md`: 변경점 요약

## 변경 요약 (A → B)

### 1) Top Navigation 구조 변경
- **A**: `position: absolute`, height 24px, padding `0px 16px`, top 54px
- **B**: Fixed Top 컨테이너 안에 포함, height **56px**, padding **16px**, 오토레이아웃 기반
- **Title 폰트 변경**:
  - A: `Noto Sans` (20px, Bold, `letter-spacing: 0.395508px`)
  - B: `Noto Sans KR` (17px, Bold) - "Mobile/Heading/17_B" 토큰 적용

### 2) Fixed Top 도입 (B 전용)
- B에서는 Status Bar + Top Navigation을 **Fixed Top** 컨테이너(height 110px)로 묶어 상단 고정 구조로 변경
- 콘텐츠 영역 top이 100px → **110px**으로 조정

### 3) Event List 영역 확장
- **Event List 높이**: A 285px → B **318px**
- **Event row 높이**: A 95px → B **106px** (padding 변경: 16px → 16px 12px)
- **Event Details 높이**: A 63px → B **74px**

### 4) Typography & Token 적용
- 전반적으로 `Noto Sans` → `Noto Sans KR`로 변경
- B에서는 디자인 토큰 주석이 명시됨:
  - Date: "Mobile/Heading/21_B" (21px, Bold, `letter-spacing: -0.005em`)
  - Day: "Mobile/Label/11_M" (11px, Regular, `letter-spacing: 0.01em`)
  - Event Name: "Mobile/Body/15_B" (15px, Bold)
  - Event Time/Organizer: "Mobile/Body/13" (13px, Regular)
  - 월 표시: "Mobile/Body/15" (15px, Regular)
- A에서는 Date가 `font-weight: 400`(Regular) → B에서 `font-weight: 700`(Bold)로 강조

### 5) 월 선택 버튼(Frame 5602) 미세 조정
- A: padding `10px`, width 51px, height 37px
- B: padding `8px 12px`, width **55px**, height **38px**
