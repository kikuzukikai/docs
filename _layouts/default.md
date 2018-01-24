<!doctype html>
<html lang="{{ site.lang | default: "en-US" }}">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <meta http-equiv="X-UA-Compatible" content="chrome=1">
    <title>{% if page.title %}{{ page.title }} | {% endif %}{{ site.title | default: site.github.repository_name }}{% if page.title %}{% else %} | {{ site.github.project_tagline | default: site.description }}{% endif %}</title>
  
    {% seo title=false %}
    
    <link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
    <link rel="stylesheet" href="//fonts.googleapis.com/css?family=Ubuntu">
    <link rel="stylesheet" href="//fonts.googleapis.com/earlyaccess/notosansjapanese.css">
    
    <link rel="stylesheet" href="{{ '/assets/css/styles.css' | relative_url }}">
    <link rel="stylesheet" href="{{ '/assets/css/pygment_trac.css' | relative_url }}">
    
    <!--[if lt IE 9]>
    <script src="//html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
  </head>
  <body>
    <div class="wrapper">
      <header>
        <a href="{{ site.github.url }}"><h1>{{ site.title | default: site.github.repository_name }}</h1></a>
        <a href="{{ '/faq' | relative_url }}"><span class="fa-stack">
          <i class="fa fa-certificate fa-stack-2x"></i>
          <i class="fa fa-check fa-stack-1x fa-inverse"></i>
        </span></a>
        <p>{{ site.description | default: site.github.project_tagline }}</p>
        <p class="view"><a href="{{ site.github.repository_url }}"><i class="fa fa-github fa-fw"></i> View this project on GitHub</a></p>
        <ul>
<li><a href="{{ '/about' | relative_url }}">About us <strong>私達について</strong></a></li>
<li><a href="{{ '/rule' | relative_url }}">Rule <strong>運営規約</strong></a></li>
<li><a href="{{ '/faq' | relative_url }}">FAQ <strong>よくある質問</strong></a></li>
        </ul>
      </header>
      <section>

      {{ content }}

      </section>
      <footer>
        <small>E-mail:</small>
        <p>contact@kikuzuki.jp</p>
        <p class="view"><a href="https://www.facebook.com/{{ site.github.owner_name }}"><i class="fa fa-facebook fa-fw"></i> @{{ site.github.owner_name }}</a>
        <p class="view"><a href="https://twitter.com/{{ site.github.owner_name }}"><i class="fa fa-twitter fa-fw"></i> @{{ site.github.owner_name }}</a>
        <p class="view"><a href="https://www.instagram.com/{{ site.github.owner_name }}"><i class="fa fa-instagram fa-fw"></i> @{{ site.github.owner_name }}</a>
        <p>This project is maintained by <a href="{{ site.github.owner_url }}">@{{ site.github.owner_name }}</a></p>
        <p><small>Hosted on GitHub Pages &mdash; Theme by <a href="https://github.com/orderedlist">@orderedlist</a></small></p>
      </footer>
    </div>
    <script src="{{ '/assets/js/scale.fix.js' | relative_url }}"></script>


  {% if site.google_analytics %}
    <script>
        (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
        (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
        m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
        })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

        ga('create', '{{ site.google_analytics }}', 'auto');
        ga('send', 'pageview');
    </script>
  {% endif %}
  </body>
</html>
