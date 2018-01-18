---
layout: default
---

<span>{{ post.date | date: "%-d %B %Y" }}</span>
<h2>{{ post.title }}</h2>

<div>{{ post.content }}</div>

<span><a href="{{ '/' | relative_url }}">ページ先頭へ戻る</a></span>
