{% for post in site.posts %}
<span>{{ post.date | date_to_string }}</span>
<h2><a class="link" href="{{ post.url | relative_url }}" role="link">{{ post.title | escape }}</a></h2>

<div>{{ post.content }}</div>

<span><a href="{{ '/' | relative_url }}">ページ先頭へ戻る</a></span>
{% endfor %}
