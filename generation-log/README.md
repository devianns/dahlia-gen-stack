# 이미지 생성 기록

최종 에셋 하나마다 아래 항목을 기록한다. 선택되지 않은 시안이나 실패한 결과는 보존할 필요가 있을 때만 `drafts/` 등 별도 위치에 두고 사유를 적는다.

## 기록 양식

```markdown
## YYYY-MM-DD — 장면 이름

- 에셋: `../images/분류/하위분류/파일명.png`
- 목적/장면:
- 참조 이미지:
- 도구/모델: (확인된 정보만 기재, 모르면 미상)
- 탐구 변수: (그림체, 재료감, 구도, 포즈, 표정, 복장 등 이번에 바꾼 요소)
- 프롬프트: (실제 입력한 전체 프롬프트)
- 검토: 외형 일관성 / 해부학 / 장면 적합성 / 표현 방식 / 구도
- 결정: 채택 또는 보류와 이유
- 배운 점: (관찰한 사실과 가설을 구분하고, 다음 생성에 반영할 내용)
- 후속 작업:
```

각 생성 묶음의 상세 기록은 주제별 파일로 분리할 수 있다. 이 목록에는 묶음 요약과 상세 기록 링크를 둔다. 실제 입력 프롬프트와 채택/보류 결과를 추적하고, 중요한 발견은 `docs/visual-study.md`로 옮긴다.

## 2026-10-16 — 달빛 창가의 차 시간

- 에셋: `../images/01_situations/daily/moonlit_window/2026-10-16-moonlit-window-tea.png`
- 목적/장면: 프로젝트 첫 장면. 달빛 드는 방에서 머그를 들고 별빛을 바라보는 일상.
- 참조 이미지: 사용자가 제공한 DAHLIA💫 캐릭터 이미지(정체성 참조, 포즈 복제 아님).
- 도구/모델: 내장 이미지 생성 도구; 모델명 미상.
- 프롬프트:

  > Create a polished portrait full-body anime illustration of the same original character in Image 1, keeping her identity recognizable while changing her pose. She sits in a cozy bedroom by a moonlit window, holding a warm mug and looking at drifting star lights. Preserve signature features: long flowing pearl-white hair shaded icy blue and lavender, vivid cyan-blue eyes, pink star hair clip, cyan ribbon, delicate white feathered wings, white frilled dress with pale-blue ruffles and subtle gold embroidery. Quiet midnight cobalt sky, constellations, small warm lamp glow. Elegant luminous painterly anime style, graceful natural pose, age-appropriate modest styling, correct anatomy, no extra limbs. No text or watermark.

- 검토: 흰색/빙청색 긴 머리, 파란 눈, 분홍 별핀, 청록 리본, 흰 날개와 흰색 프릴 의상이 보인다. 창가의 차 시간이라는 장면이 명확하다. 손은 머그를 감싸 쥔 모습으로 표현됐다. 원본 참조의 일부 세부 의상·날개 형태와는 차이가 있을 수 있으므로 후속 생성에서 기준 외형을 계속 확인한다.
- 결정: 채택.
- 후속 작업: 다른 표정과 포즈, 야외 일상 및 판타지 장면으로 확장.

## 2026-10-16 — 별빛 천문대의 성도 제작자

- 에셋: `../images/03_fantasy/astral/observatory/2026-10-16-astral-observatory-cartographer.png`
- 목적/장면: 기존 차 장면과 다른 판타지 탐험 장면. 구름 위 천문대 정원에서 성도를 살피는 달리아.
- 분류: 판타지 > 천체 > 천문대. 보조 태그: 전신, 호기심, 판타지 여행 의상.
- 참조 이미지: 사용자가 제공한 DAHLIA💫 캐릭터 이미지(정체성 참조, 구도와 착장은 새로 구성).
- 도구/모델: 내장 이미지 생성 도구; 모델명 미상.
- 프롬프트:

  > Create an original vertical full-body anime illustration, clearly distinct from a cozy bedroom tea scene: DAHLIA💫 is an astral cartographer exploring a floating observatory garden among clouds at twilight. She wears a modest fantasy travel outfit: short pearl-white capelet over a layered pale-blue tunic dress, fitted sleeves, practical white boots, small gold star clasps, cyan sash and ribbon. Keep her signature very long flowing pearl-white hair with icy-blue and lavender shading, vivid cyan-blue eyes, small pink star hair clip, cyan ribbon accents, and broad soft white feathered wings. She carefully holds an open glowing celestial map while standing beside an antique brass telescope; tiny constellations arc overhead, floating stone paths and blue flowers in the distance. Dynamic but graceful standing pose, curious determined expression, full-body composition with clear silhouette. Luminous high-detail anime illustration, painterly cel shading, cool cobalt and indigo sky, pearl white, ice blue, lavender, restrained gold glow. Age-appropriate, non-sexualized, natural hands and anatomy, coherent wings. No text, lettering, logo, watermark, extra limbs, extra wings, other characters, or bedroom elements. Use Image 1 only to preserve character identity, not its exact composition or clothing.

- 검토: 긴 흰색/빙청색 머리, 청록빛 눈, 별 핀과 리본, 흰 날개가 유지됐다. 천문대·성도·망원경으로 판타지 상황이 구분되고, 흰색과 파란색에 금색 장식이 있는 여행 착장이 기존 팔레트에 맞는다. 성도를 든 손가락은 복잡해 보여 후속 확대 검토가 유용하다.
- 결정: 채택. 손의 세부 묘사는 완벽하지 않으므로 손 클로즈업 시안으로 재생성할 후보.
- 후속 작업: 표정 분류의 독립 시트와 일상 장면을 추가하고, 같은 장면의 포즈 변주를 축적.

## 2026-10-16 — 숲속의 조용한 아침

- 에셋: `../images/01_situations/daily/forest_clearing/2026-10-16-quiet-forest-casual-wear.png`
- 목적/장면: 화려한 판타지 연출을 줄인 일상 장면. 아침 숲속에서 야생화를 바라보며 쉬는 달리아.
- 분류: 상황 > 일상 > 숲속. 보조 태그: 차분함, 일상복, 앉은 포즈.
- 참조 이미지: 사용자가 제공한 DAHLIA💫 캐릭터 이미지(정체성 참조).
- 도구/모델: 내장 이미지 생성 도구; 모델명 미상.
- 프롬프트:

  > Create a gentle, understated anime illustration of DAHLIA💫 taking a quiet walk in a peaceful forest clearing in the morning. She wears simple modest everyday clothes: a soft ivory knit cardigan over a pale blue knee-length dress, comfortable light shoes, a small cyan ribbon and her familiar pink star hair clip. Preserve her long flowing pearl-white hair with subtle icy-blue shading, vivid cyan-blue eyes, and soft white feathered wings. Her wings are relaxed and partly folded. She pauses beside a mossy tree and looks calmly at a small patch of wildflowers, with a faint peaceful smile. Soft diffuse light through leaves, muted sage green and warm ivory palette, a few tiny natural details, shallow gentle atmosphere, no sparkling magic. Half-body to three-quarter composition, relaxed natural posture, quiet and intimate mood. Refined anime illustration with delicate linework and soft painterly shading. Age-appropriate, non-sexualized, natural anatomy and hands. Avoid dramatic lighting, ornate costume, dense decoration, glowing effects, stars in the background, text, logo, watermark, extra limbs, extra wings, or other characters. Keep the scene simple, calm, and soft.

- 검토: 숲의 녹색과 부드러운 아침빛, 가디건과 옅은 파란 원피스로 차분한 일상복 분위기를 표현했다. 흰 머리와 청록빛 눈, 분홍 별 장식, 흰 날개가 유지됐다. 인물이 크게 잡힌 구도라 배경의 숲은 흐릿하게 처리됐다.
- 결정: 채택.
- 후속 작업: 숲 배경을 더 넓게 보여 주는 전신 산책 장면을 별도 에셋으로 추가할 수 있음.

## 2026-10-16 — 전신 일상복과 환영 포즈

- 에셋: `../images/05_poses/standing/full_body/2026-10-16-full-body-casual-welcome.png`
- 목적/장면: 단순한 배경에서 의상과 전신 실루엣을 확인하는 캐릭터 레퍼런스 이미지.
- 분류: 포즈 > 서기 > 전신. 보조 태그: 일상복, 환영하는 손짓, 천사족/날개 설정.
- 참조 이미지: 사용자가 제공한 다른 캐릭터 이미지. 외형·색상·의상은 참조하지 않고 전신 구도, 선명한 렌더링, 손짓 포즈 방향만 참고.
- 도구/모델: 내장 이미지 생성 도구; 모델명 미상.
- 프롬프트:

  > Create a clean, polished full-body anime illustration of DAHLIA💫 standing alone, visible from the top of her head to the soles of both shoes. Keep her identity: long flowing pearl-white hair with subtle ice-blue and lavender shading, vivid cyan-blue eyes, small pink star hair clip, cyan ribbon, and large soft white feathered wings. Give her a friendly everyday pose inspired by the reference's welcoming gesture: one hand gently extended toward the viewer with an open relaxed palm, the other resting naturally by her side; balanced stance, both legs and shoes clearly visible, no extreme foreshortening. She wears a simple modest everyday outfit: pale blue blouse, soft ivory cardigan, navy knee-length pleated skirt, white ankle socks, and simple light-blue sneakers. Wings are visible behind her without hiding her silhouette. Refined anime character art with clean confident linework, restrained soft cel shading, clear readable shapes, subtle warm rim light. Use a plain very light cool-gray background with only a faint soft ground shadow; no scenery, no decorative effects, no stars in the background. Centered portrait composition with comfortable margin around the entire figure. Non-sexualized, age-appropriate, natural proportions, accurate hands, exactly two arms and two legs, two wings. No text, logo, watermark, extra characters, ornate costume, halo, extra limbs, cropped feet, or busy background.

- 검토: 머리부터 신발까지 전신이 프레임 안에 들어오며, 단순한 밝은 배경에서 날개와 일상복 실루엣이 분명하다. 뻗은 손 포즈가 친근한 인상을 준다. 손가락과 팔의 세부는 후속 시안에서 재검토할 수 있다.
- 결정: 채택.
- 후속 작업: 이 구도를 기준으로 정면·측면·뒷모습 의상 시트와 무표정/미소 표정 시트를 만들 수 있음.

## 2026-10-16 — 맑은 바닷가 전신 이미지 세트 (8장)

- 상세 기록 및 각 이미지에 입력한 전체 프롬프트: [`beach-set-2026-10-16.md`](beach-set-2026-10-16.md)
- 참조: 바로 앞서 확정한 달리아 전신 일상복 이미지를 정체성 참조로 사용.
- 도구/모델: 내장 이미지 생성 도구; 모델명 미상. 프롬프트별로 별도 생성 호출.
- 결과: 산책복, 얕은 물 놀이용 복장, 여름 원피스, 연 날리기, 아이스크림 산책, 조수 웅덩이 관찰, 자전거, 파라솔 아래 독서 등 서로 다른 전신 이미지 8장. 모두 맑은 날씨와 밝은 표정 중심.
- 결정: 8장 모두 채택. 손발과 의상 세부는 후속 에셋 생성 시 계속 검토.

## 2026-10-16 — 불꽃놀이·단독 무대·일상·표정 세트 (8장)

- 상세 기록 및 각 이미지에 입력한 전체 프롬프트: [`variety-set-2026-10-16.md`](variety-set-2026-10-16.md)
- 사용자 제공 이미지 정책: 사용자는 예시 이미지를 상황 이해용으로만 제공했고 재사용·표절을 금지했다. 어떤 첨부 이미지도 생성 도구 입력이나 스타일 참조로 전달하지 않았다.
- 생성 방식: 장면마다 독립된 프롬프트를 사용해 8회 생성. 불꽃놀이 2장, 단독 무대 2장, 일상 3장, 표정 시트 1장.
- 표현: 수채화·구아슈풍, 셀 셰이딩, 파스텔 라인아트 등 서로 다른 새 표현을 사용.
- 검토/결정: 달리아 단독 이미지로 8장 채택. 일부 장면은 요청한 내용에 맞춰 앉기/서기 등 포즈가 다르며, 모두 기존 캐릭터의 핵심 외형 단서를 유지.

## 2026-10-16 — 계절·여행·작업·판타지·휴식 장면 세트 (8장)

- 상세 기록 및 각 이미지의 전체 프롬프트와 검토: [`variety-set-2026-10-16.md`](variety-set-2026-10-16.md)
- 참조 이미지: 없음. 캐릭터 바이블과 공통 프롬프트를 텍스트 기준으로 사용.
- 도구/모델: 내장 이미지 생성 도구; 모델명 미상.
- 결과: 봄 정원, 가을 공원, 도서관 독서, 겨울 마을, 기차 여행, 공예 작업실, 빛나는 온실, 비 오는 날 창가 휴식.
- 검토/결정: 8장 채택. 온실 초안 하나는 의상 길이를 조정해 재생성했으며 보류 결과는 에셋 폴더에 저장하지 않음.
