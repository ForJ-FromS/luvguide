# LUV GUIDE — 러브로그 · 러브인포 사용 안내 사이트

정적 사이트. 빌드 없이 그대로 GitHub Pages에 올리면 됩니다.

## 구조
- `index.html` — 입구(두 서비스 목차)
- `luvlog/*.html`, `luvinfo/*.html` — 안내 페이지(파일 하나 = 페이지 하나)
- `updates.html` — 업데이트 노트
- `assets/nav.js` — 목차·검색·이전/다음. **페이지를 추가하면 여기 NAV 배열에 한 줄** (`p` 경로, `s` 서비스, `c` 카테고리, `t` 제목, `k` 검색어)
- `assets/style.css` — 공통 스타일
- `img/` — 스크린샷. `SHOTS.md`의 파일 이름대로 넣으면 자동 표시

## 페이지 추가
1. 기존 페이지 하나를 복사해 이름을 바꾸고 본문을 채웁니다(`<main class="doc">` 안).
2. `assets/nav.js`의 NAV에 한 줄 추가. 목차 순서 = 배열 순서.
3. 사진은 `<figure class="shot">` 블록을 복사해 `img/파일이름.png`만 바꿉니다.

## 도메인
저장소 Settings → Pages에 커스텀 도메인을 넣고 루트에 `CNAME` 파일(도메인 한 줄)을 두면 됩니다.
