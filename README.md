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
