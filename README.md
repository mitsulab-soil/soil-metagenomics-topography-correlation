# 土の微生物の顔ぶれ ── 埼玉の五つの土を見くらべる

Who lives in the soil? Comparing microbial phyla across five soil types in Saitama — a teaching dashboard

公開先：https://mitsulab-soil.github.io/soil-metagenomics-topography-correlation/

## これは何か

土の中の細菌・アーキア（古細菌）と菌類を「門」という大きなまとまりで見くらべ、多様度指数（シャノン・シンプソン・ピエルー・バーガー＝パーカー）の読み方を学ぶための教材です。森・水田・丘陵・斜面など、埼玉にある五つの種類の土を想定しています。

A teaching dashboard for comparing soil bacterial/archaeal and fungal phyla and for learning how common diversity indices behave.

## データの性質（必ず読んでください）

- **数値はすべて、説明のために作った仮のデータです。実測ではありません。** 埼玉の五つの場所で土を採ったり、DNA を調べたりはしていません。
- 文献で知られる大まかな傾向（酸性の森の土ではアシドバクテリア門が多め、水田ではメタンをつくるアーキアが見つかりやすい、など）に合わせて手で置いた値で、特定のデータベースから取り出した値ではありません。
- 地図の点は地名のおおよその位置で、採取地点ではありません。pH・有機物・水分・深さも想定です。
- 多様度指数は門の単位で計算しています。研究でふつう使う細かい単位（属・種・配列の型）の値とはくらべられません。
- リポジトリ名に「topography-correlation（地形との相関）」とありますが、このページは地形との相関を分析していません。仮のデータ・五つの場所・一か所一試料では相関も因果も言えないため、ページの中で「本当に調べるには」を説明しています。

All values are hypothetical, hand-set to reflect broad patterns reported in the literature. No samples were collected or sequenced. Do not use them as evidence.

## 使い方

`index.html` をブラウザで開くだけで動きます（インターネット接続が要ります。地図とグラフのライブラリを読み込むため）。

## 参考にした資料

数値をこれらから直接取り出してはいません。土の微生物の大まかな傾向を知るために参照しました。

- Earth Microbiome Project — https://earthmicrobiome.org/
- Thompson et al. (2017) *Nature* 551: 457–463. https://doi.org/10.1038/nature24621 （論文は CC BY 4.0）
- Delgado-Baquerizo et al. (2018) *Science* 359: 320–325. https://doi.org/10.1126/science.aap9516
- Shaffer et al. (2022) *Nature Microbiology* 7: 2128–2150. https://doi.org/10.1038/s41564-022-01266-x
- Ma et al. (2023) *Nature Communications* 14: 7318. https://doi.org/10.1038/s41467-023-43000-z （論文は CC BY 4.0）
- Rodrigues, Tackmann et al. (2026) The MicrobeAtlas database. *Cell*. https://microbeatlas.org/
- Fierer & Jackson (2006) *PNAS* 103: 626–631. https://doi.org/10.1073/pnas.0507535103
- Lauber et al. (2009) *Appl. Environ. Microbiol.* 75: 5111–5120. https://doi.org/10.1128/AEM.00335-09
- Oren & Garrity (2021) *IJSEM* 71: 005056. https://doi.org/10.1099/ijsem.0.005056 （細菌の門の新しい学名）

## 使っている道具とライセンス

- [Chart.js](https://www.chartjs.org/) 4.4.1（MIT）
- [Leaflet](https://leafletjs.com/) 1.9.4（BSD-2-Clause）／地図の絵 © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright)（ODbL）
- 文字：Noto Sans JP・Source Code Pro（SIL Open Font License、Google Fonts）

プログラムは MIT License です。

## 更新の記録

- 2026-10-01：中身を点検して改訂。数値が仮のデータであることを画面の冒頭とこの説明に明記。根拠のない「評価（高い・低い）」を外し、指数の説明を門の単位に合わせて直した。細菌の門に現行の学名を併記し、アーキア（Euryarchaeota）を細菌と区別。地形との相関について言えることと言えないことを追加。参考資料の書誌を確かめて直した。スマホ表示を整えた。

---

© 2026 mitsulab ／ https://mitsulab.jp
