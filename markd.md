author: hihumikan
summary: Vue.jsの基本的な使い方の解説
id: vue-hihumikan-markdown
categories: codelab,markdown,vue,hihumikan
environments: Web
status: Published
feedback link: https://github.com/hihumikan/codelab-vue
analytics account: XXXXXXXX

# Vue勉強会 8 / 22 20~

# hihumikan - Vue勉強会 8 / 22 20~

## 待機スライド
Duration: 0:00:00
![head](./img/head.png)

## はじめに
Duration: 0:03:00

### 話す事

- Webページの概要
- Vue.jsの基礎構文
- 公開手順
- ロードマップ

Positive
: ゴール

✅ Webアプリの大体の作り方の流れ

✅ Vueをなんとなく理解


Negative
: 話さない事

❌ Vueの細かい機能

❌ 他のフレームワーク、言語の比較

❌ HTML/CSSの説明

## 作るサンプル
Duration: 0:01:00

<button>
  [サンプル](https://qqey.net/)
</button>


## 自己紹介
Duration: 0:01:00

![hihumikan](./img/hihumikan.png)

## Webページの概要
Duration: 0:06:00

### Webページについて

スマホやパソコン上で表示されているWebページは大体、**HTML/CSS/JavaScript**の３つの技術が用いられます。大まかにHTMLでWebページを作成し、CSSで見た目をデザイン、動きの部分でJavaScriptといった役割を持っています。

Webページを公開するだけならばHTMLとCSSで十分ですが、「**クリックした時にメッセージを表示させたい**」「**このツイートにいいねしたい**」「**画像が入れ替われるようにしたい**」などに、JavaScriptはよく利用されます。

つまり、クリックによって色々変えたいとかプログラミングっぽいことをするならJavaScriptは必要になるということです。

### Vue.jsとは？

今回の勉強会のテーマとなっているVue.jsはそのJavaScriptの[フレームワーク](https://www.otsuka-shokai.co.jp/words/framework.html)となっており、通常のJavaScriptよりも**少ないコード**で開発出来たり、**簡単に保守**が出来たりするなど時間的コストを**大幅に短縮出来る**ものです。

最近のWebアプリケーションの開発ではVue.jsが多くの企業で使われ、今人気のフレームワークとなっています。学習コストの低さもあるため、この機会にVue.jsを触ってみましょう。

※Vue.jsを使っているサイト一例

* note　
[https://note.com/](https://note.com/ )
* サイバーエージェント　[https://www.cyberagent.co.jp/](https://www.cyberagent.co.jp/)
* Geartics　[https://www.geartics.com/](https://www.geartics.com/)


他にも、Vue.jsに対抗するライブラリやフレームワークなどがあり、ReactやAngular、JQuery、Svelteなどが存在します。今回の勉強会ではそれらの説明は割愛させて頂きますが、興味があったら調べてみてね。

## VueでWebアプリを作成するステップ
Duration: 0:00:30

それでは、実際にWebアプリケーションを作成する方法を解説していきます。

ステップ毎に解説しております。

### STEP1:開発環境を整える

### STEP2:コードを書いてみる

### STEP3:GithubPagesにアップロードする

### STEP4:ページを公開する

一連の流れはこうなります。　次のページでSTEP1を解説していますので、Nextを押してください。

## STEP1:開発環境を整える
Duration: 0:04:00

### Vue.jsの種類

Vue.jsを使って開発する場合、**CDNを利用する方法**と**Vue CLIを利用する方法**の2種類存在します。

CDNの場合、htmlファイルに**scriptタグを読み込ませるだけ**。開発環境を整えなくても利用することができます。

Vue CLIの場合、Vue.jsの基本機能に加えて、**開発環境をすぐに作れる**優れもの。**色々な拡張機能を追加**できて、基本的にはこっちが利用される。

ただし、Vue CLIを利用するには**Node.jsをインストールする必要**があり、時間の都合上、今回の勉強会では、Vue.jsの基本機能を簡単に試せるCDN版を利用します。

### エディタについて

今回はオンラインエディタを利用して、Vue.jsを使用します。下記のリンクを踏んでいただき、こちらでコードを書いていただく形となります。

**ひな形
[https://codepen.io/hihumikan/pen/mdmvGay](https://codepen.io/hihumikan/pen/mdmvGay)**

※オンラインエディタを使用しなくとも、[Visual Studio Code](https://visualstudio.microsoft.com/ja/)を利用して、index.htmlを新規に作成して作ることもできます。

### 導入
CDNを用いて、利用する場合に、
```
<script src="https://cdn.jsdelivr.net/npm/vue@2/dist/vue.js"></script>
```
をhtmlファイルに記述することによってVue.jsの基礎機能を導入することが出来ます。
