# BISTRO LUPIN — 公式ウェブサイト

日本橋の隠れ家フレンチビストロ「BISTRO LUPIN」のウェブサイトです。

## 構成

```
.
├── index.html      # メインHTML
├── style.css       # スタイルシート
├── script.js       # JavaScript（ナビゲーション・アニメーション）
└── images/         # 画像フォルダ（以下のファイルを配置）
    ├── hero.jpg        # ヒーロー背景画像（推奨: 1920×1080px以上）
    ├── concept.jpg     # コンセプトセクションの画像（推奨: 縦長 4:5）
    ├── gallery1.jpg    # ギャラリー大（推奨: 1200×675px）
    ├── gallery2.jpg    # ギャラリー小
    ├── gallery3.jpg    # ギャラリー小
    ├── gallery4.jpg    # ギャラリー大
    ├── gallery5.jpg    # ギャラリー小
    └── gallery6.jpg    # ギャラリー小
```

## セットアップが必要な箇所

### 1. 画像の配置
`images/` フォルダに上記の画像を配置してください。
画像がない場合はダークなプレースホルダーが表示されます。

### 2. Instagram リンクの設定
`index.html` の以下の箇所を実際のInstagramアカウントURLに変更してください：

```html
<a href="https://www.instagram.com/【アカウント名】" ...>
```

### 3. Instagram 埋め込みウィジェット（オプション）
Instagramの投稿を自動表示したい場合は、Behold (https://behold.so/) や
EmbedSocial などのサービスを利用し、`instagram__placeholder` の div を
ウィジェットコードに差し替えてください。

### 4. Google マップ埋め込みURLの更新
`index.html` のiframeのsrcを正確な店舗座標に基づくURLに変更すると
より正確な地図が表示されます。

## Cloudflare Pages へのデプロイ

1. GitHubリポジトリにpush
2. Cloudflare Pages でリポジトリを接続
3. ビルドコマンド: なし（静的サイト）
4. 出力ディレクトリ: `/`（ルート）
