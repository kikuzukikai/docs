{% for post in site.posts %}
  <span>
      {{ post.date | date_to_string }}
  </span>
  <h2>
    <a href="{{ post.url }}">
      {{ post.title }}
    </a>
  </h2>
  <div>
    {{ post.content }}
  </div>
{% endfor %}
