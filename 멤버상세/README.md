# 내체육관 멤버 상세 (Before A → After B)

## 파일 구성
- `before_A.css`: 변경 전 A 원문
- `after_B.css`: 변경 후 B 원문
- `README.md`: 변경점 요약

## 변경 요약 (A → B)

### 1) Top Navigation 구조 변경
- **A**: `position: absolute`, height 24px, padding `0px 16px`, top 64px
- **B**: Fixed Top(110px) 컨테이너 안에 포함, height **56px**, padding **16px**
- **Title 폰트 변경**:
  - A: `Noto Sans` (20px, Bold, `letter-spacing: 0.395508px`)
  - B: `Noto Sans KR` (17px, Bold) - "Mobile/Heading/17_B" 토큰 적용
- B에서 Edit 아이콘은 `display: none`으로 숨김

### 2) Hero 프로필 영역 대폭 변경
- **A**: Container(174px) + 중앙 로고(120x120) + 태그 절대 배치
  - 배경: `linear-gradient(0deg, rgba(0,0,0,0.5)...)` 어두운 오버레이
  - 태그: `rgba(255,255,255,0.2)` 배경 + `border: 1px solid rgba(255,255,255,0.3)`, 흰색 텍스트
- **B**: Home Container(144px) + 오토레이아웃 기반 Info(로고 48px 원형 + 이름/체급) + Tag container
  - 배경: `linear-gradient(180deg, ...)` 하단 그라데이션
  - 태그: `rgba(255,255,255,0.8)` 배경, `#333333` 텍스트, "Mobile/Label/11_M" 토큰

### 3) 태그 시스템 변경
- **A**: 모든 태그가 `position: absolute`로 흩뿌려진 배치, 흰 텍스트(`#FFFFFF`)
- **B**: 오토레이아웃 기반 **Tag container** (가로 정렬, gap 8px), 검정 텍스트(`#333333`)
  - 태그 폰트: `Noto Sans KR` 11px, "Mobile/Label/11_M" 토큰 적용

### 4) Status Bar
- A: `background: rgba(255,255,255,0.15)` 반투명
- B: Fixed Top 컨테이너의 일부로 `background: #FFFFFF` 불투명
