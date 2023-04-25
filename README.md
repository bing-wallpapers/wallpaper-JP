# **Wallpaper-JP**

このリポジトリは、Bing から毎日取得した壁紙を保存するためのもので、日本版に特化しています。壁紙は **[Bing](https://www.bing.com/)** の毎日のホームページの背景画像から取得しています。

## **ディレクトリ構造**

```
.
├── .github
│   └── workflows
│       └── download.yml
├── src
│   └── index.ts
├── static
│   └── <date>-preview.jpg
├── .gitignore
├── README.md
├── package.json
├── tsconfig.json
└── yarn.lock
```

## **ファイル説明**

- **`.github/workflows/download.yml`**：Bing からの壁紙のダウンロードとリポジトリの更新をスケジュールおよび自動化するための GitHub Actions ワークフローファイル。
- **`src/index.ts`**：壁紙スクレイピングプログラムのメインソースコード。
- **`static`**：ダウンロードした壁紙プレビュー画像を保存するフォルダ。
- **`.gitignore`**：Git の無視ファイル設定。
- **`README.md`**：プロジェクト説明ファイル。
- **`package.json`**：プロジェクトの依存関係および関連設定。
- **`tsconfig.json`**：TypeScript 設定ファイル。
- **`yarn.lock`**：依存関係のバージョンを安定化するための Yarn ロックファイル。

## **使い方**

1. このリポジトリをクローンします。
    
    ```
    git clone https://github.com/your_username/wallpaper-JP.git
    ```
    
2. 依存関係をインストールします。
    
    ```
    cd wallpaper-JP
    yarn install
    ```
    
3. スクレイピングプログラムを実行します。
    
    ```
    yarn start
    ```
    
4. 実行後、ダウンロードした壁紙は **`static`** ディレクトリに保存されます。

## **ライセンス**

このプロジェクトは **[MIT ライセンス](https://opensource.org/licenses/MIT)** のもとでライセンスされています。
