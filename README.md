# SCP Manga Works

**非公式SCP連作漫画の制作Workspace**。財団で「ヤニカスSCP研究室」と呼ばれる、仕事は極めて優秀なのに喫煙への執着が強い3人を描きます。主人公「バット」、主任「セッター」、エージェント「峰」を固定キャストに、まずは**1話1P**で制作します。

> 制作初期段階です。作品の正式タイトル、登場人物の本名の未指定部分、細部の外見、各話の展開はまだ最終確定していません。SCP財団やSCP Wikiの公式企画ではありません。

## 目次

- 📚 **[エピソード一覧・進捗表](episodes/README.md)** — 話数、題材、ネーム、画像、公開状態を管理する**唯一の一覧**
- 📖 [連載の構想・継続設定](series/README.md)
- 👤 [固定キャラクター・登場人物一覧](characters/README.md) — **[ゴールディ（バット）のキャラクターシート v1.0](characters/CHAR-001_BAT.md)**
- 🧾 [原作クレジットとライセンス](CREDITS.md)
- 📝 [新しいエピソードの雛形](episodes/TEMPLATE.md)

## 最初のエピソード

**[EP001 — SCP-650「見てないと来る」（仮題）](episodes/EP001_SCP-650/README.md)**

現在は文章ネーム草稿の段階。完成漫画画像はまだありません。

## ディレクトリ

```text
scp-manga-works/
├── AGENTS.md                    # AI制作・更新ルール
├── README.md                    # 作品の入口
├── CREDITS.md                   # 権利表記の入口
├── series/README.md             # 世界観・連載の方向性
├── characters/README.md         # 固定人物の一覧
└── episodes/
    ├── README.md                # 話数一覧（正本）
    ├── TEMPLATE.md              # 新話の記録用雛形
    └── EP001_SCP-650/
        ├── README.md            # 第1話の状態
        ├── CREDITS.md           # SCP-650 原作の出典
        ├── name/P001.md         # 文章ネーム（草稿）
        └── images/README.md     # 画像の保存規則
```

画像は生成した段階で、各話の `images/drafts/`（生成候補）または `images/final/`（採用済み完成版）に追加します。

## 1話を追加するとき

1. `EP002_SCP-xxx` などのフォルダを作り、`episodes/TEMPLATE.md` を参考に各話 `README.md` を置く。
2. 文章ネームを `name/P001.md` に書く。1P目は `P001`、2P目は `P002`。
3. 生成した候補PNGを `images/drafts/P001-v01.png` のように保存する。不要な試行画像はGitへ追加しない。
4. レビュー済みの採用画像だけを `images/final/P001.png` に保存する。
5. **`episodes/README.md` の一覧を更新**し、原作クレジットと各話ステータスを照合する。

## 制作ルール

ネーム、Blueprint、画像生成は [Manga Blueprint Studio](https://github.com/c-a-p-engineer/manga-blueprint-studio) の**現在の**正規手順を使用します。Studioのコードや練習用fixtureはこのRepositoryに置きません。日本語ページ漫画は原則右→左、縦書きです。

### 画像容量

PNGは1枚約2MBを想定。当面は**完成原稿と残す価値のある生成候補だけ**をGitで管理します。例：100話×完成PNG1枚なら画像本体は約200MBですが、改稿・追加候補・Git履歴で増えます。容量が問題になってから保管先を再検討し、安易に全画像をGit LFSへ移行しません。

## ライセンス・出典

本プロジェクトのSCP由来の漫画・文章は、原作の著者と出典を表示し、**Creative Commons Attribution-ShareAlike 3.0 (CC BY-SA 3.0)** に基づいて提供します。各話の `CREDITS.md` も確認してください。SCPの原作記事と画像素材は権利条件を混同せず個別に確認します。

- [SCP Wiki](https://scp-wiki.wikidot.com/)
- [SCP Licensing Guide](https://scp-wiki.wikidot.com/licensing-guide)
- [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
