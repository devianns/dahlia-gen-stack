# 날개 OFF 가디건 전신 컷아웃 — 2026-10-16

- 에셋: `../images/04_outfits/everyday/no_wings/2026-10-16-everyday-no-wings-full-body.png`
- 목적: 날개 없는 일상복 변형을 배경 합성에 활용할 수 있는 전신 투명 PNG로 제작.
- 참조 이미지: 없음. 캐릭터 외형은 텍스트로 지정.
- 도구/모델: 내장 이미지 생성 도구; 모델명 미상.
- 탐구 변수: wings-OFF, 알파 투명 배경, 머리끝부터 신발까지 전신, 손인사, 가디건과 스커트.
- 프롬프트:

  > Use case: character-art. Asset type: transparent full-body character cutout for the DAHLIA💫 project. Generate a single original anime character from text description only, with no reference images. DAHLIA💫 has long flowing pearl-white hair with soft ice-blue and lavender shading, vivid cyan-blue eyes, a small pink star-shaped hair clip and a pale cyan-blue ribbon. She is shown in a wings-OFF everyday variant: a completely ordinary humanlike silhouette with NO wings, NO feathers anywhere, NO halo, NO wing-shaped accessories, and no wing shadow. Her daily outfit is modest and simple: a pale-blue knit cardigan over an ivory blouse, a navy calf-length pleated skirt, white ankle socks and clean light-blue sneakers. She stands in a relaxed friendly pose with one hand giving a small wave and the other holding a simple canvas tote bag; gentle cheerful expression, looking toward the viewer. Full-body portrait, entire hair silhouette, both arms and hands, both legs, socks, and both shoes visible, centered with generous clear transparent padding above her head and below her feet and around both sides. Keep the character fully inside the frame, do not crop any part. Clean polished anime linework, soft restrained cel shading, readable silhouette, minimal small star motif only on the hair clip. Actual transparent background with alpha, not a checkerboard or white background. No scenery, ground plane, cast shadow, text, logo, watermark, extra people, extra limbs, feathers, wings, halo, or cropping. Age-appropriate, non-sexualized, natural anatomy.

- 검토: 이미지 크기 1024×1536, PNG 색상 형식 RGBA. 네 모서리 및 위·아래 경계 중앙 픽셀의 알파값은 0으로 실제 투명함을 확인했다. 머리카락 끝, 양손, 양다리, 신발 모두 캔버스 안에 있다. 흰 머리와 빙청색 음영, 청록빛 눈, 분홍 별핀, 청록 리본이 보이며 날개·깃털은 없다.
- 결정: 채택.
- 배운 점: 투명 배경은 생성 요청만으로 판단하지 않고 RGBA 여부와 가장자리 알파를 확인한다. 전신 컷아웃은 머리 위와 발 아래 여백을 프롬프트에 함께 명시하는 편이 유용하다.
