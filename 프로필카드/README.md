# 프로필 카드 (Before A → After B)

## 파일 구성
- `before_A.css`: 변경 전 A 원문 (설정 프로필 카드)
- `after_B.css`: 변경 후 B 원문 (내 체육관 관장님)
- `README.md`: 변경점 요약

## 변경 요약 (A → B)

### 1) 화면 구조 대폭 변경
- **A**: "설정 프로필 카드" — 배경 이미지 위에 로고(120x120)를 중앙 배치 + 주변에 태그 절대 배치
- **B**: "내 체육관 관장님" — **Home Container**(144px) 안에 그라데이션 오버레이 + Info(로고 48px 원형 + 이름/체급) + Tag container를 오토레이아웃으로 정렬

### 2) Top Navigation 구조 변경
- **A**: `position: absolute`, height 44px, padding `10px 16px`, 타이틀 `Noto Sans` 20px
- **B**: Fixed Top(110px) 안에 포함, height **56px**, padding **16px**, 타이틀 `Noto Sans KR` **17px** ("Mobile/Heading/17_B" 토큰)

### 3) 프로필 정보 영역 (A: Change Container → B: Body)
- **A**: `Change container` — 배경 `#F9FAFB`, 5개의 "변경해주세요" 항목을 리스트로 나열 (편집 모드)
- **B**: `Body` — Content 목록(GYM name 카드 ×5), 각 카드는 `background: #F2F4F7`, `border: 1px solid #EAECF0`, `border-radius: 12px`로 카드형 UI

### 4) 태그 시스템 변경
- **A**: 절대 위치 기반으로 태그를 배경 이미지 위에 흩뿌림 (`position: absolute`, `#3년`, `#79kg`, 체육관명 등)
- **B**: 오토레이아웃 기반 **Tag container** (가로 정렬, gap 8px, `background: rgba(255,255,255,0.8)`, `border-radius: 8px`)
  - 태그 폰트: `Noto Sans KR` 11px, "Mobile/Label/11_M" 토큰 적용

### 5) Tab Bar 제거 (B)
- A에는 하단 Tab Bar(65px)가 있으나, B에서는 제거되고 **Home indicator**(21px)만 남음

### 6) Status Bar 아이콘 색상
- A: Battery Border `#000000` → B: 모두 `#FFFFFF`로 통일
