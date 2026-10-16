# EP006 幕間「師範の勘」 — pixiv実投稿記録

**状態：pixiv公開済み／2026-10-16に実投稿API・画像一覧を取得して確認。**

## 公開作品

- **作品URL**：https://www.pixiv.net/artworks/150922208
- **作品ID**：`150922208`
- **実登録タイトル**：`SCP-3491-JP 幕間・師範の勘｜SCPと一服`
- **公開日・時刻**：**2026-10-16 20:59 JST**（実データ`createDate=2026-10-16T11:59:00+00:00`。APIは分精度。画像パスの時刻は20:59:16）
- **投稿者**：こぴぺたん
- **作品形式**：漫画（`illustType=1`）、全**1ページ**、1024×1536px
- **実登録タグ**：`SCP`のみ（「漫画」は実登録なし。投稿前の提案と区別）
- **AI申告設定**：あり（pixiv API `aiType=2`）。本文にも明示
- **公開範囲**：`restrict=0`、`isUnlisted=false`（全体公開・非限定公開）
- **シリーズ登録状態**：`seriesNavData=null`。本文では「SCPと一服」EP006幕間と表記。**pixivのシリーズ所属は確認できない**（未登録とまでは断定しない）
- **原寸配信形式**：JPEG（`150922208_p0.jpg`）／[画像一覧API](https://www.pixiv.net/ajax/illust/150922208/pages?lang=ja)
- **GitHub保存済み原稿**：[images/final/P001.png](images/final/P001.png) ／ [同一Blob確認と保管経路](images/README.md)。pixiv側JPEGとの画素完全一致・投稿後差し替えは未検証
- **本編**：[EP006「すくえない男」pixiv 150912875](https://www.pixiv.net/artworks/150912875)。幕間は本編3Pと別投稿で、EP007ではない

## pixiv実際の説明文

以下は実投稿の`illustComment`からHTMLの改行・リンク装飾を可読化したもの。**文章自体は推敲・補筆しない**。本編への作品内リンクは参照先URLを補記。

一服のお供に、今日のSCPをひとつ。

藤崎さんの記録を読んだ新人研究員が、主任に抗議。

どうやら主任は、最初から全部知っていたようで……。

「SCPと一服」EP006「すくえない男」の幕間・全1ページ。

本編はこちら：
https://www.pixiv.net/artworks/150912875

※非公式のSCP二次創作漫画です。
※画像生成AIを使用しています。

【原作・ライセンス】
原作：SCP-3491-JP「すくえない男」
原作者：mojamoja
https://scp-jp.wikidot.com/scp-3491-jp

漫画：c-a-p-engineer

本作品は CC BY-SA 3.0 に基づき公開します。
https://creativecommons.org/licenses/by-sa/3.0/

## 取得根拠と検証境界

- [pixiv作品データ](https://www.pixiv.net/ajax/illust/150922208?lang=ja)：ID・実題名・実際の説明文・タグ・作品形式・AI申告・公開日時・シリーズ登録情報
- [pixiv画像一覧](https://www.pixiv.net/ajax/illust/150922208/pages?lang=ja)：画像1枚、1024×1536px、原寸JPEGのURL
- [pixiv作品ページ](https://www.pixiv.net/artworks/150922208)
- [GitHub完成PNG](images/final/P001.png)：作者がGitHubへアップロードした、会話中の最終生成画像と同一Git Blob SHAの原本。現場で再圧縮していない
- **未確認**：pixiv配信JPEGとGitHub PNGの画素同一性／公開後の差し替え／pixivシリーズ正式所属

## 作品の帰属

原典「SCP-3491-JP すくえない男」原作者mojamoja。漫画：c-a-p-engineer。pixiv実投稿本文で原典・作者・出典URL・CC BY-SA 3.0・画像生成AI利用の表記を確認済み。詳細は[CREDITS.md](CREDITS.md)。
