# INDEX — 자산·섹션 색인

「금융 이상탐지 모델 보안과 적대적 데이터 대응 방안」 인터랙티브 해설 페이지의 파일·그림·섹션 지도입니다.
저장소 루트에 그대로 올리는 것을 전제로 쓰였습니다(폴더 없음, GitHub 웹 업로드 가능).

---

## 1. 파일

| 파일 | 크기 | 역할 |
|---|---|---|
| `index.html` | 8 KB | 첫 화면(색인) — 썸네일 카드, 한국어·베트남어 입구, README/INDEX 링크 |
| `01_adversarial_finance.html` | 2.16 MB | 한국어 원본 — 8개 장 + 부록 K·O, 그림 4장 base64 내장 |
| `01_adversarial_finance.en.html` | 2.16 MB | 영어판 — 같은 구성, 언어 UI·hreflang 포함 |
| `01_adversarial_finance.zh.html` | 2.16 MB | 중국어판 — 같은 구성, 언어 UI·hreflang 포함 |
| `01_adversarial_finance.ja.html` | 2.17 MB | 일본어판 — 같은 구성, 언어 UI·hreflang 포함 |
| `01_adversarial_finance.uz.html` | 2.16 MB | 우즈베크어판 — 같은 구성, 언어 UI·hreflang 포함 |
| `01_adversarial_finance.ru.html` | 2.17 MB | 러시아어판 — 같은 구성, 언어 UI·hreflang 포함 |
| `01_adversarial_finance.vi.html` | 2.17 MB | 베트남어판 — 같은 구성, 언어 UI·hreflang 포함 |
| `README.md` | 19 KB | 사용 문서 — 한국어 → Tiếng Việt |
| `INDEX.md` | 6 KB | 6 KB · 이 문서 — 자산·섹션 색인, 제작 메모 |
| `bg_01.png` | 1.14 MB | 히어로 배경 1920×720 (페이지 내장본은 1600×600 최적화) |
| `sc_01_hero.png` | 1.22 MB | 히어로 무대 1200×800 (내장본 1000×667) |
| `cut_01_think.png` | 614 KB | 1장 코믹 컷 960×540 (내장본 900×506) |
| `cut_01_filter.png` | 688 KB | 6장 방어 컷 960×540 (내장본 900×506) |
| `sc_01_outro.png` | 1.23 MB | 결론 장면 1200×800 (내장본 1000×667) |
| `og_01.png` | 998 KB | 공유 미리보기 1200×630 |
| `thumb_01.png` | 292 KB | 목차 썸네일 600×400 (bg_01 우측 3:2 크롭) |

- HTML은 **한 파일에 그림·데이터·스크립트를 모두 담습니다**(base64). PNG는 같은 그림의 원본 자산이며 페이지 표시에는 쓰이지 않습니다. 지워도 페이지는 그대로 동작합니다.
- 파일 이름 규칙: `편번호_영문소문자_밑줄.html` + 번역판은 `이름.언어코드.html`. 한 번 정한 이름은 바꾸지 않습니다(언어 전환·상호 링크가 이름에 기대기 때문).

## 2. 그림 자산

| 키 | 규격 | 판 | 들어가는 곳 | 대신 쓰는 그림 |
|---|---|---|---|---|
| `bg_01` | 1920×720 | F(배경) | 히어로 뒤 | CSS 그라데이션 + 격자 무늬 |
| `sc_01_hero` | 1200×800 | E(장면) | 히어로 무대 | CSS 배경 |
| `cut_01_think` | 960×540 | G(컷) | 1장 코믹 | 컷 생략 |
| `cut_01_filter` | 960×540 | G(컷) | 6장 방어 | 컷 생략 |
| `sc_01_outro` | 1200×800 | E(장면) | 결론 | `sc_01_hero` |
| `og_01` | 1200×630 | K(OG) | 공유 미리보기 | 없음 |
| `thumb_01` | 600×400 | I(썸네일) | 첫 화면 카드 | 색 카드 |

- 그림체: 16비트 RPG 픽셀아트, 굵은 외곽선, 2~3단 명암, 야간 연구실 팔레트
  (`#1b1533` / `#120e24` / `#261e45` + 바이올렛 `#b07cff` · 시안 `#57d0dc` · 앰버 `#ffc65c` · 핑크 `#ff86b8`).
- 네 캐릭터: 박사 · 조수 · 초파리 연구원 · Money-Robo. 말풍선 아바타는 전신 원화에서 머리·상반신을 잘라 160×160으로 넣었습니다.
- 페이지에 들어가는 그림은 용량을 줄인 내장본(192색 PNG-8)이고, 루트의 PNG는 원본입니다.

## 3. 페이지 섹션 지도

| 앵커 | 섹션 | 인터랙션 | 그림 |
|---|---|---|---|
| `#hero` | 표지·KPI | — | `bg_01`, `sc_01_hero` |
| `#comic` | 1. 적대적 데이터의 본질 | — | `cut_01_think` |
| `#laundering` | 2. 자금세탁 시나리오 | — | — |
| `#imbalance` | 3. 불균형과 증강 비판 | — | — |
| `#lv1` | 4. 4대 공격 유형 | `cv-attack` (3모드) | — |
| `#lv2` | 5. 모델별 붕괴 | `cv-perf` (3상태) | — |
| `#lv3` | 6. 통계 필터링 | `cv-stat` | `cut_01_filter` |
| `#duel` | 대결 판정 | 결과 검증 버튼 | — |
| `#outro` | 결론 | — | `sc_01_outro` |
| `#kg` | K. 지식 색인 | 검색·필터 | — |
| `#export` | O. 꾸러미 | ZIP·BibTeX·Turtle | — |

## 4. 내장 데이터 블록

| id | 형식 | 내용 | 쓰는 곳 |
|---|---|---|---|
| `kg-raw` | JSON | 노드 10 · 엣지 6 (Concept/Method/Metric/Claim) | 지식 색인 카드 |
| `kg-ld` | JSON-LD | SKOS 개념 3건 | 꾸러미 내보내기 |
| `refs-csl` | CSL-JSON | 논문 서지 1건 | BibTeX·참고문헌 |
| `page-meta` | JSON | 제목·번호(FDS-01)·언어·기준 문헌 | 꾸러미 |

## 5. 언어

| 코드 | 파일 | 상태 |
|---|---|---|
| `ko` | `01_adversarial_finance.html` | 원본 |
| `en` | `01_adversarial_finance.en.html` | 번역 완료 |
| `zh` | `01_adversarial_finance.zh.html` | 번역 완료 |
| `ja` | `01_adversarial_finance.ja.html` | 번역 완료 |
| `uz` | `01_adversarial_finance.uz.html` | 번역 완료 |
| `ru` | `01_adversarial_finance.ru.html` | 번역 완료 |
| `vi` | `01_adversarial_finance.vi.html` | 번역 완료 |

- 전환: 상단 🌐 선택 상자 · 오른쪽 아래 🌐 배너 · `?lang=vi`.
- 기억: `localStorage['fds01_lang']`. 자동 전환은 한국어 원본에서만, 번역 파일 존재를 `HEAD`로 확인한 뒤에만 이동(404 방지).
- `hreflang` 8줄(ko·en·zh-CN·ja·uz·ru·vi·x-default)이 두 파일 `<head>`에 들어 있습니다.

## 6. 제작·검수 메모

1. 한국어 본문은 기존 단일 HTML 원본을 그대로 두고, 그림·언어 UI만 덧붙였습니다(본문 문장 수정 없음).
2. 그림은 `gpt-image-2`로 생성하고 캐릭터 시트(R1)와 장면 화풍(R2)을 매 생성마다 `-i`로 주입해 외형을 고정했습니다.
3. 생성 후 이미지 이해 도구로 **글자·숫자·로고 없음, 4인 외형 유지, 잘림 없음, 로봇 얼굴에 입 없음**을 확인했습니다.
4. 번역은 문장 단위 치환표로 넣었습니다(HTML 텍스트 · `alt`/`aria-label` · JS 문자열 · 온톨로지 JSON 값). 화면에 남은 한국어 0건(서지 메타데이터 제외).
5. 두 HTML 모두 `<script>` 구문 검사 통과, 1280px에서 가로 넘침 없음(스크린샷 확인).
6. 남은 일: `og:image`를 절대 URL로 바꾸기(현재 상대 경로 `og_01.png`), README의 `<사용자명>/<저장소>` 채우기.

## 7. 갱신 이력

| 날짜 | 내용 |
|---|---|
| 2026-10-25 | 그림 7장 제작(bg_01 · sc_01_hero · cut_01_think · cut_01_filter · sc_01_outro · og_01 · thumb_01) |
| 2026-10-26 | HTML에 그림·캐릭터 아바타 적용, 언어 UI(hreflang·자동 전환) 추가, 베트남어판 제작, README·INDEX 작성 |
