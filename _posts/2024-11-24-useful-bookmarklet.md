---
layout: post
title:  "ブックマークレット集"
date:   2024-11-24 10:25:22 +0900
categories: jekyll update
---

## 現在閲覧しているページのタイトルとURLをマークダウン形式に抽出してクリップボードにコピー

{% highlight javascript %}
javascript:(function() {
    const title = document.title.replace(/([\\\[\]\(\)\|\*\_\~\`])/g, '\\$1');
    const url = window.location.href.replace(/([\\\[\]\(\)\|\*\_\~\`])/g, '\\$1');
    const markdown = `[${title}](${url})`;
    navigator.clipboard.writeText(markdown).then(() => {
        alert('Copied to clipboard in Markdown format:\n' + markdown);
    }).catch(err => {
        alert('Failed to copy: ' + err);
    });
})();
{% endhighlight %}
