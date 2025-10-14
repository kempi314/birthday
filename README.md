# 謎解きサイト

GitHub Pagesで公開できる謎解きサイトです。

## セットアップ方法

### 1. 画像の準備
`images` フォルダを作成し、以下の画像を配置してください：
- `question1.png` - 第1問の画像
- `question2.png` - 第2問の画像
- `question3.png` - 第3問の画像
- `final.png` - クリア時に表示される画像

### 2. 正解の設定
各HTMLファイル（index.html, question2.html, question3.html）の中にある以下の部分を編集して、正解を設定してください：

```javascript
const correctAnswer = "答え1"; // ここに正解を設定
```

### 3. GitHub Pagesでの公開方法

1. GitHubで新しいリポジトリを作成
2. このフォルダの内容をリポジトリにプッシュ
3. リポジトリの Settings > Pages に移動
4. Source を "main" ブランチに設定
5. 数分後、`https://[ユーザー名].github.io/[リポジトリ名]/` でアクセス可能になります

## ファイル構成

```
/
├── index.html          # 問題1
├── question2.html      # 問題2
├── question3.html      # 問題3
├── success.html        # クリア画面
├── style.css           # スタイルシート
└── images/             # 画像フォルダ（作成してください）
    ├── question1.png
    ├── question2.png
    ├── question3.png
    └── final.png
```

## カスタマイズ

- 色やデザインを変更したい場合は `style.css` を編集
- 問題数を増やしたい場合は、HTMLファイルを追加してリンクを調整
- 正解判定は大文字小文字を区別します（必要に応じて変更可能）
