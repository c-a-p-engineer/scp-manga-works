# CHAR-001 — Goldie / バット：画像生成用リファレンス

> **用途**：SCP連作漫画の全話で、主人公の外見を固定するための読み取り用ショートリファレンス。画像生成のたびに確認する。  
> **ステータス**：2026-10-11 承認済み外見 v1.0。正式なフルネーム `Goldie Bateman` は未確定。  
> **詳細設定の正本**：[CHAR-001_BAT.md](CHAR-001_BAT.md)

## 採用済みの人物基準画像（必ず参照）

![ゴールディ（バット）採用済み人物リファレンス](assets/CHAR-001_BAT_reference-v1.png)

[原寸画像を開く](assets/CHAR-001_BAT_reference-v1.png)

この画像は**人物の顔・髪・体格・服装のidentity参照**。画像のポーズ、背景、喫煙の有無をすべてのコマにコピーしない。

## 固定特徴（IDENTITY — MUST PRESERVE）

- **女性／成人・20代前半／約150cm／小柄で華奢**。猫背。かわいさは「気だるい小動物美少女」。
- **金髪、柔らかい猫っ毛、肩にかかりそうなミディアム、ラフなハーフアップ、流し前髪**。
- **深紅の目、ジト目・半目ぎみ、クマなし**。普段は気だるく、研究に集中すると鋭い視線。
- **大きめの白衣を袖まくり**。**白ワイシャツは上ボタンを少し開ける**。**黒ネクタイはタイピン付き**。
- 黒～チャコールのゆったりしたスラックス、黒い革靴。白衣のポケット・収納物は目立たせない。
- イラストは基準画像の**落ち着いたアニメ画風・清潔な線・適度なセル塗り**を維持。別人になる顔立ちの変更は不可。

## 状態別に変えるもの（表情・動作だけ）

| 状態 | 目・表情 | 行動 |
| --- | --- | --- |
| 通常 | ジト目、気だるい | 猫背、無駄な動きが少ない |
| 喫煙できない | 不機嫌、目が険しくなる | 苛立つが、必要な研究はする |
| 喫煙中 | とろんと弛緩 | 作業を止め、通常の持ち方で吸い、煙を大きく上へ吐く |
| 喫煙後 | しゃっきり | 表情・姿勢が少し引き締まる |
| 研究集中 | 深紅の目が鋭い | 仕事に集中。くわえタバコで作業しない |

- 銘柄：**ゴールデンバット**。安価な100円使い捨てライター。火を点ける際は箱をポケットへ戻す流れ。
- 服や髪に染みついたタバコの強い匂いは文章・反応で表現できるが、全コマを煙だらけにしない。
- **喫煙は許可された区域のみ**。SCPの収容条件と現場安全が優先。

## Manga Blueprint Studio / 画像生成への受け渡し

1. **キャラクターの同一性**：Studioの `sheet` identityモードで、`characterId: CHAR-001` に対してこの画像を **Character Sheet画像として明示的に添付・対応付ける**。`referenceKey` は作品側の対応キーに従い、無根拠に別人の画像を使わない。
2. **空間と構図**：コンパイルされたページの `Pxxx.clean.png` が担当する。**人物シートはコマ割り・ポーズ・視点を上書きしない**。
3. **台詞・意味**：`work.manga.json`、対象ページの `Pxxx.generation.json`／プロンプト、正規ネームに従う。
4. **実体を渡す**：GitHub URLやMarkdownへの言及だけでは画像モデルへ画像バイナリは添付されない。生成ツールに実際のPNGを渡せたか確認してから生成する。
5. **検証する**：髪型・深紅の目・白衣の袖・ネクタイとタイピン・身長感・成人らしさ・描画スタイルを完成候補の各コマで目視照合。外見のズレは候補段階で修正。

### 添付用の短縮プロンプト

> Goldie “Bat”, an adult petite Japanese-anime-styled blonde female scientist in her early 20s, about 150 cm, slim and slightly hunched, languid cute small-animal charm. Fine slightly messy blonde shoulder-near medium-length hair in a loose half-up style, side-swept bangs; deep crimson half-lidded jito-me eyes, **no dark circles**. Oversized rolled-sleeve white lab coat, white collared shirt with top buttons casually open, black necktie secured with a tie clip, loose black trousers and black loafers. Maintain facial identity and clothing from the **attached approved character reference image**, NOT its original pose or smoking state. She smokes only during breaks, never while researching. Keep hair/eyes/outfit exactly consistent across panels.

## 新規生成した複数ビューの候補画像

- 2026-10-11：採用済み立ち絵を参照して、正面寄りの立ち姿・背面3/4・顔アップ・喫煙中の表情を示す**新しい参考候補画像**を生成。
- **ステータス：未承認の候補。** 既存のv1画像が人物identityの正本。候補画像に外見の差があれば正本を優先する。
- 候補画像は制作環境内にあり、このGitHubリポジトリに**画像バイナリとしてはまだ保存していない**。画像を正式採用・アップロードした場合のみ、以下にパスを追加する。

## 関連

- [詳細キャラクターシート](CHAR-001_BAT.md)
- [登場人物一覧](README.md)
- [Studioの人物参照と画像受け渡し仕様](https://github.com/c-a-p-engineer/manga-blueprint-studio/blob/master/docs/PROMPT_HANDOFF.md)
