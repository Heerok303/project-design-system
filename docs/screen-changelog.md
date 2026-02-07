## 2026-02-07 · Gym List Screen (A → B)

### Summary
- 목적: 가독성 개선 + 모바일 사용성 강화
- 범위: 해당 화면 기준 (일부 시스템 기준 후보 포함)

### Changes
📌 Design Update – Gym List Screen (A → B)
Summary
목적: 가독성 개선 + 모바일 사용성 강화
범위: 해당 화면 기준 (시스템 승격 후보 일부 포함)
1️⃣ Typography 변경
Top Navigation Title
A
font-size: 30px
font-weight: 800
font-family: Noto Sans
B
font-size: 21px
font-weight: 700
font-family: Noto Sans KR
letter-spacing: -0.005em
👉 모바일 헤더 타이틀을 과도한 강조 → 표준 헤딩 레벨로 조정
Section Title (등록된 체육관)
A: 15px / 700
B: 17px / 700
👉 섹션 인지 강화를 위해 크기 상향
Body / Description Text
설명 텍스트:
A: 12px / line-height 150%
B: 유지 (동일)
보조/라벨 텍스트:
B에서 Pretendard + 11~12px로 정리
👉 정보성 텍스트 대비 강화
2️⃣ Icon & Touch Area 변경
좋아요(Heart) 아이콘
A
icon size: 16px
B
icon size: 24px
touch area: 44 × 44
👉 모바일 터치 영역 기준 충족 (접근성 개선)
리스트 카드 내 아이콘
아이콘 시각 크기 및 터치 영역 확대
아이콘은 시각 요소 + 액션 요소로 명확히 분리
3️⃣ Input Field 변경
Search / Text Field
A
padding: 10px
height: 52px
font-size: 15px
B
padding: 8px 16px
height: 48px
font-size: 13px
border opacity 감소 (0.15 → 0.12)
👉 입력 필드 밀도 감소 + 모바일 UI 톤 정리
4️⃣ Card Layout 변경
Card Height
A: 128px 고정
B:
카드 타입에 따라 103px / 128px 혼용
콘텐츠 밀도에 따라 높이 조절
Title 영역
B에서 Title 영역 높이 확장
가격 + 아이콘 영역 분리로 시각적 충돌 감소
5️⃣ 시스템 승격 후보 (다른 화면 적용 가능)
아래 항목은 디자인 시스템 기준으로 승격 가능:
모바일 터치 영역 최소값: 44×44
아이콘 기본 사이즈: 24px
모바일 헤더 타이틀 기본 크기: ~21px
입력 필드 기본 높이: 48px

### Developer Notes
- 적용 우선순위: (예: 모바일 타이포/터치 영역 우선)
- 영향 범위: (예: Gym list 카드, Top Nav 타이틀, Search Input)

