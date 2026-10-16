# 画像生成プロンプト

『返り咲き』の画像生成用プロンプトを追記して管理します。現在のストーリーは [story.md](story.md)、動画用は [video_prompts.md](video_prompts.md) を参照してください。

シーン別プロンプトは未作成です。添付 HTML の参考画像は `assets/` に保存していますが、その生成に使用されたプロンプトは資料に記載されていません。

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

## プロンプト記録

（未登録）
