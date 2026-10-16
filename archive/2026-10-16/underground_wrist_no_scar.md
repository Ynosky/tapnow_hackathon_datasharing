---
id: "scene/underground_wrist_no_scar"
title: "地下室: 傷跡がない手首"
category: "scene"
model: ""
tags: ["s02_c01", "imported_from_job"]
status: "draft"
source_generation_id: "run_asset_0b3c6240bbd3e3b9f3eb1b19"
cut_id: "s02_c01"
created_at: "2026-10-15T13:32:06.938Z"
updated_at: "2026-10-15T13:32:06.938Z"
version: 1
prompt_checks: {"named_references_found": [], "has_negative_list": true, "warnings": [], "note": "検出は辞書の語と否定表現の有無だけ。辞書にない固有名詞や否定リストの中身の妥当性は自己点検する。"}
feedback_target_id: "run_e22261aba6ce4d92a38ae777d0daec19"
---

# 地下室: 傷跡がない手首

## Prompt

````text
Close-up in an underground chamber. Mio stands beside Yuna gripping Yuna's wrist. Strong light only on the wrist, emphasizing there is NO scar on Yuna's arm. Half of both faces lost in deep shadow. Background almost invisible, melted into deep bokeh. Visible wrist veins, fine linen weave. Yuna's calm face suddenly stiffens: brows knit, eyes wide, mouth twisting, face shape unchanged. Line: 'どうして、わたしにはないの？'. Pruning shears nearby. Photoreal slow-burn arthouse horror: restrained, naturalistic performances; long, patient locked-off or slowly creeping takes; carefully composed, often symmetrical frames with generous negative space; muted, earthy, slightly desaturated palette; motivated practical or natural light with deep, soft-edged shadows; fine 35mm film grain and gentle halation; quiet, sparse sound design where silence and small diegetic sounds carry the dread; horror that seeps out of ordinary, domestic or sunlit places instead of jump scares; grief and unease held beneath a calm surface; dark greenhouse world, dim light falling only partially on characters like a cast shadow, no blood, only Yuna and Mio show faces, both wear gardening aprons, living skin texture with slight grime. Follow style_rules. Avoid: blood, wounds or any scar on Yuna's wrist; any visible face other than Yuna's and Mio's; face shape distortion when Yuna's expression stiffens; extra or fused fingers; Mio's hand passing through Yuna's wrist; missing gardening aprons; the spoken line rendered as written text or subtitles; logos or watermark.
````

## メモ

`_jobs/done/s02_c01.json` のプロンプトを、フォルダのルール（否定リスト必須・実在の企業名/作品名を書かない）に合わせて直した下書き。生成では未確認。

変更点：
- 「Photoreal A24-style horror,」を `_model_guides/named_references.json` の `a24_horror` の言語化に置き換えた。
- 末尾に `Avoid:` の否定リストを追加した（中身はAIが作品ルールとこのカットで起こりうる失敗から作った案）。
- それ以外の文言は変えていない。末尾の「Follow style_rules.」も原文のまま残したが、画像モデルは style_rules を読めないので、送るときは削るか中身に置き換える。

対象モデル：未記録（ジョブの割り当ては gemini, codex, capcut、ジョブ記録上の成果物は codex）。使うモデルを決めたら、そのモデルの GUIDE.md に合わせて書き直し、model を入れて別IDで保存する。
参照画像（ジョブ記録）：_reference/mio_character_sheet.jpg。ユナの確定シートは未決定。
元の生成記録：run_asset_0b3c6240bbd3e3b9f3eb1b19（ジョブ指示を取り込んだ記録で、実際に送った全文と同じかは未確認）。

元の文言：

> Close-up in an underground chamber. Mio stands beside Yuna gripping Yuna's wrist. Strong light only on the wrist, emphasizing there is NO scar on Yuna's arm. Half of both faces lost in deep shadow. Background almost invisible, melted into deep bokeh. Visible wrist veins, fine linen weave. Yuna's calm face suddenly stiffens: brows knit, eyes wide, mouth twisting, face shape unchanged. Line: 'どうして、わたしにはないの？'. Pruning shears nearby. Photoreal A24-style horror, dark greenhouse world, dim light falling only partially on characters like a cast shadow, no blood, only Yuna and Mio show faces, both wear gardening aprons, living skin texture with slight grime. Follow style_rules.
