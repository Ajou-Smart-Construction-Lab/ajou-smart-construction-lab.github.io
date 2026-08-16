# Smart Construction Lab — Homepage

https://www.smartconstructionlab.com · GitHub Pages(Jekyll)로 호스팅.

## 구조

| 무엇을 고치나 | 어느 파일 |
|---|---|
| 뉴스 추가 | `_data/news.json` — 배열 **맨 앞**에 `{"year": "2026", "date": "Mar 2026", "text": "..."}` 추가. 홈의 Recent News(최신 6건)와 News 페이지에 자동 반영 |
| 논문 추가 | `publications.md` — 해당 섹션 목록 맨 위에 한 줄 추가 (번호는 기존 최대 +1, 예: `[J45]`) |
| 멤버 추가/변경 | `members.html` — member-card 블록 복사, 사진은 `assets/img/`에 800px 폭 JPEG로 |
| 연구과제 추가 | `research.md` — Research Projects 목록 맨 위에 추가 |
| 수상 추가 | `professor.md` — Awards & Honors 목록에 추가 |
| 디자인 | `assets/css/style.css`, 공통 레이아웃은 `_layouts/default.html` |

수정 후 `git add -A && git commit && git push` 하면 1~2분 내 GitHub Pages가 자동 재빌드한다. 로컬 빌드 환경 불필요.

## 규칙

- 뉴스와 논문은 새 항목이 항상 위(최신순).
- 이미지는 `assets/img/`에, 큰 원본 대신 축소본(사진 800px, 히어로 1920px)을 넣는다.
- 원본 Wix 콘텐츠 추출본과 마이그레이션 기록은 상위 폴더 `../content/` 참조 (저장소 밖).
