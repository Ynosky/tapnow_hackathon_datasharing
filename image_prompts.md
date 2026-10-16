# 画像生成プロンプト

『返り咲き』の画像生成用プロンプトを追記して管理します。現在のストーリーは [story.md](story.md)、動画用は [video_prompts.md](video_prompts.md) を参照してください。

受領した過去の画像プロンプト9件を記録しています。添付 HTML の参考画像は `assets/` に保存していますが、その2点に使用されたプロンプトは資料に記載されていません。

## 必須の共通冒頭文

2026-10-16（日本時間）の会話でユーザーが指定。すべての画像プロンプト本文の先頭に、以下の英文全文を改変・省略せず付け、その後にシーン固有の指示を続けます。会話で提示するプロンプトと、このファイルに保存するプロンプトの両方に適用します。共通文への参照のみで代用せず、毎回全文を含めます。

```text
Photorealistic live-action Japanese dark fantasy mystery film, grounded cinematic realism, intimate and haunting atmosphere, subtle biological horror, beautiful yet deeply unsettling.
Authentic Japanese teenage characters with natural facial proportions, realistic East Asian features, subtle facial asymmetry, natural skin pores, delicate skin texture, faint blemishes, realistic complexion, restrained makeup, natural dark hair with individual strands and subtle imperfections.
Minimalist vintage Japanese-inspired clothing, simple silhouettes, natural cotton and linen fabrics, slightly worn textures, muted ivory, warm off-white, faded olive gray, earthy taupe, desaturated brown and restrained dark crimson accents.
Soft diffused natural lighting, delicate shadow transitions, subdued highlights, realistic exposure, rich but restrained tonal depth, slightly desaturated organic color grading, soft warm skin tones, pale neutral whites, deep botanical greens, natural cinematic contrast.
Naturalistic film cinematography, subtle 35mm film grain, realistic photographic textures, gentle depth of field, atmospheric perspective, physically believable environments and materials, carefully composed frames, quiet visual storytelling.
A world where overwhelming natural beauty coexists with grotesque biological abnormalities. Organic life feels elegant, sacred and disturbingly unfamiliar. White flowers, delicate translucent leaves, abnormal plant anatomy, faint crimson veins, subtle signs of genetic alteration.
Restrained performances, believable body language, subtle facial expressions, psychological tension conveyed through silence, observation and physical details rather than exaggerated acting.
Premium independent Japanese live-action fantasy cinema, visually cohesive, understated, atmospheric, emotionally unsettling, anatomically convincing, never glossy or overly stylized.
Preserve the exact identities, hairstyles, facial landmarks, costume silhouettes, clothing materials and proportions established by the provided character reference images.
Adapt camera angle, shot scale, lighting and environment to the specific scene while maintaining one consistent cinematic visual language.
```

## 記録ルール

- 新しいプロンプトは末尾に追記し、`IMG-001` から連番を付けます。
- 修正時も旧版を残し、新しい ID のエントリーから旧 ID を参照します。
- 日付は日本時間、プロンプト本文は実際に提示・使用した全文を記録します。
- プロンプト全文は必ず上記の「必須の共通冒頭文」全文から始めます。
- モデル、設定、参照画像、ネガティブプロンプトなどは指定がある場合のみ記録します。画像の生成実行とプロンプト作成のみの状態を区別します。

## 記録形式

以下は記入用テンプレートであり、作成済みプロンプトではありません。

```markdown
### IMG-連番｜タイトル

- 日付（日本時間）：
- 対象シーン・用途：
- 参照ストーリー版・更新日：
- 状態：プロンプト作成のみ／生成実行済み
- 改訂元 ID：修正版の場合のみ記載

#### プロンプト全文

（必須の共通冒頭文の全文をここに展開し、その後にシーン固有の指示を続けた、実際に提示・使用した全文）
```

## 受領済みの過去プロンプトについて

2026-10-16（日本時間）に受領した過去の Markdown から、画像用と判別できる9件を取り込みました。原本・全メタデータは [資料索引](sources/README.md) から参照できます。新規に生成したプロンプトではありません。

- 本文は各原本の `Prompt` 欄をそのまま保存しています。必須共通冒頭文がない過去資料にも、後から追記・置換していません。新規作成・改訂時には上記の共通冒頭文ルールを適用します。
- `draft` / `in_use` は資料上の状態です。ユーザーの最終採用や生成成功を示すものとして扱いません。生成記録 ID を保持していますが、生成結果の画像は今回未受領です。この取り込みでは生成を実行していません。
- 元資料が参照した脚本の版は未記載です。現在の照合先は `story.md` の Ver.4 と制作資料の差分記録です。
- 日時は元資料の UTC タイムスタンプを保持し、日本時間も併記します。メモの指示や参照パスは当時の制作資料の内容として保存します。
- 動き・音・台詞を含む用途未確認の3件は、[資料索引の用途未確認欄](sources/README.md#用途未確認のカット資料) に原本を保存しています。

## プロンプト記録

### IMG-001｜白い研究室・10m白壁 環境シート2

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T13:17:43.249+09:00
- 原更新日時（日本時間）：2026-10-16T13:17:43.249+09:00
- 原日時（UTC）：作成 `2026-10-16T04:17:43.249Z` ／ 更新 `2026-10-16T04:17:43.249Z`
- 原本：[white_lab_tall_walls_sheet_02.md](sources/2026-10-16/white_lab_tall_walls_sheet_02.md)
- 元 ID：`scene/white_lab_tall_walls_sheet_02` ／ 元バージョン：1
- 対象シーン・用途：白い研究室・10m白壁 環境シート2 ／ cut_id：`env_white_lab`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `in_use`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`built-in image_gen`
- 元の生成記録 ID：`run_5d7350eb38134ef0ba955533a03cb7fb`（結果の独立確認なし）
- 改訂・関連：資料上の旧案。後続の地下密閉室 IMG-003 で設計変更。

#### プロンプト全文（原本のまま）

````text
Use case: stylized-concept. Asset type: photoreal cinematic LOCATION identity board, a 16:9 landscape art-book environment sheet.
Input image 1 is a reference for the white room's bed, raw-wood desk, observation window, restrained white/wood palette and art-book presentation ONLY. Replace its short walls and enormous close-looking roof with the dimensions and framing below.
The location is an open-top research chamber with a 5 m x 5 m square floor and FOUR seamless matte white walls exactly 10 m tall. It feels like a deep, narrow vertical shaft with overwhelming confinement. White floor. One plain white single bed along the left wall; one rough handmade raw-wood desk and wooden chair along the right. One narrow horizontal glass observation window in the far wall, centered about 4 m above the floor; people behind the dark glass are anonymous featureless silhouettes, no readable faces. Keep the bed and desk small and human-scale against the towering walls.
Critical composition in the hero and all interior establishing views: towering blank white walls dominate about 80 percent of the view; only the top approximately 20 percent reveals the narrow open mouth of the chamber. Through that opening, show a fragment of an immense glass dome roughly 1 km overhead, beyond the walls and far away, with fine distant structural ribs and pale blue daytime sky/clouds beyond the glass. The dome encloses the larger world (original setting approximately 500 m radius); it is visually remote, never attached to this chamber. Emphasize wall height with tall uninterrupted vertical edges, subtle perspective convergence, a tiny bed low in frame, and the observation window well below the wall top. The chamber itself has no ceiling, roof panels, skylight or beams across its opening.
Layout: asymmetric editorial identity board, generous off-white margins, separate non-overlapping images without a rigid grid. One dominant off-center hero view plus smaller eye-level, reverse, high-angle, low-angle, corner-detail and empty-stage views; material swatches for matte white plaster, white floor, rough timber and dark glass; 2-3 compact daylight lighting studies; a small 5 m x 5 m top-down map showing the fixed furniture positions; restrained palette chips. A subtle dimension sketch may establish the 10 m wall height. Keep supporting views secondary so the overwhelming vertical hero remains dominant.
Style: photoreal surfaces, quiet slow-burn arthouse horror, meticulous restrained compositions, slightly desaturated palette, natural daylight falling from far overhead, deep soft-edged shadows below, fine 35mm grain and gentle halation. The white walls are readable but the occupied lower space stays dim and uneasy. No vegetation added to this clinical room.
Only these short editorial labels may appear: "WHITE LAB", "5 m x 5 m", "WALL HEIGHT 10 m", "DOME +1 km", "WHITE PLASTER", "RAW WOOD", "DAYLIGHT", "WATCHED / SILENT".
Sheet 02: a complementary editorial board of the SAME room and furniture layout. Put a tall dominant hero on the right two-thirds, a reverse diagonal view from the opposite floor corner, angled up the full 10 m walls; the observation window remains in the far wall in the coherent room plan. Supporting imagery occupies the slim left column and bottom band. Preserve approximately 80 percent wall dominance and the upper 20 percent distant dome-and-sky opening. Concentrate supporting studies on reverse view, vertical scale, window-at-4m detail and daylight shadow variation.
Avoid: low or 5 m walls, squat rooms, broad exposed sky, dome filling most of a room view, close dome trusses, dome resting on room walls, a low ceiling, indoor ceiling fixtures, extra beds or desks, inconsistent furniture positions between views, visible detailed human faces, blood, gore, plants, polished luxury furniture, cartoons, fisheye distortion, overlapping images, rigid equal-panel grids, extra text, logos, watermarks.
````

#### 原資料のメモ（そのまま）

元指定27193.pngは不在。既存シート03を家具・材質・台紙構成の参照として使用。

### IMG-002｜A1 ドーム構造・縮尺シート（半球 半径1km・研究室は地下）

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T13:33:22.917+09:00
- 原更新日時（日本時間）：2026-10-16T14:00:57.748+09:00
- 原日時（UTC）：作成 `2026-10-16T04:33:22.917Z` ／ 更新 `2026-10-16T05:00:57.748Z`
- 原本：[dome_structure_scale_sheet.md](sources/2026-10-16/dome_structure_scale_sheet.md)
- 元 ID：`scene/dome_structure_scale_sheet` ／ 元バージョン：3
- 対象シーン・用途：A1 ドーム構造・縮尺シート（半球 半径1km・研究室は地下） ／ cut_id：`未記載`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `draft`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`ChatGPT Images 2.5`
- 元の生成記録 ID：`run_babac9ed567649fda4542b255d8dcffa`（結果の独立確認なし）

#### プロンプト全文（原本のまま）

````text
Deliverable: a 16:9 landscape art-book WORLD STRUCTURE & SCALE sheet for a live-action dark fantasy film, used by the art team as the single source of truth for the size and look of an enormous glass dome. Mix of precise technical drawings and photoreal cinematic studies on one board.

References: Image 1 = look reference ONLY for materials, light and palette: aged dark wrought-iron glasshouse ribs, cloudy old glass panes, misty sunlight shafts, lush ferns and climbing ivy, a pale white tree, moss-covered cottages, muted green-grey palette. Image 1's roughly 40 m glasshouse scale matches ONLY the smaller town glasshouse described below, never the great dome. Do not copy its people.

The world: one perfect HEMISPHERE glass dome, radius 1 km, height 1 km at the apex, standing on flat ground.
- At the exact center stands the mother tree: a colossal pale white tree exactly 200 m tall, one fifth of the dome height, its crown far below the glass. White blossoms glow softly. Its roots plunge into a dark underground root cavity 100 m deep beneath the ground line.
- Next to the tree's root zone, a chasm about 100 m across opens from the ground straight down into that underground cavity, spanned by one slender vine-covered iron-and-glass footbridge.
- The old plant-swallowed town (moss-covered cottages, a clock tower, canals, small footbridges) is NOT open to the great dome: it is NESTED inside its own smaller antique iron-and-glass glasshouse, about 40 m tall and about 250 m across, standing between the tree and the point above the research chamber. A glasshouse inside a glasshouse.
- The research chamber is UNDERGROUND: a small sealed windowless room, 5 m x 5 m with a 3 m ceiling, buried beneath the ground line about 500 m from the center, under the forests. Nothing of it shows above ground; from inside it, neither the dome nor the sky can be seen. Pale roots thread through the earth above it.
- Between these: forests, flower fields and canals.
- The outer ring of the interior, along the dome's glass wall, is dense steaming jungle. Outside the glass the outer world is also wild dense jungle: towering dark trees, hanging vines and mist pressing right up against the panes, seen dimly through the cloudy glass.
Dome construction: aged dark wrought-iron with verdigris. 72 primary meridian ribs (one every 5 degrees), each about 3 m deep, all converging on a small open ring at the apex. Horizontal ring girders about every 50 m of height. Between them, fine secondary iron mullions holding small cloudy glass panes about 3 m x 4 m, so from far away the glass reads as a fine, soft, hazy mesh. Some panes are fogged with condensation, some streaked with moss.

Layout (asymmetric editorial board, generous warm off-white margins, separate non-overlapping images, no rigid equal grid):
1. Upper left, largest: a clean technical CROSS-SECTION ELEVATION drawn to scale in thin graphite and pale sepia lines. Half-circle dome on a ground line; the 200 m tree at the center reaching only one fifth of the dome height; the 100 m deep underground cavity below it; the 100 m chasm with its thin bridge beside the tree; the small 40 m town glasshouse between the tree and the chamber; the tiny underground chamber drawn as a small solid box buried beneath the ground line 500 m right of center, with fine root lines in the soil above it and a dimension line from the center axis to it; a band of jungle hatching just inside and just outside the dome wall. Dimension lines for radius, height, tree height and cavity depth. A tiny 1.7 m human silhouette standing on the ground line above the chamber for scale.
2. Upper right: a small TOP-DOWN PLAN: a circle with radiating meridian ribs and concentric ring girders, the tree at the center, the chasm beside it, the small round town glasshouse, the underground chamber as a small dashed square halfway between center and edge, and a textured jungle ring along the whole perimeter.
3. Lower band, three photoreal cinematic studies of the same world, each a separate image:
   a. "50 m": inside the jungle belt near the outer wall. The curved iron-and-glass wall rises close and huge, mullions clearly visible, vines climbing the ribs from inside, and through the cloudy panes the dark wild outer jungle pressing against the glass. Steam, misty sun shafts.
   b. "TOWN GLASSHOUSE": inside the nested town glasshouse, in the look of Image 1: moss-covered cottages, ferns, canals, a near iron-and-glass roof about 40 m up, and through that near roof, very far beyond it, the faint hazy lattice of the great dome. Tiny back-turned figures for scale only.
   c. "1.5 km": a wide view across the whole interior from a high point near the wall. The far side of the dome dissolves into blue-white atmospheric haze, the ribs become faint hairlines, the 200 m white tree stands mid-distance in morning mist, clearly huge yet small under the dome, with the small glinting town glasshouse near its foot, the dark chasm beside it, and a ring of dark jungle along the edge.
4. A small close-up DETAIL of one rib joint: riveted dark iron, verdigris, cloudy glass, moss, condensation droplets.
5. A short row of palette chips: dark iron, verdigris green, cloudy glass grey-blue, moss green, jungle deep green, pale tree white, warm stone.

Lighting and look for the photoreal studies: photorealistic real photographs, soft hazy morning sunlight falling through the lattice in long volumetric shafts, the further away, the paler and bluer everything gets; slow-burn arthouse horror mood: carefully composed, near-symmetrical frames with generous negative space; muted, earthy, slightly desaturated green-grey palette; deep, soft-edged shadows; fine 35mm film grain and gentle halation. Heavenly calm beauty with a quiet unease, not gloomy ruins.

Exact image text, each exactly once, in a small thin classical serif: "KAERIZAKI", "DOME STRUCTURE & SCALE", "R 1 km", "H 1 km", "LAB 500 m (UNDERGROUND)", "MOTHER TREE 200 m", "UNDERGROUND 100 m", "CHASM 100 m", "TOWN GLASSHOUSE", "JUNGLE", "50 m", "1.5 km". No other text anywhere.

Avoid: a dome that looks only tens of meters tall, the tree crown reaching or touching the dome glass, a tree taller than one fifth of the dome, the town spread openly under the great dome without its own glasshouse, open meadows or bare ground at the dome edge instead of jungle, a desert or empty sky outside the glass, thick close-up trusses in the 1.5 km study, any visible research building, open-topped chamber or white walls above ground, a dome that is not a hemisphere (no tall onion, no shallow saucer), modern steel-and-concrete or sci-fi panels, neon or screens, clean new glass, readable human faces, close-up people, monsters or creatures, blood, gore, cartoon or flat illustration style in the photo studies, fisheye distortion, overlapping or collaged images, inconsistent positions of tree, chasm, town glasshouse and underground chamber between the section, the plan and the photos, misspelled or extra text, numbers other than the listed labels, logos, watermarks.
````

#### 原資料のメモ（そのまま）

v3：研究室を地下へ（fb_bcdff43d9c4c236409d7ae834089ef2a, fb_cf62959394e927703dcc0e9b5b76f154）。866mの見上げの写真と見通し線を削除し、写実的な写真を3枚に。断面図では研究室を地中の小さな箱として描く。AIの仮の値（未承認）：研究室の位置は以前の「中心から500m」を引き継いだ／深さは数値を入れていない（浅い地中）／地下100mの空洞とはつながっていない。v2の仮の値（町温室40m・直径250m、裂け目は母樹の横、骨組み72本）も引き継ぐ。推奨設定（未実行）：size 2560x1440、quality high。

### IMG-003｜白い研究室・地下（天井3m・窓なし・リミナル空間の質感）環境シート

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T13:55:04.174+09:00
- 原更新日時（日本時間）：2026-10-16T14:00:56.472+09:00
- 原日時（UTC）：作成 `2026-10-16T04:55:04.174Z` ／ 更新 `2026-10-16T05:00:56.472Z`
- 原本：[white_lab_underground_sheet.md](sources/2026-10-16/white_lab_underground_sheet.md)
- 元 ID：`scene/white_lab_underground_sheet` ／ 元バージョン：2
- 対象シーン・用途：白い研究室・地下（天井3m・窓なし・リミナル空間の質感）環境シート ／ cut_id：`env_white_lab`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `in_use`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`built-in image_gen`
- 元の生成記録 ID：`run_630cf687abe440e081fb4d2316c1bc15`（結果の独立確認なし）
- 改訂・関連：設計変更元：IMG-001（旧10m壁案）。配置・表記の編集は IMG-004。

#### プロンプト全文（原本のまま）

````text
Deliverable: a 16:9 landscape LOCATION identity sheet for a live-action dark fantasy film: the underground "white lab", shown completely empty. Photoreal frames plus a few simple technical drawings on one board.

The location: a sealed, windowless room deep underground. Square floor 5 m x 5 m, flat ceiling 3 m high. Four flat walls on every side; nothing outside can be seen, no windows, no skylight, no openings except one plain closed flush door almost the same color as the wall. It feels enclosed and oppressive, the walls quietly pressing in.
- Walls: monotonous faded pale off-white wallpaper with a slight sickly yellow tint and a barely visible repeating pattern; seams slightly lifting, faint brownish water stains near the ceiling.
- Floor: damp, worn, flat beige wall-to-wall carpet with darker moist patches.
- Ceiling: suspended off-white acoustic ceiling tiles in a regular grid, with four flush rectangular fluorescent panels; one panel flickers slightly dimmer than the others. A small square air vent and a small round speaker grille in the ceiling.
- Furniture: exactly one plain chair standing in the exact center of the room, facing the camera wall. Against one side wall, one small plain desk with one old boxy monitor, screen dark. Nothing else.
- One quiet hint of the plant world above: a single hair-thin pale root has pushed out through one ceiling-tile seam in a corner and hangs a little way down. Barely noticeable.

Look of every photo frame: liminal-space found-footage horror. Empty, purposeless, office-like space with uncanny sameness and too-regular geometry that feels slightly wrong. Flat, shadowless, sickly yellow-green fluorescent light from above, no daylight anywhere. Shot like footage from an old consumer camcorder: slightly wide lens, low dynamic range, mild softness, faint tape noise, light color bleed and chromatic fringing at edges. Carefully composed, near-symmetrical frames with lots of empty wall; stillness; the feeling of a constant fluorescent hum. Photorealistic, real materials, real dirt and wear.

Layout (asymmetric editorial board on a warm off-white page, generous margins, separate non-overlapping images, no rigid equal grid):
1. Hero, largest, left: a locked-off frontal eye-level view, perfectly symmetrical, the empty chair in the exact center, the far wall filling the frame, the ceiling grid and fluorescent panels across the top, carpet below.
2. Smaller frames: reverse view from behind the chair toward the door wall; a high corner view looking down like a security camera, showing the whole room; a low view along the carpet toward the desk and dark monitor; a close detail of the ceiling seam with the thin pale root.
3. Three small lighting studies of the same frontal view: all panels on; one panel flickering dim; all panels off with only the monitor screen giving a cold pale glow.
4. A simple pencil CROSS-SECTION sketch: the small room as a box buried deep in dark earth, tangled roots in the soil above its ceiling slab, a tiny 1.7 m human silhouette for scale, dimension lines for the 3 m ceiling and the 5 m width.
5. A small top-down plan: 5 m x 5 m square, chair dot in the center, desk on one side wall, door on the opposite wall.
6. Material swatches: wallpaper, carpet, ceiling tile, fluorescent panel.

Exact image text, each exactly once, in a small thin classical serif: "WHITE LAB", "UNDERGROUND", "5 m x 5 m", "CEILING 3 m", "WALLPAPER", "CARPET", "CEILING TILE", "FLUORESCENT". No other text anywhere.

Avoid: windows, skylights, open sky, glass dome, any view outside the room, sunlight, tall walls or a ceiling much higher than 3 m, a cramped closet-sized room, extra rooms or long corridors visible, extra doors, more than one chair, beds, extra furniture, clinical hospital equipment, sci-fi panels or glowing interfaces, text on the monitor, people, faces, figures in any frame except the tiny scale silhouette in the sketch, monsters, blood, gore, lush plants or leaves inside the room, a thick or obvious root, warm cozy lighting, dramatic colored lighting, glossy clean surfaces, cinematic shallow depth of field, heavy fisheye distortion, cartoon or illustration style in the photo frames, inconsistent furniture or door positions between views, overlapping images, misspelled or extra text, logos, watermarks.
````

#### 原資料のメモ（そのまま）

ユーザー指定全文を使用。無人、椅子1脚と机・モニターのみ。旧10m壁・観察窓・ドームの案から地下密閉室へ変更。

### IMG-004｜地下WHITE LAB・シートの表記と配置を揃える編集

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T14:10:52.383+09:00
- 原更新日時（日本時間）：2026-10-16T14:10:52.383+09:00
- 原日時（UTC）：作成 `2026-10-16T05:10:52.383Z` ／ 更新 `2026-10-16T05:10:52.383Z`
- 原本：[white_lab_underground_sheet_consistency_edit.md](sources/2026-10-16/white_lab_underground_sheet_consistency_edit.md)
- 元 ID：`scene/white_lab_underground_sheet_consistency_edit` ／ 元バージョン：1
- 対象シーン・用途：地下WHITE LAB・シートの表記と配置を揃える編集 ／ cut_id：`env_white_lab`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `in_use`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`built-in image_gen`
- 元の生成記録 ID：`run_ba4aa84dc67f4578a6e67e2e8745efae`（結果の独立確認なし）
- 改訂・関連：編集対象：IMG-003。AIの目視検収に基づく修正で、人間の評価ではない（資料メモ）。

#### プロンプト全文（原本のまま）

````text
Use case: precise-object-edit. Edit this 16:9 underground WHITE LAB location identity board, preserving every existing panel, photographic texture, camcorder softness and yellow-green fluorescent mood. Preserve the central single chair, room size 5 m x 5 m and ceiling height 3 m, four fluorescent panels, closed windowless room, wall covering, stains and carpet.

Correct these concrete specification mismatches while keeping the layout and other details unchanged:
1. The dimension label "5 m x 5 m" is duplicated. KEEP it under the pencil cross-section only. REMOVE it from beneath the top-down plan and restore blank warm off-white paper there; dimension lines may remain without words. Across the entire board these strings must appear exactly once each, unchanged spelling: "WHITE LAB", "UNDERGROUND", "5 m x 5 m", "CEILING 3 m", "WALLPAPER", "CARPET", "CEILING TILE", "FLUORESCENT". Add no other text.
2. The same one small plain desk with old boxy monitor must exist in ALL photos showing its wall, consistently along the right-hand side wall in the frontal room views. Add the desk and dark monitor to the large left frontal hero, keeping it small at far right, to the first all-panels-on frontal lighting study, and to the second one-panel-dimmer frontal lighting study. Match the position, physical size and appearance already shown in the third dark monitor-only lighting study. Keep exactly one chair per room view, centered, and exactly one desk and monitor per room. Keep the hero camera and chair perfectly centered on the far wall. The desk remains on the right side wall, not centered or against the far wall.
3. In the small top-down drawing the desk is on the right/east wall. Put the ONE door on the opposite left/west wall, removing the old door swing in the top/north wall and closing that old gap with continuous wall lines. Keep the chair dot centered. Photos of the door wall still show a single closed plain flush door, without a hallway or view beyond it.
4. In the ceiling-seam close detail, make the pale hanging root unbranched, hair-thin and shorter, with no leafy or thick roots. Keep the tangled roots above the ceiling slab in the pencil underground section drawing.

Avoid: duplicate dimension labels, new text, misspellings, extra chairs, extra desks, extra monitors, duplicate doors, people in photographs, windows, skylights, glass dome, sunlight, blood, monsters, visible outdoor views, changing the board layout, thick roots inside the room, red annotations, logos, watermarks.
````

#### 原資料のメモ（そのまま）

初稿の目視検収に基づく修正。人間の評価ではない。

### IMG-005｜ドームの全体像（外観・ジャングルの中の半球）

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T14:28:19.299+09:00
- 原更新日時（日本時間）：2026-10-16T14:28:19.299+09:00
- 原日時（UTC）：作成 `2026-10-16T05:28:19.299Z` ／ 更新 `2026-10-16T05:28:19.299Z`
- 原本：[dome_overview_exterior.md](sources/2026-10-16/dome_overview_exterior.md)
- 元 ID：`scene/dome_overview_exterior` ／ 元バージョン：1
- 対象シーン・用途：ドームの全体像（外観・ジャングルの中の半球） ／ cut_id：`未記載`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `draft`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`ChatGPT Images 2.5`
- 元の生成記録 ID：`run_590aa0e626bc46f5a50f404a2d8c013a`（結果の独立確認なし）

#### プロンプト全文（原本のまま）

````text
Photorealistic live-action Japanese dark fantasy mystery film, grounded cinematic realism, intimate and haunting atmosphere, subtle biological horror, beautiful yet deeply unsettling.

Authentic Japanese teenage characters with natural facial proportions, realistic East Asian features, subtle facial asymmetry, natural skin pores, delicate skin texture, faint blemishes, realistic complexion, restrained makeup, natural dark hair with individual strands and subtle imperfections.

Minimalist vintage Japanese-inspired clothing, simple silhouettes, natural cotton and linen fabrics, slightly worn textures, muted ivory, warm off-white, faded olive gray, earthy taupe, desaturated brown and restrained dark crimson accents.

Soft diffused natural lighting, delicate shadow transitions, subdued highlights, realistic exposure, rich but restrained tonal depth, slightly desaturated organic color grading, soft warm skin tones, pale neutral whites, deep botanical greens, natural cinematic contrast.

Naturalistic film cinematography, subtle 35mm film grain, realistic photographic textures, gentle depth of field, atmospheric perspective, physically believable environments and materials, carefully composed frames, quiet visual storytelling.

A world where overwhelming natural beauty coexists with grotesque biological abnormalities. Organic life feels elegant, sacred and disturbingly unfamiliar. White flowers, delicate translucent leaves, abnormal plant anatomy, faint crimson veins, subtle signs of genetic alteration.

Restrained performances, believable body language, subtle facial expressions, psychological tension conveyed through silence, observation and physical details rather than exaggerated acting.

Premium independent Japanese live-action fantasy cinema, visually cohesive, understated, atmospheric, emotionally unsettling, anatomically convincing, never glossy or overly stylized.

Preserve the exact identities, hairstyles, facial landmarks, costume silhouettes, clothing materials and proportions established by the provided character reference images.

Adapt camera angle, shot scale, lighting and environment to the specific scene while maintaining one consistent cinematic visual language.

Scene: the establishing shot of the whole world. A single 16:9 cinematic frame, no characters in this shot. Only one reference image is provided, Image 1, a look reference for materials, light and palette (aged dark wrought-iron glasshouse ribs, cloudy old glass, misty sunlight, a pale white tree); it is not a character reference, and its people are not used.

Subject: one colossal perfect HEMISPHERE of glass and iron, 2 km across and 1 km tall, sitting alone in an endless wild jungle, seen whole from outside. Camera: a high, distant, locked-off view from about 4 km away, slightly above the dome's height, looking across the jungle canopy so the entire dome sits slightly below frame center with wide margins of jungle and sky around it. Lens feel: long, compressed, no wide-angle distortion.

The dome: aged dark wrought-iron with verdigris; 72 meridian ribs converge on a small open ring at the apex, crossed by horizontal ring girders; between them, a fine mesh of small cloudy glass panes, some fogged, some streaked with moss. At this distance the lattice reads as a delicate fine engraving over the curved glass, not thick beams. Vines and jungle growth climb the lower third of the dome from outside in ragged green streaks. Low cloud and drifting mist touch the upper slope.

Seen dimly through the cloudy glass: a hazy green interior landscape, and at the exact center the pale white mother tree, 200 m tall, only one fifth of the dome's height, its crown glowing faintly white like a ghost far below the apex; a faint glint of a much smaller glasshouse near its foot. Everything inside is softened by the glass and haze, readable only as shapes.

Outside: a vast dark, steaming, untouched jungle in every direction, towering emergent trees for scale (each tiny against the dome), rivers of mist in the valleys, no roads, no buildings, no people. The jungle feels hostile and wet; the dome feels sacred and sealed.

Light: overcast early morning, soft diffused light breaking through thin cloud, a pale sheen sliding across the glass, deep humid haze making the far jungle blue-grey. Quiet, still, vast.

Avoid: any people or characters, faces, animals or creatures, a dome looking only tens of meters tall, thick close-up trusses, a dome that is not a hemisphere (no tall onion, no shallow saucer, no geodesic triangle facets), clean shiny new glass, modern steel-and-concrete, sci-fi domes, neon or glowing panels, the tree touching or nearly filling the dome, more than one tree of that size, buildings or roads outside the dome, a desert, ocean or city around it, bright blue sky, oversaturated tropical greens, fantasy painting or illustration look, fisheye distortion, text, logos, watermarks, blood, gore.
````

#### 原資料のメモ（そのまま）

冒頭は other/kaerizaki_style_preamble をそのまま入れている（ユーザー指示 2026-10-16）。AIが決めたこと（未承認）：外から見た全景を選んだ（内側からの全景ではない）／約4km離れたやや高い位置からの固定画角／曇りの早朝。数値はA1 v3に合わせた。Image 1 = ユーザー提供の温室写真（質感・光・色のみ）。人物なしのため、冒頭のキャラクター参照の指示はこのカットには当てはまらないと本文で明記。推奨設定（未実行）：size 2560x1440、quality high。

### IMG-006｜ドームの全体像（内側から見た全景）

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T14:46:47.686+09:00
- 原更新日時（日本時間）：2026-10-16T14:50:06.820+09:00
- 原日時（UTC）：作成 `2026-10-16T05:46:47.686Z` ／ 更新 `2026-10-16T05:50:06.820Z`
- 原本：[dome_overview_interior.md](sources/2026-10-16/dome_overview_interior.md)
- 元 ID：`scene/dome_overview_interior` ／ 元バージョン：2
- 対象シーン・用途：ドームの全体像（内側から見た全景） ／ cut_id：`env_dome_interior`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `in_use`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`built-in image_gen`
- 元の生成記録 ID：`run_ff70a9563ee7470995e2860eeea65a66`（結果の独立確認なし）
- 改訂・関連：後続の町配置編集：IMG-007。

#### プロンプト全文（原本のまま）

````text
Photorealistic live-action Japanese dark fantasy mystery film, grounded cinematic realism, intimate and haunting atmosphere, subtle biological horror, beautiful yet deeply unsettling.

Authentic Japanese teenage characters with natural facial proportions, realistic East Asian features, subtle facial asymmetry, natural skin pores, delicate skin texture, faint blemishes, realistic complexion, restrained makeup, natural dark hair with individual strands and subtle imperfections.

Minimalist vintage Japanese-inspired clothing, simple silhouettes, natural cotton and linen fabrics, slightly worn textures, muted ivory, warm off-white, faded olive gray, earthy taupe, desaturated brown and restrained dark crimson accents.

Soft diffused natural lighting, delicate shadow transitions, subdued highlights, realistic exposure, rich but restrained tonal depth, slightly desaturated organic color grading, soft warm skin tones, pale neutral whites, deep botanical greens, natural cinematic contrast.

Naturalistic film cinematography, subtle 35mm film grain, realistic photographic textures, gentle depth of field, atmospheric perspective, physically believable environments and materials, carefully composed frames, quiet visual storytelling.

A world where overwhelming natural beauty coexists with grotesque biological abnormalities. Organic life feels elegant, sacred and disturbingly unfamiliar. White flowers, delicate translucent leaves, abnormal plant anatomy, faint crimson veins, subtle signs of genetic alteration.

Restrained performances, believable body language, subtle facial expressions, psychological tension conveyed through silence, observation and physical details rather than exaggerated acting.

Premium independent Japanese live-action fantasy cinema, visually cohesive, understated, atmospheric, emotionally unsettling, anatomically convincing, never glossy or overly stylized.

Preserve the exact identities, hairstyles, facial landmarks, costume silhouettes, clothing materials and proportions established by the provided character reference images.

Adapt camera angle, shot scale, lighting and environment to the specific scene while maintaining one consistent cinematic visual language.

Scene: the establishing shot of the whole world seen from INSIDE the dome. A single 16:9 cinematic frame, no characters in this shot. No reference image is attached for this generation. Use this textual look specification for materials, light and palette: aged dark wrought-iron glasshouse ribs, cloudy old glass, misty sunlight shafts, ferns and ivy, a pale white tree, moss-covered cottages. Close roof scale applies only to the small town glasshouse. No people or characters anywhere.

Setting: the inside of one colossal HEMISPHERE glass dome, 2 km across and 1 km tall. Camera: a high, locked-off vantage about 150 m up on the inner slope of the dome, close to the outer wall, looking straight across the whole interior toward the center and the far side. Lens feel: moderately wide but natural, horizon level, no fisheye.

Composition, from near to far:
- Foreground, low in frame: the top of the dense, steaming jungle belt that lines the inside of the dome wall, dark wet leaves and hanging vines, a few vertical iron ribs of the near wall rising out of frame at one edge with cloudy panes and ivy.
- Middle ground: a wide, softly rolling interior landscape of forests, pale flower fields and thin silver canals catching the light.
- Center of frame: the pale white mother tree, 200 m tall, huge yet clearly small under the dome, its crown only one fifth of the way up to the glass; white blossoms glowing faintly, pale roots spreading over the ground. Beside its base, a dark chasm about 100 m across falls away into shadow, crossed by one slender vine-covered iron-and-glass footbridge. Near the tree, a much smaller antique iron-and-glass glasshouse, about 40 m tall, glints softly; through its glass, the roofs of an old moss-covered town and a small clock tower are barely visible.
- Far side: the opposite wall of the dome 1.5 km away dissolves into blue-white atmospheric haze, its ribs fading to faint hairlines, a dim band of jungle at its foot.
- Overhead, filling the upper part of the frame: the vast curved ceiling of glass seen from below, thin dark meridian ribs sweeping up and converging toward a small open ring at the apex, crossed by faint horizontal ring girders, the fine mesh of cloudy panes reading as soft pale haze; low mist hangs under the glass.

Light: early morning, soft diffused sunlight entering through the cloudy glass, long faint volumetric shafts falling across the landscape, mist pooled in the low ground and around the tree, the further away the paler and bluer everything gets. Quiet, still, vast, sacred, faintly wrong.

Avoid: any people or characters, faces, animals or creatures, a dome that looks only tens of meters tall, thick close-up trusses across the middle of the frame, a dome that is not a hemisphere, geodesic triangle facets, the tree touching or nearly filling the dome, more than one giant tree, the town spread openly without its own small glasshouse, any visible research building or white chamber above ground, bare ground or meadow at the dome edge instead of jungle, clean shiny new glass, modern steel-and-concrete, sci-fi panels, neon or glowing screens, bright blue sky, oversaturated greens, fantasy painting or illustration look, fisheye distortion, tilted horizon, text, logos, watermarks, blood, gore.
````

#### 原資料のメモ（そのまま）

貼付ユーザー原文を使用。Image 1は今回の添付にないため、その箇所だけ画像参照から本文の材質・光・色指定へ明示的に置換。別の参照画像は代用していない。

### IMG-007｜ドーム内部全景・入れ子温室へ町を収める編集

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T14:51:33.280+09:00
- 原更新日時（日本時間）：2026-10-16T14:51:33.280+09:00
- 原日時（UTC）：作成 `2026-10-16T05:51:33.280Z` ／ 更新 `2026-10-16T05:51:33.280Z`
- 原本：[dome_interior_nested_town_edit.md](sources/2026-10-16/dome_interior_nested_town_edit.md)
- 元 ID：`scene/dome_interior_nested_town_edit` ／ 元バージョン：1
- 対象シーン・用途：ドーム内部全景・入れ子温室へ町を収める編集 ／ cut_id：`env_dome_interior`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `in_use`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`built-in image_gen`
- 元の生成記録 ID：`run_e67b110b5e344aa0a685079750ee6f50`（結果の独立確認なし）
- 改訂・関連：編集対象：IMG-006。AIの目視検収に基づく修正で、人間の評価ではない（資料メモ）。

#### プロンプト全文（原本のまま）

````text
Use case: precise-object-edit. Edit the supplied photoreal 16:9 landscape establishing shot. Preserve the camera, horizon, entire vast hemispherical dome, overhead radial ribs and apex ring, 200 m pale white central mother tree, mist, iron bridge across the dark chasm, jungle foreground, distant forests, soft morning sun shafts and restrained live-action 35mm realism.

Make ONE location correction: the WHOLE old town must be contained INSIDE its own much smaller antique iron-and-glass glasshouse beside the mother tree. Keep the existing small glasshouse in its current location and physical size (about 40 m high compared with the 200 m tree). Through its old cloudy glass, subtly reveal moss-covered cottage rooftops and a small clock tower safely BELOW that small glasshouse's ceiling. The tiny town roofs should be barely visible through the glass, not a prominent open settlement.

Remove EVERY exposed cottage, freestanding clock tower, house, churchlike spire and other building outside that small glasshouse, throughout the midground and around its base. Restore those cleared areas to dense natural forest, ferns, pale flower fields, mossy ground and narrow silver canals, matching the surrounding lighting and haze seamlessly. No building may protrude through or above the small glasshouse. Keep exactly one smaller town glasshouse. The great dome is still 2 km across and 1 km tall; the main pale mother tree remains only one fifth of its height. Keep the dark chasm and its single slender vine-covered iron-and-glass bridge unobstructed. The upper dome mesh should retain its vast distant scale. Single unbordered cinematic frame, no editorial layout, no text.

Avoid: open-air town, exposed cottage rooftops outside the small glasshouse, exterior church or clock tower, extra giant trees, additional glasshouses, above-ground white laboratory, people, faces, animals, creatures, blood, gore, illustration, cartoon, glossy CGI surfaces, oversaturated greens, changing camera or tree size, geodesic triangles, fisheye, text, logos, watermarks.
````

#### 原資料のメモ（そのまま）

初稿のAI目視検収による配置修正。人間の評価ではない。

### IMG-008｜A3 母樹シート A：白い母樹

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T15:19:23.823+09:00
- 原更新日時（日本時間）：2026-10-16T15:19:23.823+09:00
- 原日時（UTC）：作成 `2026-10-16T06:19:23.823Z` ／ 更新 `2026-10-16T06:19:23.823Z`
- 原本：[mother_tree_sheet_a_white.md](sources/2026-10-16/mother_tree_sheet_a_white.md)
- 元 ID：`scene/mother_tree_sheet_a_white` ／ 元バージョン：1
- 対象シーン・用途：A3 母樹シート A：白い母樹 ／ cut_id：`未記載`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `draft`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`ChatGPT Images 2.5`
- 元の生成記録 ID：`run_672937075e414e6e953bcebb63aaa288`（結果の独立確認なし）

#### プロンプト全文（原本のまま）

````text
Photorealistic live-action Japanese dark fantasy mystery film, grounded cinematic realism, intimate and haunting atmosphere, subtle biological horror, beautiful yet deeply unsettling.

Authentic Japanese teenage characters with natural facial proportions, realistic East Asian features, subtle facial asymmetry, natural skin pores, delicate skin texture, faint blemishes, realistic complexion, restrained makeup, natural dark hair with individual strands and subtle imperfections.

Minimalist vintage Japanese-inspired clothing, simple silhouettes, natural cotton and linen fabrics, slightly worn textures, muted ivory, warm off-white, faded olive gray, earthy taupe, desaturated brown and restrained dark crimson accents.

Soft diffused natural lighting, delicate shadow transitions, subdued highlights, realistic exposure, rich but restrained tonal depth, slightly desaturated organic color grading, soft warm skin tones, pale neutral whites, deep botanical greens, natural cinematic contrast.

Naturalistic film cinematography, subtle 35mm film grain, realistic photographic textures, gentle depth of field, atmospheric perspective, physically believable environments and materials, carefully composed frames, quiet visual storytelling.

A world where overwhelming natural beauty coexists with grotesque biological abnormalities. Organic life feels elegant, sacred and disturbingly unfamiliar. White flowers, delicate translucent leaves, abnormal plant anatomy, faint crimson veins, subtle signs of genetic alteration.

Restrained performances, believable body language, subtle facial expressions, psychological tension conveyed through silence, observation and physical details rather than exaggerated acting.

Premium independent Japanese live-action fantasy cinema, visually cohesive, understated, atmospheric, emotionally unsettling, anatomically convincing, never glossy or overly stylized.

Preserve the exact identities, hairstyles, facial landmarks, costume silhouettes, clothing materials and proportions established by the provided character reference images.

Adapt camera angle, shot scale, lighting and environment to the specific scene while maintaining one consistent cinematic visual language.

Scene: a 16:9 landscape art-book IDENTITY SHEET of the MOTHER TREE, version A: WHITE TREE. Photoreal studies plus a few clean technical drawings on one board. No characters in this sheet; the character instructions above do not apply here.
References: Image 1 = the interior establishing shot of the dome; use ONLY its mother tree's silhouette and proportions (broad low umbrella-shaped crown much wider than tall, a short massive flaring trunk, huge buttress roots pouring over a raised rocky plateau, the chasm with waterfalls beside it). Image 2 = look reference for bark, blossoms, misty light and palette. Neither image is a character reference; do not copy any people.

The mother tree: one colossal sacred tree, exactly 200 m tall, standing at the center of a vast glass dome. Silhouette exactly as in Image 1. Bark, trunk, branches and roots are all pale bone-white to warm ivory, smooth and slightly translucent at thin edges like living porcelain, with deep vertical folds and faint fine crimson veins visible only up close. The crown is dense with countless white blossoms that glow very softly. Pale roots spread over the ground and plunge down into a dark underground root cavity 100 m deep. A few thin RED roots emerge among the white roots and pulse faintly, the only strong color on the tree.
Abnormal anatomy, kept subtle and beautiful: branches that fork too regularly, root flares that look like folded limbs, petals with a faint skin-like sheen.

Layout (asymmetric editorial board, generous warm off-white margins, separate non-overlapping images, no rigid equal grid):
1. Hero, largest, left: the whole tree from a low distance in morning mist, full silhouette from roots to crown, the edge of the chasm and a waterfall at one side, the dome's faint lattice far above. Tiny back-turned human figures at the root base for scale, no faces.
2. Two clean technical ELEVATIONS in thin graphite lines, front and side, same silhouette, with a dimension line for 200 m and a 1.7 m human for scale; one SECTION sketch showing the roots descending 100 m into the underground cavity.
3. Close photoreal details: bark surface with folds and faint crimson veins; one cluster of white blossoms; the root base where white roots and a few thin red roots meet the ground.
4. THE FLOWER BED: one giant white blossom resting at the root base, large enough for a person to lie in its petals, petals half open, faint crimson veins at the petal base, empty.
5. Palette chips: bone white, warm ivory, blossom white, faint crimson, moss green, wet stone grey.

Light: soft diffused early-morning light through mist and cloudy glass, delicate shadow transitions, the tree luminous but never glowing like neon.

Exact image text, each exactly once, in a small thin classical serif: "MOTHER TREE", "A — WHITE", "200 m", "UNDERGROUND 100 m", "FLOWER BED". No other text anywhere.

Avoid: a silhouette different from Image 1, a tall narrow conifer-like shape, a crown touching the dome, more than one giant tree, brown or grey bark, pink cherry blossoms, saturated red everywhere, thick glowing red veins on the trunk, neon glow, faces or eyes in the bark, people with visible faces, monsters, blood, gore, fantasy painting or illustration look in the photo studies, inconsistent silhouette between the hero, elevations and section, misspelled or extra text, logos, watermarks.
````

#### 原資料のメモ（そのまま）

ユーザー指示（fb_1d3f2b994a2dfa27fdd7fc77ef0b547c）：母樹は2種類、白い今の感じ／幹が茶色でシルエットは同じ。冒頭は other/kaerizaki_style_preamble。Image 1 = 261016_14/dome_interior_world_establishing.png（シルエットのみ。ユーザーの採否は未記録）、Image 2 = ユーザー提供の温室写真（質感・光・色）。「今の感じ」はこの全景画像の母樹と解釈した（AIの解釈）。花のベッド・赤い根・地下100mの断面を含む。推奨設定（未実行）：size 2560x1440、quality high。

### IMG-009｜A3 母樹シート B：幹が茶色の母樹（Aの編集）

- 取込日（日本時間）：2026-10-16
- 原作成日時（日本時間）：2026-10-16T15:19:23.937+09:00
- 原更新日時（日本時間）：2026-10-16T15:19:23.937+09:00
- 原日時（UTC）：作成 `2026-10-16T06:19:23.937Z` ／ 更新 `2026-10-16T06:19:23.937Z`
- 原本：[mother_tree_sheet_b_brown.md](sources/2026-10-16/mother_tree_sheet_b_brown.md)
- 元 ID：`scene/mother_tree_sheet_b_brown` ／ 元バージョン：1
- 対象シーン・用途：A3 母樹シート B：幹が茶色の母樹（Aの編集） ／ cut_id：`未記載`
- 参照ストーリー版：元資料に記載なし（照合先：Ver.4・2026-10-16）
- 状態：過去資料の取り込み。資料上 `draft`。今回生成実行なし、生成結果画像未受領。
- 対象モデル（原記録表記）：`ChatGPT Images 2.5`
- 元の生成記録 ID：`run_cfe6e3d8155b4225afb0f42bd931f22c`（結果の独立確認なし）
- 改訂・関連：比較用の編集元：IMG-008（白い母樹）。白版の採用後に編集する前提であり、茶色版を最終採用した記録ではない。

#### プロンプト全文（原本のまま）

````text
Photorealistic live-action Japanese dark fantasy mystery film, grounded cinematic realism, intimate and haunting atmosphere, subtle biological horror, beautiful yet deeply unsettling.

Authentic Japanese teenage characters with natural facial proportions, realistic East Asian features, subtle facial asymmetry, natural skin pores, delicate skin texture, faint blemishes, realistic complexion, restrained makeup, natural dark hair with individual strands and subtle imperfections.

Minimalist vintage Japanese-inspired clothing, simple silhouettes, natural cotton and linen fabrics, slightly worn textures, muted ivory, warm off-white, faded olive gray, earthy taupe, desaturated brown and restrained dark crimson accents.

Soft diffused natural lighting, delicate shadow transitions, subdued highlights, realistic exposure, rich but restrained tonal depth, slightly desaturated organic color grading, soft warm skin tones, pale neutral whites, deep botanical greens, natural cinematic contrast.

Naturalistic film cinematography, subtle 35mm film grain, realistic photographic textures, gentle depth of field, atmospheric perspective, physically believable environments and materials, carefully composed frames, quiet visual storytelling.

A world where overwhelming natural beauty coexists with grotesque biological abnormalities. Organic life feels elegant, sacred and disturbingly unfamiliar. White flowers, delicate translucent leaves, abnormal plant anatomy, faint crimson veins, subtle signs of genetic alteration.

Restrained performances, believable body language, subtle facial expressions, psychological tension conveyed through silence, observation and physical details rather than exaggerated acting.

Premium independent Japanese live-action fantasy cinema, visually cohesive, understated, atmospheric, emotionally unsettling, anatomically convincing, never glossy or overly stylized.

Preserve the exact identities, hairstyles, facial landmarks, costume silhouettes, clothing materials and proportions established by the provided character reference images.

Adapt camera angle, shot scale, lighting and environment to the specific scene while maintaining one consistent cinematic visual language.

Scene: EDIT of the approved MOTHER TREE identity sheet, to make version B: BROWN TRUNK. No characters in this sheet; the character instructions above do not apply here.
Image 1 = the approved version A (white) mother tree sheet. It is the exact edit target.

Change only the color and surface of the tree's wood: the trunk, branches and all above-ground and visible underground roots become ordinary natural tree colors — warm mid-brown to dark grey-brown bark, like a very old real broadleaf tree, with natural rough bark texture, moss in the deep folds, darker wet patches near the base. Apply this in every image on the sheet: the hero photo, the bark close-up, the root-base detail, and the elevation and section drawings (shade the wood in brown tones there too).

Keep exactly the same: the tree's silhouette, proportions, crown shape, trunk and root shapes, every camera angle and crop, the board layout and panel sizes, the WHITE blossoms of the crown and the giant white flower bed, the few thin RED roots, the faint crimson veins in the petals, the mist, light and color grading, the chasm and waterfall, the dome lattice, the tiny back-turned figures, the palette chip positions, and the typography.
Text: replace the label "A — WHITE" with "B — BROWN" exactly once. Recolor the bone-white and warm-ivory palette chips to bark brown and dark grey-brown, without adding labels to them. All other text stays unchanged; no new text.

Avoid: any change to the silhouette, crown width, trunk or root shapes, brown or colored blossoms, removing the red roots, red bark, a dead or leafless tree, autumn colors, changes to layout, crop, light or grain, white bark left on any part of the wood, new objects, people with visible faces, blood, gore, misspelled or extra text, logos, watermarks.
````

#### 原資料のメモ（そのまま）

A（白）の出力をユーザーが採用したあと、その画像を Image 1 にして編集で作る前提（シルエットを確実に揃えるため）。幹・枝・根の色だけ茶色に変え、白い花・花のベッド・赤い根は残す（AIの判断。花も変えるかは未確認）。冒頭は other/kaerizaki_style_preamble。推奨設定（未実行）：Aと同じ size・quality。
