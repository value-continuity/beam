# BEAM — Business Event Anchored Mapping

BEAM (Business Event Anchored Mapping): a method for resolving cross-system relationships at the moment of a business event and accumulating them as human-confirmed decision history — building bridges, not unified models.

**BEAMは、業務イベントを起点として異なるシステムの対象間関係をその都度解決し、その対応を人が確認した判断履歴として蓄積する方法論です。システムを統一するのではなく、判断可能な橋を育てていきます。**

仕様書本文は [specs.md](specs.md)（v1.0）を参照してください。

## 構成要素

BEAMは次の4要素だけで構成します。

| 要素 | 定義 |
| --- | --- |
| イベント | 業務が動いたきっかけ。既存システムに記録があるもの |
| 対象 | イベントが何についてのものか |
| 判断の記録 | 何と何を、どのような関係として、どの根拠で対応づけたか |
| 人 | 判断を確かめる役割 |

本体は「業務イベント → 対象 → 関係の判断 → 判断履歴」です。名称辞書は判断を効率化する補助機構であり、BEAMの本体ではありません。

## 基本原則

これに違反していたらBEAMではない、という8つの原則です。

1. マスタキーを探さない
2. モデルを統一しない
3. つなぐのはイベント
4. 対応関係は判断として扱う
5. 判断は書き換えず、履歴にする
6. 最後に確かめるのは人
7. 参照は候補でよく、書込みは確認済みを要する
8. 新しい入口を強要しない

## 位置づけ

BEAMは Value Continuity の下に、VCDesign v2・CCP と並列に置かれます。責任境界の記述のみ VCDesign v2 を参照します。
