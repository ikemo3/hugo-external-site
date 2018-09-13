# hugo-external-site

[Hugo][]で、外部リンクを利用するためのテーマです。

## 前提条件

[Theme Components][]を使用するため、[Hugo][] 0.42以上が必要です。

## サポートしているサイト

* 公式サイト: `official`
* 一般の外部サイト: `external`
* [Wikipedia(日本語)](https://ja.wikipedia.org/): `wpja`
* [Wikipedia(英語)](https://en.wikipedia.org/): `wpen`
* [ニコニコ大百科](http://dic.nicovideo.jp/): `nico`
* [ピクシブ百科事典 ](http://dic.pixiv.net/): `pixiv`
* [IT用語辞典 e-Words](http://e-words.jp/): `ewords`
* [Weblio辞書](https://www.weblio.jp/): `weblio`

## テンプレートへの組み込み方法

以下のように、partialを使ってください。

* 公式サイト: `{{- partial "official" . }}`
* 外部サイト: `{{- partial "external-site" . }}`

## 記述方法

Front Matterに記載します。以下は全てYAMLを使う場合の例です。

### 公式サイト

Front Matterに以下のように記載してください。

```yaml
official:
  - title: "The world’s fastest framework for building websites | Hugo"
    url: https://gohugo.io/
```

### 一般の外部サイト

Front Matterに以下のように記載してください。

```yaml
external:
  - title: "The world’s fastest framework for building websites | Hugo"
    url: https://gohugo.io/
```

### その他

Front Matterに以下のように記載してください。
(全て複数形に統一しました)

```yaml
wpja: ["Linux", "Windows", "macOS"]
```

または以下のように書けます。

```yaml
wpja:
  - Linux
  - Windows
  - macOS
```

## ライセンス

MITライセンスです。

[Hugo]: https://gohugo.io/
[Theme Components]: https://gohugo.io/themes/theme-components/
