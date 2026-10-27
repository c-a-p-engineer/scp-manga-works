# 「SCPと一服」シリーズ標準ビジュアル v2.0

- **status**: author-approved / active
- **effective**: 2026-10-26
- **scope**: 本シリーズの新規漫画、幕間、キャラクター演技・塗り・背景演出
- **supersedes**: 2026-10-12の「低彩度グレースケール主体」の既定彩色。旧方針は履歴として [PIXIV_PUBLICATION_TEMPLATE.md](PIXIV_PUBLICATION_TEMPLATE.md) に保存
- **reference**: 2026-10-26にマスターが「いいね。絵柄とこの塗りを標準にしたい」と承認した **EP015 / SCP-914 幕間「喫煙革命」再生成候補**
- **reference generation ID**: `07a13ea9-3c34-4765-aee7-8908675396d6`
- **reference image SHA-256**: `1340fb614b09c817b05b5eb1609da4f5565aa6bceb6fbd3db5b54046fb66521b` (1024 × 1536 PNG)
- **reference image (adopted)**: [EP015 幕間「喫煙革命」P001](../episodes/EP015_SCP-914/interlude/images/final/P001.png)（2026-10-27アップロード、前述のSHA-256と一致。元画像を無加工で保存）。
- **image-use boundary**: このPNGはシリーズの絵柄・塗り・背景密度の実画像参照。画像生成時は実体PNGを提供すること。Character Sheetの人物同一性や作品ごとのネームを上書きしない。

## 目的と境界

**「読みやすい漫画絵 ＋ 上品なライトセル塗り」**をシリーズの既定にする。キャラクターの承認済み同一性、各話の台詞・ネーム・右→左の読順、SCPの原典、実際のストーリーが優先。**採用画像を丸ごと次話へ複製しない**。特に「喫煙革命」由来の群衆、スローガン、帽子、タバコ、コマ構成、特定の表情をすべての話に自動継承してはいけない。

### 1. 顔・線画

- クリーンな現代アニメ／漫画の線。人物の輪郭・瞳・表情・手を明瞭にし、少しだけ自然な線幅差を残す。
- 顔の同一性・年齢感・髪型・体格は [ゴールディ](../characters/CHAR-001_BAT_REFERENCE.md)、[七星](../characters/CHAR-002_SETTER_REFERENCE.md)、他の各Character Sheetと承認済み参照PNGを優先。画風が別人化を許すことはない。
- ゴールディ：深紅の目、金髪ハーフアップ、気だるいジト目を基本に、企み・歓喜・軽蔑等は意図的にデフォルメ可能。**邪悪可愛い**表情では目尻と口角を変え、無邪気さの中に悪巧みを見せる。過度な色気や幼児化で代用しない。
- 七星：四角い眼鏡、短い無精髭、こめかみの微かな白髪、**熊のように肩幅・胸・腕の厚い大柄な体格**。細身の若い男性へ寄せない。
- 髪束は不透明。目・皮膚や背景が髪の内部に透けない。

### 2. 塗りと色

- **落ち着いたフルカラーを既定**：金髪／赤目／白衣／濃紺・黒い衣装を区別する。2026-10-12のモノクロ主体は以降の既定ではない。
- **セル塗り寄りの明瞭な面と少数の柔らかい陰影**。完全フラットではなく、顔・髪・白衣に小さな立体感を残す。
- 高光沢CG、肌・髪のプラスチック的反射、全面厚塗り、過剰な光源演出を避ける。
- 肌は自然な薄い血色。瞳と表情が主役になる箇所だけ彩度・ハイライトを強める。白衣はニュートラル〜少し暖かい白、背景は低彩度で人物と分離。
- 質感は必要な箇所のみ。不要な粒子・点描・壁材や小物の微細テクスチャを増やさない。

### 3. 背景・小物の情報量

**背景は記号化し、人物・吹き出し・オチの視認性を優先。**

- 喫煙室は最初の場所説明に `喫煙室` 表示、ソファ／椅子、テーブル、灰皿、煙のうち**必要な少数だけ**を使う。毎コマすべて再描画しない。
- 会話・リアクションは無地、薄いトーン、壁の一部、机の縁だけでもよい。場所が分かる最小限を残す。
- 演説、怒り、邪悪可愛いオチは集中線・ベタ・空白・簡素なシルエットへ移行。群衆はシンプルなモブ数人で十分。
- SCP本体や実験資料など**環境そのものが主題**のコマでは、必要な形状・識別情報・資料文字に描写予算を集中してよい。
- 同じ密度の背景を全コマへ敷き詰めず、絵の重要度に応じて省略／描き込みに差をつける。

### 4. 漫画・文字・演出

- 日本式**右上→左、上→下**の読順を物理コマ位置で固定し、縦書き台詞・同コマ内の吹き出し順・尻尾の向きを照合。作品画像に制作番号や意図しない解説文を入れない。
- ゴールディの会話吹き出し＝薄赤。七星＝白。資料や地の文の役割は混同しない。文字の可読性と余白を守る。
- コマサイズは均等割りにしない。静かな「間」、説明、演説や感情の最大コマ、脱力したオチで視覚重量を変える。
- タイトル `SCPと一服`、各話のSCP番号、幕間であることが必要な場合の見出しは、コマ・話数に応じて明確にする。例示の「SCP-914」「喫煙革命」は別話に持ち込まない。
- 喫煙の煙は自然に上へ流れる。紙巻きの向き・持ち手・火種・灰皿との位置関係を確認。喫煙室と実験／収容区画の区別は[シリーズ設定](README.md)に従う。

## 短い生成向けプロファイル

> Japanese full-color manga, clean hand-drawn anime lineart with subtle lineweight variation, tasteful restrained cel shading with a little soft dimensionality, natural skin tones, clear character silhouettes, subdued low-detail backgrounds, visual hierarchy prioritizing faces, readable speech balloons and expressions. Minimal props and texture outside the focal subject, gentle tonal simplicity in conversational panels; bold shapes and selective emphasis for comedy, but no overly rendered CGI gloss or all-over detail. Match the **actual attached approved character sheets** for character identity. Maintain RTL Japanese manga panel order and vertical Japanese dialogue. Goldie speech balloons pale pink, Nanahoshi white. Do not copy story content, hats, crowd, panel grid or slogans from the style example.

この文章は**雰囲気を伝えるプロファイル**であり、各ページの具体的なネームと実画像参照の代わりにはならない。

## 制作・受入の確認

1. **Identity**：二人の顔・瞳色・髪・白衣・体格を承認済み人物参照と照合。スタイル見本のキャラ描写が食い違えばCharacter Sheetを優先。
2. **Story / Layout**：その話の正規文章ネームから、全コマの物理位置・読み順・台詞・状態を確定。
3. **Rendering**：背景を過剰に作らず、塗りの面・色・影を重要箇所へ集中。過剰な線・質感・群衆を削る。
4. **Review**：完成画像を実際に見て、文字・尻尾・話者・読順・キャラの顔と手・煙草・画面端・SCPの情報を確認。**プロンプトの存在だけでは合格にしない**。
5. **Exceptions**：モノクロ、シリアスな高密度背景、特殊な劇画表現等は作品上の理由があれば可能。ただし新たなシリーズ既定へ恒久昇格させない。

## 優先順位

1. 作者の当回の明示指定、公開原稿や確定ネーム
2. [承認済み人物基準画像・Character Sheet](../characters/README.md)
3. 本書のシリーズ画風・彩色・背景既定
4. 汎用Coreの画風と漫画制作Skill、および局所的な演出装飾

本書は **scp-manga-works のシリーズ固有標準**。綴理本人の公式ビジュアル `tsuzuri-core/identity/visual-style.md` を変更・上書きしない。
