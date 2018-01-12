{% for post in site.posts %}
<span>
  {{ post.date | date_to_string }}
</span>
<h2>
  {{ post.title }}
</h2>
<div>
  {{ post.content }}
</div>
<span>
  <a href="{{ '/' | relative_url }}">先頭に戻る</a>
</span>
{% endfor %}
