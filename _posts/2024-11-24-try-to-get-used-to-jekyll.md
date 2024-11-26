---
layout: post
title:  "Jekyllと仲良くなる"
date:   2024-11-24 10:25:22 +0900
categories: jekyll update
---

[Github公式のチュートリアル](https://docs.github.com/ja/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll)に従って、ページを作成・公開まで漕ぎ着けることはできました。

## 記事の追加方法

- `_post`ディレクトリに記事を書いていく。
- `jekyll serve`を実行することでローカルで動作確認できる。
- 各記事のファイル名は次のフォーマットに従う必要がある
  - `YEAR-MONTH-DAY-title.MARKUP`
  - 例）`2024-11-24-try-to-get-used-to-jekyll.md`

## コードスニペット

``` raw
{% raw %}{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}{% endraw %}
```

と書くと記事上では以下のように見えます。

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
<!-- markdownlint-disable-next-line no-missing-space-atx -->
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

### 役立ちそうなリンク

[ドキュメント][jekyll-docs]

[Github][jekyll-gh]

[フォーラム][jekyll-talk]

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
