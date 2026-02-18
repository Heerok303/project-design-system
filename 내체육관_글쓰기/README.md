# 내 체육관 글쓰기 (Before A → After B)

## 파일 구성
- `before_A.css`: 변경 전 A 원문
- `after_B.css`: 변경 후 B 원문
- `README.md`: 변경점 요약

## 변경 요약 (A → B)

### 1) 화면 높이 확장
- 전체 컨테이너 높이: **A 1139px → B 1251px**
- 내부 콘텐츠 영역이 확장되면서 전체 스크롤 영역이 늘어났습니다.

### 2) Top Navigation (상단 네비게이션)
- **Title 폰트 변경**:
  - A: `Noto Sans` (20px, Bold)
  - B: `Noto Sans KR` (17px, Bold) - "Mobile/Heading/17_B" 토큰 적용
- **Complete 버튼 (완료)**:
  - A: `Noto Sans`
  - B: `Noto Sans KR` - "Mobile/Body/15" 토큰 적용, `letter-spacing: 0.005em` 추가

### 3) Typography & Token 적용
- 전반적으로 `Noto Sans` → `Noto Sans KR`로 변경되었습니다.
- B안에서는 "Mobile/Heading/..." 또는 "Mobile/Body/..."와 같은 디자인 토큰 주석이 명시되어 있어, 시스템화된 스타일을 따르고 있습니다.
- 텍스트의 `line-height`가 정교하게 조정됨 (예: Title Container의 제목 Line height 150% → 22px 고정 등).

### 4) 레이아웃 디테일
- **Title Container 높이**: A 66px → B 64px (2px 축소)
- **Content Container 높이**: A 112px → B 108px (4px 축소)
- 미세한 패딩 및 높이 조정으로 컴포넌트 밀도가 정리되었습니다.
