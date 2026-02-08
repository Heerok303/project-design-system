# 자유게시판 UI 스펙 변경 (A → B)

- 대상: 자유게시판 (Mobile 393)
- 목적: Figma CSS Export 기준으로 **변경 전(A)** / **변경 후(B)** 스펙을 개발 전달용으로 정리
- 파일 구성:
  - `freeboard_after_B.css` : 변경 후(B) 원문
  - `freeboard_before_A.css`: 변경 전(A) 원문

## 참고
- CSS 내 `url( ...png )` 는 Figma Export 원문입니다. 실제 개발 적용 시 asset 경로로 치환 필요합니다.
- 일부 항목은 Figma Export 특성상 `position: absolute` + 수치가 많습니다(원문 유지).

## 체크 포인트(대표)
- Root 스크롤 컨테이너 높이: A `652px` ↔ B `657px`
- Tab / Label / Typography 값들 일부 상이(파일 비교로 확인)
