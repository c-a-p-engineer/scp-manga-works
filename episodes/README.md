# エピソード一覧

このファイルは **SCP漫画の話数・制作状況の一覧表（正本）** です。新話の追加、ネーム更新、画像の採用・公開時には必ず更新します。

| 話数 | 題材 | 仮タイトル | ネーム | 画像 | 公開 | 各話 |
| --- | --- | --- | --- | --- | --- | --- |
| EP001 | [SCP-403](https://scp-jp.wikidot.com/scp-403) | 新人歓迎（2P）／pixiv「SCP-403 段階的過熱ライター」 | 草稿あり（公開原稿と差分） | **完成2P・GitHub保存済み** | **[pixiv公開済み](https://www.pixiv.net/artworks/150764451)** | [制作Workspace](EP001_SCP-403/README.md) ／ [公開記録](EP001_SCP-403/PUBLICATION.md) |
| EP002 | [SCP-9908](https://scp-jp.wikidot.com/scp-9908) | 喫煙。（2P）／pixiv「SCP-9908 喫煙。｜SCPと一服」 | 改訂ネーム確定 | **2P候補をGitHub保存・公開画像との同一性未確認** | **[pixiv公開済み](https://www.pixiv.net/artworks/150784921)**（2026-10-12公開） | [制作Workspace](EP002_SCP-9908/README.md) ／ [公開記録](EP002_SCP-9908/PUBLICATION.md) ／ [幕間ネーム](EP002_SCP-9908/interlude/name/P001.md) |
| **EP003** | [SCP-710-JP-J](https://scp-jp.wikidot.com/scp-710-jp-j) | 財団神拳（2P）／pixiv「SCP-710-JP-J 財団神拳｜SCPと一服」 | P001=v5／P002=v6、公開画像が正本 | **完成2P・GitHub保存済み**（pixiv原画像のバイナリ未照合） | **[pixiv公開済み](https://www.pixiv.net/artworks/150809472)**（2026-10-13 19:11 JST） | [EP003](EP003_SCP-710-JP-J/README.md) ／ [公開記録](EP003_SCP-710-JP-J/PUBLICATION.md) ／ [P001](EP003_SCP-710-JP-J/images/final/P001.png)・[P002](EP003_SCP-710-JP-J/images/final/P002.png) |

## 幕間（本編の話数には含めない）

- **[SCP-9908 幕間「翌朝」](https://www.pixiv.net/artworks/150797153)** — EP002の翌朝を描く**1ページのpixiv公開作品**（2026-10-13 09:53 JST）。[実投稿を正本とする公開記録](EP002_SCP-9908/interlude/PUBLICATION.md)／[制作ネーム](EP002_SCP-9908/interlude/name/P001.md)。[原寸完成原稿P001](EP002_SCP-9908/interlude/images/final/P001.png)をユーザーのルート直下アップロードからGit Blob SHA保持で整理。[画像管理](EP002_SCP-9908/interlude/images/README.md)。pixiv実掲載とのバイナリ照合は未確認。**EP003には採番しない。**

- **[EP003 / SCP-710-JP-J 幕間「現実だ」](https://www.pixiv.net/artworks/150832515)** — **2026-10-14 08:27 JST公開**。1ページ（1055×1491 px）、実登録タグ `漫画`、シリーズ第5掲載作品。[完成原稿](EP003_SCP-710-JP-J/interlude/images/final/P001.png)／[実投稿記録](EP003_SCP-710-JP-J/interlude/PUBLICATION.md)／[ネームv7](EP003_SCP-710-JP-J/interlude/name/P001.md)。EP003本編2ページには含めず、EP004へ採番しない。

旧案 [SCP-650「見てないと来る」](EP001_SCP-650/README.md) は**不採用の初期草稿として保存**。現在のEP001には含めず、制作・公開ステータスも付けない。

## 番号未確定の作品

- **[EPXXXX / SCP-4999「私たちを見守るもの」](EPXXXX_SCP-4999/README.md)** — 2P文章ネーム保存済み（[P001](EPXXXX_SCP-4999/name/P001.md)・[P002](EPXXXX_SCP-4999/name/P002.md)）。画像は候補あり・未採用、未公開。**正式な話数は未決定**であり、EP002に割り当てない。配列確定後に正式採番する。


## ステータスの意味

- **ネーム**：未着手 / 草稿 / レビュー中 / 確定
- **画像**：未生成 / 候補あり / 修正中 / 完成
- **公開**：未公開 / 公開済（公開先URLと確認日を各話 PUBLICATION.md に記録）

ネーム確定と画像完成は別の状態です。完成した画像は当該話の images/final/Pxxx.png（例：P001、P002）へ保存します。未確認の生成候補を「完成」としません。

## 話数・ファイル名

- 話数：EP001 のように3桁。SCP番号は独立で、同一SCPが別話へ再登場しても構いません。
- 各話フォルダ：EP001_SCP-650/ のように話数と主題を含めます。話数未確定の制作物のみ EPXXXX_SCP-<number>/ の仮IDで保管し、正式採番後に移動する。
- ページ：P001 から採番。複数ページ回でも話数の中でページ番号を管理します。
- 追加時は [TEMPLATE.md](TEMPLATE.md) を利用し、この一覧に新しい行を追加してください。
