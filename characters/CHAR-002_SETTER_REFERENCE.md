# CHAR-002 — セッター：画像生成用リファレンス

> **Studio Character Identity用の短縮参照**。人物の外見の正本は[詳細キャラクターシート](CHAR-002_SETTER.md)と、承認済みのセッター立ち絵。下の名前「燻」は仮。

## 人物同一性の正本

![セッター採用済みキャラクター画像](assets/CHAR-002_SETTER_reference-v1.png)

[採用済み基準画像PNG](assets/CHAR-002_SETTER_reference-v1.png)

## 角度別・顔アップの補助リファレンス

![セッター正面・側面・背面・顔アップ設定資料](assets/CHAR-002_SETTER_turnaround-v1.png)

[三面図・顔アップPNG](assets/CHAR-002_SETTER_turnaround-v1.png)

## 画像ファイルの役割

| 種別 | GitHub保存先 | 使用上の扱い |
| --- | --- | --- |
| **正本**：ユーザーが承認済みの全身＋顔アップ＋ジッポ着火画像 | [assets/CHAR-002_SETTER_reference-v1.png](assets/CHAR-002_SETTER_reference-v1.png) | **identity第一基準** |
| **補助**：正面・側面・背面・顔アップの三面図 | [assets/CHAR-002_SETTER_turnaround-v1.png](assets/CHAR-002_SETTER_turnaround-v1.png) | **角度別の補助参照**。本書と正本より優先しない |

**現状**：2点ともGitHub保存済み。画像モデルへ渡す際はPNGの実体を添付し、単なるURL指定で添付済みと誤認しないこと。

## IDENTIFY（毎回必須）

- **40代前半の男性・主任研究員、身長約190cm／体重約100kg**。肩・胸・腕・手の厚みが大きく、**熊のようにでかく頼れる**。
- やや四角い顎のある顔、**無精髭、疲れた重い目、黒縁スクエア眼鏡**。
- **黒髪・やや長めの無造作ヘア、こめかみに少量の白髪**。髪はボサつき気味。
- **使い込んだ白のロング白衣（袖まくり）**、襟を少し開けた白～薄灰シャツ、**緩い濃紺ネクタイ**、黒～チャコールのスラックス、黒革靴。
- セブンスター愛煙家。ライターは**使い込まれたジッポ**。喫煙は場面・区域の条件が許すときだけ。
- 普段は猫背・眠たげ・無愛想だが、研究集中時は鋭い眼差しで判断。顔と装いはユーザー承認画像の印象から逸らさない。

## NEVER

痩せた男性にする／若返らせる／誇張した筋骨隆々へ変える／眼鏡を消す／白髪を大量に増やす／整髪しすぎる／長い髭にする／白衣やタイの色を勝手に変更／ライターを100円品にする／ゴールディの約150cmとの大きな身長差を消す。

## 状態差分

| `default` | `no_smoking` | `smoking` | `research_focus` |
| --- | --- | --- | --- |
| 疲れ顔・脱力 | 眉間に皺、苛立つ | 慣れた手つきとジッポ、くわえタバコ | 眼光が鋭く指示が的確 |

## 生成・検査での参照方法

1. `sheet` identityモードでセッターに**実体のPNGを添付**する。仮の`referenceKey`や出力パスだけで添付済みとしない。
2. **Character Sheet＝外見、Clean＝コマ割りと配置、生成プロンプト＝行動・意味・衣装の場面差分**として権限を分ける。
3. 三面図は側面・背面の髪とシルエットの補助。原画と矛盾する場合は原画＋明示的な設定が優先。
4. 完成画像では眼鏡・髭・体格・顔・衣装を各コマでチェック。別人化したらページ候補を修正する。

### Prompt（外見のみ・ポーズはシーンで指定）

> Setter / Nanahoshi is an adult Japanese-anime-style male lead researcher in his early forties, approximately 190 cm tall and 100 kg, a huge broad-shouldered heavyset bear-like build with thick arms and large hands (NOT thin, NOT a bodybuilder). Preserve the approved character illustration's heavy-lidded tired eyes, short rough stubble, slightly square face, medium black rectangular glasses, thick tousled dark hair with small gray streaks only at the temples. Worn white knee-length lab coat with rolled sleeves, slightly open white-gray shirt and loosely knotted dark navy tie, charcoal trousers, black leather shoes. He smokes Seven Stars and owns a well-used hinged metal Zippo lighter. His posture is slightly stooped and he is exhausted but capable. **Follow the attached reference PNG for facial and outfit identity, not for repeated pose, smoke, or composition.**

[詳細設定](CHAR-002_SETTER.md) ／ [登場人物一覧](README.md) ／ [StudioのCharacter Sheet handoff](https://github.com/c-a-p-engineer/manga-blueprint-studio/blob/master/docs/PROMPT_HANDOFF.md)
