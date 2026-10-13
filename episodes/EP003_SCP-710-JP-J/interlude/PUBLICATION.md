# EP003 幕間「現実だ」— pixiv実投稿記録

**2026-10-14、pixiv公開データを直接取得し照合。** 本編EP003とは別に投稿された1ページ漫画。

| 項目 | pixivの確認値 |
| --- | --- |
| 作品URL | [https://www.pixiv.net/artworks/150832515](https://www.pixiv.net/artworks/150832515) |
| ID | `150832515` |
| 実タイトル | **SCP-710-JP-J 幕間「現実だ」｜SCPと一服** |
| 公開日時 | **2026-10-14 08:27:21 JST**（`2026-10-13T23:27:00+00:00`、一覧に秒まで表示） |
| 作者 | **こぴぺたん**（ユーザーID `50553719`） |
| 種別・枚数 | 漫画（`illustType=1`）、**1ページ／1055×1491 px** |
| pixivシリーズ | **SCPと一服**（series ID `362543`、第5掲載作品、`order=5`） |
| 直前の掲載作品 | [EP003「財団神拳」本編2P](https://www.pixiv.net/artworks/150809472) |
| 実登録タグ | **`漫画` のみ**（公開前の提案タグは実登録扱いしない） |
| AI作品分類 | pixiv API値 `aiType=2`（UIの未確認表示名は推測しない） |

取得元：`https://www.pixiv.net/ajax/illust/150832515`、`https://www.pixiv.net/ajax/illust/150832515/pages`。ページ投稿の本文、タグ、日時、寸法、シリーズ紐付けを確認。

## pixiv実際の説明文

以下はHTML改行を普通の改行へ変換し、pixivリンク表示を元のURLへ戻したもので、文章の校正はしていない。

```text
昨日の大騒動は夢だった――はずなのに。

財団神拳は科学的根拠に基づく徒手武術。
非科学的な性質は一切ありません。

しかも、ちゃんと訓練制度まであるらしい。

「SCPと一服」EP003「財団神拳」の後日談です。

本編はこちら：
https://www.pixiv.net/artworks/150809472

※非公式SCP二次創作漫画です。
※画像生成AIを使用しています。

【原作・ライセンス】
原作：SCP-710-JP-J「財団神拳」
著者：Kwana
https://scp-jp.wikidot.com/scp-710-jp-j

漫画：c-a-p-engineer
本作品は CC BY-SA 3.0 に基づいて公開します。
https://creativecommons.org/licenses/by-sa/3.0/
```

## 原稿との対応・検証範囲

- [GitHub保存済み完成PNG](images/final/P001.png)は、公開後にユーザーがルートへ置いた `file_00000000c6b48206a59c170b72dfe85e.png`（**2,786,697 bytes／1055×1491 px**）。元画像とGit Blob SHA **`b3ec23b162e252815033ccb341b99b8e4678f0ab`** が一致し、無加工で移動。
- ローカルの生成画像 `scp神拳と一服の漫画幕間.png` ともBlob SHAが完全一致。
- **pixiv配信PNGそのものとのバイナリ／画素完全一致は未検証**。ページ数・寸法は一致。
- [文章ネームv7](name/P001.md)は制作意図であり、公開後の実画像テキストを正本へ都合よく書き換えない。
- pixiv説明文にKwana・原作リンク・非公式二次創作・AI使用・CC BY-SA 3.0の明記を確認。実際の投稿タグは `漫画` だけ。

[幕間トップ](README.md) ／ [画像管理](images/README.md) ／ [ネーム](name/P001.md) ／ [EP003本編](../PUBLICATION.md)
