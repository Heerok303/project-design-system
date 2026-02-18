# project-design-system

이 레포는 이 프로젝트의 **디자인 기준 저장소**입니다.

## 사용 원칙
- Figma는 참고용
- 실제 기준은 GitHub 문서 기준
- 디자인 변경은 기록으로 남긴다

## Figma
- CURRENT SPEC 페이지 참고
- https://figma.com/file/design/vYI2XpqPZpnfPHezZ7TFjA/THE-CORNER?node-id=118-556&t=BisFsu2I1N6l0avn-1

---

## Preview / Sample UI (Home)

Figma export로 나온 스타일을 실제 웹에서 유지보수 가능한 구조로 정리한 샘플입니다.

### Run
- `src/index.html`을 브라우저에서 열면 됩니다.

### Structure
- `src/styles/tokens.css` : 디자인 토큰(색/타이포/라운드/쉐도우)
- `src/styles/base.css` : reset, 공통 레이아웃
- `src/styles/components.css` : 버튼/카드/탭바 등 재사용 컴포넌트
- `src/styles/pages/home.css` : Home 페이지 전용 스타일
- `docs/figma-export/*` : Figma 원본 덤프 보관(비교용)

### Change Log
- 디자인 변경 이력은 `docs/CHANGELOG.md`에 기록합니다.
