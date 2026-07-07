# 아트 생성 프롬프트 (GPT / 이미지 생성 AI용)

레퍼런스: **"미송자의 노래" 스타일** — 정교한 손그림 도트(픽셀) 판타지 RPG.
따뜻하고 채도 있는 팔레트, 또렷한 외곽선, 부드러운 셰이딩.

게임 배경: **탑다운 그리드 타워디펜스**. 어두운 돌바닥 던전 위에서 청록빛 마법 코어를 지키는 게임.
아래 프롬프트는 각 에셋을 **투명 배경 단일 스프라이트**로 만드는 용도입니다.

> 공통 접미 프롬프트(모든 캐릭터/오브젝트에 붙이기):
> `detailed pixel art, hand-crafted dot art RPG style, crisp outline, soft shaded, high fantasy, single sprite centered, transparent background, front / slight top-down view, no text, no border, no grid`
>
> 저장: **PNG (투명 배경)**, 정사각 캔버스 권장. 캐릭터는 여백 최소화·가운데 정렬.

---

## 적 (enemies)

### 1) enemy_grunt.png — 정령 (기본)
```
A small floating fantasy spirit creature, rounded body, glowing lavender-violet color (#CBC2FF) with pale highlights, two tiny glowing eyes, wisp-like lower body, gentle magical aura. Cute but eerie. detailed pixel art, hand-crafted dot art RPG style, crisp outline, soft shaded, single sprite centered, transparent background, front view, no text.
```

### 2) enemy_runner.png — 돌격병 (빠름)
```
A fast agile fantasy scout/charger creature, lean and dynamic, warm orange body (#F79A3C) with cream highlights, forward-leaning pose suggesting speed, small sharp limbs, motion-ready silhouette. detailed pixel art, hand-crafted dot art RPG style, crisp outline, soft shaded, single sprite centered, transparent background, 3/4 front view, no text.
```

### 3) enemy_swarm.png — 군체 (소형·다수)
```
A tiny swarming fantasy critter, small round body, vivid green color (#3ECB84) with light green highlights, big simple eyes, many-legged or insectoid feel, reads clearly at small size. detailed pixel art, hand-crafted dot art RPG style, crisp outline, soft shaded, single sprite centered, transparent background, front view, no text.
```

### 4) enemy_breaker.png — 파괴자 (벽 공략, 대형)
```
A heavy bulky fantasy brute that smashes walls, thick armored body, crimson-red color (#EF5A57) with golden accents (#FFD36B), oversized fists or ram-like head, menacing and sturdy, larger than other enemies. detailed pixel art, hand-crafted dot art RPG style, crisp outline, soft shaded, single sprite centered, transparent background, front view, no text.
```

---

## 오브젝트 (objects)

### 5) core.png — 방어 코어 (크리스탈)
```
A glowing magical defense crystal core, floating teal-cyan gemstone (#5fd6c0) with bright white inner glow, faceted crystalline shape, radiant energy, precious and central. detailed pixel art, hand-crafted dot art RPG style, crisp outline, soft shaded, single sprite centered, transparent background, front view, no text.
```

### 6) tower_gem.png — 타워 젬 (성벽 포탑)
```
A small faceted teal-cyan magic gem (#5fd6c0) with white sparkle highlight, mounted turret crystal, subtle glow, compact. detailed pixel art, hand-crafted dot art RPG style, crisp outline, soft shaded, single sprite centered, transparent background, front view, no text.
```

---

## 바닥 타일 (floor tiles) — 선택

바닥은 34×34px(또는 배수 68×68) **정사각·불투명**, 상하좌우 이음매 없이 **타일링** 되도록.

### 7) floor_a.png — 바닥 타일 A
```
A seamless tileable dark stone dungeon floor tile, dark blue-gray slate (#25324f), subtle cracks and specks, faint moss, top-down view, muted, no strong highlights so characters pop. seamless tiling texture, pixel art, no text, no border.
```

### 8) floor_b.png — 바닥 타일 B (교차용, A보다 살짝 밝게)
```
A seamless tileable dark stone dungeon floor tile, slightly lighter blue-gray slate (#2c3c5e), subtle cracks and faint teal magic rune specks, top-down view, muted. Must tile seamlessly with floor_a. seamless tiling texture, pixel art, no text, no border.
```

---

## 사용 순서
1. 위 프롬프트로 이미지 생성 → 배경 투명 PNG로 저장(필요 시 배경 제거)
2. `assets/` 폴더에 정해진 파일명으로 저장 (규칙은 `assets/README.md`)
3. `block_maze_td_v4.html` 브라우저 새로고침 → 자동 반영

**한 번에 다 만들 필요 없습니다.** 만든 것부터 넣으면 그 부분만 교체되고 나머지는 도트 아트로 유지됩니다.
