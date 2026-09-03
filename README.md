# project-design-system

이 레포는 **디자인 기준(Design Source of Truth)** 저장소입니다.

## 원칙
- Figma는 참고용(Source)
- **실제 기준은 GitHub 문서 기준**
- 디자인 변경은 반드시 기록으로 남긴다(CHANGELOG)

## 문서 구조
- `docs/spec/` : 화면/컴포넌트 스펙 (최종 기준)
- `docs/CHANGELOG.md` : 변경 기록

## Figma
- CURRENT SPEC 페이지 참고
- https://figma.com/file/design/vYI2XpqPZpnfPHezZ7TFjA/THE-CORNER?node-id=118-556&t=BisFsu2I1N6l0avn-1

---

## Typography (Text Styles)

Figma에서 추출된 모바일(Mobile) 및 웹(Web) 환경별 타이포그래피 디자인 토큰 시스템입니다. 
기본 폰트는 모두 `Noto Sans KR`을 사용합니다.

### 📱 Mobile

| Category | Token Name | Weight | Size | Line Height | Letter Spacing |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Label** | `11` | Regular (400) | 11px | 16px | 1% |
| | `11_M` | Medium (500) | 11px | 16px | 1% |
| | `13_M` | Medium (500) | 13px | 16px | 0.5% |
| **Body** | `13` | Regular (400) | 13px | 18px | 0.5% |
| | `13_M` | Medium (500) | 13px | 18px | 0.5% |
| | `13_B` | Bold (700) | 13px | 18px | 0.5% |
| | `15` | Regular (400) | 15px | 22px | 0.5% |
| | `15_M` | Medium (500) | 15px | 22px | 0.5% |
| | `15_B` | Bold (700) | 15px | 22px | 0.5% |
| | `17` | Regular (400) | 17px | 24px | 0% |
| | `17_M` | Medium (500) | 17px | 24px | 0.5% |
| | `17_B` | Bold (700) | 17px | 24px | 0% |
| **Heading** | `17_B` | Bold (700) | 17px | 24px | 0% |
| | `19_B` | Bold (700) | 19px | 24px | -0.5% |
| | `21_B` | Bold (700) | 21px | 26px | -0.5% |
| | `25_B` | Bold (700) | 25px | 28px | -1% |
| | `31_B` | Bold (700) | 31px | 32px | -1.5% |
| **Button** | `11_SB` | SemiBold (600) | 11px | 100% | 0% |
| | `13_SB` | SemiBold (600) | 13px | 100% | 0% |
| | `15_M` | Medium (500) | 15px | 100% | -1% |
| | `15_SB` | SemiBold (600) | 15px | 100% | -1% |
| | `17_SB` | SemiBold (600) | 17px | 100% | -1% |

### 💻 Web

| Category | Token Name | Weight | Size | Line Height | Letter Spacing |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Display** | `35_B` | Bold (700) | 35px | 42px | -1.5% |
| **Title** | `19_B` | Bold (700) | 19px | 26px | -1% |
| | `25_B` | Bold (700) | 25px | 32px | -1% |
| **Body** | `13` | Regular (400) | 13px | 20px | 1% |
| | `13_M` | Medium (500) | 13px | 20px | 1% |
| | `15` | Regular (400) | 15px | 24px | 0.5% |
| | `15_M` | Medium (500) | 15px | 24px | 0.5% |
| | `17_M` | Medium (500) | 17px | 26px | -0.5% |
| **Button** | `13_M` | Medium (500) | 13px | 100% | 1% |
| | `15_SB` | SemiBold (600) | 15px | 100% | 0.5% |

---

## Color System

Figma에서 추출된 컬러 디자인 토큰입니다. 
시맨틱(Semantic) 토큰과 프리미티브(Primitive) 팔레트로 구분하여 관리합니다.

### 🎨 Brand & Semantic

| Category | Token Name | Value / Reference |
| :--- | :--- | :--- |
| **Brand** | `--Brand-Brand-Primary-Default`<br>`-Hover`<br>`-Pressed`<br>`-Light` | `var(--Red-500)`<br>`var(--Red-600)`<br>`var(--Red-700)`<br>`var(--Red-200)` |
| **Text** | `--Text-Title`<br>`--Text-Body`<br>`--Text-Sub`<br>`--Text-Placeholder`<br>`--Text-White` / `--Text-Inverse` | `var(--Gray-900)`<br>`var(--Gray-800)`<br>`var(--Gray-700)`<br>`var(--Gray-400)`<br>`var(--White-Default)` |
| **Surface & Bg** | `--Surface-Default`<br>`--Background-Default`<br>`--Surface-Alt`<br>`--Background-Inverse_Hover`<br>`--Background-Inverse_Pressed`<br>`--Neutral-Back`<br>`--Neutral-Main` | `#FFFFFFFF`<br>`var(--White-Default)`<br>`var(--Gray-100)`<br>`var(--White-Alpha_10)`<br>`var(--White-Alpha_20)`<br>`#F2F4F7FF`<br>`#475467FF` |
| **Border** | `--Border-Default`<br>`--Border-Divider` | `var(--Gray-200)`<br>`var(--Gray-100)` |
| **Icon** | `--Icon-Default`<br>`--Icon-Sub`<br>`--Icon-Inverse`<br>`--Icon-Brand` | `var(--Gray-800)`<br>`var(--Gray-500)`<br>`#FFFFFFFF`<br>`var(--Brand-Brand-Primary-Default)` |
| **Button** | `--Gray-Button-Default`<br>`-Hover`<br>`-Pressed` | `var(--Gray-100)`<br>`var(--Gray-200)`<br>`var(--Gray-300)` |

### 🚨 Status Colors

| Status | Text Color | Background Color |
| :--- | :--- | :--- |
| **Success** | `var(--Green-500)` | `#ECFDF3FF` |
| **Warning** | `var(--Orange-500)` | `#FFFAEBFF` |
| **Error** | `var(--Red-500)` | `#FEF3F2FF` |
| **Info** | `#1F75FEFF` | `#F5F9FFFF` |
| **Neutral** | `#475467FF` | `#F2F4F7FF` |

> *Note: Error 상태는 Hover(`var(--Red-600)`), Pressed(`var(--Red-700)`) 토큰을 추가로 가집니다.*

### 🖌 Primitive Palette (Base Colors)

| Color | 50 | 100 | 200 | 300 | 400 | 500 (Base) | 600 | 700 | 800 | 900 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Gray** | `#F9FAFB` | `#F2F4F7` | `#EAECF0` | `#D0D5DD` | `#98A2B3` | `#667085` | `#475467` | `#1D2939` | `#1D2939` | `#101828` |
| **Red** | - | - | `#FBEBEB` | `#F9E1E1` | `#F3C0C0` | `#D93434` | `#C32F2F` | `#AE2A2A` | `#A32727` | `#821F1F` |
| **Blue** | - | `#F5F9FF` | `#E9F1FF` | `#DDEAFF` | `#BAD4FF` | `#1F75FE` | `#1C69E5` | `#195ECB` | `#1758BF` | `#134698` |
| **Teal** | - | - | - | - | - | `#1CA9C9` | `#1998B5` | `#1687A1` | - | - |

*(기타 Base: `Green-500`: `#28C488`, `Orange-500`: `#F2994A`)*
*(투명도 Base: `--White-Alpha_10`, `--White-Alpha_20`, `--Blcak-Alpha_40`)*

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
