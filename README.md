# training-guide
AI新人研修用

## 🎉 GitHub Pages

このリポジトリは GitHub Pages で公開されています！

**公開URL:** https://megasinja.github.io/training-guide/

## 📖 セットアップ手順

### ステップ1: GitHub Pagesを有効化する

1. リポジトリの **「Settings」** タブをクリック
2. 左メニューの **「Pages」** をクリック
3. Source セクションで以下を設定：
   - **Source:** GitHub Actions（推奨）または Deploy from a branch
   - （ブランチから直接デプロイする場合）**Branch:** main、**Folder:** / (root)
4. **「Save」** をクリック

### ステップ2: 公開を確認する 🎉

数分後、以下のURLでページが公開されます：
- https://megasinja.github.io/training-guide/

## 🚀 GitHub Actions による自動デプロイ

このリポジトリには GitHub Actions ワークフローが設定されており、`main` ブランチへのプッシュ時に自動的に GitHub Pages にデプロイされます。

ワークフローファイル: `.github/workflows/pages.yml`

## 📝 コンテンツ

- `index.html` - 新卒AI研修のスタートページ
- `least-squares-simulator.html` - 単回帰分析（最小二乗法）シミュレータ
- `polynomial-overfitting-simulator.html` - sin関数近似で過学習を学ぶシミュレータ（次数・L1/L2正則化対応）
- `svm-separation-simulator.html` - クラスタ状2クラスデータをSVMで分割して学ぶシミュレータ
- `svm-step-by-step-explainer.html` - SVMの1更新ステップを式と意図つきで同期解説するページ
- `gradient-descent-visualizer.html` - 勾配降下法の探索軌跡・損失推移を可視化するシミュレータ
- `gradient-descent-step-by-step-explainer.html` - 勾配降下法の1更新ステップを計算意図つきで同期解説するページ
- `mnist-tsne-explorer.html` - MNIST 1000件をt-SNEで2次元可視化し、ホバーで元画像を表示するページ
- `nn-finetuning-training.html` - NNファインチューニングの実務手順・比較・失敗対策を学ぶ研修資料
- `decision-tree-binary-split-visualizer.html` - 決定木（二分木）で2次元データを段階分割する可視化ページ
- `clustering-hub.html` - クラスタリング教材の入口ページ（K-means / DBSCAN / 階層クラスタリング）
- `clustering-kmeans-simulator.html` - K-means の目的関数・パラメータ説明つきシミュレータ
- `clustering-dbscan-simulator.html` - DBSCAN の定義式・探索手順をステップ実行できるシミュレータ
- `clustering-hierarchical-simulator.html` - 階層クラスタリングの linkage 比較とマージ過程を可視化するシミュレータ
- `clustering-gmm-em-simulator.html` - GMMをEM法で学習し、尤度・責務・楕円成分を可視化するシミュレータ
- `clustering-spectral-simulator.html` - Spectral Clusteringのグラフ埋め込みと割当更新を可視化するシミュレータ
- `clustering-mean-shift-simulator.html` - Mean Shiftのモード探索と統合過程を可視化するシミュレータ
- `clustering-optics-simulator.html` - OPTICSの処理順・reachabilityプロット・閾値抽出を可視化するシミュレータ
- `clustering-birch-simulator.html` - BIRCHのCF要約更新と圧縮挙動を可視化するシミュレータ
- `README.md` - このファイル
