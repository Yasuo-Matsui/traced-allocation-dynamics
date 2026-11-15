# Traced Allocation Dynamics (TAD)

## このリポジトリについて

TADに関する論文と解説資料を公開します。

## 概要

TAD（Traced Allocation Dynamics）は、入力された履歴が時間とともに蓄積・減衰・出力される動的系を記述する数理フレームワークです。

観測時刻を t、履歴の生成時刻を T とする履歴分布 g(t,T) を用い、総量だけでは捉えにくい履歴の構造を扱います。

## 母艦論文

[TAD理論とその応用（Jxiv）](https://doi.org/10.51094/jxiv.1593)

# TADを知る：履歴を状態として見る

**TAD（Traced Allocation Dynamics）** は、現在の総量を、その背後にある「いつ生まれ、どれだけ残っているか」という履歴に分けて捉えるための数理的な枠組みです。

同じ在庫量でも、入荷したばかりのものと長く残っているものでは、次の判断が変わります。このような履歴の違いを、在庫だけでなく人口、待ち行列、物理、記憶、マーケティングなどにも広げて考えます。

この資料集は、研究者、技術者、データサイエンティストや、実業務でデータを扱う方に向けた短い解説です。各資料は独立したテーマを扱っています。まず **00** から入り、関心に合わせて読み進めてください。

> 資料はPDF形式です。各リンクからご覧いただけます。

## 読者別のおすすめルート

### はじめてTADに触れる方

1. [00｜TADとは何か](00_TAD_introduction.pdf) — 基本となる考え方
2. [10｜在庫鮮度から始まったTAD](10_TAD_inventory_freshness.pdf) — 実務からの出発点
3. [50｜TADの応用地図](50_TAD_application_map.pdf) — どんな分野につながるか

その後は、一覧から興味のある分野を選んでください。

### 数理・データ分析の研究者、技術者

1. [00｜TADとは何か](00_TAD_introduction.pdf)
2. [20｜履歴を状態として記述する](20_TAD_basic_structure.pdf)
3. [21｜履歴構成を測る](21_TAD_history_metrics.pdf)
4. [60｜拡張TADの概要](60_TAD_extended_framework.pdf)
5. [70〜75｜各分野への接続](#分野への接続) のうち、関心のある資料
6. [90｜TADの今後の展望](90_TAD_future_directions.pdf)

### 企業のデータ活用・業務改善に関わる方

1. [00｜TADとは何か](00_TAD_introduction.pdf)
2. [10｜在庫鮮度から始まったTAD](10_TAD_inventory_freshness.pdf)
3. [30｜TAD-DB](30_TAD_DB_introduction.pdf) — 履歴を分析できるデータにする
4. [40｜履歴地形を読む](40_TAD_history_landscape.pdf) — 履歴分布を可視化する
5. [50｜TADの応用地図](50_TAD_application_map.pdf)
6. [73｜マーケティングと資本動学](73_TAD_advertising_and_capital.pdf) など、関心のある応用例

## 資料一覧

### 基本・実務への入口

| ID | 資料 | 主な内容 |
| --- | --- | --- |
| 00 | [TADとは何か](00_TAD_introduction.pdf) | 総量の背後にある履歴を見る |
| 10 | [在庫鮮度から始まったTAD](10_TAD_inventory_freshness.pdf) | 同じ在庫量でも中身は違う |
| 20 | [履歴を状態として記述する](20_TAD_basic_structure.pdf) | 入力・残存・出力と履歴状態 |
| 21 | [履歴構成を測る](21_TAD_history_metrics.pdf) | 平均履歴年齢と履歴エントロピー |
| 30 | [TAD-DB](30_TAD_DB_introduction.pdf) | 履歴を分析できるデータにする |
| 40 | [履歴地形を読む](40_TAD_history_landscape.pdf) | ヒートマップで見る履歴分布 |
| 50 | [TADの応用地図](50_TAD_application_map.pdf) | 異なる分野に共通する履歴構造 |
| 60 | [拡張TADの概要](60_TAD_extended_framework.pdf) | 自然減衰、出力換算、非対角入力 |

### 分野への接続

| ID | 資料 | 主な内容 |
| --- | --- | --- |
| 70 | [物理・生物物理への接続](70_TAD_physics_and_turnover.pdf) | 線形応答、タンパク質ターンオーバー |
| 71 | [人口・感染症との接続](71_TAD_population_and_sir.pdf) | 人口の年齢構造、SIR・感染コホート |
| 72 | [記憶とKovacs効果](72_TAD_memory_and_kovacs.pdf) | 復習計画最適化、多時間尺度の応答 |
| 73 | [マーケティングと資本動学](73_TAD_advertising_and_capital.pdf) | 広告残効、Solow型の資本蓄積 |
| 74 | [LLMと待ち行列](74_TAD_attention_and_queues.pdf) | Attentionへの応用構想、待ち行列 |
| 75 | [生物進化と総量成長](75_TAD_evolution_and_growth.pdf) | 系統の生成・消失、ロジスティック成長 |

### 今後の展望

| ID | 資料 | 主な内容 |
| --- | --- | --- |
| 90 | [TADの今後の展望](90_TAD_future_directions.pdf) | 理論・実装・分野横断の展開 |

資料番号は読み順を強制する連番ではなく、各資料を区別するためのIDです。

## 資料について

- 資料はTADの考え方と応用への入口を紹介するもので、証明や各分野の既存研究を網羅するものではありません。
- 図表の数値例は、特に断りのない限り説明用の合成例です。理論上の対応、応用構想、実データによる検証は区別して記載しています。
- 各資料の内容は、参照原稿の版や今後の検討に応じて更新される場合があります。

## 参照論文

松井泰生「TAD理論とその応用：履歴を可視化する数理フレームワーク」参照原稿 ver10（2026年11月7日付）をもとに構成しています。

関連プレプリント：<https://doi.org/10.51094/jxiv.1593>  
公開ページの版と参照原稿ver10は、内容や章立てが異なる場合があります。
