---
id: "scene/white_lab_underground_sheet_consistency_edit"
title: "地下WHITE LAB・シートの表記と配置を揃える編集"
category: "scene"
model: "built-in image_gen"
tags: ["underground", "consistency_edit"]
status: "in_use"
source_generation_id: "run_ba4aa84dc67f4578a6e67e2e8745efae"
cut_id: "env_white_lab"
created_at: "2026-10-16T05:10:52.383Z"
updated_at: "2026-10-16T05:10:52.383Z"
version: 1
prompt_checks: {"named_references_found": [], "has_negative_list": true, "warnings": [], "note": "検出は辞書の語と否定表現の有無だけ。辞書にない固有名詞や否定リストの中身の妥当性は自己点検する。"}
feedback_target_id: "run_ab5108bfdcbd4d79a1aadd3fef530b8d"
---

# 地下WHITE LAB・シートの表記と配置を揃える編集

## Prompt

````text
Use case: precise-object-edit. Edit this 16:9 underground WHITE LAB location identity board, preserving every existing panel, photographic texture, camcorder softness and yellow-green fluorescent mood. Preserve the central single chair, room size 5 m x 5 m and ceiling height 3 m, four fluorescent panels, closed windowless room, wall covering, stains and carpet.

Correct these concrete specification mismatches while keeping the layout and other details unchanged:
1. The dimension label "5 m x 5 m" is duplicated. KEEP it under the pencil cross-section only. REMOVE it from beneath the top-down plan and restore blank warm off-white paper there; dimension lines may remain without words. Across the entire board these strings must appear exactly once each, unchanged spelling: "WHITE LAB", "UNDERGROUND", "5 m x 5 m", "CEILING 3 m", "WALLPAPER", "CARPET", "CEILING TILE", "FLUORESCENT". Add no other text.
2. The same one small plain desk with old boxy monitor must exist in ALL photos showing its wall, consistently along the right-hand side wall in the frontal room views. Add the desk and dark monitor to the large left frontal hero, keeping it small at far right, to the first all-panels-on frontal lighting study, and to the second one-panel-dimmer frontal lighting study. Match the position, physical size and appearance already shown in the third dark monitor-only lighting study. Keep exactly one chair per room view, centered, and exactly one desk and monitor per room. Keep the hero camera and chair perfectly centered on the far wall. The desk remains on the right side wall, not centered or against the far wall.
3. In the small top-down drawing the desk is on the right/east wall. Put the ONE door on the opposite left/west wall, removing the old door swing in the top/north wall and closing that old gap with continuous wall lines. Keep the chair dot centered. Photos of the door wall still show a single closed plain flush door, without a hallway or view beyond it.
4. In the ceiling-seam close detail, make the pale hanging root unbranched, hair-thin and shorter, with no leafy or thick roots. Keep the tangled roots above the ceiling slab in the pencil underground section drawing.

Avoid: duplicate dimension labels, new text, misspellings, extra chairs, extra desks, extra monitors, duplicate doors, people in photographs, windows, skylights, glass dome, sunlight, blood, monsters, visible outdoor views, changing the board layout, thick roots inside the room, red annotations, logos, watermarks.
````

## メモ

初稿の目視検収に基づく修正。人間の評価ではない。
