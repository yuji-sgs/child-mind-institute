# child-mind-institute
Kaggleコンペ「Child Mind Institute — Problematic Internet Use」のリポジトリ

# アイデアメモ
- 目的変数siiが欠損している部分があるため、その部分は教師なし学習で予測して保管

# EDAメモ
- 親子インターネット中毒テスト（PCIAT）は20項目（PCIAT-PCIAT_01～PCIAT-PCIAT_20）からなり、項目は0点から5点までの5段階で回答され、その合計点でインターネット依存症の重症度を知ることができる。
  - 0〜30：0
  - 31〜49：1
  - 50〜79：2
  - 80〜：3
- siiの欠損値は1224件ある。
- siiの値は記録されているが、PCIATの回答漏れ（1〜20の回答のうち、いくつかの回答がNan）のデータが65件ある。
- テストデータには、PCIATの20項目とPCIAT-PCIAT_Total, PCIAT-Season, sii（目的変数）が含まれていない。
- 年齢とsiiの関係が特に重要そう。
  - siiのスコアが高いほど、年齢が高い傾向にある。
  - しかし、青年期（13〜18歳）において、PCIATスコアの中央値が最も高い
- インターネット利用とsiiの関係も重要そう。
  - siiスコアが高いほど、オンライン利用時間が長い傾向
  - 青少年はインターネット利用のすべてのカテゴリーにおいて、最も影響を受けている年齢層として際立っている。
  - とはいえ、ほとんどすべての年齢層（5～21歳）で、1日1時間未満しかインターネットを利用せず、SIIスコアが高い参加者がいる。
