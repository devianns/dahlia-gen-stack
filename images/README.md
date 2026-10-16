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
├── 05_poses/               # 포즈 시트와 동작 비교
    ├── standing/           # 전신 서 있는 구도 포함
    ├── sitting/ action/ portrait/
└── 06_backgrounds/         # 투명 캐릭터를 합성하기 위한 배경판
    └── for_character/      # 인물 배치 공간이 비어 있는 환경 배경
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
- `01_situations/seasonal/spring_garden/2026-10-16-spring-garden-flower-basket.png` — 봄 정원에서 꽃바구니에 리본을 묶는 달리아
- `01_situations/seasonal/autumn_park/2026-10-16-autumn-park-lantern.png` — 낙엽 지는 공원에서 등불을 든 산책
- `01_situations/seasonal/winter_village/2026-10-16-winter-village-lantern.png` — 눈 내리는 마을의 등불 산책
- `01_situations/work/library/2026-10-16-library-reading.png` — 도서관에서 책을 읽는 모습
- `01_situations/work/craft_studio/2026-10-16-craft-studio-star-ornament.png` — 별 모양 도자 장식을 채색하는 작업실 장면
- `01_situations/travel/train/2026-10-16-train-window-journey.png` — 기차 창가에서 산과 구름을 바라보는 여행
- `03_fantasy/magic/conservatory/2026-10-16-luminous-conservatory.png` — 빛나는 온실에서 푸른 꽃을 살피는 판타지 장면
- `01_situations/rest/rainy_window/2026-10-16-rainy-window-reading.png` — 비 오는 오후 창가에서 쉬는 모습
- `01_situations/daily/flower_shop/2026-10-16-wingless-flower-shop.png` — 날개 없는 달리아의 꽃가게 작업
- `01_situations/daily/cafe/2026-10-16-wingless-cafe-tea.png` — 날개 없는 달리아가 카페에서 차를 마시며 웃는 장면
- `01_situations/daily/rainy_city/2026-10-16-wingless-rainy-city-walk.png` — 우산을 쓰고 빗속을 걷는 날개 없는 달리아
- `01_situations/seasonal/autumn_leaf/2026-10-16-wingless-autumn-leaf.png` — 가을 낙엽을 살펴보는 날개 없는 달리아
- `01_situations/seasonal/ice_skating/2026-10-16-wingless-ice-skating.png` — 빈 링크장에서 스케이트를 타는 날개 없는 달리아
- `03_fantasy/mythic/moonlit_garden/2026-10-16-wingless-moonlit-garden.png` — 달빛 정원의 별꽃을 살피는 장면
- `03_fantasy/magic/workshop/2026-10-16-wingless-potion-workshop.png` — 마법 작업실에서 물약을 만드는 장면
- `02_expressions/wingless_variety/2026-10-16-wingless-six-expressions.png` — 날개 없는 달리아의 여섯 표정 시트
- `05_poses/action/wingless_dance/2026-10-16-wingless-solo-dance.png` — 연습실의 날개 없는 단독 춤 동작
- `01_situations/rest/rooftop_night/2026-10-16-wingless-rooftop-rest.png` — 옥상에서 달을 바라보며 쉬는 장면
- `01_situations/celebration/night_market/2026-10-16-wingless-canal-lantern-market.png` — 운하 야시장에서 등불을 물에 띄우는 날개 없는 달리아
- `01_situations/travel/aquarium_tunnel/2026-10-16-wingless-underwater-aquarium-tunnel.png` — 수족관 유리 터널에서 물고기 떼를 올려다보는 장면
- `03_fantasy/adventure/clocktower/2026-10-16-wingless-clocktower-mechanism.png` — 거대한 시계탑에서 별 모양 기어를 움직이는 장면
- `01_situations/daily/laundromat/2026-10-16-wingless-retro-laundromat.png` — 심야 코인 세탁소에서 수건을 개는 장면
- `01_situations/travel/mountain_cable_car/2026-10-16-wingless-mountain-cable-car.png` — 산악 케이블카에서 지도를 보며 풍경을 감상
- `01_situations/daily/natural_history_museum/2026-10-16-wingless-dinosaur-museum.png` — 자연사 박물관의 공룡 화석을 올려다보는 장면
- `01_situations/daily/retro_arcade/2026-10-16-wingless-retro-arcade.png` — 레트로 오락실에서 리듬 게임을 하는 장면
- `01_situations/seasonal/sunflower_harvest/2026-10-16-wingless-sunflower-harvest.png` — 해바라기 수확철의 꽃바구니와 들판
- `01_situations/work/cinema_projection/2026-10-16-wingless-cinema-projection.png` — 오래된 영화관 영사실에서 필름을 끼우는 장면
- `03_fantasy/adventure/cloud_canyon/2026-10-16-wingless-cloud-canyon-crossing.png` — 구름 협곡 회랑을 건너며 풍경을 바라보는 장면
- `01_situations/travel/night_ferry/2026-10-16-wingless-night-ferry-map.png` — 야간 페리 객실에서 항로 지도를 읽는 모습
- `05_poses/action/indoor_climbing/2026-10-16-wingless-indoor-climbing.png` — 안전 하네스를 착용하고 실내 클라이밍을 하는 장면
- `01_situations/travel/polar_station/2026-10-16-wingless-polar-weather-station.png` — 오로라 아래 극지 기상 장비를 확인하는 모습
- `01_situations/work/science_fair/2026-10-16-wingless-kinetic-science-fair.png` — 달·별 기어 모형을 소개하는 과학 전시
- `01_situations/travel/botanical_station/2026-10-16-wingless-botanical-train-station.png` — 유리 지붕 기차역의 감귤나무를 살피는 장면
- `05_poses/standing/full_body/wingless/2026-10-16-wing-off-full-body-transparent.png` — 투명 배경, 잘림 없는 날개 OFF 전신 캐릭터 이미지
- `05_poses/standing/full_body/wingless/casual/2026-10-16-wing-off-casual-tshirt-shorts.png` — 흰 티셔츠와 파란 반바지, 인사 포즈
- `05_poses/standing/full_body/wingless/casual/2026-10-16-wing-off-casual-cardigan-skirt.png` — 블라우스·가디건과 무릎 길이 스커트, 토트백
- `05_poses/standing/full_body/wingless/casual/2026-10-16-wing-off-casual-overalls.png` — 줄무늬 티셔츠와 데님 오버롤
- `04_outfits/everyday/no_wings/2026-10-16-everyday-no-wings-full-body.png` — 실제 투명 배경, 가디건과 무릎 길이 스커트의 날개 OFF 전신 컷아웃
- `06_backgrounds/for_character/beach/2026-10-16-background-beach-center-clear.png` — 중앙 전경을 비워 둔 맑은 해변 배경
- `06_backgrounds/for_character/forest/2026-10-16-background-forest-clearing.png` — 중앙에 인물이 설 자리를 둔 숲속 공터 배경

합성할 때 캐릭터 발이 닿는 지점을 배경의 전경 바닥면에 맞추고, 광원 방향과 색온도를 배경에 맞춥니다. 이 배경 두 장은 중앙 전경을 비워 두고 인물과 접지 그림자를 얹을 수 있도록 구성했습니다.
