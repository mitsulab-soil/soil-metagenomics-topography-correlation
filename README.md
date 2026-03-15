# 埼玉県内における地形的多様性と土壌微生物相（細菌・真菌）のメタゲノム相関分析

（GitHub Pages）https://mitsulab-soil.github.io/soil-metagenomics-topography-correlation/


# 🧬 土壌メタゲノム解析ダッシュボード
### Soil Metagenome Analysis Dashboard — mitsulab / 醸す谷 Vallis Fermenti

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Data: Simulation](https://img.shields.io/badge/Data-Simulation%20%28EMP%20based%29-amber)
![Lang: Vanilla JS](https://img.shields.io/badge/Stack-HTML%20%2F%20Vanilla%20JS-blue)
![Project: Vallis Fermenti](https://img.shields.io/badge/Project-醸す谷%20Vallis%20Fermenti-violet)

---

## 概要 / Overview

埼玉県内5地点（秩父・入間・所沢・飯能・比企丘陵）の土壌微生物群集を、Earth Microbiome Project（EMP）等のオープンデータにおける典型的な門レベル組成パターンに基づいてシミュレートし、インタラクティブに可視化するダッシュボードです。

An interactive dashboard that simulates and visualizes soil microbial community composition across 5 sites in Saitama Prefecture, based on typical phylum-level patterns from the Earth Microbiome Project (EMP) and related open datasets.

> ⚠️ **注意**: 本データは実際のeDNAサンプリング・シーケンシングによるものではなく、EMP等のオープンデータに基づくシミュレーション値です。  
> This is simulated data based on open datasets, not actual sequencing results from field sampling.

---

## スクリーンショット / Screenshots

| 地図 / Map | 組成比較 / Composition | 多様性指標 / Diversity |
|---|---|---|
| 埼玉5地点のLeafletマップ | 積み上げ棒グラフ・レーダーチャート | Shannon / Simpson / Pielou / Berger-Parker |

---

## 機能 / Features

- **📍 Leafletマップ** — 埼玉県内5サンプリング地点のインタラクティブマップ（ダークスタイル）
- **🧫 門組成比較** — 細菌・真菌の切り替えが可能な積み上げ棒グラフ・比較テーブル
- **🕸️ レーダーチャート** — 主要門の地点間比較（Chart.js）
- **🧬 多様性評価** — 4指標の自動計算と評価ランク
  - Shannon多様度指数 H'
  - Simpson多様度指数 1−D
  - Pielou均等度 J'
  - Berger-Parker優占度 d
- **📋 生データ表示** — 全サンプルの門レベル相対存在比（%）
- **📚 参照データソース** — EMP等のオープンアクセス論文リスト

---

## サンプリング地点 / Sampling Sites

| 地点名 | 英名 | 場所 | pH | 有機物 | 環境タイプ |
|--------|------|------|-----|--------|-----------|
| 森林土壌 | Forest Soil | 秩父・奥武蔵 | 4.8 | 12.3% | ブナ・コナラ混交林 |
| 水田土壌 | Paddy Soil | 入間市・谷戸田 | 6.2 | 8.7% | 谷戸地形の湛水水田 |
| 狭山丘陵 | Sayama Hills | 所沢 | 5.6 | 9.8% | コナラ・クヌギ里山雑木林 |
| 斜面土壌 | Slope Soil | 飯能・山間部 | 5.3 | 6.2% | 急傾斜の崩積土 |
| 比企丘陵 | Hiki Hills | 比企郡 | 5.8 | 10.1% | 二次林・草地境界の里山混合土壌 |

---

## 使用データ / Data Sources

| データソース | 概要 | ライセンス |
|-------------|------|-----------|
| [Earth Microbiome Project (EMP)](https://earthmicrobiome.org/) | 27,000+環境サンプルの16S rRNAメタ解析 | CC BY 4.0 |
| [Thompson et al. 2017](https://doi.org/10.1038/nature24621) *Nature* | EMP Release 1 — 地球規模の微生物多様性 | Open Access |
| [Delgado-Baquerizo et al. 2018](https://doi.org/10.1126/science.aap9516) *Science* | GlobalSoilBiome — 全球土壌細菌多様性 | Open Access |
| [EMP500 / Shaffer et al. 2022](https://doi.org/10.1038/s41564-022-01266-x) *Nat Microbiology* | 880サンプルのマルチオミクス解析 | Open Access |
| [MicrobeAtlas 2026](https://microbeatlas.org/) *Cell* | 2,390,937サンプルの統合DB | Open Access |
| [SMAG Catalogue / Ma et al. 2023](https://doi.org/10.1038/s41467-023-43000-z) *Nat Commun* | 3,304土壌メタゲノムから40,039 MAGs | CC BY 4.0 |

---

## 技術スタック / Tech Stack

```
HTML / CSS / Vanilla JavaScript（フレームワーク不使用）
├── Chart.js 4.4.1     — 積み上げ棒グラフ・レーダーチャート
├── Leaflet 1.9.4      — インタラクティブマップ
└── Google Fonts       — Zen Kaku Gothic New / Source Code Pro / Noto Sans JP
```

---

## ローカルで開く / Local Usage

```bash
git clone https://github.com/mitsulab/soil-metagenome-dashboard.git
cd soil-metagenome-dashboard
# ブラウザで index.html を開くだけ
open index.html
```

サーバー不要。`index.html` をブラウザで直接開くだけで動作します。  
No server required — open `index.html` directly in your browser.

---

## 今後の展望 / Roadmap

- [ ] 実際のeDNAサンプリングデータへの差し替え（岸田んぼ・六道山公園等）
- [ ] Qualium（土壌生態系シミュレーター）との統合
- [ ] 時系列データ対応（季節変動の可視化）
- [ ] 草堆肥・有機資材施用前後の比較モジュール
- [ ] 土壌医診断スコアとの照合インターフェース

---

## ライセンス / License

MIT License © 2026 [mitsulab](https://github.com/mitsulab)

---

## 関連プロジェクト / Related Projects

- 🌱 [醸す谷 / Vallis Fermenti](https://note.com/mitsulab) — 有機農業×有機土木×発酵の統合フレームワーク
- 🧪 [Qualium](https://github.com/mitsulab/qualium) — 土壌生態系センシング・可視化システム
- 📝 [note @mitsulab](https://note.com/mitsulab) — 実践記録・思想論考

---

<div align="center">
土壌メタゲノム解析 — mitsulab / 醸す谷 Vallis Fermenti<br>
<em>「土を診る」から「土を醸す」へ</em>
</div>

🌱 醸す谷 / Vallis Fermenti — 有機農業×有機土木×発酵の統合フレームワーク
🧪 Qualium — 土壌生態系センシング・可視化システム
📝 note @mitsulab — 実践記録・思想論考
