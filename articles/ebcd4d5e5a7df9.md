---
title: "CSSの擬似要素を使ってwebサイトに図形を追加する"
emoji: "🦁"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: []
published: false
---
# 擬似要素とは
擬似要素とは指定した特定の要素にスタイルをつけることができるものです。よく、CSSで::afterや::beforeを見かけることがあルトもいます。
# 実際に擬似要素をつかってwebサイトを作ってみる
## 完成形のイメージ
<!-- ここの完成した画像とイメージのメモ書きを載せておく -->
## HTMl
擬似要素を使うためにあHTMLの一部に何かを加える必要はありません。いつも通り、HTNLを書いていくだけです。(HTMLに関しての説明は今回省きます。)
```html

```

## CSS
早速擬似要素を使っていきます。
### 擬似要素を使う時のポイント
擬似要素は表示されない時は、positionやcontentプロパティを書き忘れていないか確認してみてください.
```css
body {
    width:100%;
    height:100vh;
    backgroud-color: white;
}


body::before {
    content = "";
    position: absolute;
    width: 100%;
    height: 100%;
    backgroud: liner-graduent(#fff, #fff);
    /* クリップスタジオパスで図形を作成 */
}

```
また、今回は円形の図形を作る時のクリップパスメーカーを使います。クリップパスメーカーでは簡単に擬似要素での図形を簡単に作成できる。
