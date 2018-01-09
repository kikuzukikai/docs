{% for post in site.posts %}
<article>
  <h2>
    <a href="{{ post.url }}">
      {{ post.title }}
    </a>
  </h2>
  <div class="post-meta">
    <span class="post-date">
      {{ post.date | date_to_string }}
    </span>
  </div>
  <div class="post-content">
    {{ post.content }}
  </div>
</article>
{% endfor %}
