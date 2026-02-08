# Design Update — 내체육관 > 운동게시판 (A → B)
date: 2026-02-08

## Summary
- 홈 상단을 “정보 중심 헤더”로 재구성 (그라데이션 오버레이 + 하단 정렬 + 로고/이름/관장정보)
- 탭/액션바/카드 타이포를 Mobile 기준(Noto Sans KR)으로 정리
- 터치 영역/위계(활성 탭/배지) 명확화

---

## 1) Home Header 구조 변경 (핵심)
### A
- Container(144px): 로고 90px 사각 + 태그(배경 rgba(255,255,255,0.35))

### B
- Home Container
  - justify-content: flex-end
  - padding: 16px
  - gap: 12px
  - background:
    - linear-gradient(180deg, rgba(0,0,0,0) 0%, rgba(0,0,0,0.5) 100%), url(...)
- Info Row (신규)
  - Logo: 48x48, radius 100px(원형)
  - Gym name: Noto Sans KR 15/700/22, #FFFFFF
  - Coach: Noto Sans KR 13/500/16, rgba(255,255,255,0.6)
- Tags(칩) 변경
  - bg: rgba(255,255,255,0.8)
  - padding: 4px 8px
  - typo: Noto Sans KR 11/400/16, color #333333, letter-spacing 0.01em

의도: 배경 이미지 위 텍스트 가독성 확보 + 헤더를 브랜드/정보 요약 영역으로 고정

---

## 2) Action Bar(글쓰기/멤버수) 텍스트 정리
- Member count
  - A: Noto Sans 13/400/14 (line-height 110%)
  - B: Noto Sans KR 13/400/18 + letter-spacing 0.005em (Mobile/Body/13)

---

## 3) Tab 영역 변경
- Container height
  - A: 47px
  - B: 52px
- Inactive label
  - A: Noto Sans 13/400/14
  - B: Noto Sans KR 13/500/16 + letter-spacing 0.005em
- Active label
  - A: Noto Sans 15/700/17
  - B: Noto Sans KR 15/700/22 + letter-spacing 0.005em
- Active underline: border-bottom 2px solid #D93434 (동일)

---

## 4) Card(영상 카드) 배지/타이포 정리
- Time badge
  - B: height 24px, typo Noto Sans KR 11/400/16
  - 컨텐츠 길이에 따라 width만 가변 (예: 38x24, 44x24 등)
- Title/Specs
  - B: Noto Sans KR (15/700/22, 11/400/16) 기준

---

## Dev Checklist
- [ ] Home Header 배경: 이미지 + 그라데이션 오버레이 적용
- [ ] 헤더 콘텐츠 하단 정렬 + padding 16
- [ ] 로고 48 원형 + border 유지
- [ ] 태그칩 padding/bg/typo 반영
- [ ] Tab 높이 52 + 활성 라벨 line-height 22 반영
- [ ] Time badge typo 11/16으로 통일
