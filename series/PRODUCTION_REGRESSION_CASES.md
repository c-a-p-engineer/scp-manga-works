# 実制作からの回帰ケース — SCPと一服

この記録は作品固有の **検証用Evidence / Acceptance** であり、汎用SkillやStudio実装の第二の正規定義ではない。通常の漫画制作は文章ネームから直接生成し、綴理コアの漫画制作Skillと本作品の `AGENTS.md` を正とする。Studioを**任意採用したケースに限って**、[Studio AGENTS.md](https://github.com/c-a-p-engineer/manga-blueprint-studio/blob/master/AGENTS.md) と `docs/PROMPT_HANDOFF.md` を参照する。

以下は「以前問題になったため、次の制作で実際の出力から再確認したい」項目。文章ネーム、SCP原典、参照画像の内容を「生成画像を観測した証拠」として代用しない。

## R01 — 人物Identityと塗りStyleの分離（SCP-4999試作）

**出典**: [EPXXXX / SCP-4999](../episodes/EPXXXX_SCP-4999/README.md)、[彩色・投稿テンプレート](PIXIV_PUBLICATION_TEMPLATE.md)。

- **再発した問題**: 試作画像の塗りを採用した後、その画像の人物の顔・髪・体格まで次の画像へ引き継ぎ、EP001採用済み人物と違う顔になった。
- **Identity正本**: [ゴールディ](../characters/CHAR-001_BAT_REFERENCE.md)、[七星](../characters/CHAR-002_SETTER_REFERENCE.md)、[峰](../characters/CHAR-003_MINE_REFERENCE.md)と各参照PNGの実画像。画像に写っている人物Identityだけを比較する。
- **Styleのみ採用**: 低彩度のグレー、柔らかい陰影、スクリーントーン、意味がある部分だけのスポットカラー。SCP-4999の候補から顔・衣装・人物サイズを推定しない。
- **受入**: ページの全コマで各人物の顔・髪・体格・服装がIdentity/連続性を満たし、指定のStyleも満たす。Style適合だけでは人物Identityをpassにしない。
- **検証境界**: 画風参照だけでは人物同一性を保証できない。実体のCharacter Sheet画像を生成時に参照し、出力の人物を実画像で比較する。Blueprintを任意利用する場合は `referenceAssets[].role=style` と `identityMode=sheet` の契約も適用する。

## R02 — 日本語RTLと単一吹き出し内の語順（EP002）

**出典**: [EP002 P001ネーム](../episodes/EP002_SCP-9908/name/P001.md)。

- **再発した問題**: 「……そうか。なら話が早い」を2つの吹き出しに分けた結果、読む順番が「なら話が早い → そうか」と逆転した。
- **作者指定**: この一文は **一つの縦書き吹き出し** にまとめる。
- **受入**: ページRTL、吹き出しの配置、縦書きglyphの列順が揃い、正確な全文を右上から読める。コマ番号・制作用注記は出力画像に見せない。
- **検証境界**: 通常工程では文章ネームの正確な文と生成画像の文字・吹き出し順を照合する。Blueprint採用時はName→deterministic letteringのglyph順も確認する。視認性・文字欠けは最終画像で判定する。

## R03 — 物語アンカーを優先する生成画像レビュー（EP002・SCP-4999）

**出典**: [EP002 P002ネーム](../episodes/EP002_SCP-9908/name/P002.md)、[SCP-4999試作](../episodes/EPXXXX_SCP-4999/README.md)。

- **EP002ラスト**: 直前に無言の手元コマ。最終コマは黒ベタ、離れた小さな橙の炎が **2つ**、「シュッ」が **2つ**、下部に短いSCP説明。選んだ素材や結果は描写しない。物語の追加コマも置かない。
- **SCP-4999**: P002の3コマ目で解析依頼が明らかになる。患者の死後もベッドの遺体を消さない。最後のセリフは「とりあえず吸いに行くか」。
- **受入**: コマ数やグリッドが合っていても、上記の意味アンカーが欠落・逆転・別ストーリー化したページは不合格。生成されたページを実際に観測してから判定する。
- **自動検証対象**: 独立した image observation の不足は `unverified`、具体的な誤描写は `repair`。期待ネームを観測値として複写しない。

## R04 — 原典の事実と漫画上の脚色（EP001）

**出典**: [EP001公開記録](../episodes/EP001_SCP-403/PUBLICATION.md)、[EP001クレジット](../episodes/EP001_SCP-403/CREDITS.md)。

- **確認対象**: SCP-403の発火段階と使用条件、原作の収容・実験方針、漫画の演出上の脚色との差分。
- **受入**: 新話や再改稿では原作記事の現行記述を確認する。異常性の誤表示や意図しない設定改変を「演出」として自動許容しない。SCP原作者・原典URL・CC BY-SA 3.0の表示を維持する。
- **検証境界**: コマ配置や文字の構造検証では原典の事実は保証できない。作品固有の出典確認として分離する。

## R05 — 公開済み画像とGitHub候補の同一性（EP002）

**出典**: [EP002公開記録](../episodes/EP002_SCP-9908/PUBLICATION.md)、[画像管理](../episodes/EP002_SCP-9908/images/README.md)。

- **現状**: pixiv掲載作品は確認済み。GitHubの `images/drafts/P001-v01.png`・`P002-v01.png` が掲載画像と一致するかは未確認。
- **受入**: 実画像を照合してページ対応・視覚的一致を記録し、人間が採用したものだけを `images/final/Pxxx.png` へ移す。公開したという事実だけで候補をfinalへ昇格しない。
- **注意**: pixiv画像は再符号化され得るため、バイナリSHA不一致だけで「別の絵」と断定しない。

## 実行・検証境界

**通常の完成原稿採否**: 文章ネームとSCP原典・人物参照 → 1ページずつ画像生成 → 実画像のStructural/Narrative/Lettering/Identity/小道具状態レビュー → 修正 → 作者の採用判断。BlueprintのmanifestやClean/Annotated画像は前提にしない。URLやPNGファイル名を示しただけでは画像モデルへの参照画像の実体提供や視覚確認を代替できない。

**Blueprintを選択した場合のみ**: 現行のStudio `manifest.json`、Clean、参照画像、生成用handoffに従う。Studioの `scripts/validate-production-regressions.mjs` は **synthetic fixturesに対する現行コードの振る舞い**を検証するものであって、実際のEP完成画像の合否を判定するものではない。

**次の制作で再確認する具体的な回帰**: 発話順/尻尾の多重化と話者誤接続、煙草を消した後の口元や手、左右位置の反転、モブ過密、台詞と地の文の混同。形式上正しいネームや自動テスト結果を、生成画像の実観測として扱わない。
