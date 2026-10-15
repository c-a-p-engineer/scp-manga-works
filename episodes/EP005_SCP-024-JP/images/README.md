# SCP-024-JP「東弊カラオケ」— 完成原稿画像

## 保存状態
- **GitHub整理完了**：2026-10-15、masterに完成原稿4枚を配置。
- **公開**：2026-10-15、[pixiv artwork 150872458](https://www.pixiv.net/artworks/150872458)（実投稿を確認）。
- **ページ数**：全4ページ。
- **保存方式**：元ファイルと同一のGit Blob SHAを新しいパスへ参照し直し、ルート直下の元パスを削除。画像の再生成・再圧縮・再エンコードなし。
- **正式話数**：**EP005**（2026-10-15、マスター指示により採番。画像は同一Blob SHAでフォルダ移動）。
- **pixivとの同一性**：公開ページの作品ID・画像枚数・公開情報は確認した。GitHubの4枚とpixiv配信画像のバイナリ／ピクセル同一性は未検証。

## 完成原稿と移動元

| ページ | 保存先 | Git Blob SHA | ルート直下の元ファイル | サイズ |
| --- | --- | --- | --- | ---: |
| P001 | [P001.png](final/P001.png) | `fe4e03ad526f3b1a96d46c2c7f9fe38fa72e2f7d` | `file_0000000054608209a7514336fd5baa2c.png` | 2,715,722 bytes |
| P002 | [P002.png](final/P002.png) | `265410385d359f82ec513f8271c4d6f0803b3bcb` | `file_00000000b6588206bc9aa4daa5505191.png` | 2,385,163 bytes |
| P003 | [P003.png](final/P003.png) | `a2bde1503619b01e1f1d2b6f849526a07eb29142` | `file_000000009154821190f79b92fe9a1327.png` | 2,848,246 bytes |
| P004 | [P004.png](final/P004.png) | `8a89cc85304501ace77baebdd5b07cc605b0b977` | `file_0000000052dc820984180b9aa7990372.png` | 2,713,964 bytes |

上記対応はチャット内生成時のファイルIDと、GitHubルートの実ファイルID／Blob SHAから確認した。移動後は `master` 上で同じSHAを再照合済み。

## 来歴・証拠

- ユーザーは2026-10-15に「完成原稿はルート直下に置いた」「pixiv公開した」と報告。
- GitHub画像移動コミット：[fb70c97](https://github.com/c-a-p-engineer/scp-manga-works/commit/fb70c97ada1b30730d4361c80d8add734f2bc039)。
- pixiv API [作品情報](https://www.pixiv.net/ajax/illust/150872458)・[ページ情報](https://www.pixiv.net/ajax/illust/150872458/pages)から作品のタイトル、タグ、ページ数、公開時刻などを確認。
- pixiv公開原稿の画像そのものとGitHubファイルのバイト一致までは検証していない。公開前に使った別候補があるかどうかを推定で確定しない。

## 関連資料

- [文章ネーム P001〜P004](../name/)
- [作品README](../README.md)
- [公開情報（pixiv実投稿の正本）](../PUBLICATION.md)
- [原作クレジット](../CREDITS.md)
