# 이가영 — Portfolio

Infrastructure / Cloud Security Engineer 포트폴리오. 빌드 과정 없는 순수 HTML/CSS/JS 정적 사이트 (GitHub Pages).

## 구조

- `index.html` — 홈. **gayoungOS**: 부팅 화면 뒤에 데스크톱이 뜨고, 아이콘을 누르면 창이 열립니다.
  - 창은 제목 표시줄을 끌어서 이동, 빨간 점으로 닫기, `ESC`로도 닫힘
  - 오른쪽 위 **색 조절** — 색조/채도 슬라이더, 어두운/밝은 배경, 무채색. 고른 값은 브라우저에 저장됨
- `plain.html` — 같은 내용의 평범한 스크롤 버전 (자바스크립트 없이도 전부 읽힘)
- `project-1-aws-devsecops.html` — AI 기반 AWS DevSecOps Control Plane
- `project-2-security-automation.html` — Rocky Linux & DB 시스템 보안 자동화
- `project-3-incident-response.html` — 보안 사고 원인 분석 및 대응 방안 도출

`design-*.html`, `pick.html` 은 디자인 고를 때 쓴 미리보기 파일입니다. 배포에 필요 없으니 지워도 됩니다.

## 색

기본 팔레트는 `index.html` 안의 `DEFAULT = {h:222, s:71, mode:'dark'}` 에서 계산됩니다.
나머지 페이지는 그 값에서 나온 색을 CSS 변수로 박아둔 상태입니다.

| 용도 | 값 |
| --- | --- |
| 배경 | `#090a0e` |
| 강조 | `#85a3ea` |
| 보조 강조 | `#8f73e7` |
| 본문 | `#e8eaed` |

색을 바꾸려면 `index.html`의 `DEFAULT` 값과, 나머지 페이지 `:root` 블록의 값을 같이 고쳐야 합니다.

## 배포

`main` 브랜치에 푸시하면 GitHub Pages가 자동으로 반영합니다.
Settings → Pages 에서 Source 가 `main` / `/ (root)` 인지 확인하세요.

사이트 주소: https://yve0n.github.io/
