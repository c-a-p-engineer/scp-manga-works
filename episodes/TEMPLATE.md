# エピソード雛形

新話を作る際のコピー用例です。テンプレート自体は連載の話数には数えません。

## 保存先

`episodes/EP###_SCP-xxx/`

## README.md に記載する項目

```markdown
# EP### — SCP-xxx「仮タイトル」

**ステータス：企画中／画像未生成／未公開**

- ページ：P001（1P予定）
- 題材：SCP-xxx（一次情報のURL）
- ジャンル：
- 連載上の役割：
- 出演人物：

## 制作物
- 文章ネーム：name/P001.md
- 画像：images/drafts/ と images/final/
- 出典：CREDITS.md

## 進捗チェック
- [ ] 原作・収容条件確認
- [ ] キャラ・人物関係を確認
- [ ] 文章ネーム確定
- [ ] 必要ならBlueprintをコンパイル
- [ ] 生成候補をレビュー
- [ ] 最終版の画像を採用
- [ ] episodes/README.md を更新
```

## 推奨画像名

- `images/drafts/P001-v01.png` — 初回生成など、残したい候補
- `images/final/P001.png` — 採用済み完成原稿

画像は最初の追加時にフォルダを作成します。未生成のまま架空のPNGリンクをREADMEへ設けないでください。

## 公開後の記録

公開作品ができたら、同じエピソードフォルダに `PUBLICATION.md` を追加する。

- pixivなどの**正しい公開URL・表示題名・公開日**を記録。未確認の時刻・タグを創作しない。
- 公開原稿は `images/final/P001.png` の形式で保管し、**GitHubで画像リンクを検証**する。
- 各話の `CREDITS.md` に**SCP原作者・原作URL・CC BY-SA 3.0**を保持し、投稿先本文の表記も確認。
- `episodes/README.md` の公開ステータスと `README.md` の入口を更新。
- 見せ方・pixiv投稿の書き方は[「SCPと一服」テンプレート](../series/PIXIV_PUBLICATION_TEMPLATE.md)を参照。

## 更新する一覧

**[episodes/README.md](README.md)** の表に、エピソード番号、SCP、仮タイトル、ネーム、画像、公開状態、各話リンクを追加します。行は話数順に整理します。
