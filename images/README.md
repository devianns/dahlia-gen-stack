# 이미지 에셋 라이브러리

모든 채택 이미지는 이 폴더 아래 한 경로에 저장합니다. 폴더 이름은 영어 소문자와 숫자 접두사로 고정해 정렬을 유지하고, 기록과 설명은 한국어로 작성합니다.

PNG/JPEG/WebP 등 래스터 이미지 파일은 용량 때문에 `.gitignore` 처리되어 로컬에만 남습니다. 이 폴더의 분류 안내, `.gitkeep`, 생성 프롬프트, 메타데이터와 기록은 Git에 포함합니다. 저장소를 새로 받은 작업자는 이미지 파일을 별도로 전달받거나 생성 원본 위치에서 가져와야 합니다.

`/images`는 생성 에셋의 루트이며 Git에서 항상 유지합니다. **새 하위 폴더에는 즉시 `.gitkeep`을 만들고, 기존 `.gitkeep`은 이미지가 없어도 삭제하지 않습니다.** 이 규칙으로 이미지 파일을 업로드하지 않아도 분류 폴더 구조 전체가 저장소에 남습니다.

## 폴더 트리

```text
images/
├── 01_situations/          # 장면의 주된 상황
│   ├── daily/              # 차, 독서, 산책, 창가 등 일상
│   ├── seasonal/           # 봄·여름·가을·겨울
│   ├── travel/             # 이동과 여행
│   ├── celebration/        # 축제와 기념일
│   ├── rest/               # 휴식과 수면
│   └── work/               # 공부, 만들기, 연습
├── 02_expressions/         # 표정이 핵심인 이미지·표정 시트
│   ├── joy/ calm/ surprise/
│   ├── sadness/ shy/ sleepy/ anger/
├── 03_fantasy/             # 현실 일상과 구별되는 판타지 배경/사건
│   ├── astral/             # 별, 달, 천문대, 우주
│   ├── magic/              # 주문과 마법 현상
│   ├── adventure/          # 탐험과 퀘스트
│   ├── mythic/             # 신화적 장소와 존재
│   └── royal/              # 궁정, 의식, 왕실풍 장면
├── 04_outfits/             # 의상 디자인이 중심인 시트와 착장 비교
│   ├── everyday/ fantasy/ seasonal/ formal/
└── 05_poses/               # 포즈 시트와 동작 비교
    ├── standing/           # 전신 서 있는 구도 포함
    ├── sitting/ action/ portrait/
```

`daily/moonlit_window/`와 `fantasy/astral/observatory/`처럼 장면이 축적되면 하위 폴더를 추가합니다. 표정이나 착장 한 가지가 이미지의 주된 목적이면 각각 `02_expressions/` 또는 `04_outfits/`를 우선합니다. 한 이미지가 여러 특성을 가지더라도 복제하지 말고 가장 중요한 목적의 경로 하나를 정한 뒤 다른 특성은 생성 로그의 보조 태그에 적습니다.

## 파일과 검토

- 권장 형식: PNG. 파일명은 `YYYY-MM-DD-짧은-장면-이름.png`.
- 같은 날짜에 같은 장면을 재생성하면 기존 파일을 덮어쓰지 말고 `-v2`, `-v3`를 붙입니다.
- 에셋이 있는 분류 폴더도 이미지가 Git에서 제외되므로 `.gitkeep`으로 Git에 유지합니다.
- 검토 전 시안은 이 라이브러리에 넣지 않습니다. 채택 이미지는 파일, 분류 위치, 전체 프롬프트, 검토 메모를 `generation-log/README.md`에 함께 기록합니다.
- 생성 도구가 내보낸 원본 파일은 작업 환경에 보존하고 프로젝트에 넣을 채택본을 복사합니다. 이미지 출처와 도구/모델 정보를 알 수 있는 범위에서 기록합니다.

## 현재 에셋

- `01_situations/daily/moonlit_window/2026-10-16-moonlit-window-tea.png` — 달빛 창가의 차 시간
- `01_situations/daily/forest_clearing/2026-10-16-quiet-forest-casual-wear.png` — 숲속의 조용한 아침, 편안한 일상복
- `03_fantasy/astral/observatory/2026-10-16-astral-observatory-cartographer.png` — 구름 위 천문대의 성도 제작자
- `05_poses/standing/full_body/2026-10-16-full-body-casual-welcome.png` — 깔끔한 배경의 전신 일상복과 환영 포즈
- `01_situations/travel/beach/` — 맑은 날씨의 바닷가 전신 이미지 8종
  - `2026-10-16-beach-promenade.png` — 산책로와 밀짚모자
  - `2026-10-16-shallow-water-fun.png` — 얕은 물에서 파도 맞이
  - `2026-10-16-seaside-summer-dress.png` — 여름 원피스와 수건 바구니
  - `2026-10-16-beach-kite-walk.png` — 바닷바람과 연 날리기
  - `2026-10-16-beach-ice-cream-walk.png` — 해변 산책로의 아이스크림
  - `2026-10-16-tide-pool-discovery.png` — 조수 웅덩이 구경
  - `2026-10-16-seaside-bicycle.png` — 해변 자전거 산책
  - `2026-10-16-parasol-reading.png` — 파라솔 아래 독서
- `01_situations/celebration/fireworks/2026-10-16-fireworks-yukata-watch.png` — 유카타를 입고 강가 불꽃놀이를 보는 달리아
- `01_situations/celebration/fireworks/2026-10-16-fireworks-hilltop-fan.png` — 언덕에서 부채를 들고 불꽃놀이를 보는 달리아
- `01_situations/work/solo_stage/2026-10-16-solo-stage-performance.png` — 달리아의 단독 야외 무대 공연
- `01_situations/work/rehearsal/2026-10-16-solo-stage-rehearsal.png` — 단독 무대 리허설
- `01_situations/daily/cafe/2026-10-16-morning-cafe-tea.png` — 아침 카페의 차 한잔
- `01_situations/daily/home_baking/2026-10-16-star-cookie-baking.png` — 별 모양 쿠키 굽기
- `01_situations/daily/rainy_walk/2026-10-16-after-rain-park-walk.png` — 비가 그친 공원 산책
- `02_expressions/variety/2026-10-16-six-expressions-sheet.png` — 기쁨·차분함·놀람·수줍음·졸림·결심 표정
