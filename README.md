# hugo-external-site

[Hugo][]で、外部リンクを利用するためのテーマです。

## 前提条件

[Theme Components][]を使用するため、[Hugo][] 0.42以上が必要です。

## サポートしているサイト

* 一般の外部サイト: `external`
* [Wikipedia(日本語)](https://ja.wikipedia.org/)
    * 単数: `wpja`
    * 複数: `wpjas`
* [Wikipedia(英語)](https://en.wikipedia.org/)
    * 単数: `wpen`
    * 複数: `wpens`
* [ニコニコ大百科](http://dic.nicovideo.jp/)
    * 単数: `nico`
    * 複数: `nicos`
* [ピクシブ百科事典 ](http://dic.pixiv.net/)
    * 単数: `pixiv`
    * 複数: `pixivs`
* [IT用語辞典 e-Words](http://e-words.jp/)
    * 単数: `ewords`
    * 複数: `ewordss`
* [Weblio辞書](https://www.weblio.jp/)
    * 単数: `weblio`
    * 複数: `weblios`

## 記述方法

Front Matterに記載します。以下は全てYAMLを使う場合の例です。

### 一般の外部サイト

Front Matterに以下のように記載してください。

```yaml
external:
  - title: "The world’s fastest framework for building websites | Hugo"
    url: https://gohugo.io/
```

### その他

Front Matterに以下のように記載してください。

単数形の場合

```yaml
wpja: Linux
```

複数形の場合

```yaml
wpjas: ["Linux", "Windows", "macOS"]
```

## ライセンス

MITライセンスです。

[Hugo]: https://gohugo.io/
[Theme Components]: https://gohugo.io/themes/theme-components/
