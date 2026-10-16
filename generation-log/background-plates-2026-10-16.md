# 투명 캐릭터 합성용 배경판 — 2026-10-16

- 목적: 투명 배경의 전신 달리아를 자연스럽게 배치할 수 있는 해변·숲 배경 2장 제작.
- 참조 이미지: 없음. 캐릭터 이미지나 다른 배경을 입력으로 사용하지 않음.
- 도구/모델: 내장 이미지 생성 도구; 모델명 미상.
- 공통 구성: 세로 2:3, 서 있는 인물 눈높이, 중앙 아래쪽에 인물을 배치할 빈 전경, 글자·사람·동물 없음.

## 1. 맑은 해변

- 에셋: `../images/06_backgrounds/for_character/beach/2026-10-16-background-beach-center-clear.png`
- 검토: 모래사장이 중앙 아래쪽에 넓게 이어지고 바다 수평선은 위쪽 1/3 부근에 있다. 중앙 전경에 인물을 배치할 공간이 충분하다.
- 프롬프트:

  > Create a high-quality vertical portrait 2:3 background plate for compositing a full-body character cutout into it. Background only: absolutely no people, no animals, no characters, no silhouettes, no text, no signs, no logos, no props in the center. Scene: a calm sunny beach, viewed at natural standing eye level. Keep the central lower half of the image as a broad unobstructed area of gently textured dry sand where a full-body person could stand; preserve a believable flat ground plane and subtle soft contact-shadow area at the bottom center. Place the turquoise sea and clean horizon in the upper third, with soft blue sky and a few light clouds. Keep visual detail low in the center and edges softly scenic, with no strong object behind where a person's head or body would be. Warm clear afternoon daylight from upper left, natural perspective, soft anime background painting, restrained color and texture, peaceful summery mood. The scene must read as a clean environment plate designed to receive one separately supplied standing full-body character in the center foreground. No foreground objects crossing the central standing area, no people or implied figures.

## 2. 숲속 공터

- 에셋: `../images/06_backgrounds/for_character/forest/2026-10-16-background-forest-clearing.png`
- 검토: 좌우의 나무가 화면 가장자리를 잡고 중앙 숲길이 뒤로 이어진다. 낮은 중앙 전경은 비어 있어 전신 캐릭터와 발 접지점을 놓기 쉽다.
- 프롬프트:

  > Create a high-quality vertical portrait 2:3 background plate for compositing a full-body character cutout into it. Background only: absolutely no people, no animals, no characters, no silhouettes, no text, no signs, no logos, no props in the center. Scene: a quiet green forest clearing with a natural path and soft morning sunlight. Camera at natural standing eye level. Keep the central lower half broad, clear, and unobstructed, with a believable level patch of earth and short grass where a full-body person could stand; leave a subtle soft contact-shadow area at bottom center. Tree trunks frame the far left and far right edges, while the open clearing recedes into the distance; do not place a trunk or branch behind the central standing area. Gentle filtered sunbeams from upper left, calm sage and fern greens, soft depth in the distant trees, modest detail, original soft anime background painting. Designed as an environment plate for adding one separately supplied standing character in the center foreground. No figures, animals, objects, or strong visual clutter in the central area.

## 합성 메모

달리아를 중앙 전경에 배치하고 신발 밑창이 바닥면에 닿도록 크기와 위치를 맞춘다. 배경의 왼쪽 위 광원에 맞춰 인물의 명암과 접지 그림자를 조정하면 자연스럽다. 이 두 배경은 PNG로 생성했으며 프로젝트의 `.gitignore` 규칙에 따라 파일은 로컬에 두고 폴더·기록만 Git에 포함한다.
