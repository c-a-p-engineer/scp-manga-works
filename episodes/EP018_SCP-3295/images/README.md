# EP018 SCP-3295 — 完成画像と来歴

作者の2026-11-04公開・Root直下アップロード報告に基づく、カラー2ページ原稿。

| Page | 採用原稿 | 元rootファイル | Git Blob SHA（移動前） |
| --- | --- | --- | --- |
| P001 | [P001.png](final/P001.png) | `file_00000000f5e88206a56549c8c43cdc58.png` | `78fe356c98f7c8bd835c92b55ecace76a39f46fc` |
| P002 | [P002.png](final/P002.png) | `file_00000000ea588206af9929af32f0ceb4.png` | `37c6d766b73fca2f6ed1dd886fa770c85a3240b8` |

- **保存方法**：既存Blobをそのまま`images/final/P001.png`と`P002.png`に割り当て、Rootの重複ファイルを削除する。画像の再生成・再圧縮・再符号化を行わない。
- **完成画像の一次証拠**：作者が提供したrootファイルと、採用画像へのGitオブジェクト参照。移動後も同一Blob SHAであることを検証する。
- **pixiv作品**：https://www.pixiv.net/artworks/151666999
- **文章ネームとの差分**：[PUBLISHED_NOTES.md](../name/PUBLISHED_NOTES.md)。
- **確認境界**：画像を原稿として保存する作者の公開・アップロード判断は確認済み。pixivの実配信ファイルとのバイト一致は未検証。
