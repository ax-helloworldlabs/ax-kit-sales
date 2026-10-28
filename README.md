# AX 키트 영업·고객관리

생성형 AI로 고객 상담 내용을 요약하고, 고객 요구사항을 구조화해 맞춤형 제안서 초안과 고객 대응 운영안을 만드는 8시간 실습 과정의 수강생 안내 페이지입니다. 2026년 10월 30일(금) 09:00–18:00, 향군타워 9층 소강의실.

## 무엇을 어디서 고치나

| 고칠 내용 | 파일 · 위치 |
|---|---|
| 페이지 제목·검색/공유 설명 | `index.html` `<head>`의 `<title>`, `meta description`, `og:*` |
| 사업명·과정명·소개 문구 | `index.html` `section.hero` (`.eyebrow`, `.course-label`, `h1`, `.hero-sub`, `.hero-desc`) |
| 날짜·시간·장소 요약 띠 | `index.html` `.event-strip` |
| 신분증 안내 배너 | `index.html` `.id-notice` |
| 준비물 카드 | `index.html` `#preparation` `.prep-card` |
| 일정 카드·장소·엘리베이터 안내·지도 링크 | `index.html` `#place` (`.schedule-card`, `.venue-card`, `.elevator-note`) |
| 주소 복사 버튼의 주소 | `script.js` 첫 줄 `const address` |
| 커리큘럼 모듈(시간·과목명·세부 내용) | `index.html` `#curriculum` 의 `<details class="module">` 5개 |
| 점심시간 줄 | `index.html` `.lunch-break` |
| 교육 결과물 3가지 | `index.html` `.outcome` |
| 사전 안내 PDF·SafariON·카카오 채널·전화 | `index.html` `#resources`, 파일은 `assets/course-guide.pdf` |
| 하단 사업명·운영기관·홈페이지 | `index.html` `<footer>` |
| 모바일 하단 고정 바 | `index.html` `.mobile-bar` |
| Claude 유료 계정 1개월 지원·계정 정보 안내 | `index.html` `#support`, `<head>` description |
| 색상 | `styles.css` 첫 줄 `:root` (`--green`, `--lime`, `--ink` 등) |

CSS·JS를 고친 뒤에는 `index.html`의 `styles.css?v=20261028-1`, `script.js?v=20261028-1` 끝 숫자를 1 올려 주세요(브라우저 캐시 갱신).

## 아직 넣지 않은 정보 / 확인할 정보

- **교육 대상**: 이번 자료에 근거가 없어 페이지에 넣지 않았습니다. 확정되면 `#curriculum` `.journey-intro` 안에 `<p><b>교육 대상</b> …</p>` 형태로 추가하세요.
- **Claude 계정 지원 여부**: 자료에 없어 넣지 않았습니다.
- **강사명**: 시간표에 있으나 지난 페이지와 같이 표기하지 않았습니다.
- **지난 과정(ax-kit-quality-1026) 공통 정보를 사용자 지시로 재사용**: 아래 항목은 이번 자료(시간표·교안 목차)에는 없고, 지난 과정 페이지의 값을 그대로 가져왔습니다. 이번 과정에서 달라지면 수정하세요.
  - 준비물(실물·모바일 신분증 필수·캡처본 불가, 개인 노트북, 노트북 충전기) — `.id-notice`, `#preparation`, `.mobile-bar`, `og:description`
  - 장소 부가 안내(쿠차라 방면 엘리베이터·보안게이트, 잠실역 인근) — `.event-strip`, `#place`
  - 실습 도구 태그 "Claude Cowork 실습" — `.journey-intro`
  - 교육 사전 안내 PDF(`assets/course-guide.pdf`, SafariON 공통 이용 가이드)
  - SafariON 교안·실습 자료 링크, 카카오톡 채널 Hello, AX, 전화 070-8833-7771 — `#resources`
- **점심시간 12:00–13:00**: 사용자 확인 완료(2026-10-28).
- **SafariON 로그인 안내**: 아이디 = 교육 안내를 받은 메일 주소, 비밀번호 = `safarion` — 사용자 지시로 `#resources` 교안·실습 자료 카드에 표기(2026-10-28).

- **캘린더 일정 저장(.ics)**: 사용자 요청으로 제거(2026-10-28).
- **계정 정보 시트 링크(보류)**: 지금은 링크 없이 "계정 정보는 교육 당일 제공됩니다"만 표시(`#support` `.support-button.is-pending`). 당일 연결할 때 `<span …is-pending>`을 `<a class="button support-button" href="시트 URL" target="_blank" rel="noopener noreferrer">교육 계정 정보 확인하기 ↗</a>`로 바꾸고 캐시 버전을 올립니다. 시트 URL은 공개 저장소에 두지 않고 하네스 `_workspace/ax-kit-sales/02_builder_notes.md`에만 기록.
