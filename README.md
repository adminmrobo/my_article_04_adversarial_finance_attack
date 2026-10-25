# 금융 이상탐지 모델 보안과 적대적 데이터 대응 방안 — 인터랙티브 해설 페이지

안상선(2024) 「금융 분야의 이상탐지 모델 보안을 위한 통계 기반의 적대적 데이터 대응 방안 — 실증적 분석과 시뮬레이션 결과」(*미래사회* 15(3), 147–166)를 한 장의 인터랙티브 HTML로 풀어낸 해설 페이지입니다. 사기꾼이 위장 데이터를 섞어 넣을 때 **어떤 모델이 끝까지 사기를 잡아내는가**를, 직접 버튼을 눌러 확인할 수 있습니다. 빌드 과정 없이 파일 하나만 열면 동작합니다.

**한국어 원본**과 **6개 외국어판(English · 中文 · 日本語 · Oʻzbekcha · Русский · Tiếng Việt)**, 그리고 이 문서·그림 자산이 들어 있습니다.

---

## 바로 보기

| 구분 | 주소 |
|---|---|
| 첫 화면(색인) | `https://<사용자명>.github.io/<저장소>/` |
| 한국어 | `https://<사용자명>.github.io/<저장소>/01_adversarial_finance.html` |
| English | `https://<사용자명>.github.io/<저장소>/01_adversarial_finance.en.html` |
| 中文 | `https://<사용자명>.github.io/<저장소>/01_adversarial_finance.zh.html` |
| 日本語 | `https://<사용자명>.github.io/<저장소>/01_adversarial_finance.ja.html` |
| Oʻzbekcha | `https://<사용자명>.github.io/<저장소>/01_adversarial_finance.uz.html` |
| Русский | `https://<사용자명>.github.io/<저장소>/01_adversarial_finance.ru.html` |
| Tiếng Việt | `https://<사용자명>.github.io/<저장소>/01_adversarial_finance.vi.html` |
| 로컬 실행 | 내려받아 `01_adversarial_finance.html`을 더블클릭 |

> 위 `<사용자명>`·`<저장소>`는 업로드 전에 실제 값으로 바꿔 주세요. 그림·스크립트·데이터가 모두 파일 안에 들어 있어 **인터넷 없이도** 열립니다(글꼴만 Google Fonts에서 받아 옵니다).

## 저자

글 · 안상선 ((주)M-Robo 대표) · 원 논문: *미래사회* 15(3), 147–166, DOI [10.22987/jifso.2024.15.3.147](https://doi.org/10.22987/jifso.2024.15.3.147)

## 언어

| 언어 | 파일 | 상태 |
|---|---|---|
| 한국어 | `01_adversarial_finance.html` | 원본 |
| English | `01_adversarial_finance.en.html` | 번역 완료 |
| 中文 | `01_adversarial_finance.zh.html` | 번역 완료 |
| 日本語 | `01_adversarial_finance.ja.html` | 번역 완료 |
| Oʻzbekcha | `01_adversarial_finance.uz.html` | 번역 완료 |
| Русский | `01_adversarial_finance.ru.html` | 번역 완료 |
| Tiếng Việt | `01_adversarial_finance.vi.html` | 번역 완료 |

- 바꾸는 방법은 세 가지입니다. ① 상단 메뉴 오른쪽 **🌐 선택 상자**, ② 오른쪽 아래 **🌐 배너**, ③ 주소 뒤에 `?lang=vi`(예: `...01_adversarial_finance.html?lang=vi`).
- 고른 언어는 브라우저(`localStorage` 키 `fds01_lang`)에 기억되고, 페이지를 옮겨도 `#섹션` 위치가 유지됩니다.
- **자동 전환은 한국어 원본에서만** 일어납니다. 브라우저 언어가 vi면 베트남어판으로 넘어갑니다. 다만 번역 파일이 없으면(영어·중국어·일본어·우즈베크어·러시아어) 이동하지 않고 한국어에 머뭅니다. 파일 존재를 먼저 확인(`HEAD`)하기 때문에 깨진 링크(404)가 생기지 않습니다.
- 번역판 주소로 들어온 사람은 자동 전환하지 않습니다(공유한 링크는 그 언어로 열립니다).

## 구성 (한 페이지 = 8개 장 + 부록 2개)

| # | 섹션 | 다루는 것 | 만질 수 있는 것 |
|---|---|---|---|
| 1 | 코믹 AI 낚시 | 적대적 섭동의 원리, 팬더→긴팔원숭이, STOP 표지판 사례 | — |
| 2 | 불법자금 세탁 | 모델 탐색 → 스몰 드롭 → 통계적 세탁 3단계 | — |
| 3 | 불균형 & 증강 비판 | 89.9 : 10.1 불균형, SMOTE 무용론 | — |
| 4 | 4대 공격 유형 | 거래량·가격·금액·추세 조작 | 분포 곡선 3종 전환 |
| 5 | 모델별 붕괴 | SVM·RF·LR·LSTM의 Acc/Recall 변화 | Clean / 8.1% 주입 / KS 필터 |
| 6 | 통계 필터링 | KS·T·F 검정의 차단율 | — |
| 대결 | 초파리 vs Money-Robo | RF+KS 0.94 vs LSTM 0.00 판정 | 결과 검증 버튼 |
| 결론 | 방어 전략 | RF 앙상블 + KS 필터 선제 배치 | — |
| K | 지식 색인 | 개념 10건 검색·필터 | 검색창, 필터 버튼 |
| O | 꾸러미 | 지식 그래프·서지 추출 | ZIP / BibTeX 복사 / Turtle |

## 핵심 숫자 (논문 실측)

| 지표 | 값 | 출처 |
|---|---|---|
| KS-test 적대적 데이터 차단율 | **94.59%** | 그림 17, 161쪽 |
| T-test 차단율 | 73.96% | 같은 절 |
| F-test 차단율 | 0.00% | 같은 절 |
| LSTM 재현율(공격 주입 후) | **0.00** | 표 6, 160쪽 |
| Random Forest 재현율 | 0.94 → 0.98 | 표 6, 160쪽 |
| 데이터 불균형(정상:이상) | 89.9% : 10.1% | 3장 |
| 적대적 데이터 주입률 | 8.1% | 5장 |

## 파일

```
.
├── index.html                        첫 화면(색인, 한국어·베트남어 입구)
├── 01_adversarial_finance.html       한국어 원본 (약 2.2 MB)
├── 01_adversarial_finance.en.html    English판 (2.16 MB)
├── 01_adversarial_finance.zh.html    中文판 (2.16 MB)
├── 01_adversarial_finance.ja.html    日本語판 (2.17 MB)
├── 01_adversarial_finance.uz.html    Oʻzbekcha판 (2.16 MB)
├── 01_adversarial_finance.ru.html    Русский판 (2.17 MB)
├── 01_adversarial_finance.vi.html    Tiếng Việt판 (2.17 MB)
├── README.md                         이 문서 (한국어 + Tiếng Việt)
├── INDEX.md                          자산·섹션 색인 (제작 메모 포함)
├── og_01.png                         공유 미리보기 1200×630
├── thumb_01.png                      목차 카드 썸네일 600×400
├── bg_01.png                         히어로 배경 1920×720
├── sc_01_hero.png                    히어로 무대 1200×800
├── cut_01_think.png                  생각 구름 컷 960×540
├── cut_01_filter.png                 통계 필터 컷 960×540
└── sc_01_outro.png                   아웃트로 1200×800
```

- 폴더 없이 **저장소 루트에 그대로** 올리면 GitHub Pages가 바로 열립니다.
- HTML 안의 그림은 `base64`로 내장되어 있고, 위 PNG는 같은 그림의 **원본 자산**(재사용·수정용)입니다. 페이지 표시에는 쓰이지 않으므로 지워도 페이지는 그대로 동작합니다.
- GitHub 웹 업로드 화면에 파일을 끌어다 놓으면 되고, `og_01.png`는 저장소 주소를 넣은 뒤 `og:image`를 절대 URL로 바꾸면 SNS 미리보기가 살아납니다(현재는 상대 경로).

## 그림

| 파일 | 규격 | 쓰는 곳 | 내용 |
|---|---|---|---|
| `bg_01.png` | 1920×720 | 히어로 배경 | 밤의 연구실. 왼쪽 45%는 제목을 얹는 빈 벽, 오른쪽에 서버랙·모니터 3대·봉인 봉투 상자·노트·데이터 카드 |
| `sc_01_hero.png` | 1200×800 | 히어로 무대 | 데이터 파이프라인에 가면 쓴 위장 카드 한 장이 섞여 들어오는 순간, 네 캐릭터 전원 |
| `cut_01_think.png` | 960×540 | 1장 코믹 | 박사의 생각 구름 — 정규분포 안에 숨어든 가면 쓴 이상점 |
| `cut_01_filter.png` | 960×540 | 6장 방어 | 곡선형 메시 필터를 통과한 정상 카드 / 걸러져 반려조로 떨어진 위장 카드 |
| `sc_01_outro.png` | 1200×800 | 결론 | 판정 뒤의 연구실 — 초파리 승리, 로봇 손절, 박사 승인, 조수 박수 |
| `og_01.png` | 1200×630 | 공유 미리보기 | 중앙 게이트 + 4인, 축소 판독 대응 |
| `thumb_01.png` | 600×400 | 첫 화면 카드 | `bg_01` 우측 3:2 크롭 |

그림체는 16비트 RPG 픽셀아트(굵은 외곽선, 2~3단 명암)로 통일했고, 캐릭터는 **박사 · 조수 · 초파리 연구원 · Money-Robo** 네 명입니다. 말풍선 아바타는 캐릭터 원화를 잘라 160×160으로 넣었습니다.

## 데이터와 이미지 — 무엇이 실측이고 무엇이 설명용인가

| 요소 | 성격 |
|---|---|
| 표(4대 공격 유형, 모델별 지표, 차단율) | **논문 실측값**을 그대로 옮김 |
| 히어로 KPI 4칸, 결론 문장의 숫자 | 논문 실측값 |
| 캔버스 3개(분포·막대·차단율) | 논문 값과 같은 축으로 **브라우저에서 다시 그린 시각화**. 막대·차단율은 논문 값 고정, 분포 곡선은 모양을 설명하기 위한 **예시 곡선** |
| 삽화 4장 | **설명용 모형**. 실제 연구 현장 사진이 아니고, 인물은 픽셀아트 캐릭터입니다. 그림 안의 그래프는 모양만 있는 추상 도형이며 글자·숫자가 없습니다 |
| 데이터 | 합성 틱 데이터(10,000건) 기준. 실제 사람의 거래 기록은 쓰지 않았습니다 |

## 용어 표기

- **재현율(Recall)** — 실제 이상 거래 중 모델이 잡아낸 비율. 이 페이지의 결론을 떠받치는 지표라, 처음 나올 때 영어를 함께 적었습니다.
- **적대적 데이터** — 정상처럼 보이도록 미세하게 변조해 모델을 속이려는 입력. 논문 표기를 따라 '적대적'으로 통일했습니다.
- **차단율** — 통계 검정 필터가 적대적 데이터를 걸러낸 비율.
- **판정** — 대결 섹션에서 두 선택(RF+KS / LSTM 단독)의 결과를 가르는 말.

## 라이선스

이 페이지와 그림은 **CC BY-NC 4.0**(저작자표시–비영리 4.0 국제)으로 공유합니다. 수업·강의·비영리 연구에서 자유롭게 쓰실 수 있고, 상업적 이용은 별도 문의가 필요합니다.

출처 표기 예:

```
안상선. (2024). 금융 분야의 이상탐지 모델 보안을 위한 통계 기반의 적대적 데이터 대응 방안.
미래사회, 15(3), 147–166. https://doi.org/10.22987/jifso.2024.15.3.147
해설 페이지: <저장소 주소> (CC BY-NC 4.0)
```

## 기술 메모

- 단일 HTML · 외부 라이브러리 없음 · Canvas 2D + 바닐라 JS. 그림은 base64 내장.
- `prefers-reduced-motion`에서 애니메이션 정지, 캔버스에 `aria-label`, 결과 문구에 `aria-live`.
- 용어 말풍선·지식 색인은 `<script type="application/json" id="kg-raw">` 한 곳에서 만들어집니다. 용어를 고치려면 그 블록과 본문을 함께 고치면 됩니다.

---

<a id="en"></a>

# Financial Anomaly-Detection Model Security and Adversarial Data Response — interactive explainer

One interactive HTML that unpacks Ahn Sangsun (2024), *A Statistical Approach to Adversarial Data for Anomaly-Detection Model Security in Finance — Empirical Analysis and Simulation Results* (*Mirae Sahoe* 15(3), 147–166). Press the buttons and see which model still catches fraud once disguised data slips in. No build step — open the file and it runs.

| Item | Address |
|---|---|
| Explainer (English) | `https://<user>.github.io/<repo>/01_adversarial_finance.en.html` |
| Index page | `https://<user>.github.io/<repo>/index.html` |
| Korean original | `https://<user>.github.io/<repo>/01_adversarial_finance.html` |

Written by Ahn Sangsun (CEO, M-Robo Co., Ltd.) · original paper DOI [10.22987/jifso.2024.15.3.147](https://doi.org/10.22987/jifso.2024.15.3.147)

**Language.** Switch with the 🌐 box in the top bar, the 🌐 button in the bottom-right corner, or `?lang=`. Your choice is stored in `localStorage['fds01_lang']` and the `#section` anchor is kept. Automatic switching happens only on the Korean original, and only after a `HEAD` request confirms the translated file exists, so a missing translation never produces a 404.

**Structure (one page = 8 chapters + 2 appendices).** 1 Comic: what adversarial data really is · 2 The three-step money-laundering script · 3 The imbalance trap and why SMOTE does not help · 4 Four attack types (switch the distribution) · 5 Model collapse (clean / 8.1% injected / KS-filtered) · 6 Statistical filtering · Showdown: fly vs Money-Robo (verify button) · Conclusion · K Knowledge index (search, filter) · O Toolkit (ZIP, BibTeX, Turtle).

**Key numbers (measured in the paper).** KS-test blocks **94.59%** of adversarial data; T-test 73.96%; F-test 0.00%. LSTM recall after attack **0.00**; Random Forest recall 0.94 → 0.98. Imbalance 89.9% : 10.1%, adversarial injection 8.1%.

**What is measured, what is illustrative.** Tables, KPI cards and the bar/block-rate charts carry the paper's measured values; the two distribution curves are drawn to show shape. The four illustrations are **illustrative mock-ups** — not photographs of a real lab, and the charts inside them are abstract shapes with no text or numbers. Data is synthetic (10,000 tick records); no real customer data is used.

**Files.** `index.html` · `01_adversarial_finance{,.en,.zh,.ja,.uz,.ru,.vi}.html` · `README.md` · `INDEX.md` · 7 PNG assets. Licence: CC BY-NC 4.0.

---

<a id="zh"></a>

# 金融异常检测模型安全与对抗数据应对方案 — 交互式图解

用一个交互式 HTML 拆解安相善（2024）《金融领域异常检测模型安全：基于统计的对抗数据应对方案——实证分析与模拟结果》（《未来社会》15(3)，147–166）。按下按钮，就能看到伪装数据混入后哪个模型仍能抓住诈骗。无需构建，打开文件即可运行。

| 项目 | 地址 |
|---|---|
| 图解（中文） | `https://<user>.github.io/<repo>/01_adversarial_finance.zh.html` |
| 首页 | `https://<user>.github.io/<repo>/index.html` |
| 韩文原文 | `https://<user>.github.io/<repo>/01_adversarial_finance.html` |

安相善（M-Robo 株式会社代表）· 原文 DOI [10.22987/jifso.2024.15.3.147](https://doi.org/10.22987/jifso.2024.15.3.147)

**语言切换。** 可使用顶部菜单右侧的 🌐 选择框、右下角的 🌐 按钮，或在地址后加 `?lang=`。选择保存在 `localStorage['fds01_lang']`，`#章节` 位置保持不变。自动跳转只在韩文原文上发生，并且先用 `HEAD` 确认译文文件存在，因此不会出现 404。

**结构（一页 = 8 章 + 2 个附录）。** 1 漫画：对抗数据的本质 · 2 洗钱三步剧本 · 3 不平衡陷阱与 SMOTE 无用 · 4 四类攻击（切换分布） · 5 模型崩塌（干净 / 注入 8.1% / KS 过滤） · 6 统计过滤 · 对决：果蝇 vs Money-Robo（验证按钮） · 结论 · K 知识索引（搜索、过滤） · O 资料包（ZIP、BibTeX、Turtle）。

**核心数字（论文实测）。** KS 检验拦截 **94.59%** 的对抗数据；T 检验 73.96%；F 检验 0.00%。攻击后 LSTM 召回率 **0.00**；随机森林召回率 0.94 → 0.98。不平衡 89.9% : 10.1%，对抗数据注入 8.1%。

**哪些是实测，哪些是示意。** 表格、指标卡与柱状图/拦截率图使用论文实测值；两条分布曲线只用于说明形状。四张插画是**说明用模型**，并非真实实验室照片，画中的图表只是抽象图形，不含文字与数字。数据为合成数据（10,000 条逐笔记录），不使用真实客户数据。

**文件。** `index.html` · `01_adversarial_finance{,.en,.zh,.ja,.uz,.ru,.vi}.html` · `README.md` · `INDEX.md` · 7 个 PNG 素材。许可证：CC BY-NC 4.0。

---

<a id="ja"></a>

# 金融異常検知モデルのセキュリティと敵対的データ対応策 — インタラクティブ解説

アン・サンソン（2024）『金融分野の異常検知モデルのセキュリティのための統計ベースの敵対的データ対応策 — 実証的分析とシミュレーション結果 —』（『未来社会』15(3)、147–166）を、一枚のインタラクティブHTMLで読み解く。ボタンを押せば、偽装データが紛れ込んだときにどのモデルが詐欺を捕まえられるかが分かる。ビルド不要で、ファイルを開けばそのまま動く。

| 項目 | アドレス |
|---|---|
| 解説（日本語） | `https://<user>.github.io/<repo>/01_adversarial_finance.ja.html` |
| 最初の画面 | `https://<user>.github.io/<repo>/index.html` |
| 韓国語の原文 | `https://<user>.github.io/<repo>/01_adversarial_finance.html` |

アン・サンソン（株式会社M-Robo代表）· 原文 DOI [10.22987/jifso.2024.15.3.147](https://doi.org/10.22987/jifso.2024.15.3.147)

**言語の切り替え。** 上部メニュー右の 🌐 選択ボックス、右下の 🌐 ボタン、またはアドレスの末尾に `?lang=` を付ける。選択は `localStorage['fds01_lang']` に保存され、`#セクション` の位置も保たれる。自動切り替えは韓国語の原文でのみ働き、しかも `HEAD` で翻訳ファイルの存在を確認してから移動するので、404 は起きない。

**構成（1ページ = 8章 + 付録2つ）。** 1 コミック：敵対的データの本質 · 2 資金洗浄の三段階シナリオ · 3 不均衡の罠とSMOTEの無用 · 4 四大攻撃類型（分布を切り替え） · 5 モデルの崩壊（クリーン／8.1%注入／KSフィルタ） · 6 統計フィルタ · 対決：ハエ対Money-Robo（検証ボタン） · 結論 · K 知識索引（検索・フィルタ） · O パッケージ（ZIP・BibTeX・Turtle）。

**主要な数字（論文の実測）。** KS検定は敵対的データの **94.59%** を遮断。T検定は73.96%、F検定は0.00%。攻撃後のLSTM再現率は **0.00**、Random Forestの再現率は0.94 → 0.98。不均衡は89.9% : 10.1%、敵対的データの注入率は8.1%。

**実測と示意の区別。** 表・指標カード・棒グラフと遮断率の図は論文の実測値をそのまま使っている。二本の分布曲線は形を示すためのものである。四枚の挿絵は**説明用の模型**であり、実際の研究室の写真ではない。絵の中のグラフは抽象的な図形だけで、文字も数字もない。データは合成のティックデータ10,000件で、実在の顧客データは使っていない。

**ファイル。** `index.html` · `01_adversarial_finance{,.en,.zh,.ja,.uz,.ru,.vi}.html` · `README.md` · `INDEX.md` · PNG素材7点。ライセンス：CC BY-NC 4.0。

---

<a id="uz"></a>

# Moliya anomaliya aniqlash modeli xavfsizligi va qarshi maʼlumotlarga qarshi chora — interaktiv tushuntirish

Ahn Sangsun (2024) «Moliya sohasida anomaliya aniqlash modeli xavfsizligi uchun statistikaga asoslangan qarshi maʼlumotlarga qarshi chora — amaliy tahlil va simulyatsiya natijalari» («Mirae Sahoe» 15(3), 147–166) maqolasini bitta interaktiv HTML da ochib beradi. Tugmalarni bosib, niqobli maʼlumot aralashganda qaysi model firibgarlikni ushlab qolishini koʻrasiz. Hech qanday yigʻish kerak emas — faylni ochsangiz ishlaydi.

| Boʻlim | Manzil |
|---|---|
| Tushuntirish (oʻzbekcha) | `https://<user>.github.io/<repo>/01_adversarial_finance.uz.html` |
| Bosh sahifa | `https://<user>.github.io/<repo>/index.html` |
| Koreyscha asl nusxa | `https://<user>.github.io/<repo>/01_adversarial_finance.html` |

Muallif: Ahn Sangsun (M-Robo kompaniyasi rahbari) · asl maqola DOI [10.22987/jifso.2024.15.3.147](https://doi.org/10.22987/jifso.2024.15.3.147)

**Tilni almashtirish.** Yuqori menyuning oʻng tomonidagi 🌐 tanlash maydoni, pastki oʻng burchakdagi 🌐 tugmasi yoki manzil oxiriga `?lang=` qoʻshish orqali. Tanlov `localStorage['fds01_lang']` da saqlanadi, `#boʻlim` joyi ham saqlanib qoladi. Avtomatik oʻtish faqat koreyscha asl nusxada ishlaydi va avval `HEAD` soʻrovi bilan tarjima fayli borligini tekshiradi — shuning uchun 404 boʻlmaydi.

**Tuzilma (bir sahifa = 8 bob + 2 ilova).** 1 Komiks: qarshi maʼlumotlarning mohiyati · 2 Pul yuvishning uch bosqichli syenariysi · 3 Nomutanosiblik tuzogʻi va SMOTE ning foydasizligi · 4 Toʻrtta hujum turi (taqsimotni almashtirish) · 5 Modellarning qulashi (toza / 8.1% kiritilgan / KS filtri) · 6 Statistik filtr · Bellashuv: drozofila va Money-Robo (tekshirish tugmasi) · Xulosa · K Bilim indeksi (qidirish, filtrlash) · O Toʻplam (ZIP, BibTeX, Turtle).

**Asosiy raqamlar (maqolada oʻlchangan).** KS-test qarshi maʼlumotlarning **94.59%** ini toʻsadi; T-test 73.96%; F-test 0.00%. Hujumdan keyin LSTM toʻliqligi **0.00**, Random Forest toʻliqligi 0.94 → 0.98. Nomutanosiblik 89.9% : 10.1%, qarshi maʼlumot ulushi 8.1%.

**Nima oʻlchangan, nima shartli.** Jadvallar, koʻrsatkich kartalari, ustunli diagramma va toʻsish darajasi grafigi maqoladagi oʻlchangan qiymatlarni oladi; ikki taqsimot egri chizigʻi faqat shaklni koʻrsatish uchun chizilgan. Toʻrtta rasm — **illyustrativ maket**, haqiqiy laboratoriya fotosurati emas; rasmlardagi grafiklar faqat mavhum shakllar, ularda matn va raqam yoʻq. Maʼlumotlar sintetik (10,000 tick yozuvi), haqiqiy mijoz maʼlumotlari ishlatilmagan.

**Fayllar.** `index.html` · `01_adversarial_finance{,.en,.zh,.ja,.uz,.ru,.vi}.html` · `README.md` · `INDEX.md` · 7 ta PNG. Litsenziya: CC BY-NC 4.0.

---

<a id="ru"></a>

# Безопасность модели финансового обнаружения аномалий и противодействие состязательным данным — интерактивный разбор

Один интерактивный HTML разбирает статью Ан Сансона (2024) «Безопасность модели финансового обнаружения аномалий: статистический подход к противодействию состязательным данным — эмпирический анализ и результаты симуляции» («Мирэ сахве» 15(3), 147–166). Нажимайте кнопки и смотрите, какая модель всё ещё ловит мошенничество, когда в данные проникает маскировка. Сборка не нужна — откройте файл, и всё работает.

| Пункт | Адрес |
|---|---|
| Разбор (по-русски) | `https://<user>.github.io/<repo>/01_adversarial_finance.ru.html` |
| Начальная страница | `https://<user>.github.io/<repo>/index.html` |
| Корейский оригинал | `https://<user>.github.io/<repo>/01_adversarial_finance.html` |

Автор: Ан Сансон (генеральный директор M-Robo Co., Ltd.) · DOI оригинала [10.22987/jifso.2024.15.3.147](https://doi.org/10.22987/jifso.2024.15.3.147)

**Переключение языка.** Поле 🌐 в правой части верхнего меню, кнопка 🌐 в правом нижнем углу или `?lang=` в конце адреса. Выбор хранится в `localStorage['fds01_lang']`, якорь `#раздел` сохраняется. Автопереключение работает только на корейском оригинале и лишь после `HEAD`-запроса, подтверждающего наличие перевода, поэтому 404 не возникает.

**Структура (одна страница = 8 глав + 2 приложения).** 1 Комикс: суть состязательных данных · 2 Трёхшаговый сценарий отмывания денег · 3 Ловушка дисбаланса и бесполезность SMOTE · 4 Четыре типа атак (переключение распределения) · 5 Обвал моделей (чистые / 8.1% внедрённых / фильтр KS) · 6 Статистическая фильтрация · Поединок: дрозофила против Money-Robo (кнопка проверки) · Вывод · K Индекс знаний (поиск, фильтры) · O Пакет данных (ZIP, BibTeX, Turtle).

**Ключевые числа (измерены в статье).** KS-тест блокирует **94.59%** состязательных данных; T-тест — 73.96%; F-тест — 0.00%. Полнота LSTM после атаки **0.00**; полнота Random Forest 0.94 → 0.98. Дисбаланс 89.9% : 10.1%, доля внедрённых состязательных данных 8.1%.

**Что измерено, а что иллюстративно.** Таблицы, карточки показателей, столбчатая диаграмма и график доли блокировки берут измеренные значения из статьи; две кривые распределения нарисованы, чтобы показать форму. Четыре иллюстрации — **иллюстративный макет**, а не фотографии реальной лаборатории; графики внутри них — только абстрактные фигуры без текста и чисел. Данные синтетические (10,000 тиковых записей), реальные данные клиентов не используются.

**Файлы.** `index.html` · `01_adversarial_finance{,.en,.zh,.ja,.uz,.ru,.vi}.html` · `README.md` · `INDEX.md` · 7 PNG. Лицензия: CC BY-NC 4.0.

---

<a id="vi"></a>

# Bảo mật mô hình phát hiện bất thường tài chính và giải pháp ứng phó dữ liệu đối kháng — trang giải thích tương tác

Đây là trang HTML tương tác diễn giải bài báo của Ahn Sangsun (2024), *Bảo mật mô hình phát hiện bất thường trong lĩnh vực tài chính: giải pháp ứng phó dữ liệu đối kháng dựa trên thống kê — phân tích thực nghiệm và kết quả mô phỏng* (*Mirae Sahoe* 15(3), 147–166). Bạn có thể tự bấm nút để xem **mô hình nào vẫn bắt được gian lận** khi kẻ gian trộn dữ liệu ngụy trang vào. Chỉ cần mở một tệp, không cần cài đặt hay biên dịch.

Kho lưu trữ có **bản gốc tiếng Hàn** và **bản tiếng Việt**, kèm tài liệu và các tệp hình.

## Xem ngay

| Mục | Địa chỉ |
|---|---|
| Trang đầu (mục lục) | `https://<tên-tài-khoản>.github.io/<kho>/` |
| Tiếng Hàn | `https://<tên-tài-khoản>.github.io/<kho>/01_adversarial_finance.html` |
| Tiếng Việt | `https://<tên-tài-khoản>.github.io/<kho>/01_adversarial_finance.vi.html` |
| Chạy tại máy | Tải về rồi mở `01_adversarial_finance.vi.html` |

> Hãy thay `<tên-tài-khoản>` và `<kho>` bằng giá trị thật trước khi công bố. Hình, mã và dữ liệu đều nằm trong tệp nên trang **chạy được khi không có Internet** (chỉ phông chữ lấy từ Google Fonts).

## Tác giả

Ahn Sangsun (Giám đốc điều hành, M-Robo Co., Ltd.) · Bài gốc: *Mirae Sahoe* 15(3), 147–166, DOI [10.22987/jifso.2024.15.3.147](https://doi.org/10.22987/jifso.2024.15.3.147)

## Ngôn ngữ

| Ngôn ngữ | Tệp | Trạng thái |
|---|---|---|
| 한국어 (tiếng Hàn) | `01_adversarial_finance.html` | Bản gốc |
| Tiếng Việt | `01_adversarial_finance.vi.html` | Đã dịch |
| English | `01_adversarial_finance.en.html` | Mới có chỗ, chưa có tệp |
| 中文 | `01_adversarial_finance.zh.html` | Mới có chỗ |
| 日本語 | `01_adversarial_finance.ja.html` | Mới có chỗ |
| Oʻzbekcha | `01_adversarial_finance.uz.html` | Mới có chỗ |
| Русский | `01_adversarial_finance.ru.html` | Mới có chỗ |

- Ba cách đổi ngôn ngữ: ① hộp chọn **🌐** ở bên phải thanh menu trên, ② nút **🌐** ở góc phải dưới, ③ thêm `?lang=vi` vào cuối địa chỉ.
- Lựa chọn được ghi nhớ trong trình duyệt (khoá `fds01_lang`) và vị trí `#mục` được giữ nguyên khi chuyển trang.
- **Chỉ trang gốc tiếng Hàn tự chuyển ngôn ngữ**: nếu ngôn ngữ trình duyệt là tiếng Việt, trang sẽ mở bản tiếng Việt. Nếu tệp dịch chưa tồn tại (en, zh, ja, uz, ru), trang kiểm tra trước bằng `HEAD` rồi ở lại bản tiếng Hàn — không bao giờ tạo liên kết hỏng 404.
- Người vào thẳng địa chỉ bản dịch sẽ không bị tự chuyển, để liên kết đã chia sẻ mở đúng ngôn ngữ đó.

## Cấu trúc (một trang = 8 phần + 2 phụ lục)

| # | Phần | Nội dung | Có thể thao tác |
|---|---|---|---|
| 1 | Góc hài: lừa AI | Nguyên lý nhiễu đối kháng, gấu trúc → vượn, biển STOP | — |
| 2 | Rửa tiền bất hợp pháp | Ba bước: dò mô hình → small drop → rửa bằng thống kê | — |
| 3 | Mất cân bằng & tăng cường dữ liệu | Tỉ lệ 89,9 : 10,1, phê bình SMOTE | — |
| 4 | Bốn kiểu tấn công | Thao túng khối lượng, giá, giá trị, xu hướng | Đổi 3 dạng đường cong |
| 5 | Mô hình sụp đổ | Acc/Recall của SVM, RF, LR, LSTM | Clean / chèn 8,1% / lọc KS |
| 6 | Lọc bằng thống kê | Tỉ lệ chặn của KS, T, F | — |
| Đối đầu | Ruồi giấm vs Money-Robo | RF+KS 0,94 so với LSTM 0,00 | Nút kiểm chứng kết quả |
| Kết luận | Chiến lược phòng thủ | Đặt ensemble RF + bộ lọc KS lên trước | — |
| K | Chỉ mục tri thức | Tìm và lọc 10 khái niệm | Ô tìm kiếm, nút lọc |
| O | Gói dữ liệu | Trích xuất đồ thị tri thức, thư mục | ZIP / sao chép BibTeX / Turtle |

## Con số cốt lõi (thực đo trong bài báo)

| Chỉ số | Giá trị | Nguồn |
|---|---|---|
| Tỉ lệ chặn dữ liệu đối kháng của KS-test | **94,59%** | Hình 17, tr. 161 |
| Tỉ lệ chặn của T-test | 73,96% | Cùng mục |
| Tỉ lệ chặn của F-test | 0,00% | Cùng mục |
| Recall của LSTM (sau khi bị tấn công) | **0,00** | Bảng 6, tr. 160 |
| Recall của Random Forest | 0,94 → 0,98 | Bảng 6, tr. 160 |
| Mất cân bằng dữ liệu (bình thường:bất thường) | 89,9% : 10,1% | Ch. 3 |
| Tỉ lệ chèn dữ liệu đối kháng | 8,1% | Ch. 5 |

## Tệp

```
.
├── index.html                        Trang đầu (mục lục, vào bản Hàn / Việt)
├── 01_adversarial_finance.html       Bản gốc tiếng Hàn (~2,2 MB)
├── 01_adversarial_finance.vi.html    Bản tiếng Việt (~2,2 MB)
├── README.md                         Tài liệu này (tiếng Hàn + tiếng Việt)
├── INDEX.md                          Mục lục tài sản và các phần
├── og_01.png                         Ảnh xem trước khi chia sẻ 1200×630
├── thumb_01.png                      Ảnh thu nhỏ cho thẻ mục lục 600×400
├── bg_01.png                         Nền hero 1920×720
├── sc_01_hero.png                    Sân khấu hero 1200×800
├── cut_01_think.png                  Ảnh cắt "đám mây suy nghĩ" 960×540
├── cut_01_filter.png                 Ảnh cắt "bộ lọc thống kê" 960×540
└── sc_01_outro.png                   Ảnh kết 1200×800
```

Đưa thẳng các tệp vào **thư mục gốc** của kho là GitHub Pages chạy được ngay. Hình trong HTML đã được nhúng dạng `base64`; các tệp PNG ở trên là **bản gốc** để tái sử dụng, không dùng để hiển thị nên xoá đi trang vẫn chạy bình thường.

## Hình ảnh

| Tệp | Kích thước | Dùng ở | Nội dung |
|---|---|---|---|
| `bg_01.png` | 1920×720 | Nền hero | Phòng lab ban đêm: 45% bên trái là mảng tường trống để đặt tiêu đề, bên phải có tủ server, 3 màn hình, hộp phong bì niêm phong, sổ tay, thẻ dữ liệu |
| `sc_01_hero.png` | 1200×800 | Sân khấu hero | Khoảnh khắc một thẻ dữ liệu đeo mặt nạ lọt vào đường ống dữ liệu, đủ bốn nhân vật |
| `cut_01_think.png` | 960×540 | Phần 1 | Đám mây suy nghĩ của Tiến sĩ — điểm bất thường đeo mặt nạ ẩn trong phân phối chuẩn |
| `cut_01_filter.png` | 960×540 | Phần 6 | Thẻ bình thường đi qua lưới cong, thẻ ngụy trang bị giữ lại và rơi vào khay loại |
| `sc_01_outro.png` | 1200×800 | Kết luận | Sau phán quyết: Ruồi giấm thắng, robot nhận thua, Tiến sĩ gật đầu, Trợ lý vỗ tay |
| `og_01.png` | 1200×630 | Xem trước khi chia sẻ | Cổng ở giữa cùng bốn nhân vật, đọc rõ khi thu nhỏ |
| `thumb_01.png` | 600×400 | Thẻ trang đầu | Cắt 3:2 bên phải của `bg_01` |

Toàn bộ hình theo phong cách pixel art RPG 16-bit (viền đậm, 2–3 lớp sáng tối). Bốn nhân vật: **Tiến sĩ · Trợ lý · Nhà nghiên cứu Ruồi giấm · Money-Robo**. Ảnh đại diện trong bong bóng thoại được cắt 160×160 từ hình gốc.

## Dữ liệu và hình ảnh — đâu là số thật, đâu là minh hoạ

| Thành phần | Bản chất |
|---|---|
| Bảng (bốn kiểu tấn công, chỉ số theo mô hình, tỉ lệ chặn) | **Số thực đo** trong bài báo, chép nguyên |
| Bốn ô KPI ở hero, số trong phần kết luận | Số thực đo |
| Ba canvas (phân phối, cột, tỉ lệ chặn) | **Trực quan hoá vẽ lại trên trình duyệt** theo cùng thang với bài báo. Cột và tỉ lệ chặn cố định theo số của bài; đường cong phân phối là **đường minh hoạ** để giải thích hình dạng |
| Bốn tranh minh hoạ | **Mô hình minh hoạ** — không phải ảnh chụp nghiên cứu thật, nhân vật là thiết kế pixel art. Đồ thị trong tranh chỉ là hình khối trừu tượng, không có chữ hay số |
| Dữ liệu | Dữ liệu tick tổng hợp 10.000 bản ghi; không dùng dữ liệu giao dịch của người thật |

## Cách gọi thuật ngữ

- **Độ phủ (Recall)** — tỉ lệ giao dịch bất thường thật mà mô hình bắt được. Vì đây là chỉ số quyết định kết luận của trang, lần đầu xuất hiện luôn kèm tiếng Anh.
- **Dữ liệu đối kháng** — đầu vào bị biến đổi rất nhỏ để trông như bình thường hòng đánh lừa mô hình.
- **Tỉ lệ chặn** — phần trăm dữ liệu đối kháng bị bộ lọc kiểm định thống kê giữ lại.
- Số thập phân giữ nguyên như bản gốc (dấu phẩy thập phân theo cách viết tiếng Việt: 94,59%).

## Giấy phép

Trang và hình ảnh phát hành theo **CC BY-NC 4.0** (Ghi công – Phi thương mại 4.0 Quốc tế). Bạn được dùng tự do cho lớp học, bài giảng và nghiên cứu phi thương mại; dùng cho mục đích thương mại cần liên hệ riêng.

Mẫu ghi công:

```
Ahn Sangsun. (2024). Bảo mật mô hình phát hiện bất thường trong lĩnh vực tài chính:
giải pháp ứng phó dữ liệu đối kháng dựa trên thống kê. Mirae Sahoe, 15(3), 147–166.
https://doi.org/10.22987/jifso.2024.15.3.147
Trang giải thích: <địa chỉ kho> (CC BY-NC 4.0)
```

## Ghi chú kỹ thuật

- Một tệp HTML duy nhất, không thư viện ngoài, Canvas 2D + JavaScript thuần, hình nhúng base64.
- Có `aria-label` cho canvas, `aria-live` cho câu kết quả, tôn trọng `prefers-reduced-motion`.
- Bảng thuật ngữ và chỉ mục tri thức sinh ra từ một khối `<script type="application/json" id="kg-raw">`; muốn sửa thuật ngữ thì sửa cả khối đó và phần thân trang.
