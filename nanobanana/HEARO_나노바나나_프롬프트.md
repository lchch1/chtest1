# HEARO 소개 이미지 키트 (나노바나나 프로용)

`refs/` 폴더의 레퍼런스 10장과 아래 프롬프트 4종을 함께 씁니다. 프롬프트는 영어로 썼고(모델이 가장 잘 따르는 쪽), 이미지에 들어갈 **한글 문구는 따옴표 안에 그대로** 넣었습니다.

## 0. 시작 전에 알아둘 것

1. **앱 화면은 생성이 아니라 "복제"를 시키는 게 핵심입니다.** 이미지 생성 모델은 UI의 작은 글자와 아이콘을 자주 바꿉니다. 그래서 실제 화면 이미지를 레퍼런스로 올리고 "그대로 재현"하라고 적었습니다. 그래도 어긋나면 **5번(합성)** 방법이 가장 확실합니다.
2. **업로드 순서가 곧 번호입니다.** 프롬프트의 `Image 1, Image 2…`는 올린 순서입니다. 각 프롬프트 맨 위에 올릴 파일 순서를 적어 두었으니 그대로 올려 주세요.
3. **한글 문구는 꼭 눈으로 검수하세요.** 짧은 제목은 대체로 맞게 나오지만 받침이 바뀌는 일이 있습니다. 계속 틀리면 `텍스트 없는 버전` 문장으로 바꿔 만들고, 글자는 Figma/Canva에서 얹으세요. (웹 페이지와 같은 폰트: Black Han Sans + Noto Sans KR)
4. 이미지 크기는 **프롬프트에 쓰지 말고 앱의 비율/해상도 설정**에서 고르세요. 글자가 들어가면 2K 이상을 권합니다.
5. 모델 이름·참조 이미지 한도(제가 알기로 최대 14장, 고충실도 6장 안팎)는 바뀔 수 있으니 사용 중인 화면에서 확인해 주세요. 아래 프롬프트는 한 번에 4~5장만 씁니다.
6. 레퍼런스 화면은 **실기기 캡처가 아니라 앱의 레이아웃·이미지 파일로 다시 그린 것**입니다. 아이콘 원본이 작아서(60~170px) 확대하면 조금 부드럽게 보입니다. 에뮬레이터나 폰에서 직접 캡처한 화면이 있으면 그걸로 바꾸는 것이 더 좋습니다.

## 1. 레퍼런스 이미지

| 파일 | 내용 | 용도 |
|---|---|---|
| `01_app_main_home.png` | 메인 화면(홈 모드) | 기능 개요, 3컷 설명 |
| `02_app_alert_doorbell.png` | 초인종 소리 감지된 화면 | 히어로, 스토리 |
| `03_app_alert_baby_cry.png` | 아기 울음소리 감지된 화면 | 아기 울음 버전으로 바꿀 때 02 대신 |
| `04_app_sound_settings.png` | 소리 설정 화면(홈 모드) | 설정 기능을 보여 줄 때 |
| `05_app_chat.png` | 대화 화면 | 대화 기능을 보여 줄 때 |
| `06_watch_alerts.png` | 워치 알림 2종(왼쪽 초인종, 오른쪽 아기 울음) | 워치가 나오는 모든 이미지 |
| `07_logo_on_brand_blue.png` | HEARO 로고(흰색, 파란 바탕) | 로고를 그대로 쓰게 할 때 |
| `08_splash_full.png` | 앱 시작 화면 원본 | 분위기 참고(선택) |
| `09_palette_swatches.png` | 브랜드 색 견본(글자 없음) | 색 맞추기 |
| `10_icon_sheet.png` | 앱의 3D 아이콘 모음 | 아이콘 스타일 통일 |

## 2. 브랜드 색 (모든 프롬프트에 공통)

| 용도 | 색 |
|---|---|
| 브랜드 그라데이션 | 보라 `#7C60FF` → 선명한 파랑 `#3B64FE` → 연한 하늘 `#83A0FE` |
| 헤더 파랑 | `#5B6FFF` |
| 신호 노랑(소리·알림 표시 전용) | `#FFE500`, 연한 노랑 `#FFF598` |
| 짙은 남색(글자) | `#121A3A` |
| 바탕 | 흰색, `#F3F5FC`, 회색 `#EEEEEE` |

앱의 인상은 "차분하고 밝은 파랑 + 소리를 뜻하는 노란 신호"입니다. 노랑은 소리·알림에만 쓰도록 프롬프트에 못 박았습니다.

## 3. 프롬프트

### A. 히어로 이미지 (16:9, 2K 이상) — 웹/발표 표지용

**올릴 순서:** `02_app_alert_doorbell` → `06_watch_alerts` → `07_logo_on_brand_blue` → `09_palette_swatches`

```text
Create a 16:9 hero key visual for HEARO, a mobile app that turns sounds such as a doorbell or a crying baby into visual and vibration alerts for deaf and hard-of-hearing people.

Reference images, in upload order:
- Image 1: the EXACT phone screen UI showing the doorbell alert. Reproduce this screen faithfully on the phone in the scene: same layout, icons, colors, the white banner at the top, and the white circle with the bell and the Korean text "초인종 소리". Do not redesign, translate or simplify it.
- Image 2: the EXACT smartwatch alert. Use the LEFT watch face (the bell, doorbell alert) on the wrist smartwatch. Reproduce it faithfully.
- Image 3: the HEARO logo. Use it unchanged, small, in the top-left corner.
- Image 4: the brand color palette. Match these colors for the atmosphere and graphics.

Scene: a bright, modern apartment living room at early evening. A young adult (natural, relaxed and dignified, gender-neutral styling) sits on a sofa reading a book, calm and absorbed. On the coffee table in front of them a generic smartphone (no brand logos) stands at a slight angle with its screen showing Image 1. On their wrist, a round smartwatch shows Image 2. In the far background there is a front door with a small wall doorbell.

Make the invisible sound visible: soft concentric ring pulses in signal yellow (#FFE500 fading to #FFF598) radiate from the doorbell, travel across the room and land on the phone and the watch, so the sound visibly turns into the alert.

Light and color: large window with soft violet-to-blue dusk light (#7C60FF to #83A0FE), gentle bloom, clean airy feeling. Keep the rest of the palette to white, soft off-white (#F3F5FC) and deep navy (#121A3A).

Composition: person and devices in the left two-thirds, clean empty space in the right third for text. Camera 35mm, eye level, shallow depth of field, photographic realism with a clean, slightly stylized color grade.

Text, render exactly and nothing else: headline "들리지 않아도, 놓치지 않게." in a bold, friendly Korean sans-serif, deep navy #121A3A, in the empty right-hand space. Small tagline under it: "소리를 눈으로, 손끝으로". No other text, no watermark, no extra logos.

Tone: reassuring and empowering, never pitying. Avoid sad or dramatic expressions, avoid close-ups of hearing aids, avoid any real-world brand logos on the devices.
```

**텍스트 없는 버전:** 위 프롬프트에서 `Text, render exactly…` 단락 전체를 아래 한 줄로 바꾸세요.
```text
Do not render any text except the HEARO logo from Image 3. Keep the right third clean and empty for text that will be added later.
```

---

### B. 3컷 설명 이미지 (4:5, 2K) — 인스타그램/소개서용

**올릴 순서:** `01_app_main_home` → `02_app_alert_doorbell` → `06_watch_alerts` → `10_icon_sheet` → `09_palette_swatches`

```text
Create a 4:5 vertical explainer illustration made of three stacked panels that read top to bottom as a story. One consistent style: soft glossy 3D illustration that matches the icon style of Image 4 (blue gradients, a pastel yellow accent, rounded forms, gentle shadows), on a clean off-white (#F3F5FC) background with generous spacing. Thin rounded arrows in brand blue (#3B64FE) connect the panels.

Reference images, in upload order:
- Image 1: the EXACT phone screen of the app's main screen. Reproduce faithfully.
- Image 2: the EXACT phone screen with the doorbell alert. Reproduce faithfully.
- Image 3: the EXACT smartwatch alerts. Use the LEFT face (bell). Reproduce faithfully.
- Image 4: the app's icon style sheet. Match the 3D style, gradients and rounded shapes of these icons for all objects.
- Image 5: the brand color palette.

Panel 1, caption "초인종이 울려요": a front door with a wall doorbell. Concentric ring pulses in signal yellow (#FFE500 to #FFF598) radiate from the doorbell. No people.

Panel 2, caption "HEARO가 소리를 들어요": a smartphone showing Image 1, with a small floating blue sound-wave equalizer above it that is turning into a bell icon in the style of Image 4.

Panel 3, caption "화면, 진동, 워치로 알려줘요": the smartphone now showing Image 2, beside a round smartwatch showing Image 3, with small curved vibration lines around both devices.

Captions are in a bold friendly Korean sans-serif, deep navy #121A3A, centered under each panel. Render the three captions exactly as written. No other text, no numbers, no logos on the devices, no watermark.
```

**텍스트 없는 버전:** `Captions are in…` 단락을 `Render no text at all; leave a clean band under each panel for captions added later.` 로 바꾸세요.

---

### C. 주요 기능 한눈에 (16:9, 2K 이상) — 기능 소개 슬라이드용

**올릴 순서:** `01_app_main_home` → `06_watch_alerts` → `10_icon_sheet` → `07_logo_on_brand_blue` → `09_palette_swatches`

```text
Create a 16:9 product overview image for the app HEARO.

Reference images, in upload order:
- Image 1: the EXACT phone screen (main screen). Reproduce faithfully on the central phone.
- Image 2: the EXACT smartwatch alerts. Use the LEFT face. Reproduce faithfully.
- Image 3: the app's 3D icon sheet. Take the bell, the chat bubble, the whistle and the word-tag from it and keep their exact style.
- Image 4: the HEARO logo, unchanged, small, top-left.
- Image 5: the brand color palette.

Layout: a smartphone in the center, tilted about 8 degrees, showing Image 1. Around it, four floating rounded white cards with soft shadows, each holding one icon from Image 3 and a short Korean label, exactly as written: top-left "소리 감지" with the bell and small yellow pulse rings; top-right "대화" with the chat bubble; bottom-left "호출" with the whistle; bottom-right "단어 인식" with the word tag. A round smartwatch overlaps the bottom-right corner of the phone, showing Image 2.

Background: the brand gradient from violet #7C60FF at the top-left through vivid blue #3B64FE to periwinkle #83A0FE at the bottom-right, with a soft glow behind the phone. Signal yellow (#FFE500, #FFF598) appears only in the pulse rings and small accents.

Headline at the top center, exactly: "소리가 보이는 앱". White, bold, friendly Korean sans-serif. No other text, no watermark, no brand logos on devices.
```

**텍스트 없는 버전:** 카드 라벨과 `Headline…` 문장을 지우고 `Render no text except the HEARO logo.` 를 넣으세요. 아이콘만으로도 뜻이 전해집니다.

---

### D. 세로 히어로 (9:16, 2K 이상) — 스토리/앱스토어 첫 장

**올릴 순서:** `02_app_alert_doorbell` → `06_watch_alerts` → `07_logo_on_brand_blue` → `09_palette_swatches`

```text
Create a 9:16 vertical hero image for the app HEARO.

Reference images, in upload order:
- Image 1: the EXACT phone screen with the doorbell alert. Reproduce faithfully on the phone.
- Image 2: the EXACT smartwatch alerts. Use the LEFT face. Reproduce faithfully.
- Image 3: the HEARO logo, unchanged.
- Image 4: the brand color palette.

Scene: a large smartphone fills the lower two-thirds of the frame, floating and tilted slightly, showing Image 1. A round smartwatch overlaps its bottom-left corner, showing Image 2. From the phone's top banner, concentric ring pulses in signal yellow (#FFE500 fading to #FFF598) expand outward like a sound wave. Soft light streaks and a gentle glow. No people, no hands.

Background: the exact brand gradient from violet #7C60FF at the top through vivid blue #3B64FE to periwinkle #83A0FE at the bottom, smooth and clean.

Top area: the HEARO logo from Image 3 (unchanged), and below it the headline in two lines, exactly: "들리지 않아도,"
"놓치지 않게." White, bold, friendly Korean sans-serif, left-aligned. No other text, no watermark, no brand logos on devices.
```

**아기 울음 버전:** `02_app_alert_doorbell` 대신 `03_app_alert_baby_cry`를 올리고, 프롬프트의 `doorbell alert`를 `crying-baby alert`로 바꾸세요. 워치는 `the LEFT face`를 `the RIGHT face`로 바꿉니다.

## 4. 결과가 마음에 안 들 때 (이어서 붙여 쓰는 수정 문장)

생성된 이미지를 그대로 둔 채 아래 중 필요한 것만 이어서 입력하세요.

- **화면이 달라졌을 때**
  `Keep everything else exactly the same. Replace the phone screen content with an exact, faithful reproduction of Image 1 from the first message: same layout, icons, colors and Korean text. Do not invent new UI.`
- **한글이 틀렸을 때**
  `Keep the image identical. Only fix the headline so it reads exactly "들리지 않아도, 놓치지 않게." Check every syllable.`
- **색이 브랜드와 다를 때**
  `Keep the composition. Shift the blue background to the brand gradient: violet #7C60FF at the top, vivid blue #3B64FE, periwinkle #83A0FE at the bottom. Keep yellow only on the sound ring pulses.`
- **불필요한 글자/로고가 생겼을 때**
  `Remove all text, logos and watermarks except the HEARO logo. Keep everything else unchanged.`
- **사람 분위기를 바꾸고 싶을 때**
  `Keep the scene. Change the person to <나이/분위기>, calm and dignified, still looking relaxed. No pitying or dramatic expression.`

## 5. 앱 화면을 100% 정확하게 만들고 싶다면 (합성)

생성 모델은 화면 속 작은 글자를 완벽히 지키지 못할 수 있습니다. 가장 확실한 방법은 **화면을 비워서 만들고 진짜 캡처를 붙이는 것**입니다.

1. 위 프롬프트의 `showing Image 1`(또는 `Image 2`) 부분을 `with its screen filled with a flat solid #3B64FE color, no UI at all` 로 바꿔 생성합니다. 워치도 같게 `flat solid white` 로 바꿉니다.
2. Figma/Photoshop/Canva에서 그 파란(흰) 영역에 `01`·`02`·`06` 이미지를 올리고 기기 기울기에 맞춰 변형(원근)합니다.
3. 가능하면 레퍼런스 대신 에뮬레이터에서 직접 캡처한 고해상도 화면을 쓰세요.

## 6. 사용 팁

- 같은 프롬프트로 **4장씩 여러 번** 뽑고 가장 좋은 한 장을 골라 4번의 수정 문장으로 다듬는 편이 빠릅니다.
- 문구(제목, 태그라인)는 제가 지은 초안입니다. `소리를 눈으로, 손끝으로`, `소리가 보이는 앱`은 마음대로 바꾸세요. 바꿀 때는 따옴표 안만 고치면 됩니다.
- 앱이 아직 지원하지 않는 소리(화재 경보 등)를 이미지에 그리지 마세요. 지금 감지하는 소리는 **초인종과 아기 울음소리** 둘뿐입니다.
- 사람을 그릴 때는 장애를 "불쌍함"으로 연출하지 않도록 프롬프트에 `never pitying`을 넣어 두었습니다. 결과물에서 그런 느낌이 나면 4번의 마지막 문장으로 고치세요.
