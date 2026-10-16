# EP006 / SCP-3491-JP「すくえない男」— pixiv公開記録

**状態：pixiv公開済み（実投稿のAPIメタデータを照合）**  
**データ確認日：2026-10-16**  
**内部作品番号：EP006（pixivシリーズ内の順序は9）**

## 公開作品（pixiv実投稿を正本とする）

- **pixiv作品ID**：`150912875`
- **作品URL**：https://www.pixiv.net/artworks/150912875
- **pixiv登録タイトル**：`SCP-3491-JP すくえない男｜SCPと一服`
- **公開日時（JST）**：2026-10-16 16:34:40（pixiv AJAX `userIllusts["150912875"].createDate`）。作品本体 `createDate` は 2026-10-16 07:34:00 UTC（分単位）。
- **pixivシリーズ**：「SCPと一服」（`seriesId=362543`、シリーズ内登録順 `order=9`）。**内部話数 EP006 と一致する番号ではない**。
- **登録タグ（全2件、実測）**：`漫画`、`SCP`。投稿前の候補タグを実登録として補わない。
- **作品形式**：マンガ（`illustType=1`）。
- **ページ数（実測）**：3。pixivのpages APIも3件で一致。
- **配信画像サイズ（pages API）**：P001 1055×1491 px、P002 1055×1491 px、P003 1055×1490 px。
- **AI申告設定**：pixiv `aiType=2`（AI生成作品として申告）。説明欄にも「画像生成AIを使用しています」と記載。
- **投稿ユーザー**：`userId=50553719`（pixiv表示名「こぴぺたん」）。
- **作品の公開範囲**：`restrict=0`、`isUnlisted=false`。全年齢公開設定 `xRestrict=0`。
- **公開後の画像差し替え**：未確認。APIの日時だけから差し替えの有無は断定しない。
- **GitHub保存済み選定画像**：[images/README.md](images/README.md)／[P001](images/final/P001.png)・[P002](images/final/P002.png)・[P003](images/final/P003.png)。pixiv配信画像と各PNGの**バイナリ一致は未検証**。

## pixiv登録済み説明文（原文の文字と改行）

一服のお供に、今日のSCPをひとつ。

ちょっとしたお使いのはずが、タバコとライターが消えていた！？

犯人は、かつて「箱師のマサ」と呼ばれた伝説のスリ師。
その意外な過去と、彼が最後にすくったものとは――。

「SCPと一服」第6話。全3ページ。

※非公式のSCP二次創作漫画です。
※画像生成AIを使用しています。

【原作・ライセンス】
原作：SCP-3491-JP「すくえない男」
原作者：mojamoja
https://scp-jp.wikidot.com/scp-3491-jp

漫画：c-a-p-engineer

本作品は CC BY-SA 3.0 に基づき公開します。
https://creativecommons.org/licenses/by-sa/3.0/

> pixivから取得した `illustComment` のHTML改行 `<br />` と作品外リンクの `/jump.php` を、読みやすい通常の改行・元リンクに正規化。**日本語の本文、句読点、表現そのものは修正していない**。上記は投稿前草稿ではなく、実投稿由来の本文。

## 原作・クレジット

- **原作**：[SCP-3491-JP「すくえない男」](https://scp-jp.wikidot.com/scp-3491-jp)
- **原作者**：mojamoja
- **漫画作者表記**：c-a-p-engineer
- **ライセンス**：[CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
- **公開本文での帰属確認**：原作SCP番号・記事名、原作者、原作URL、ライセンスURL、漫画作者名、非公式二次創作の断り、AI生成使用の申告が実際の説明文に含まれる。

## データの検証元

- 実投稿のJSON：https://www.pixiv.net/ajax/illust/150912875?lang=ja
- 実投稿の画像一覧：https://www.pixiv.net/ajax/illust/150912875/pages?lang=ja
- pixiv作品ページ：https://www.pixiv.net/artworks/150912875
- 作者の公開連絡：2026-10-16、本会話中で上記pixiv作品URLを提示。
- GitHub原稿管理：[images/README.md](images/README.md)（アップロード元ファイル名とGit Blob SHA）。
- 先行の[公開用文面案](../../series/PIXIV_PUBLICATION_TEMPLATE.md)は権威ではなく、実投稿のJSONを優先。

## 現時点での未確認項目

- pixiv配信原寸画像3枚と、GitHubに保存した選定PNG3枚の**バイナリ同一性**。ページ数と画像サイズだけでは一致を証明できない。
- pixiv投稿公開後の差し替えの有無。
- [ネーム](name/P003.md)と実投稿全コマ・全台詞の完全一致。確定ネームは制作過程の記録として保存し、公開した絵の正本と混同しない。
- 作品公開時のAI設定以外の投稿画面上の非公開設定や操作履歴。

## 制作メモ

- P001〜P003の完成候補に至るまで、参照画像からの旧話内容混入、ネームと画像生成要求の食い違い、P003の説明→驚きの因果順、回想の藤崎と七星の描き分け、3Pだけに不要なタイトル表示を除去する修正を行った。
- GitHubの[文章ネーム](name/P003.md)は制作上の意図の保存先。画像の実演出・実文字と一致しない場合、**公開済みの原稿画像を優先**する。
- [ページ3枚の保存記録](images/README.md)は原データBlobを保つことを確認済みだが、pixivが配信する実ファイルとの照合が済んだことは意味しない。
