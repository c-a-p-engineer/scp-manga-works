# SCP-9908 幕間「翌朝」— pixiv公開記録

**pixiv公開済み。2026-10-13、pixiv作品データ取得により、実際のタイトル・説明文全文・タグ・投稿日時・シリーズ登録・ページ数を確認。**

## 正規情報源の運用

**公開された作品に関する情報はpixivの実投稿がSource of Truth（正本）。** GitHubの[PIXIV_DRAFT.md](PIXIV_DRAFT.md)はあくまで公開前の提案・履歴であり、pixiv本文・タグ・タイトルと食い違った場合は**pixivを優先**する。pixivが後日編集された場合は実投稿の最新情報を再取得し、本記録の検証日時を更新する。GitHubの文章ネームは**制作意図**の正本であって、pixivの実掲載画像や投稿内容の正本ではない。

## 実投稿情報（pixiv照合済み）

| 項目 | 実際の値 |
| --- | --- |
| 作品URL | [https://www.pixiv.net/artworks/150797153](https://www.pixiv.net/artworks/150797153) |
| pixiv作品ID | `150797153` |
| 投稿タイトル | **SCP-9908 幕間「翌朝」｜SCPと一服** |
| 公開日時 | **2026-10-13 09:53 JST**（pixiv投稿データの`createDate`/`uploadDate`） |
| 投稿者（pixiv表示名） | **こぴぺたん**（userId `50553719`） |
| 作品区分 | 漫画（`illustType=1`） |
| 掲載ページ | **1ページ**、1055×1491 px |
| pixiv実登録タグ | **漫画、SCP**（提案タグとは異なる） |
| pixivシリーズ | **SCPと一服**、シリーズID `362543`、シリーズ内**第3掲載作品** |
| 前作品 | [SCP-9908「喫煙。」](https://www.pixiv.net/artworks/150784921)（pixiv作品ID `150784921`） |
| AI作品申告（API生値） | `aiType=2` |
| 公開範囲等（API生値） | `restrict=0`, `xRestrict=0` |
| 内部管理区分 | **EP002に紐付く幕間**。EP003として採番しない |

取得元：`https://www.pixiv.net/ajax/illust/150797153` と `https://www.pixiv.net/ajax/illust/150797153/pages`。照合日：**2026-10-13（JST）**。数値のAPIフラグは元の数値を記録し、未確認のUIラベルを推測しない。

## pixivに実際に掲載された説明文全文（正本）

以下は取得時点での実投稿を**一字一句そのまま**記録したもの。pixivのHTML上の改行 `<br />` は実際の改行へ、リンク要素は表示URLへ変換した。それ以外の表記・文章の自然さ・URLの有無を勝手に修正しない。

```text
一服のお供に、今日のSCPをひとつ。

SCP-9908「喫煙。」の実験から一夜明けて。

目を覚ました研究員、なぜか昨夜の記憶がない。服もない。
一方、主任のすっかりお疲れの様子。

いったい、あの実験で何があったのか……？

「SCPと一服」SCP-9908使用後の翌朝を描く、1ページの幕間です。

※本作はSCP財団の非公式二次創作漫画です。研究員や実験の展開は創作上の脚色です。
※漫画画像の制作に画像生成AIを使用しています。

【原作・クレジット】

原作：SCP-9908「Smoke.」／Akumeoy
https://scp-wiki.wikidot.com/scp-9908

日本語訳：SCP-9908「喫煙。」／C-Dives
https://scp-jp.wikidot.com/scp-9908

漫画制作：c-a-p-engineer

ライセンス：CC BY-SA 3.0
https://creativecommons.org/licenses/by-sa/3.0/

本作品はCC BY-SA 3.0に基づき公開します。
```

原作`SCP-9908`の著者・出典、翻訳者、**CC BY-SA 3.0**の投稿本文表記はpixivの実投稿から確認済み。

## pixivに実際に登録されていたタグ（正本）

- `漫画`
- `SCP`

提案稿の `SCP財団`、`SCP-9908`、`SCP漫画`、`AI生成` 等は**実際の登録タグにはない**。pixiv実投稿を正本として記録する。AI設定値とタグは別項目である。

## 公開画像の確認範囲

- pixivは**1ページ・1055×1491 px**を返却。ページデータの元画像URLは`https://i.pximg.net/img-original/img/2026/10/13/09/53/29/150797153_p0.png`。
- **2026-10-13保存**：GitHubルート直下にユーザーがアップロードした `file_00000000e6f88206adb2fbc0db785764.png`（2,824,252 bytes、Git Blob SHA `e9072a7344bd228cdb17f8c50614f5de39a5c00b`）を、**[images/final/P001.png](images/final/P001.png)**へ元のGit Blob SHAを保持して移動した。ルートの旧ファイルを新しいGitツリーから削除。
- この画像は、ChatGPTで生成した**肩幅調整済み**の `SCP-9908_interlude_P001.png` と**Git Blob SHAが完全一致**（2,824,252 bytes、1055×1491 px）。今回再圧縮・ピクセル変更を行っていない。
- ユーザーの公開・再アップロードを受入根拠とし、GitHub上は**完成原稿P001**として管理する。[画像管理](images/README.md)。
- ただし**pixivから配信される実PNGとのバイナリ・ピクセル同一性は未検証**。pixivメタデータの寸法とページ数は一致。全吹き出しの読順や人物参照の視覚QAも実施済みとは扱わない。
- [事前レビューと留意点](PRE_PUBLISH_CHECKLIST.md)は過去の事前QA記録。掲載完了を理由に未確認チェックを自動完了にはしない。

## 公開前下書きとの差異（意図的に維持）

- 実投稿は「**目を覚ました研究員**」であり、下書きの「目を覚ましたゴールディ」ではない。
- 実投稿は「**一方、主任のすっかりお疲れの様子。**」であり、下書きの「主任の七星は…」とは異なる。文章表現は本人の投稿どおり保存し、無断校正しない。
- 実投稿では**本編へのURLが説明文中に含まれない**が、シリーズ内の前作品リンクはpixiv登録により確認できる。
- 提案タグ10個に対し、実登録は **漫画、SCP** の2つのみ。

## 著作権と公開済みクレジット

- 原作著者：**Akumeoy**
- 原文：[SCP-9908](https://scp-wiki.wikidot.com/scp-9908)
- 日本語訳：**C-Dives** — [SCP-9908「喫煙。」](https://scp-jp.wikidot.com/scp-9908)
- 漫画：**c-a-p-engineer**
- ライセンス：[CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)

**すべて実際のpixiv説明文に記載されていることを確認。**

[幕間README](README.md) ／ [完成原稿PNG](images/final/P001.png) ／ [画像管理](images/README.md) ／ [文章ネーム](name/P001.md) ／ [公開前の履歴稿](PIXIV_DRAFT.md) ／ [エピソード一覧](../../README.md)
