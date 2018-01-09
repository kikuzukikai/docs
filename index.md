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
  EOF
</span>
{% endfor %}
