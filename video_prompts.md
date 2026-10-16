# 動画生成プロンプト

『返り咲き』の動画生成用プロンプトを追記して管理します。現在のストーリーは [story.md](story.md)、画像用は [image_prompts.md](image_prompts.md) を参照してください。

現在の生成用は **VID-003：実験室のみ15秒** です。旧24秒版VID-001・VID-002は履歴として保持します。完成版の24秒と今回生成する15秒を区別してください。コピー用：[PROLOGUE_実験室のみ_15秒_プロンプトのみ.md](prompts/PROLOGUE_実験室のみ_15秒_プロンプトのみ.md)。

受領した試作カット3件（線路の導入・傷跡がない手首・指切りと花びら）は、2026-10-16（日本時間）のユーザー指定により [archive/](archive/README.md) へ保存済みです。現行の制作候補・用途の分類待ちから外し、動画用には分類していません。

## 記録ルール

- 新しいプロンプトは末尾に追記し、`VID-001` から連番を付けます。
- 修正時も旧版を残し、新しい ID のエントリーから旧 ID を参照します。
- 日付は日本時間、プロンプト本文は実際に提示・使用した全文を記録します。
- モデル、尺、縦横比、カメラ、動き、音、参照画像などは指定がある場合のみ記録します。動画の生成実行とプロンプト作成のみの状態を区別します。

## 記録形式

以下は記入用テンプレートであり、作成済みプロンプトではありません。

```markdown
### VID-連番｜タイトル

- 日付（日本時間）：
- 対象シーン・用途：
- 参照ストーリー版・更新日：
- 状態：プロンプト作成のみ／生成実行済み
- 改訂元 ID：修正版の場合のみ記載

#### プロンプト全文

（実際に提示・使用した全文）
```

## プロンプト記録

### VID-001｜PROLOGUE・24秒（共有チャット旧版の取込）

- 取込日（日本時間）：2026-10-16
- 対象：PROLOGUE 00-1〜00-6
- 参照版：前チャットでのVer.4解釈。今回の台詞・参照・人物不登場指定を反映する前の版。
- 状態：過去プロンプトの原文取込。動画生成はこの作業では未実施。現行の使用案はVID-002。
- 出典：「脚本をシーン別Klingプロンプト化」、thread ID 01a142eb-6787-7fc2-8e52-6fa2378b2dbe、最終応答のコードブロック。
- 保存元：[旧プロンプト本文](sources/2026-10-16/prologue_24s_previous_prompt_from_codex.md)。Macのファイルを直接コピーしたものではなく、チャットに記録された全文を復元。
- 生成設定（旧本文の記載）：Kling 4.0、Reference to Video、24秒、16:9。モデルの稼働・参照割当・生成結果は未検証。

#### プロンプト全文

```text
【参照素材】
ユナ：@ユナ（人物シート。身長170cm）
ミオ：@ミオ（人物シート。身長165cm）
温室：@環境ドーム（大ドームの環境シート。建築・母樹・植生の参照）
以下の本文では「ユナ」「ミオ」「温室」と記載し、この参照素材を一貫して使用する。

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

【生成設定】
Kling 4.0、Reference to Video、24秒、16:9。
PROLOGUE全体を1本の映像として1回で生成する。以下の時間指定は、この1本の内部の編集指示。別クリップには分けない。

【人物・参照・世界の固定】
ユナ：身長170cm。参照画像どおりの黒髪ボブと前髪、右頬のほくろ、生成りに近い白い長袖ロングワンピース、茶色の紐靴。
ミオ：身長165cm。参照画像どおりの乱れを残した黒髪、そばかす、耳元の赤い房状の飾り、生成りのシャツ、オリーブブラウンのサスペンダー付きパンツ、茶色の編み上げブーツ。約束の記憶の中だけに登場する。

二人の顔、髪、衣装、体格を維持する。人物シートの白背景、複数パネル、見本の立ちポーズを映像にしない。環境シートは建築・素材・植生の参考とし、画像内の人物や文字は再現しない。

舞台は平面で縦約1km、横約4kmの巨大温室。全区域の上に連続した透明なドーム型のガラス屋根がある。森、水路、橋、白い花、巨大な母樹がその内部に広がり、キメラやケンタウロスに似た多様な生物が棲息する。今回の短い記憶に映す生物は剪定獣だけに絞る。

白い研究所も温室の内側にある。継ぎ目の目立たない白壁、マットな白い床、白い椅子一脚。透明な天井のさらに上に外殻ドームがあり、引きの画面上端にガラスと遠い鉄骨の弧がわずかに見える。室内は清潔で、植物や生物を入れない。接写時も同じ屋根の下にいる空間の連続性を保つ。

【0–7秒｜問診】
50mm相当、座った人物の目線の高さ、正面固定のミディアムワイド。中央に座るユナを膝下まで収め、頭上に静かな余白。両手はそれぞれ腿の上、足は床。柔らかな拡散光。顔はわずかに焦点が甘いが、顔立ちと表情は判別できる。肌と白い布の質感を残す。

0–0.8秒は空調音と浅い呼吸だけ。
0.8–4.0秒、カメラ右側の画面外から、成人女性の研究者が落ち着いた自然な日本語で「どうされました？ 具合はどうですか」。二つの問いの間に短い間。

ユナは口を閉じたまま答えない。
4–7秒、吸いかけた息が一度だけ浅く途切れ、喉が小さく動く。瞬きはほとんどない。手や肩を大きく動かさない。カメラは動かない。

【7–9秒｜視線】
目元の極端なクローズアップへハードカット。正面からわずかに横へ寄った角度、85mmマクロ相当。カメラ固定。ユナの両眼が本人の右へ小さく急に動き、その先で焦点を結べずに止まる。眼球の動きは人体として自然な範囲。

8.5秒頃、角膜に細い赤い反射が一瞬だけ走る。虹彩そのものを発光させない。空調音が遠のき、小さな吸気が手前に聞こえる。

【9–11秒｜記憶の破片】
短い露光の断絶を伴う、4つの記憶のハードカット。連続したカメラ移動や物体の変身でつながない。

9.0–9.5秒：
24mm相当のローアングル。白い母樹と、それを覆う途方もなく大きな透明ドーム。奥へ鉄骨の反復が続く。短い上向きのティルト。遠い水音。

9.5–10.0秒：
白い花の接写。半透明の花弁の裏に細い赤い葉脈。花弁がわずかに震え、乾いた葉擦れ。

10.0–10.5秒：
濡れた石畳を這う赤い根のマクロ。表面が一度だけ膨らみ、内部の光が先端へ走る。湿った繊維の軋み。

10.5–11.0秒：
橋の高さからの広角。白く半透明で、鹿に似た長い首、六本の脚、花弁状の顔を持つ巨大な剪定獣が横から画面へ飛び込む。橋のガラス欄干に前脚が衝突し、破片が接触点から散る。上方のドーム屋根は残る。短いガラスの破砕音と非音楽的な電気ノイズ。血や負傷者は映さない。

【11–17秒｜否定】
11秒ちょうどで、最初の研究所の正面固定画面へ戻る。カメラ位置、焦点距離、椅子、手の位置、照明、構図を0–7秒と完全に一致させる。破砕音を断ち切り、同じ空調音へ戻す。

11.3–12.6秒：
先ほどと同じ女性研究者、同じ画面外の位置と声で「どうされました？」。

12.6–14.1秒：
沈黙。ユナが視線を研究者の方向へゆっくり戻す。

14.1–16.0秒：
ユナが低く自然な少女の声で「……どうもしてないです」。抑揚をほとんどつけず、小さな口の動きで話す。研究者は重ねて話さない。

16–17秒：
唇を閉じ、視線を置いたまま静止する。空調音と微かな衣擦れ。

【17–21秒｜約束の断片】
17.0–17.5秒：
幼い二人の少女が小指を重ねている、手だけの記憶。浅い被写界深度、柔らかな温室の光。顔は映さない。

17.5–18.0秒：
同じ指の位置に合わせて突然切り替える。白い研究台の上で、研究用手袋をした大人の手が少女の小指をそっと動かす。画面上端に手術灯の一部、その上方に透明な天井。医療処置や傷は映さない。手袋の擦れる音と短い電気ノイズ。

18.0–21.0秒：
温室の白い花の回廊。画面左にユナ、右にミオ。斜め横からの手元の接写。白い袖と、生成りのシャツの袖で左右を識別できる。二人がそれぞれ片手を差し出し、小指を重ねたまま、親指の腹を互いに二度だけ軽く触れ合わせる。二度の接触の間に短い間。指の接触がはっきり見える安定した画面。

接触後、最後の0.6秒だけ焦点を奥のミオの顔へ移す。耳元の赤い飾りと、小さく緩む口元。ユナの白い肩は手前に残す。背景上部にはぼけたガラス屋根の弧と植物。水路の細い水音、葉擦れ、袖の擦れる音。台詞なし。

【21–24秒｜タイトル】
21秒ちょうどで完全な黒画面にハードカットし、すべての音を止める。
黒地の中央に、静かな白文字で正確に「返り咲き」。
このタイトルだけを24秒まで保持する。文字の変形、追加文字、発光、粒子、動く背景なし。

【全編の音・連続性】
BGMなし。
劇伴、歌唱、子守歌、旋律、音楽的ドローン、音楽的な衝撃音、リズムに合わせた編集なし。

音は指定した日本語の台詞、呼吸、空調、水音、葉擦れ、衣擦れ、手袋の擦れ、根の軋み、ガラスの破砕音、短い非音楽的ノイズのみ。ノイズを長く引き延ばさず、静かな場面の小さな音が聞こえる音量にする。

指定された話者だけが話し、台詞を追加しない。研究者は画面に映さない。台詞の字幕や説明テロップなし。表示文字は最後の「返り咲き」だけ。

記憶の切り替わりは編集で表現し、顔の変形、人物の融合、衣装の変身で表現しない。手指は自然な本数と関節を保ち、接触時に融合させない。
```

### VID-002｜PROLOGUE・24秒（最新指示反映案）

- 日付（日本時間）：2026-10-16
- 対象：PROLOGUE 00-1〜00-6、1生成
- 参照ストーリー版：Ver.4＋2026-10-16の当チャット改訂。今回の指示と追加回答は [受領指示](sources/2026-10-16/prologue_revision_request.md)。
- 改訂元ID：VID-001。旧版は履歴として保持。
- 状態：プロンプト作成のみ。動画生成・結果確認は未実施。今回の新規参照画像は未取得。
- 設定：Kling 4.0、Reference to Video、24秒。16:9は前稿から引き継ぐ仮設定。
- 参照：今回の2枚目のユナ、3枚目の研究所、指定キメラ。画像未確認につき旧画像で代用しない。1枚目「ミナ」の顔・姿は使用しない。
- 追加回答で確定：シーン5は二人の手元だけで指切りを残す。
- 名前対応未確定：「ミナ」と旧脚本「ミオ」の関係は未確認。全編改名はしていない。
- 演出上の仮定：右への視線はユナ本人の右。50mm/85mm/24mmの画角、発話と細かな時間配分、タイトルのフェード時間は今回の演出案。
- 室内参照にない透明天井や外殻ドームの眺望は追加しない。温室の1km×4kmと別資料の直径2kmは未整合で、共有チャットのユーザー指定を継承。
- 各参照のメンションは冒頭に1回ずつ。生成画面で実際の素材に対応付けて使用する。
- [コピー用MD](prompts/PROLOGUE_24秒_プロンプトのみ.md)

#### プロンプト全文

```text
【参照素材】
ユナ：@ユナ（今回の2枚目。顔・髪・衣装・体格の参照）
白い研究所：@白い研究所（今回の3枚目。室内・椅子・配置・素材・照明の参照）
キメラ：@キメラ（シーン3に使用する異形生物の参照）
本文では上記の素材名だけを使い、同じ参照を全編で維持する。

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

【生成設定・全体の固定】
Kling 4.0、Reference to Video、24秒、16:9。
プロローグのシーン1〜6を、編集を含む1本の映像として1回で生成する。以下は同じ映像内の時間指定。

ユナは身長170cm。今回の人物参照の顔、髪、衣装、体格を保つ。自然な皮膚、髪、布の質感を残す。人物シートの白背景、パネル配置、見本のポーズは映像へ持ち込まない。
人物の顔と姿が明確に映るのはユナだけ。指切りの記憶は二人の手元だけを映し、相手の顔・頭・胴体は画面に入れない。

研究所は指定の室内参照に従い、壁・天井・椅子・設備・照明・距離関係を維持する。シーン1と4は、同じ場所で同じカメラが同じユナを撮っている。室内参照にない窓や天窓、ドームの眺望を加えない。環境シートの文字、寸法線、複数パネルは再現しない。
研究所の照明は室内参照を優先し、自然な肌と布の質感を保つ。温室の記憶には柔らかな拡散光を用いる。
世界全体は平面で縦約1km・横約4kmに広がる巨大温室。地上の森、水路、橋、白い花、母樹の上方には、連続した透明なドーム屋根がある。記憶の遠景にも鉄骨とガラスの奥行きを保つ。

【シーン1｜0–7秒：問診】
50mm相当、座ったユナの目線の高さ、真正面の固定カメラ。膝下まで入るミディアムワイド。椅子に座るユナの周囲に静かな余白を残す。パン、ズーム、手ブレなし。

ユナは少しだるそうに、顔と視線をやや斜め下へ向けている。表情は暗く、無機質で、感情の抜けた真顔。眉や口角で感情を強調せず、唇は軽く閉じている。両手を腿に置き、足は床につける。瞬きはほぼない。

0–1秒：微かな空調音と浅い呼吸だけ。
1–2.8秒：画面外の落ち着いた成人女性の研究者が、ナレーションのように平坦で単調な日本語で「具合はどうですか」。
2.8–7秒：ユナは答えない。目線も表情もほぼ変えず、吸いかけた息が一度だけ浅く途切れる。喉と胸がごく小さく動く。研究者の声のあとに、長く感じられる沈黙を残す。

【シーン2｜7–9秒：視線】
ユナの両目を収めた極端なクローズアップへハードカット。85mmマクロ相当、正面寄り、固定カメラ。まつ毛と角膜の反射は見えるが、ユナの視線は何にも焦点を結んでいない。

7.3秒頃、両眼だけが本人の右へ、唐突でぎこちなく動いて止まる。頭は追従しない。動きのタイミングに不自然さを感じさせ、眼球の形や位置は人体として保つ。
8.2–8.7秒、瞳の表面に細い赤い光が一瞬映り、消える。赤い光は角膜の反射として見せる。空調音が遠のき、小さな吸気だけが近くに残る。

【シーン3｜9–11秒：記憶の破片】
短いグリッチとともに、次の記憶を高速のハードカットで切り替える。瞬間的なフレームずれと露光の断絶。物体の変身や連続したカメラ移動でつながない。

9.0–9.5秒：巨大なガラス温室と母樹を見上げる24mm相当の広角。遠くまで反復する鉄骨、透明な屋根、植物の層。遠い水音。
9.5–10.0秒：白い花の接写。半透明の花弁の裏に細い赤い葉脈。微かな葉擦れ。
10.0–10.5秒：湿った地面を這う赤い根のマクロ。内部の赤い光が一度脈動する。短い湿った繊維の軋み。
10.5–11.0秒：参照したキメラが、温室内の橋の横から突然画面へ飛び込む。参照どおりの輪郭、頭部、四肢の構造、体表を維持する。身体がガラス欄干へ衝突し、接触点から破片が飛ぶ。短いガラスの破砕音と鋭い非音楽的ノイズ。屋根全体は崩落させない。

【シーン4｜11–17秒：否定】
11秒でシーン1の白い研究所へ突然戻る。カメラ位置、高さ、50mm相当の画角、椅子、設備、照明、ユナの姿勢をシーン1と一致させる。破砕音を切り、同じ微かな空調音へ戻す。

11.2–12.7秒：同じ女性研究者が同じ画面外の位置から、落ち着いた単調な声で「どうされましたか」。
12.7–14.2秒：沈黙。ユナは視線を元の斜め下へゆっくり戻す。暗い真顔のまま、口を閉じている。
14.2–16.2秒：ユナが暗いトーンの小さな声で「動揺していないです」。ほとんど抑揚をつけず、最小限の口の動きで話す。自然な日本語で、語尾を上げない。研究者は重ねて話さない。
16.2–17秒：口を閉じ、その姿勢で静止する。空調音と微かな呼吸だけ。

【シーン5｜17–21秒：約束の断片】
17.0–17.5秒：短いグリッチ。幼い少女二人の小指が重なる、手だけの接写。柔らかな温室の光。顔や体は映さない。
17.5–18.0秒：同じ指の位置に合わせたマッチカット。白い研究台。研究用手袋をした大人の手が、少女の指をそっと動かしている。手術灯が一瞬だけ画面に差し込まれる。短い電気ノイズと手袋の擦れる音。傷や医療処置は映さない。
18.0–21.0秒：柔らかな光の中で、ユナと相手の手だけへ切り替わる。小指を重ねたまま、親指の腹を互いに二度だけ軽く触れ合わせる。二度の接触の間に短い間。手指の動きが読める、安定した近接画面。最後まで手元に留まり、相手の顔へカメラや焦点を移さない。肌の接触と袖の微かな擦れ、遠い水音だけ。台詞も子守歌も入れない。

【シーン6｜21–24秒：タイトル】
21秒で完全な黒画面へ切り替わり、すべての音が途切れる。
21.0–21.3秒：無音の黒画面。
21.3–22.2秒：黒地の中央に、静かな細いオフホワイトの文字で、正確に「返り咲き」がゆっくりフェードインする。文字の位置と大きさは一定。
22.2–24.0秒：タイトルを動かさず、完全な無音のまま保持する。広い黒の余白。光のフレア、粒子、揺れ、衝撃音を加えない。

【音・台詞・連続性】
BGMなし。劇伴、歌唱、子守歌、旋律、音楽的ドローン、音楽的な盛り上げ音なし。
音は指定した日本語の台詞、呼吸、空調、衣擦れ、水音、葉擦れ、根の軋み、手袋の擦れ、ガラスの破砕音、短い非音楽的ノイズだけ。静かな場面と記憶の断絶に音量差をつける。タイトルは完全な無音。

研究者は画面外の声のみ。ユナに研究者の台詞を話させない。指定した三つの台詞以外の発話、字幕、説明テロップ、識別番号は入れない。画面文字は最後の「返り咲き」だけ。
グリッチは編集上の断絶として表現し、顔・身体・衣装の変形にしない。手指の本数と関節を保ち、指切りの接触で手を融合させない。
```


### VID-003｜PROLOGUE・実験室のみ15秒

- 日付（日本時間）：2026-10-16
- 対象：00-1 問診7秒、00-2 目元2秒、00-4 返答6秒。合計15秒・1生成。
- 参照ストーリー版：Ver.4＋当チャットのプロローグ改訂と実験室のみ生成の指示。
- 改訂元ID：VID-002。旧24秒稿は原文のまま保持。
- 状態：プロンプト作成のみ。動画生成・結果確認は未実施。
- 尺の計算：24−2−4＝18秒（タイトル込み）。「実験室のみ」という指定に合わせてタイトル3秒も別編集と解釈し、今回の生成は18−3＝15秒。完成版からのシーン削除ではない。
- 設定：Kling 4.0、Reference to Video、15秒。16:9は前稿から引き継ぐ仮設定。
- 参照：ユナ、白い研究所のみ。画像実体の未取得状態は前稿と同じ。キメラ・相手の人物参照はこの生成では使用しない。
- 台詞は前稿どおり。00-4の時間を2秒前へ移し、生成素材内9–15秒に配置。
- 連続性：同じ人物・室内・照明、正面固定→目元→同一正面固定。空調を連続させ、通常のカットで接続。
- 後編集：15秒素材を9秒で分け、そこへ00-3の2秒を挿入。実験室素材の後へ00-5の4秒とタイトル3秒を接続すると24秒。素材の生成済み・検収済みとは主張しない。
- 目元の赤い反射は実験室の動作として残す。グリッチ・指切り・キメラ・タイトル・暗転は今回の生成対象外。
- [コピー用MD](prompts/PROLOGUE_実験室のみ_15秒_プロンプトのみ.md)

#### プロンプト全文

```text
【参照素材】
ユナ：@ユナ（人物の顔・髪・衣装・体格の参照）
白い研究所：@白い研究所（室内・椅子・配置・素材・照明の参照）
以降は素材名だけを使い、同じ参照を全編で維持する。

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

【生成設定】
Kling 4.0、Reference to Video、15秒、16:9。
白い研究所での「問診7秒→目元2秒→返答6秒」を、カットを含む1本の映像として1回で生成する。全編を同じ研究所内で撮影する。

【人物・室内・連続性】
ユナは身長170cm。人物参照の顔、髪、衣装、体格を全編で維持する。肌、髪、布は自然な実写の質感。画面内の人物はユナだけ。研究者は成人女性の画面外の声のみ。

研究所は室内参照の壁、天井、椅子、設備、配置、照明、距離関係を維持する。室内参照にない窓や天窓、外の景色を加えない。共有の画風は質感と色調へ適用し、舞台はこの研究所内に固定する。人物・環境シートのパネル配置、文字、寸法線、見本のポーズは映像にしない。
冒頭と最後の正面ショットは、カメラ位置、高さ、画角、椅子の位置、背景、照明、ユナの顔の角度、手と足の位置まで一致させる。空調音はカットをまたいで同じ音量・音色で続ける。

【0–7秒｜シーン1：問診】
50mm相当。座ったユナの目線の高さ、真正面からの固定カメラ。膝下まで入るミディアムワイド。ユナの周囲に静かな余白を残す。パン、ズーム、手ブレなし。

ユナは少しだるそうに、顔と視線をやや斜め下へ向けている。暗く、無機質な真顔。眉や口角で感情を強調せず、唇は軽く閉じる。両手を腿に置き、足を床につける。瞬きはほぼない。

0–1秒：微かな空調音と浅い呼吸だけ。
1–2.8秒：画面外の落ち着いた女性研究者が、ナレーションのように平坦で単調な日本語で「具合はどうですか」。
2.8–7秒：ユナは答えない。口を動かさず、視線も表情もほぼ変えない。吸いかけた息が一度だけ浅く途切れ、喉と胸がごく小さく動く。長く感じられる沈黙。カメラは固定を保つ。

【7–9秒｜シーン2：目元】
同じユナの両目を収める極端なクローズアップへ通常のハードカット。85mmマクロ相当、正面寄りの固定カメラ。頭の角度、光の向き、肌の色を前のショットから引き継ぐ。
まつ毛と角膜の反射は見えるが、ユナの視線は何にも焦点を結んでいない。画面全体をぼかさない。

7.3秒頃、両眼だけが本人の右へ、唐突でぎこちなく動いて止まる。頭は追従しない。動きのタイミングに不自然さを感じさせ、眼球の形や位置は人体として保つ。
8.2–8.7秒、瞳の表面に細い赤い光が一瞬映り、消える。角膜上の小さな反射として見せ、虹彩そのものは発光させない。室内全体の照明や色は変わらない。
微かな空調音と小さな吸気。音楽や衝撃音は入れない。

【9–15秒｜シーン4：返答】
9秒で、冒頭と完全に同じ正面固定のミディアムワイドへ通常のハードカット。研究所の位置関係、50mm相当の画角、ユナの姿勢、両手、足、背景、露出を一致させる。空調音を途切れさせない。

9.2–10.7秒：同じ女性研究者が、同じ画面外の位置と単調な声で「どうされましたか」。
10.7–12.2秒：沈黙。ユナの視線が元の斜め下へゆっくり戻る。顔は暗い真顔のまま、口は閉じている。
12.2–14.2秒：ユナが暗いトーンの小さな声で「動揺していないです」。ほとんど抑揚をつけず、最小限の口の動きで、自然な日本語を話す。語尾を上げない。研究者は重ねて話さない。
14.2–15秒：ユナは口を閉じ、同じ姿勢と表情で静止する。微かな呼吸と空調音を保ち、その正面画面のまま終える。

【音・制約】
BGMなし。劇伴、歌唱、子守歌、旋律、音楽的ドローンなし。
音は指定した日本語の台詞、微かな呼吸、空調、自然な衣擦れだけ。研究者の声は画面外の同じ位置から聞こえ、ユナの声と明確に区別する。
指定した三つの台詞以外の発話なし。研究者の台詞中、ユナは口を動かさない。

全編で研究所の空間とユナの外見を維持する。グリッチ、記憶映像、指切り、キメラ、温室への場面転換、ガラスの破砕、電気ノイズを入れない。
タイトル、字幕、テロップ、識別番号、画面文字なし。冒頭や末尾の黒画面、暗転、フェードなし。顔・身体・衣装を変形させない。
```

### VID-004｜PROLOGUE・実験室のみ15秒（参照素材の固定文・研究室シート・蛍光灯点滅を反映）

- 日付（日本時間）：2026-10-16
- 対象：cut1。00-1 問診7秒、00-2 目元2秒、00-4 返答6秒。合計15秒・1生成。
- 参照ストーリー版：Ver.4＋2026-10-16 の会話での改訂（実験室のみ15秒、研究室の環境シート、蛍光灯の激しい点滅、参照素材の固定文）。
- 改訂元ID：VID-003。台詞・時間配分の骨格は VID-003 を引き継ぐ。
- 状態：プロンプト作成のみ。動画生成・結果確認は未実施。
- 生成環境（ユーザー指定）：Tapnow 上の Kling 4.0、Omni Reference。参照画像は人物シートと研究室の環境シート。縦横比は未指定のため本文に記載しない。
- VID-003 からの変更：
  - 冒頭の参照をユーザー指定の固定文の全文へ差し替え、白い研究所の環境シートを {{Image 4}} として追記。{{Image 4}} は今回の割り当て案で、実際の番号は生成画面で対応付ける。
  - 受領した環境シートの室内仕様を本文に明記。
  - 蛍光灯が時に激しく点滅する指定を追加。点滅の位置（4.5–5.3秒と14.2–15秒）、目元ショットでは点滅させないこと、ユナが点滅に反応しないことは今回の演出案。
  - 正面ショットを50mm相当から35mm相当へ変更し、天井の蛍光灯と右壁の机・モニターを画面に入れる（演出案）。
  - 点滅時の電気ノイズを許可。
- ユナの最新人物シートの画像実体は、このリポジトリでは未取得。
- [コピー用MD](prompts/CUT01_実験室15秒_VID-004_プロンプトのみ.md)

#### プロンプト全文

```text
【参照素材】

ユナ：{{Image 2}} （人物シート。身長170cm）

ミオ：{{Image 1}} （人物シート。身長165cm）

温室：{{Image 3}} （大ドームの環境シート。建築・母樹・植生の参照）

以下の本文では「ユナ」「ミオ」「温室」と記載し、この参照素材を一貫して使用する。

白い研究所：{{Image 4}} （研究室の環境シート。室内・椅子・机・モニター・素材・照明の参照）
本文では「白い研究所」と記載する。

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

【生成設定】
Kling 4.0、Omni Reference、15秒。
白い研究所での「問診7秒→目元2秒→返答6秒」を、カットを含む1本の映像として1回で生成する。全編を同じ研究所内で撮影する。登場人物はユナだけ。ミオと温室はこの映像に登場させない。

【人物】
ユナの顔、黒髪のボブと前髪、右頬の小さなほくろ、衣装、体格を人物シートどおりに全編で維持する。身長170cmの細身の少女として、椅子との比率を自然にする。肌、髪、布は自然な実写の質感。研究者は成人女性の画面外の声のみ。人物シートの白背景、パネル配置、見本のポーズは映像にしない。

【空間】
白い研究所の環境シートの室内をそのまま使う。地下の窓のない密閉室で、床は5m×5m、天井高3m。黄ばんだオフホワイトの壁紙、継ぎ目の浮きと天井近くの水染み、湿ったベージュのカーペット、吊り天井と蛍光灯パネル4枚、換気口とスピーカー。部屋の中央に椅子1脚。正面から見て右の壁際に小さな机と古い箱型モニター（画面は暗い）。天井の隅の継ぎ目から、細く短い淡色の根が1本だけ垂れている。
窓、天窓、ドーム、空、外の眺望、植物の葉、追加の家具、ほかの人物は加えない。環境シートの文字、寸法線、図面、複数パネルは再現しない。

【照明】
研究所の照明は環境シートを優先する。上からの平坦で影の少ない、病的な黄緑色の蛍光灯。自然光はない。肌と布の質感は自然に残す。
蛍光灯は普段は微かに唸りながら点いているが、時に激しく点滅する。点滅の瞬間は複数のパネルが不規則に明滅し、部屋が一瞬ほぼ暗くなってはすぐ戻る。点滅は照明の変化だけで表し、カメラ、構図、ユナの姿を崩さない。蛍光灯が激しく点滅しても、ユナはまったく反応せず、顔も視線も向けない。

【連続性】
冒頭と最後の正面ショットは、カメラ位置、高さ、画角、椅子の位置、背景、照明、ユナの顔の角度、手と足の位置まで一致させる。空調音と蛍光灯の唸りは、カットをまたいで同じ音量・音色で続ける。

【0–7秒｜シーン1：問診】
座ったユナの目線の高さから、真正面の固定カメラ。35mm相当のやや広めの画角で、ほぼ左右対称。ユナと椅子を画面中央に置き、全身と足元のカーペット、奥の壁、上辺の天井グリッドと蛍光灯パネル、右端の机とモニターが入る。周囲の壁に大きな余白を残す。パン、ズーム、ドリー、手ブレなし。

ユナは少しだるそうに、顔と視線をやや斜め下へ向けて座っている。暗く無機質な真顔。眉や口角で感情を強調せず、唇は軽く閉じる。両手は腿の上、足は床につける。瞬きはほぼない。

0–1秒：蛍光灯の唸りと空調音、浅い呼吸だけ。
1–2.8秒：画面外の落ち着いた女性研究者が、ナレーションのように平坦で単調な日本語で「具合はどうですか」。
2.8–4.5秒：ユナは答えない。口を動かさず、視線も表情もほぼ変えない。吸いかけた息が一度だけ浅く途切れ、喉と胸がごく小さく動く。
4.5–5.3秒：蛍光灯が突然激しく点滅する。唸りが途切れ、電気的なパチパチという音。すぐに元の明るさへ戻る。ユナは動かない。
5.3–7秒：長く感じられる沈黙。蛍光灯の唸りと空調音だけ。

【7–9秒｜シーン2：目元】
同じユナの両目を収める極端なクローズアップへ通常のハードカット。85mmマクロ相当、正面寄りの固定カメラ。頭の角度、蛍光灯の光の向き、肌の色を前のショットから引き継ぐ。
まつ毛と角膜の反射は見えるが、ユナの視線は何にも焦点を結んでいない。画面全体をぼかさない。

7.3秒頃、両眼だけが本人の右へ、唐突でぎこちなく動いて止まる。頭は追従しない。動きのタイミングに不自然さを感じさせ、眼球の形や位置は人体として保つ。
8.2–8.7秒、瞳の表面に細い赤い光が一瞬映り、消える。角膜上の小さな反射として見せ、虹彩そのものは発光させない。このショットでは蛍光灯を点滅させず、室内の照明や色を変えない。
蛍光灯の唸り、空調音、小さな吸気。音楽や衝撃音は入れない。

【9–15秒｜シーン4：返答】
9秒で、冒頭と完全に同じ正面固定のショットへ通常のハードカット。35mm相当の画角、研究所の位置関係、ユナの姿勢、両手、足、背景、露出を一致させる。空調音と蛍光灯の唸りを途切れさせない。

9.2–10.7秒：同じ女性研究者が、同じ画面外の位置と単調な声で「どうされましたか」。
10.7–12.2秒：沈黙。ユナの視線が元の斜め下へゆっくり戻る。顔は暗い真顔のまま、口は閉じている。
12.2–14.2秒：ユナが暗いトーンの小さな声で「動揺していないです」。ほとんど抑揚をつけず、最小限の口の動きで、自然な日本語を話す。語尾を上げない。研究者は重ねて話さない。
14.2–15秒：ユナは口を閉じ、同じ姿勢と表情で静止する。言い終えた直後、蛍光灯が一度だけ短く激しく点滅して元に戻り、その正面画面のまま終える。

【音・制約】
BGMなし。劇伴、歌唱、子守歌、旋律、音楽的ドローンなし。
音は指定した日本語の台詞、微かな呼吸、空調音、蛍光灯の唸りと点滅時の電気ノイズ、自然な衣擦れだけ。研究者の声は画面外の同じ位置から聞こえ、ユナの声と明確に区別する。
指定した三つの台詞以外の発話なし。研究者の台詞中、ユナは口を動かさない。

全編で研究所の空間とユナの外見を維持する。グリッチ、記憶映像、指切り、キメラ、温室への場面転換、ガラスの破砕を入れない。
タイトル、字幕、テロップ、識別番号、画面文字なし。モニターは暗いまま文字を出さない。冒頭や末尾の黒画面、暗転、フェードなし。顔・身体・衣装を変形させない。手指の本数と関節を保つ。
```

### VID-005｜PROLOGUE・実験室のみ15秒（7ショット構成・一人称視点・暗めの雰囲気・自然なちらつき）

- 日付（日本時間）：2026-10-16
- 対象：cut1。PROLOGUE の実験室部分（00-1・00-2・00-4 の内容）を15秒・1生成。
- 参照ストーリー版：Ver.4＋2026-10-16 の会話での改訂（下記のショット構成・雰囲気の指定を含む）。
- 改訂元ID：VID-004。
- 状態：プロンプト作成のみ。動画生成・結果確認は未実施。
- 生成環境（ユーザー指定）：Tapnow 上の Kling 4.0、Omni Reference。参照画像は人物シートと研究室の環境シート。縦横比は未指定。
- ユーザー指定の変更点：
  - アップから始め、次のカットでさらに寄り（ドアップ）、最後に引きの映像で終える。間に真横・手元・監視カメラ風のカットを挟む。
  - 最初の5秒ほど、ユナはうなだれて目の焦点が合っていない。
  - ユナの一人称視点を入れる。視界が少しぼやけ、視線が定まらずさまよい、頭がぐるぐる回るような感じ。
  - もっと雰囲気のある映像にする。明るすぎず、キャラクターが背景から浮かないようにする。
  - 蛍光灯の点滅をより自然にする。
- 今回の演出案（ユーザー未確認）：7ショットの秒割り（アップ0–4.5／目元4.5–6.3／真横6.3–7.5／手元7.5–8.5／一人称8.5–10.5／監視カメラ10.5–12.3／引き12.3–15）、2つ目の質問を監視カメラのショットに置きスピーカーからの声にすること、一人称視点の間は音をこもらせること、引きでユナが顔をわずかに上げてから答えること、ちらつきを1枚の古い管の不規則な瞬きにして位置を3.5秒頃と14.6秒以降にすること。
- 一人称視点の見え方は、ユーザーの説明にあった病名をプロンプトに書かず、ぼやけ・さまよう視線・回転するめまいの視覚表現として記述した。
- 従来の「冒頭と最後を同じ正面固定ショットにする」連続性は、このショット構成の指定により今回は適用しない。
- ユナの最新人物シートの画像実体は、このリポジトリでは未取得。
- [コピー用MD](prompts/CUT01_実験室15秒_VID-005_プロンプトのみ.md)

#### プロンプト全文

```text
【参照素材】

ユナ：{{Image 2}} （人物シート。身長170cm）

ミオ：{{Image 1}} （人物シート。身長165cm）

温室：{{Image 3}} （大ドームの環境シート。建築・母樹・植生の参照）

以下の本文では「ユナ」「ミオ」「温室」と記載し、この参照素材を一貫して使用する。

白い研究所：{{Image 4}} （研究室の環境シート。室内・椅子・机・モニター・素材・照明の参照）
本文では「白い研究所」と記載する。

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

【生成設定】
Kling 4.0、Omni Reference、15秒。
白い研究所でのユナの問診を、7つのショットをハードカットでつないだ1本の映像として1回で生成する。全編を同じ研究所内で撮影する。登場人物はユナだけ。ミオと温室はこの映像に登場させない。
ショットの流れは「アップ → 目元のドアップ → 真横 → 手元 → ユナの一人称視点 → 監視カメラ → 引き」。寄りから始めてさらに寄り、最後に初めて部屋全体を見せる。

【人物】
ユナの顔、黒髪のボブと前髪、右頬の小さなほくろ、衣装、体格を人物シートどおりに全編で維持する。身長170cmの細身の少女として、椅子との比率を自然にする。研究者は成人女性の画面外の声のみ。人物シートの白背景、パネル配置、見本のポーズは映像にしない。

【空間】
白い研究所の環境シートの室内をそのまま使う。地下の窓のない密閉室で、床は5m×5m、天井高3m。黄ばんだオフホワイトの壁紙、継ぎ目の浮きと天井近くの水染み、湿ったベージュのカーペット、吊り天井と蛍光灯パネル4枚、換気口とスピーカー。部屋の中央に椅子1脚。正面から見て右の壁際に小さな机と古い箱型モニター（画面は暗い）。天井の隅の継ぎ目から、細く短い淡色の根が1本だけ垂れている。
窓、天窓、ドーム、空、外の眺望、植物の葉、追加の家具、ほかの人物は加えない。環境シートの文字、寸法線、図面、複数パネルは再現しない。

【映像の雰囲気と照明】
このシーンの照明と質感は以下を優先する。全体を暗めに、重く湿った空気感で撮る。明るく均一な画にしない。
光源は天井の古い蛍光灯だけ。くすんだ黄緑色の弱い光で、部屋の隅、壁の上部、カーペットの奥へ向かって暗く沈む。影は柔らかく、ユナの眼窩、首の下、椅子の下に深い影が落ちる。白い部分も白飛びさせず、くすんだ灰色がかったオフホワイトに抑える。空気中にごく薄い埃が漂う。
ユナを部屋の光の中に溶け込ませる。ユナの顔、髪、白い服にも同じ黄緑色の蛍光灯の色かぶりと同じ明るさを当て、服は真っ白に光らせない。椅子とカーペットの接地面に接地影を出す。人物だけのライティング、輪郭を縁取る光、美肌の補正、背景からの切り抜きのような見え方にしない。人物と背景に同じ粒子、同じ柔らかさ、同じ露出を適用する。
古い家庭用ビデオカメラのような控えめなソフトさ、低いコントラストの暗部、薄いノイズ。

【蛍光灯のちらつき】
蛍光灯は古く、普段は低く唸りながらわずかに不安定に点いている。時々、4枚のうち1枚だけが寿命の近い管のように不規則にちらつく。数回すばやく瞬いて少し暗くなり、安定器のジジッという音とともに元に戻る。ほかのパネルは点いたまま。部屋は真っ暗にならず、点滅のリズムは規則的にしない。ちらつきに合わせて、ユナの顔と壁の明るさもほんのわずかに揺れる。演出的なストロボや全灯の点滅にしない。ユナはちらつきにまったく反応しない。

【0–4.5秒｜ショット1：アップ】
ユナの胸から上のアップ。座ったユナの目線よりわずかに上からの固定カメラ、ほぼ正面。パン、ズーム、手ブレなし。
ユナはうなだれている。首の力が抜けて頭が前に落ち、前髪が目元に少しかかる。視線は下へ落ち、目の焦点がまったく合っていない。暗く無機質な真顔。唇は軽く閉じる。瞬きはほぼない。
0–1秒：蛍光灯の唸り、空調音、浅い呼吸だけ。
1–2.8秒：画面外の落ち着いた女性研究者が、ナレーションのように平坦で単調な日本語で「具合はどうですか」。
2.8–4.5秒：ユナは答えない。口を動かさず、うなだれたまま。吸いかけた息が一度だけ浅く途切れ、喉がごく小さく動く。3.5秒頃、背後の蛍光灯の1枚が数回ちらつき、顔の明るさがわずかに揺れて戻る。

【4.5–6.3秒｜ショット2：目元のドアップ】
ユナの両目を収める極端なクローズアップへハードカット。85mmマクロ相当、正面寄りの固定カメラ。うなだれたままの角度で、前髪の影が目元にかかり、蛍光灯の弱い光が角膜に小さく映る。視線は何にも焦点を結んでいない。
4.8秒頃、両眼だけが本人の右へ、唐突でぎこちなく動いて止まる。頭は追従しない。眼球の形や位置は人体として保つ。
5.5–6.0秒、瞳の表面に細い赤い光が一瞬映り、消える。角膜上の小さな反射として見せ、虹彩そのものは発光させない。このショットでは蛍光灯をちらつかせない。

【6.3–7.5秒｜ショット3：真横】
ユナの真横からのミディアムショットへハードカット。座った腰の高さの固定カメラ。うなだれた頭、丸まった背中、膝の上の手、椅子の輪郭が横から見える。背景は暗く沈む黄ばんだ壁。沈黙。ユナは動かない。

【7.5–8.5秒｜ショット4：手元】
腿の上に置かれたユナの両手のクローズアップへハードカット。指は力なく揃い、白い服の布地が膝の上でわずかに皺をつくる。人差し指だけがごく小さく一度ぴくりと動く。手指の本数と関節を保つ。微かな衣擦れ。

【8.5–10.5秒｜ショット5：ユナの一人称視点】
ユナの目から見た一人称視点へハードカット。手持ちのような不安定なカメラ。
視界は少しぼやけ、焦点が合いそうで合わずに揺れ続ける。視線が定まらず、部屋の中をあてもなくさまよう。膝の上の自分の手、湿ったカーペット、黄ばんだ壁の模様、右の壁際の暗いモニター、天井の蛍光灯パネルへと、ゆっくり、ときに不意に流れていく。
頭がぐらりと回るように、視界全体がゆっくり傾き、ぐるりと回り込むように揺れる。水平が保てず、めまいのように画面がわずかに回転する。蛍光灯を見上げた瞬間に光がにじみ、視界の端が暗くかすむ。
ユナの体は手の一部しか映らない。音はこもり、空調音と蛍光灯の唸りが遠く、くぐもって聞こえる。自分の呼吸だけが近い。

【10.5–12.3秒｜ショット6：監視カメラ】
天井の隅に設置された監視カメラの映像へハードカット。部屋を高い角から見下ろす広角の固定画角で、椅子にうなだれて座るユナが小さく映る。低画質の監視映像らしく、粗いノイズ、わずかな走査線、にじみ、暗部のつぶれ、やや歪んだ広角。画面上の文字、時刻表示、録画マークは入れない。
10.6–12.1秒：同じ女性研究者が同じ単調な声で「どうされましたか」。声は天井のスピーカーから鳴っているように、わずかにこもって聞こえる。ユナは動かない。

【12.3–15秒｜ショット7：引き】
初めて部屋全体を見せる引きのショットへハードカット。環境シートの主画と同じ構図。座ったユナの目線の高さから、真正面の固定カメラ、35mm相当、ほぼ左右対称。椅子に座るユナを画面中央に小さく置き、奥の壁、天井の蛍光灯パネル、右の壁際の机とモニター、湿ったカーペットが入る。暗い部屋の中にユナが孤立して見える。
12.3–12.9秒：沈黙。ユナがゆっくりと顔をわずかに上げる。焦点は合わないまま。
12.9–14.6秒：ユナが暗いトーンの小さな声で「動揺していないです」。ほとんど抑揚をつけず、最小限の口の動きで、自然な日本語を話す。語尾を上げない。研究者は重ねて話さない。
14.6–15秒：ユナは口を閉じ、そのまま静止する。奥の蛍光灯の1枚が短くちらついて落ち着き、その画面のまま終える。

【音・制約】
BGMなし。劇伴、歌唱、子守歌、旋律、音楽的ドローンなし。
音は指定した日本語の台詞、微かな呼吸、空調音、蛍光灯の低い唸りとちらつき時の安定器の小さな音、自然な衣擦れだけ。ショットが変わっても空調音と蛍光灯の唸りは途切れずに続く（一人称視点の間だけ、こもって遠く聞こえる）。
指定した三つの台詞以外の発話なし。研究者の台詞中、ユナは口を動かさない。

全編で研究所の空間、照明の色、ユナの外見と衣装を維持する。グリッチ、記憶映像、指切り、キメラ、温室への場面転換、ガラスの破砕を入れない。
タイトル、字幕、テロップ、識別番号、画面文字なし。モニターは暗いまま文字を出さない。冒頭や末尾の黒画面、暗転、フェードなし。顔・身体・衣装を変形させない。手指の本数と関節を保つ。
```

### VID-006｜PROLOGUE・実験室のみ15秒（人間らしい微細な動き・左右で違う瞳孔・重いまぶた）

- 日付（日本時間）：2026-10-16
- 対象：cut1。PROLOGUE の実験室部分を15秒・1生成。
- 参照ストーリー版：Ver.4＋2026-10-16 の会話での改訂。
- 改訂元ID：VID-005。ショット構成・照明・ちらつき・台詞と秒割りは VID-005 を維持。
- 状態：プロンプト作成のみ。動画生成・結果確認は未実施。
- 生成環境（ユーザー指定）：Tapnow 上の Kling 4.0、Omni Reference。縦横比は未指定。
- ユーザー指定の変更点（feedback.md FB-012・FB-013）：
  - さりげない人間らしい動きをさせる。
  - 虹彩と瞳孔まで見えるようにし、左右の瞳孔の開き方を違くする。まぶたが若干落ちそうな感じにする。
- 今回の演出案（ユーザー未確認）：本人の右目の瞳孔を小さく、左目を大きくした向き。微細な動きの内容（呼吸の上下、頭の揺れ、嚥下、指先、髪の揺れ）。「瞬きはほぼない」を「少なく、ゆっくり重い瞬き」に変え、目元のドアップ冒頭と最後に重い瞬きを置いたこと。
- [コピー用MD](prompts/CUT01_実験室15秒_VID-006_プロンプトのみ.md)

#### プロンプト全文

```text
【参照素材】

ユナ：{{Image 2}} （人物シート。身長170cm）

ミオ：{{Image 1}} （人物シート。身長165cm）

温室：{{Image 3}} （大ドームの環境シート。建築・母樹・植生の参照）

以下の本文では「ユナ」「ミオ」「温室」と記載し、この参照素材を一貫して使用する。

白い研究所：{{Image 4}} （研究室の環境シート。室内・椅子・机・モニター・素材・照明の参照）
本文では「白い研究所」と記載する。

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

【生成設定】
Kling 4.0、Omni Reference、15秒。
白い研究所でのユナの問診を、7つのショットをハードカットでつないだ1本の映像として1回で生成する。全編を同じ研究所内で撮影する。登場人物はユナだけ。ミオと温室はこの映像に登場させない。
ショットの流れは「アップ → 目元のドアップ → 真横 → 手元 → ユナの一人称視点 → 監視カメラ → 引き」。寄りから始めてさらに寄り、最後に初めて部屋全体を見せる。

【人物】
ユナの顔、黒髪のボブと前髪、右頬の小さなほくろ、衣装、体格を人物シートどおりに全編で維持する。身長170cmの細身の少女として、椅子との比率を自然にする。
全編でユナに、さりげない人間らしい動きを残す。完全に静止させず、呼吸に合わせた胸と肩のごく小さな上下、首と頭のわずかな揺れ、ときどきの小さな嚥下、指先の微かな動き、前髪や髪の毛先の微かな揺れを自然に続ける。動きは小さく不規則で、意識的な演技やポーズに見せない。
【目の状態】
ユナの目は、虹彩の模様と瞳孔の輪郭がはっきり見えるように映す。左右の瞳孔の開き方が違い、本人の右目の瞳孔は小さく収縮し、左目の瞳孔は大きく開いている。左右の差は目元に寄ると分かる程度に、自然な範囲で保つ。まぶたは重く、上まぶたが瞳の上部にわずかにかかり、今にも落ちそうな半ば閉じかけた状態を保つ。ときどき、ゆっくりと重い瞬きをし、まぶたが一瞬落ちかけてから、また重たげに持ち上がる。
研究者は成人女性の画面外の声のみ。人物シートの白背景、パネル配置、見本のポーズは映像にしない。

【空間】
白い研究所の環境シートの室内をそのまま使う。地下の窓のない密閉室で、床は5m×5m、天井高3m。黄ばんだオフホワイトの壁紙、継ぎ目の浮きと天井近くの水染み、湿ったベージュのカーペット、吊り天井と蛍光灯パネル4枚、換気口とスピーカー。部屋の中央に椅子1脚。正面から見て右の壁際に小さな机と古い箱型モニター（画面は暗い）。天井の隅の継ぎ目から、細く短い淡色の根が1本だけ垂れている。
窓、天窓、ドーム、空、外の眺望、植物の葉、追加の家具、ほかの人物は加えない。環境シートの文字、寸法線、図面、複数パネルは再現しない。

【映像の雰囲気と照明】
このシーンの照明と質感は以下を優先する。全体を暗めに、重く湿った空気感で撮る。明るく均一な画にしない。
光源は天井の古い蛍光灯だけ。くすんだ黄緑色の弱い光で、部屋の隅、壁の上部、カーペットの奥へ向かって暗く沈む。影は柔らかく、ユナの眼窩、首の下、椅子の下に深い影が落ちる。白い部分も白飛びさせず、くすんだ灰色がかったオフホワイトに抑える。空気中にごく薄い埃が漂う。
ユナを部屋の光の中に溶け込ませる。ユナの顔、髪、白い服にも同じ黄緑色の蛍光灯の色かぶりと同じ明るさを当て、服は真っ白に光らせない。椅子とカーペットの接地面に接地影を出す。人物だけのライティング、輪郭を縁取る光、美肌の補正、背景からの切り抜きのような見え方にしない。人物と背景に同じ粒子、同じ柔らかさ、同じ露出を適用する。
古い家庭用ビデオカメラのような控えめなソフトさ、低いコントラストの暗部、薄いノイズ。

【蛍光灯のちらつき】
蛍光灯は古く、普段は低く唸りながらわずかに不安定に点いている。時々、4枚のうち1枚だけが寿命の近い管のように不規則にちらつく。数回すばやく瞬いて少し暗くなり、安定器のジジッという音とともに元に戻る。ほかのパネルは点いたまま。部屋は真っ暗にならず、点滅のリズムは規則的にしない。ちらつきに合わせて、ユナの顔と壁の明るさもほんのわずかに揺れる。演出的なストロボや全灯の点滅にしない。ユナはちらつきにまったく反応しない。

【0–4.5秒｜ショット1：アップ】
ユナの胸から上のアップ。座ったユナの目線よりわずかに上からの固定カメラ、ほぼ正面。パン、ズーム、手ブレなし。
ユナはうなだれている。首の力が抜けて頭が前に落ち、前髪が目元に少しかかる。視線は下へ落ち、目の焦点がまったく合っていない。まぶたは重く落ちかけている。暗く無機質な真顔。唇は軽く閉じる。瞬きは少なく、するときはゆっくりと重い。呼吸に合わせて肩がごく小さく上下し、頭がわずかに揺れる。
0–1秒：蛍光灯の唸り、空調音、浅い呼吸だけ。
1–2.8秒：画面外の落ち着いた女性研究者が、ナレーションのように平坦で単調な日本語で「具合はどうですか」。
2.8–4.5秒：ユナは答えない。口を動かさず、うなだれたまま。吸いかけた息が一度だけ浅く途切れ、喉がごく小さく動く。3.5秒頃、背後の蛍光灯の1枚が数回ちらつき、顔の明るさがわずかに揺れて戻る。

【4.5–6.3秒｜ショット2：目元のドアップ】
ユナの両目を収める極端なクローズアップへハードカット。85mmマクロ相当、正面寄りの固定カメラ。うなだれたままの角度で、前髪の影が目元にかかるが、両目の虹彩の模様と瞳孔の輪郭ははっきり見える。蛍光灯の弱い光が角膜に小さく映る。本人の右目の瞳孔は小さく、左目の瞳孔は大きく開き、左右の違いがこのショットで分かる。上まぶたは重く垂れ、瞳の上部にわずかにかかっている。視線は何にも焦点を結んでいない。
4.5–4.8秒、まぶたがゆっくり少し落ちかけて、また重たげに持ち上がる。
4.8秒頃、両眼だけが本人の右へ、唐突でぎこちなく動いて止まる。頭は追従しない。眼球の形や位置は人体として保つ。
5.5–6.0秒、瞳の表面に細い赤い光が一瞬映り、消える。角膜上の小さな反射として見せ、虹彩そのものは発光させない。このショットでは蛍光灯をちらつかせない。

【6.3–7.5秒｜ショット3：真横】
ユナの真横からのミディアムショットへハードカット。座った腰の高さの固定カメラ。うなだれた頭、丸まった背中、膝の上の手、椅子の輪郭が横から見える。背景は暗く沈む黄ばんだ壁。沈黙。ユナは大きくは動かないが、呼吸で背中と肩がわずかに上下し、喉が一度小さく動く。

【7.5–8.5秒｜ショット4：手元】
腿の上に置かれたユナの両手のクローズアップへハードカット。指は力なく揃い、白い服の布地が膝の上でわずかに皺をつくる。人差し指だけがごく小さく一度ぴくりと動く。手指の本数と関節を保つ。微かな衣擦れ。

【8.5–10.5秒｜ショット5：ユナの一人称視点】
ユナの目から見た一人称視点へハードカット。手持ちのような不安定なカメラ。
視界は少しぼやけ、焦点が合いそうで合わずに揺れ続ける。視線が定まらず、部屋の中をあてもなくさまよう。膝の上の自分の手、湿ったカーペット、黄ばんだ壁の模様、右の壁際の暗いモニター、天井の蛍光灯パネルへと、ゆっくり、ときに不意に流れていく。
頭がぐらりと回るように、視界全体がゆっくり傾き、ぐるりと回り込むように揺れる。水平が保てず、めまいのように画面がわずかに回転する。蛍光灯を見上げた瞬間に光がにじみ、視界の端が暗くかすむ。
ユナの体は手の一部しか映らない。音はこもり、空調音と蛍光灯の唸りが遠く、くぐもって聞こえる。自分の呼吸だけが近い。

【10.5–12.3秒｜ショット6：監視カメラ】
天井の隅に設置された監視カメラの映像へハードカット。部屋を高い角から見下ろす広角の固定画角で、椅子にうなだれて座るユナが小さく映る。ユナの頭がごくわずかに揺れている。低画質の監視映像らしく、粗いノイズ、わずかな走査線、にじみ、暗部のつぶれ、やや歪んだ広角。画面上の文字、時刻表示、録画マークは入れない。
10.6–12.1秒：同じ女性研究者が同じ単調な声で「どうされましたか」。声は天井のスピーカーから鳴っているように、わずかにこもって聞こえる。ユナは顔を上げない。

【12.3–15秒｜ショット7：引き】
初めて部屋全体を見せる引きのショットへハードカット。環境シートの主画と同じ構図。座ったユナの目線の高さから、真正面の固定カメラ、35mm相当、ほぼ左右対称。椅子に座るユナを画面中央に小さく置き、奥の壁、天井の蛍光灯パネル、右の壁際の机とモニター、湿ったカーペットが入る。暗い部屋の中にユナが孤立して見える。
12.3–12.9秒：沈黙。ユナがゆっくりと顔をわずかに上げ、小さく息を吸う。焦点は合わず、まぶたは重いまま。
12.9–14.6秒：ユナが暗いトーンの小さな声で「動揺していないです」。ほとんど抑揚をつけず、最小限の口の動きで、自然な日本語を話す。語尾を上げない。研究者は重ねて話さない。
14.6–15秒：ユナは口を閉じ、ゆっくり一度重い瞬きをする。奥の蛍光灯の1枚が短くちらついて落ち着き、その画面のまま終える。

【音・制約】
BGMなし。劇伴、歌唱、子守歌、旋律、音楽的ドローンなし。
音は指定した日本語の台詞、微かな呼吸、空調音、蛍光灯の低い唸りとちらつき時の安定器の小さな音、自然な衣擦れだけ。ショットが変わっても空調音と蛍光灯の唸りは途切れずに続く（一人称視点の間だけ、こもって遠く聞こえる）。
指定した三つの台詞以外の発話なし。研究者の台詞中、ユナは口を動かさない。

全編で研究所の空間、照明の色、ユナの外見と衣装を維持する。グリッチ、記憶映像、指切り、キメラ、温室への場面転換、ガラスの破砕を入れない。
タイトル、字幕、テロップ、識別番号、画面文字なし。モニターは暗いまま文字を出さない。冒頭や末尾の黒画面、暗転、フェードなし。顔・身体・衣装を変形させない。手指の本数と関節を保つ。
```
