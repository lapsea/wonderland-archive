# 《奇境档案馆》阶段二：逐图 Prompt 清单

**使用方式**：每张图直接复制 Prompt 到 AI 生图工具。清单按生产顺序排列，同一批次内可以并行生成。
**输出目录**：所有图片输出到 `demo/public/assets/` 对应子目录。
**路径来源**：[demo/src/assets/manifest.ts](../demo/src/assets/manifest.ts)。
**风格依据**：[docs/04-美术资产清单与风格规范.md](04-美术资产清单与风格规范.md)。

---

## 全局负向 Prompt（每张图必加）

```
modern, flat vector, cartoon, disney, tim burton, anime, 3d render, plastic, neon, glossy, photo, corporate, minimal, geometric, digital art smooth, clean white background
```

---

# 第一批：封面与地图（演示前10秒定成败）

---

## 1. 封面河岸全景

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/scenes/cover-riverbank.jpg` |
| **尺寸** | 2560×1440（16:9） |
| **正向 Prompt** | Oil painting storybook illustration of an afternoon riverbank, a massive ancient oak tree on the right side with a dark glowing rabbit-hole opening at its base emitting warm golden light. Soft green grassy riverbank on the left. Misty particles floating in the air. Dreamy pastoral landscape. Hand-painted gouache watercolor textures, soft painterly brushstrokes, aged parchment tones, warm nostalgic lighting, gentle whimsical storybook mood. Faded antique paper border with distressed edges. |
| **补充叙事引导** | "一本旧手账翻开的第一页——河岸的午后，树洞在发光。" |

---

## 2. 地图底图

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/scenes/map-base.jpg` |
| **尺寸** | 2560×1440（16:9） |
| **正向 Prompt** | A worn parchment map scroll unrolled on a wooden desk, hand-drawn wonderland-style map with 8 whimsical landmark icons scattered across the scroll connected by dashed ink paths — a rabbit-hole, a small hall, a teardrop pond, mushroom forest, a long tea table, a palace, croquet grounds, and a courtroom. Compass rose in corner, sea-monster marginalia, tattered deckled edges, warm sepia and faded ink tones, water stains and foxing marks, aged paper creases. Tea-stained paper texture, antique cartography aesthetic. |
| **补充叙事引导** | "书房墙上挂着的旧地图，纸已经脆了，折痕很深。" |

---

## 3. 地图中景剪影层

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/scenes/map-mid.png` |
| **尺寸** | 2560×1440（16:9），**透明底 PNG** |
| **正向 Prompt** | Semi-transparent silhouette cutouts of whimsical landmarks on transparent background — a tall ancient tree, a giant mushroom cluster, a faint castle turret outline, rolling gentle hills. Paper-cut shadow style, soft dark sepia tones, vintage storybook paper diorama layers. Isolated on transparent background, no background fill, no shadow beneath. |
| **补充叙事引导** | "从旧书页剪下来的地标，贴在透光的描图纸上。" |

---

## 4. 地图前景雾层

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/scenes/map-front.png` |
| **尺寸** | 2560×1440（16:9），**透明底 PNG** |
| **正向 Prompt** | Translucent mist patches and ink splatter blots floating above transparent background, low opacity, foreground grass blade silhouettes along the bottom edge, soft dreamy fog wisps. Vintage paper ephemera overlay. Isolated on transparent background, no background fill. |
| **补充叙事引导** | "贴在玻璃上的雾斑，从纸上轻轻浮起来。" |

---

## 5. 兔子洞隧道（转场用）

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/scenes/cover-tunnel.jpg` |
| **尺寸** | 2560×1440（16:9） |
| **正向 Prompt** | A dizzying downward view into a deep rabbit-hole well shaft, concentric ring structure — shelves with books and jars embedded in the circular walls, floating objects silhouettes (a pocket watch, an orange marmalade jar, a key) drifting in the dark void. The center fades to deep darkness. Warm dim amber light at the top, fading to black at the bottom. Hand-painted storybook depth, soft painterly textures, mysterious downward spiral. Vintage paper grain and aged tones. |
| **补充叙事引导** | "往下看。在掉进去的前一秒，所有东西都是飘着的。" |

---

# 第二批：茶会场景（深度场景的肉）

---

## 6. 茶会舞台全景

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/scenes/teaparty-stage.jpg` |
| **尺寸** | 4320×1440（3:1 超宽） |
| **正向 Prompt** | A magical pop-up storybook opening into a whimsical tea party stage. An impossibly long tea table stretches across the entire scene, piled high with stacked teacups, toppled teapots, mismatched plates, and scattered cutlery in beautiful chaos. A Alice-blue tablecloth drapes across the table with watercolor bleeding edges. Checkered storytelling ground beneath. Warm afternoon light from the left. No characters visible — this is the empty stage waiting for its cast. Hand-painted paper diorama with layered depth, soft painterly gouache textures, aged paper background, vintage theatrical set design, dreamy and slightly surreal atmosphere. |
| **补充叙事引导** | "翻开立体书，舞台亮了。长桌上的茶还没凉，但喝茶的人不知去了哪儿。" |

---

## 7. 茶会远景

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/scenes/teaparty-bg.jpg` |
| **尺寸** | 4320×1440（3:1 超宽） |
| **正向 Prompt** | Soft out-of-focus background layer of a garden courtyard behind the tea party — blurred tree silhouettes, dappled afternoon sunlight filtering through leaves, warm hazy atmosphere, low contrast, dreamy pastoral backdrop. Hand-painted watercolor wash, very soft brushstrokes, vintage muted palette. Meant to sit behind a sharper foreground diorama. |
| **补充叙事引导** | "远处是花园。看不清，也不需要看清——茶桌在前面就够了。" |

---

## 8. 疯帽匠

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/characters/hatter.png` |
| **尺寸** | 768×1024（3:4），**透明底 PNG** |
| **正向 Prompt** | A whimsical storybook character sticker of the Mad Hatter — tall top hat with a small price tag reading "10/6", wild unkempt hair, holding a teacup in one hand and a pocket watch chain in the other, slightly unsteady eccentric pose, mischievous expression. Hand-painted gouache illustration with soft painterly brushstrokes, gentle warm colors, die-cut white border sticker effect, paper ephemera aesthetic, scrapbook charm, vintage children's book character. Isolated on transparent background. |
| **补充叙事引导** | "帽匠被剪下来贴在纸上——标签还在，10/6，疯了的价格。" |

---

## 9. 三月兔

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/characters/march-hare.png` |
| **尺寸** | 768×1024（3:4），**透明底 PNG** |
| **正向 Prompt** | A whimsical storybook character sticker of the March Hare — straw-colored messy fur, one ear pointing up and one flopping down, clutching a butter knife and a teacup, equally unhinged expression as his tea companion. Hand-painted gouache illustration with soft painterly brushstrokes, gentle warm colors, die-cut white border sticker effect, paper ephemera aesthetic, vintage children's book character. Isolated on transparent background. |
| **补充叙事引导** | "三月兔是帽匠的同谋——疯会传染，尤其是隔着一张茶桌的时候。" |

---

## 10. 睡鼠

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/characters/dormouse.png` |
| **尺寸** | 768×1024（3:4），**透明底 PNG** |
| **正向 Prompt** | A tiny dormouse character sticker curled up asleep at the spout opening of a teapot, only head and tail visible, eyes closed, peaceful dreamy expression. Very small and delicate, miniature storybook creature. Hand-painted gouache illustration with soft painterly brushstrokes, gentle warm colors, die-cut white border sticker effect, paper ephemera aesthetic. Isolated on transparent background. |
| **补充叙事引导** | "睡在茶壶里的那位——梦话比醒话有信息量。" |

---

## 11. 茶杯

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/props/teacup.png` |
| **尺寸** | 1024×1024（1:1），**透明底 PNG** |
| **正向 Prompt** | A chipped porcelain teacup with matching saucer, the chip on the left rim, delicate floral or gold-rim pattern, vintage heirloom china. Die-cut paper embellishment floating above aged paper with soft shadow, hand-painted watercolor texture, warm sepia-tinted whites, scrapbook ephemera charm. Isolated on transparent background. |
| **补充叙事引导** | "缺口朝左——帽匠啃的。这件档案值得归档。" |

---

## 12. 茶壶

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/props/teapot.png` |
| **尺寸** | 1024×1024（1:1），**透明底 PNG** |
| **正向 Prompt** | A plump round-bellied ceramic teapot, the spout opening clearly visible and slightly oversized, vintage floral pattern, warm cream and faded blue tones. Die-cut paper embellishment with soft shadow, hand-painted watercolor texture, scrapbook ephemera charm. Isolated on transparent background. |
| **补充叙事引导** | "壶嘴要够大——修好怀表后，会有东西从里面流出来。" |

---

## 13. 怀表

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/props/pocket-watch.png` |
| **尺寸** | 1024×1024（1:1），**透明底 PNG** |
| **正向 Prompt** | An open antique gold pocket watch, the watch face visible with hands pointing at 6 o'clock, several loose gears floating nearby as if disassembled, delicate engraving inside the lid, warm brass and gold tones. Die-cut paper embellishment with soft shadow, hand-painted watercolor texture, intricate vintage detail. Isolated on transparent background. |
| **补充叙事引导** | "打开的表，散落的齿轮——修好它，它会告诉你时间停了。" |

---

## 14. 帽子

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/props/hat.png` |
| **尺寸** | 1024×1024（1:1），**透明底 PNG** |
| **正向 Prompt** | A tall vintage top hat with a small dangling price tag reading "10/6", slightly worn and weathered, deep brown and warm olive tones. Die-cut paper embellishment with soft shadow, hand-painted watercolor texture, scrapbook ephemera charm. Isolated on transparent background. |
| **补充叙事引导** | "比它主人清醒——至少它知道自己是商品。" |

---

## 15. 笑容碎片

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/props/smile-shard.png` |
| **尺寸** | 512×512（1:1），**透明底 PNG** |
| **正向 Prompt** | A small glowing crescent-shaped smile fragment floating in the air, like a broken piece of a grin, purple and gold dual-tone, luminous but not neon — more like magical stained glass or trapped starlight, delicate shimmer. Paper ephemera charm, die-cut with soft glow effect, isolated on transparent background. |
| **补充叙事引导** | "一片笑容。馆长失踪前留给这个世界的……债。" |

---

# 第三批：档案卡（20张：10水彩版 + 10素描版）

---

## 档案卡通用 Prompt 公式

水彩版统一公式（替换 `[SUBJECT]`、`[TITLE_TEXT]`、`[ACCENT_COLOR]`）：

```
Vintage luggage tag antique library card, aged paper tag with faded red border and distressed edges, [SUBJECT] as a hand-painted miniature watercolor portrait in the center, gold foil stamping "ARCHIVE" accent, tea stained paper, water spots, foxing marks, old handwritten text "[TITLE_TEXT]" in faded sepia calligraphy, museum archive tag, Victorian curiosity cabinet ephemera, warm [ACCENT_COLOR] tint bleeding from the edges, scrapbook charm, 5:7 vertical card proportion.
```

素描版统一公式：

```
Vintage luggage tag antique library card, aged paper tag with faded grey border and distressed worn edges, [SUBJECT] as a delicate pencil sketch portrait in the center, fine graphite crosshatching, no color — only sepia greys and paper tones, old handwritten text "[TITLE_TEXT]" in faint pencil script, tea stained paper, water spots, foxing marks, the tag looks unfinished, waiting to be colored in. 5:7 vertical card proportion.
```

**统一参数**：700×980（5:7），JPG 文件。

---

## 16. 白兔卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/white-rabbit-color.jpg` |
| **[SUBJECT]** | White Rabbit half-body portrait in waistcoat with pocket watch chain, looking back anxiously over his shoulder |
| **[TITLE_TEXT]** | The White Rabbit · ARCHIVE No.001 |
| **[ACCENT_COLOR]** | amber gold |

---

## 17. 白兔卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/white-rabbit-sketch.jpg` |
| **[SUBJECT]** | White Rabbit half-body portrait in waistcoat with pocket watch chain, looking back anxiously over his shoulder |
| **[TITLE_TEXT]** | The White Rabbit · ARCHIVE No.001 |

---

## 18. 药瓶卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/drink-me-color.jpg` |
| **[SUBJECT]** | A small glass bottle with "Drink Me" label, with a tiny Alice silhouette growing larger behind the bottle, playing with scale and proportion |
| **[TITLE_TEXT]** | Drink Me · ARCHIVE No.014 |
| **[ACCENT_COLOR]** | dream blue |

---

## 19. 药瓶卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/drink-me-sketch.jpg` |
| **[SUBJECT]** | A small glass bottle with "Drink Me" label, with a tiny Alice silhouette growing larger behind the bottle |
| **[TITLE_TEXT]** | Drink Me · ARCHIVE No.014 |

---

## 20. 疯帽匠卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/hatter-color.jpg` |
| **[SUBJECT]** | Mad Hatter half-body portrait with tall hat and "10/6" price tag, holding teacup, slightly unhinged expression |
| **[TITLE_TEXT]** | The Hatter · ARCHIVE No.005 |
| **[ACCENT_COLOR]** | warm olive gold |

---

## 21. 疯帽匠卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/hatter-sketch.jpg` |
| **[SUBJECT]** | Mad Hatter half-body portrait with tall hat and "10/6" price tag, holding teacup |
| **[TITLE_TEXT]** | The Hatter · ARCHIVE No.005 |

---

## 22. 茶杯卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/teacup-color.jpg` |
| **[SUBJECT]** | A chipped porcelain teacup with saucer as a still life, chip on the left rim |
| **[TITLE_TEXT]** | The Chipped Teacup · ARCHIVE No.007 |
| **[ACCENT_COLOR]** | soft blue |

---

## 23. 茶杯卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/teacup-sketch.jpg` |
| **[SUBJECT]** | A chipped porcelain teacup with saucer as a still life, chip on the left rim |
| **[TITLE_TEXT]** | The Chipped Teacup · ARCHIVE No.007 |

---

## 24. 怀表卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/pocket-watch-color.jpg` |
| **[SUBJECT]** | An open antique gold pocket watch, hands frozen at 6:00, delicate inner engraving visible |
| **[TITLE_TEXT]** | The Stopped Watch · ARCHIVE No.009 |
| **[ACCENT_COLOR]** | warm gold |

---

## 25. 怀表卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/pocket-watch-sketch.jpg` |
| **[SUBJECT]** | An open antique gold pocket watch, hands frozen at 6:00, delicate inner engraving visible |
| **[TITLE_TEXT]** | The Stopped Watch · ARCHIVE No.009 |

---

## 26. 帽子卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/hat-color.jpg` |
| **[SUBJECT]** | A tall vintage top hat as a still life with dangling "10/6" price tag, slightly worn |
| **[TITLE_TEXT]** | The 10/6 Hat · ARCHIVE No.010 |
| **[ACCENT_COLOR]** | warm olive brown |

---

## 27. 帽子卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/hat-sketch.jpg` |
| **[SUBJECT]** | A tall vintage top hat as a still life with dangling "10/6" price tag, slightly worn |
| **[TITLE_TEXT]** | The 10/6 Hat · ARCHIVE No.010 |

---

## 28. 黑桃侍卫卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/card-spade-color.jpg` |
| **[SUBJECT]** | A playing card soldier — a spade-suited guard standing at attention holding a spear, large ♠ symbol, playing card framing with antique deck border |
| **[TITLE_TEXT]** | EVIDENCE ♠-1 · The Spade |
| **[ACCENT_COLOR]** | deep ink black |

---

## 29. 黑桃侍卫卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/card-spade-sketch.jpg` |
| **[SUBJECT]** | A playing card soldier — a spade-suited guard standing at attention holding a spear, large ♠ symbol, playing card framing |
| **[TITLE_TEXT]** | EVIDENCE ♠-1 · The Spade |

---

## 30. 红心传令兵卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/card-heart-color.jpg` |
| **[SUBJECT]** | A playing card soldier — a heart-suited herald blowing a trumpet, large ♥ symbol, playing card framing with antique deck border |
| **[TITLE_TEXT]** | EVIDENCE ♥-2 · The Heart |
| **[ACCENT_COLOR]** | deep rose red |

---

## 31. 红心传令兵卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/card-heart-sketch.jpg` |
| **[SUBJECT]** | A playing card soldier — a heart-suited herald blowing a trumpet, large ♥ symbol, playing card framing |
| **[TITLE_TEXT]** | EVIDENCE ♥-2 · The Heart |

---

## 32. 梅花园丁卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/card-club-color.jpg` |
| **[SUBJECT]** | A playing card soldier — a club-suited gardener holding a paintbrush with red paint stains on his hands, large ♣ symbol, playing card framing with antique deck border |
| **[TITLE_TEXT]** | EVIDENCE ♣-3 · The Club |
| **[ACCENT_COLOR]** | earthy green-brown |

---

## 33. 梅花园丁卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/card-club-sketch.jpg` |
| **[SUBJECT]** | A playing card soldier — a club-suited gardener holding a paintbrush with paint stains on his hands, large ♣ symbol, playing card framing |
| **[TITLE_TEXT]** | EVIDENCE ♣-3 · The Club |

---

## 34. 方块司库卡 · 水彩版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/card-diamond-color.jpg` |
| **[SUBJECT]** | A playing card soldier — a diamond-suited treasurer holding a ring of keys, large ♦ symbol, playing card framing with antique deck border |
| **[TITLE_TEXT]** | EVIDENCE ♦-4 · The Diamond |
| **[ACCENT_COLOR]** | warm amber gold |

---

## 35. 方块司库卡 · 素描版

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/cards/card-diamond-sketch.jpg` |
| **[SUBJECT]** | A playing card soldier — a diamond-suited treasurer holding a ring of keys, large ♦ symbol, playing card framing |
| **[TITLE_TEXT]** | EVIDENCE ♦-4 · The Diamond |

---

# 第四批：宫殿 + 补充角色

---

## 36. 红桃宫殿

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/scenes/palace-hall.jpg` |
| **尺寸** | 2560×1440（16:9） |
| **正向 Prompt** | A theatrical pop-up storybook stage of the Queen of Hearts palace garden. On the left, a white rose bush half-painted red with a tipped-over paint bucket dripping crimson. In the middle ground, rows of playing card soldiers standing in formation as flat paper cutout silhouettes. At the far right end, a grand arched dark wooden door with four suit-symbol slots carved into it — mysterious and sealed. Deep red and warm gold accents bleeding from the roses and cards. Hand-painted paper diorama with layered depth, soft gouache textures, aged parchment border, vintage theatrical set design, slightly ominous but whimsical fairy-tale mood. |
| **补充叙事引导** | "王后的花园。玫瑰正在被涂红——那些不合规矩的白，必须消失。" |

---

## 37. 白玫瑰树

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/props/white-rose-tree.png` |
| **尺寸** | 1024×1024（1:1），**透明底 PNG** |
| **正向 Prompt** | A white rose bush with half of the roses hastily painted red, red paint dripping and splattered on leaves, a tipped-over paint bucket nearby, the white roses still visible underneath the messy red brushstrokes. Hand-painted watercolor texture, vintage botanical illustration charm, die-cut paper embellishment with soft shadow. Isolated on transparent background. |
| **补充叙事引导** | "三张扑克牌花了整个下午涂这些玫瑰。刷子还在滴。" |

---

## 38. 密码门

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/props/code-door.png` |
| **尺寸** | 1024×1024（1:1），**透明底 PNG** |
| **正向 Prompt** | A grand arched double door of dark aged wood with brass hinges, four carved suit symbol recesses (♠ ♥ ♣ ♦) arranged vertically in the center as if awaiting something to be pressed into them. Mysterious and slightly foreboding, warm amber glow seeping from the crack between the doors. Hand-painted watercolor texture, vintage storybook prop. Isolated on transparent background. |
| **补充叙事引导** | "门只听'点名'——依队列先后，一色一声，不可抢先。" |

---

## 39. 扑克牌背

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/props/card-back.png` |
| **尺寸** | 600×900（2:3），**透明底 PNG** |
| **正向 Prompt** | Antique playing card back design, symmetrical copperplate-style geometric pattern, small crown emblem at center, faded navy and faded gold tones, vintage deck feel, worn card edges, tea-stained paper texture. Isolated on transparent background. |
| **补充叙事引导** | "牌背。拼在一起，或许能拼出点什么。" |

---

## 40. 白兔立绘

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/characters/white-rabbit.png` |
| **尺寸** | 768×1024（3:4），**透明底 PNG** |
| **正向 Prompt** | A storybook character sticker of the White Rabbit — wearing a waistcoat with pocket watch chain, looking back anxiously over his shoulder as if late for something, one paw holding a pocket watch, rabbit ears alert. Hand-painted gouache illustration with soft painterly brushstrokes, gentle warm cream and amber tones, die-cut white border sticker effect, paper ephemera aesthetic, vintage children's book character. Isolated on transparent background. |
| **补充叙事引导** | "永远迟到的信使——他掉落的不是怀表，是整个故事的入场券。" |

---

## 41. 白兔奔跑剪影

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/characters/white-rabbit-silhouette.png` |
| **尺寸** | 768×1024（3:4），**透明底 PNG** |
| **正向 Prompt** | A pure black silhouette of the White Rabbit running in profile, ears streaming behind, pocket watch clearly visible in hand, dynamic running pose, classic storybook cutout style, crisp clean edges. Isolated on transparent background. |
| **补充叙事引导** | "封面循环跑的那只——树洞里的光一闪，它先钻了进去。" |

---

## 42. 爱丽丝

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/characters/alice.png` |
| **尺寸** | 768×1024（3:4），**透明底 PNG** |
| **正向 Prompt** | A storybook character sticker of Alice — a young girl in a blue dress with blonde hair, curious and gentle expression, classic Victorian children's book illustration style, standing pose with hands slightly open as if discovering something. Hand-painted gouache illustration with soft painterly brushstrokes, dream blue dress tones, die-cut white border sticker effect, paper ephemera aesthetic. Isolated on transparent background. |
| **补充叙事引导** | "她的笔记散落各处——我们现在走的，正是她走过的路。" |

---

## 43. 柴郡猫 · 完整形态

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/characters/cheshire-cat.png` |
| **尺寸** | 768×1024（3:4），**透明底 PNG** |
| **正向 Prompt** | A storybook character sticker of the Cheshire Cat — a striped cat with vivid purple and magenta fur, perched on an invisible branch, enormous mischievous grin, glowing yellow-green eyes, body fading slightly at the edges as if dissolving into air. Hand-painted gouache illustration with soft painterly brushstrokes, saturated dream purple tones, die-cut white border sticker effect, paper ephemera aesthetic, magical mysterious creature. Isolated on transparent background. |
| **补充叙事引导** | "他从不指路，只提问。然后慢慢溶解——先笑容，再眼睛，最后是「你确定？」" |

---

## 44. 柴郡猫 · 仅笑容（残卡）

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/characters/cheshire-smile.png` |
| **尺寸** | 768×1024（3:4），**透明底 PNG** |
| **正向 Prompt** | The same composition as the Cheshire Cat but the body has disappeared — only the enormous glowing grin and two luminous yellow-green eyes remain floating in the air, everything else is gone, as if the cat dissolved and left only its smile behind. Hand-painted gouache texture, dream purple and ethereal gold tones, slightly haunting but whimsical. Isolated on transparent background. |
| **补充叙事引导** | "馆长只剩笑容了。其余部分——还在找。" |

---

# 第五批：材质与收尾

---

## 45. 共用羊皮纸纹理

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/materials/parchment-tile.jpg` |
| **尺寸** | 1024×1024（1:1），**可平铺** |
| **正向 Prompt** | Aged parchment paper texture, tea stained, warm cream and sepia tones, water spots, subtle foxing marks, faint crease lines, deckled edge feel, antique handmade paper, suitable for seamless tiling, no text or markings. Rich paper grain visible. |
| **补充叙事引导** | "全项目唯一的共用纸底。所有占位处从它裁切。一张纸，打天下。" |

---

## 46. 胡桃木纹理（可选）

| 项 | 值 |
|---|---|
| **输出路径** | `demo/public/assets/materials/walnut-tile.jpg` |
| **尺寸** | 1024×1024（1:1），**可平铺** |
| **正向 Prompt** | Dark walnut wood grain texture, rich brown tones, fine wood grain lines, antique furniture surface, suitable for seamless tiling, no text or markings. Warm dark brown with subtle reddish undertones, Victorian cabinet quality. |
| **补充叙事引导** | "档案库的抽屉墙。胡桃木，黄铜件，绿灯罩台灯——书房到了。" |

---

## 汇总速查表

| # | 文件名 | 批 | 尺寸 | 格式 |
|---|---|---|---|---|
| 1 | `cover-riverbank.jpg` | 1 | 2560×1440 | JPG |
| 2 | `map-base.jpg` | 1 | 2560×1440 | JPG |
| 3 | `map-mid.png` | 1 | 2560×1440 | 透明PNG |
| 4 | `map-front.png` | 1 | 2560×1440 | 透明PNG |
| 5 | `cover-tunnel.jpg` | 1 | 2560×1440 | JPG |
| 6 | `teaparty-stage.jpg` | 2 | 4320×1440 | JPG |
| 7 | `teaparty-bg.jpg` | 2 | 4320×1440 | JPG |
| 8 | `hatter.png` | 2 | 768×1024 | 透明PNG |
| 9 | `march-hare.png` | 2 | 768×1024 | 透明PNG |
| 10 | `dormouse.png` | 2 | 768×1024 | 透明PNG |
| 11 | `teacup.png` | 2 | 1024×1024 | 透明PNG |
| 12 | `teapot.png` | 2 | 1024×1024 | 透明PNG |
| 13 | `pocket-watch.png` | 2 | 1024×1024 | 透明PNG |
| 14 | `hat.png` | 2 | 1024×1024 | 透明PNG |
| 15 | `smile-shard.png` | 2 | 512×512 | 透明PNG |
| 16 | `white-rabbit-color.jpg` | 3 | 700×980 | JPG |
| 17 | `white-rabbit-sketch.jpg` | 3 | 700×980 | JPG |
| 18 | `drink-me-color.jpg` | 3 | 700×980 | JPG |
| 19 | `drink-me-sketch.jpg` | 3 | 700×980 | JPG |
| 20 | `hatter-color.jpg` | 3 | 700×980 | JPG |
| 21 | `hatter-sketch.jpg` | 3 | 700×980 | JPG |
| 22 | `teacup-color.jpg` | 3 | 700×980 | JPG |
| 23 | `teacup-sketch.jpg` | 3 | 700×980 | JPG |
| 24 | `pocket-watch-color.jpg` | 3 | 700×980 | JPG |
| 25 | `pocket-watch-sketch.jpg` | 3 | 700×980 | JPG |
| 26 | `hat-color.jpg` | 3 | 700×980 | JPG |
| 27 | `hat-sketch.jpg` | 3 | 700×980 | JPG |
| 28 | `card-spade-color.jpg` | 3 | 700×980 | JPG |
| 29 | `card-spade-sketch.jpg` | 3 | 700×980 | JPG |
| 30 | `card-heart-color.jpg` | 3 | 700×980 | JPG |
| 31 | `card-heart-sketch.jpg` | 3 | 700×980 | JPG |
| 32 | `card-club-color.jpg` | 3 | 700×980 | JPG |
| 33 | `card-club-sketch.jpg` | 3 | 700×980 | JPG |
| 34 | `card-diamond-color.jpg` | 3 | 700×980 | JPG |
| 35 | `card-diamond-sketch.jpg` | 3 | 700×980 | JPG |
| 36 | `palace-hall.jpg` | 4 | 2560×1440 | JPG |
| 37 | `white-rose-tree.png` | 4 | 1024×1024 | 透明PNG |
| 38 | `code-door.png` | 4 | 1024×1024 | 透明PNG |
| 39 | `card-back.png` | 4 | 600×900 | 透明PNG |
| 40 | `white-rabbit.png` | 4 | 768×1024 | 透明PNG |
| 41 | `white-rabbit-silhouette.png` | 4 | 768×1024 | 透明PNG |
| 42 | `alice.png` | 4 | 768×1024 | 透明PNG |
| 43 | `cheshire-cat.png` | 4 | 768×1024 | 透明PNG |
| 44 | `cheshire-smile.png` | 4 | 768×1024 | 透明PNG |
| 45 | `parchment-tile.jpg` | 5 | 1024×1024 | JPG |
| 46 | `walnut-tile.jpg` | 5 | 1024×1024 | JPG |

---

**文档结束。** 共 46 张图，每张都有独立的正向 Prompt、尺寸、输出路径。按批次顺序生成，同一批次内可并行。
