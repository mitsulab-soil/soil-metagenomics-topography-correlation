# 埼玉県内における地形的多様性と土壌微生物相（細菌・真菌）のメタゲノム相関分析

## 概要
本プロジェクトは、埼玉県内の異なる地形（森林、水田、丘陵、斜面等）における土壌微生物群集（細菌・真菌）の構造を可視化・分析するためのインタラクティブ・ダッシュボードです。

「醸す谷 / Vallis Fermenti Project」の一環として、土木工学的な地形解釈と、農学・微生物学的なメタゲノム解析を統合し、環境DNAデータ（シミュレーション値）に基づいた生態系の「環世界（Umwelt）」を探索することを目的としています。

## 主な機能
- **地理空間プロット**: Leaflet.jsを用いた埼玉県内サンプリング地点の可視化。
- **細菌・真菌組成分析**: 門（Phylum）レベルでの相対存在比をスタックバーチャートで比較。
- **多様性評価**: 以下の指標を用いた多角的な生態系評価。
  - シャノン多様度指数 ($H' = -\sum p_i \ln p_i$)
  - シンプソン多様度指数 ($1 - D$)
  - ピエルー均等度 ($J'$)
- **環境パラメータ相関**: pH、有機物含有量、水分量などの物理化学的性質と微生物相の対照。

## 技術スタック
- **Frontend**: HTML5, CSS3 (Modern Dark UI)
- **Visualization**: [Chart.js](https://www.chartjs.org/) (Charts), [Leaflet.js](https://leafletjs.org/) (Maps)
- **Data Handling**: JavaScript (Vanilla JS)

## データソースについて
本ダッシュボードで使用されているデータは、以下のオープンデータプロジェクトの門レベル組成パターンに基づくシミュレーション値です。
- **Earth Microbiome Project (EMP)**
- **GlobalSoilBiome (Delgado-Baquerizo et al. 2018)**
- **MicrobeAtlas**

## 使用方法
1. 本リポジトリをクローンまたはダウンロードします。
2. `soil_metagenome_v3.html` をブラウザで開くだけで閲覧可能です（サーバー設定不要）。

## 開発者情報
**mitsulab / 醸す谷 Vallis Fermenti**
元土木エンジニアの視点から、有機農業、土壌学、複雑系科学を融合させた持続可能な居住圏モデルを研究しています。

## ライセンス
[MIT License](LICENSE)
