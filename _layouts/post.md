---
layout: default
---

<span>{{ page.date | date: "%-d %B %Y" }}</span>
<h2>{{ page.title }}</h2>

<div>{{ content }}</div>

<span><a href="{{ '/' | relative_url }}">ページ先頭へ戻る</a></span>
