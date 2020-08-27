# コーディング

## 📗 概要

この文書は【loading-screen】のコーディング規約です。  
命名規則や禁則事項などを定め、見やすさや保守性、統一感を高める為に作成しました。

## 💻 プロジェクト構成

- ブラウザは『Google Chrome』を使用する
  - 開発時点ではバージョン: 85.0.4183.83
- エディタは『Visual Studio Code』を使用する
  - デバッグには『Live Server』を使用する
    - [VS Marketplace リンク](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
  - Sassのコンパイルには『Live Sass Compiler』を使用する
    - [VS Marketplace リンク](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)

## 命名規約

### 全般

- ファイルやフォルダ名は原則として全て小文字のケバブケースを使用する
  - `README.md`のようなファイル名が大文字である必要があるものは例外とする
- 文字コードはUTF-8（BOM無し）を使用する
- インデントはスペース2文字を使用する

### 📝 HTML

- HTMLタグの属性やclass、idの指定にケバブケースを使用する
  - 属性やclassは全て小文字とする

## コーディングスタイル

### 📝 HTML

- HTMLタグの属性やclassを指定する文字列は『`""`』で囲む

### 🎨 CSS

- Sass（SCSS）で記述する
- CSSは原則としてクラスのみに記述する
  - 要素にスタイルをあてると、打ち消しのためのCSSが増え煩雑になるため
  - IDにスタイルをあてると、詳細度の計算が複雑になるため
- コメントはSassの『`//`』を使用する
  - 『`/**/`』はメンテナンスがしにくいので
- ネストは深くならないように意識する
  - ネストは原則として孫までとする

## 禁止事項

### 🎨 CSS
- 『`/**/`』の使用を禁止する
  - メンテナンスがしにくいので
  - かわりにSassの『`//`』を使用する

## 推奨事項

- コメントを積極的に記述する
