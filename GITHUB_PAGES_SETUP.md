# GitHub Pages 設定手順書

このドキュメントは、GitHub Pages を手動で有効化する手順を説明します。

## 📋 前提条件

- このリポジトリ (Megasinja/training-guide) の管理者権限が必要です
- ブラウザで GitHub にログインしている必要があります

## 🚀 設定手順

### ステップ1: リポジトリの Settings にアクセス

1. ブラウザで以下のURLにアクセス：
   ```
   https://github.com/Megasinja/training-guide
   ```

2. リポジトリページ上部の **「Settings」** タブをクリック

### ステップ2: Pages 設定にアクセス

1. 左側のメニューから **「Pages」** をクリック
   - メニューの「Code and automation」セクション内にあります

### ステップ3: Source の設定

Pages の設定画面で、以下のように設定します：

#### オプション A: GitHub Actions を使用（推奨）

1. **Source** セクションで **「GitHub Actions」** を選択
2. すでに `.github/workflows/pages.yml` ワークフローが設定されているため、追加の設定は不要です
3. 自動的にワークフローが実行されます

#### オプション B: ブランチから直接デプロイ

1. **Source** セクションで **「Deploy from a branch」** を選択
2. **Branch** のドロップダウンから **「main」** を選択
3. **Folder** のドロップダウンから **「/ (root)」** を選択
4. **「Save」** ボタンをクリック

### ステップ4: 公開を確認する 🎉

1. 設定を保存すると、デプロイメントが自動的に開始されます
2. 数分後（通常1-3分）、ページが公開されます
3. 以下のURLでアクセス可能になります：
   ```
   https://megasinja.github.io/training-guide/
   ```

4. Pages 設定画面の上部に、公開されたURLが表示されます

### ステップ5: デプロイ状況の確認

1. リポジトリの **「Actions」** タブをクリック
2. 最新のワークフロー実行を確認
3. 緑色のチェックマークが表示されれば、デプロイ成功です

## 🔍 トラブルシューティング

### ページが表示されない場合

1. **キャッシュをクリア**：ブラウザのキャッシュをクリアしてから再読み込み
2. **デプロイ状況を確認**：Actions タブでワークフローが成功しているか確認
3. **待機時間**：初回デプロイは最大10分程度かかることがあります

### 404 エラーが表示される場合

1. リポジトリが公開（Public）設定になっているか確認
2. GitHub Pages の設定が正しく保存されているか確認
3. index.html ファイルがリポジトリのルートに存在するか確認

### ワークフローが失敗する場合

1. リポジトリの Settings → Actions → General で、Workflow permissions が「Read and write permissions」に設定されているか確認
2. Pages の設定で Source が「GitHub Actions」になっているか確認

## 📚 参考リンク

- [GitHub Pages 公式ドキュメント](https://docs.github.com/ja/pages)
- [GitHub Actions によるデプロイ](https://docs.github.com/ja/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-with-a-custom-github-actions-workflow)

## ✅ 完了確認

以下のチェックリストで設定が完了したか確認してください：

- [ ] Settings → Pages にアクセスできた
- [ ] Source が設定されている（GitHub Actions または Deploy from a branch）
- [ ] 設定を保存した
- [ ] https://megasinja.github.io/training-guide/ にアクセスできる
- [ ] ページが正しく表示される

---

**注意**: このドキュメントの手順は、GitHub の UI が変更された場合、内容が古くなる可能性があります。
