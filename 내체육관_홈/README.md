# 내체육관 홈 (Before A → After B)

## 파일 구성
- `before_A.css`: 변경 전 A 원문
- `after_B.css`: 변경 후 B 원문
- `README.md`: 변경점 요약 및 사용법

## 사용법
- 두 CSS를 diff로 비교:
  - 예) `git diff --no-index before_A.css after_B.css`
- 또는 GitHub PR에서 파일 2개를 같이 올려 변경점 확인

## A → B 변경점 요약(핵심)
- 전체 아트보드(회색 배경 컨테이너) 높이: **A 1344px → B 1233px**
- 내체육관 홈 프레임 높이: **A 1251px → B 1046px**
- Hero(상단 커버) 구성 변화:
  - A: 큰 로고(90x90) 중심
  - B: Info(로고 48 + 센터명/관장 텍스트) + 태그 박스 형태로 구조 확장
- 타이포/토큰 변화(대표):
  - A는 `Noto Sans`와 `line-height: 110%` 중심
  - B는 `Noto Sans KR` 사용이 많고, 13px 계열에서 `line-height: 18px` 등 토큰화된 스펙이 다수 포함
- 커뮤니티 프리뷰 카드:
  - A: 더 많은 행/높이(168px) 기반의 프리뷰 구조
  - B: 더 컴팩트(108px) + 행 단위 구성(공지/운동/중고) 명확
- Home Date(이벤트 리스트):
  - A: 이벤트 row 높이 95px
  - B: 이벤트 row 높이 108px + Date/Day/Details 토큰(Heading/Label/Body) 정리
