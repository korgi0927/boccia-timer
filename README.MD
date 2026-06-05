# ボッチャ競技タイマー 🎯

携帯対応のボッチャ競技用タイマーアプリです。

## 機能

- **白タイマー**（上部）：残り15秒・終了でバイブ
- **青タイマー**（下部左）：残り1分・30秒・10秒・終了でバイブ
- **赤タイマー**（下部右）：残り1分・30秒・10秒・終了でバイブ
- 各タイマーの分・秒を個別設定可能
- 1つのタイマー動作中は他をロック（薄表示）
- 起動時に免責事項への同意が必要

-----

## GitHub へのアップロード手順

### 1. GitHubアカウントを作成 / ログイン

<https://github.com> にアクセスしてログインしてください。

### 2. 新しいリポジトリを作成

1. 右上の「＋」→「New repository」をクリック
1. Repository name: `boccia-timer`（任意）
1. Public を選択
1. 「Create repository」をクリック

### 3. ファイルをアップロード

**方法A：ブラウザでアップロード（簡単）**

1. 作成したリポジトリのページで「uploading an existing file」をクリック
1. `index.html` と `vercel.json` を両方ドラッグ＆ドロップ
1. 「Commit changes」をクリック

**方法B：Git コマンド（上級者向け）**

```bash
git init
git add .
git commit -m "初回コミット：ボッチャタイマー"
git branch -M main
git remote add origin https://github.com/あなたのユーザー名/boccia-timer.git
git push -u origin main
```

-----

## Vercel で公開する手順

### 1. Vercelアカウントを作成

<https://vercel.com> にアクセスし、「Continue with GitHub」でGitHubアカウントと連携してサインアップ。

### 2. 新しいプロジェクトをインポート

1. Vercelダッシュボードで「Add New… → Project」をクリック
1. GitHubのリポジトリ一覧から `boccia-timer` を選択して「Import」
1. Framework Preset: **Other** のまま（変更不要）
1. Root Directory: そのまま（変更不要）
1. 「Deploy」をクリック

### 3. 公開完了！

デプロイが完了すると  
`https://boccia-timer-xxxx.vercel.app`  
のようなURLが発行されます。

スマホのブラウザでそのURLを開けばそのまま使えます。  
ホーム画面に追加すると、アプリのように使えます（PWA的な利用）。

-----

## ファイル構成

```
boccia-timer/
├── index.html    # アプリ本体（全機能）
├── vercel.json   # Vercel設定ファイル
└── README.md     # この説明書
```

-----

## 注意事項

本アプリは非公式ツールです。公式競技においては必ず公式の計時装置・審判の判断に従ってください。
