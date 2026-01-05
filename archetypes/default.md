---
draft: false

date: '{{ .Date }}'
lastmod: '{{ .Date }}'
archives: '{{ dateFormat "2006/01" .Date }}'

title: ''
slug: ''
thumbnail: ''
description: ''

categories:
  - ''
tags:
  - ''

toc: true
fixed: false # _index.md only
build:
  publishResources: false
---

## はじめに

<code>
&lt;!--more--&gt;
</code>
より下は一覧ページに出力されません

<!--more-->

## Markdown CheetSheet

### Text Format

Italic: *Italic（斜体）*

Emphasis: __Emphasis（強調）__

Strikethrough:  ~~Strikethrough（取り消し線）~~

This is `inline`.

### List

- text
  - test
  - test

1. text1
1. test2
    1. test2-1  
       multiline
    1. test2-2

### Horizontal rules

---

### Annotation

注釈は英語で *annotation* とか *footnotes* とかいいます[^1]。  
この単語は、文書やテキストに対する説明、コメント、または補足情報を指す一般的な用語です[^2]。

[^1]: しらんけど

### Blockquotes

> This is Blockquotes

### Details

{{< details summary="See the details" >}}
This is a __bold__ word.
{{< /details >}}

### Links

[Google](https://www.google.com/)

### Tables

| id     | name    | date       |
| -----: | :-----: | :--------- |
| 1      | test    | 2019-01-01 |
| 2      | test    | 2019-01-02 |
| 3      | test    | 2019-01-03 |

### Images

- リンクがついてるときは画像クリックで `link` に飛ぶ
  {{< img
    src="/images/default.jpg"
    width="300"
    height="200"
    loading="lazy"
    link="https://en.wikipedia.org/wiki/Lorem_ipsum"
    target="_blank"
    title="img shortcodes with link"
    caption="enabled link"
    attr="Referenced from wikipedia."
    attrlink="https://en.wikipedia.org/wiki/Lorem_ipsum"
  >}}
- リンクがついてないときは画像クリックでオリジナル画像に飛ぶ
  {{< img
    src="/images/default.jpg"
    width="300"
    height="200"
    loading="lazy"
    title="img shortcodes without link"
    caption="disabled link"
    attr="Referenced from wikipedia."
    attrlink="https://en.wikipedia.org/wiki/Lorem_ipsum"
  >}}

### Twitter

{{< x user="nyaburo" id="1434390439868600326" >}}

### YouTube

{{< youtube 3CzgJK6bm2s >}}

[^2]: どこに書いてもOK
