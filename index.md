---
layout: default
title: Home
---
<body>
    <div class="site-wrapper"></div>
        <header class="site-header">
            <div class="site-title">Reuben Mergard</div>
        </header>
    <div class="home-layout">
        <main class="home-main">
    {% for post in site.posts limit:20 %}
            <div class="post-item">
            <div class="post-title-meta">
            <a href="{{ post.url }}">{{ post.title }}</a>
            <span class="post-meta">{{ post.date | date: "%d %b %Y" }}</span>
            </div>
            </div>
    {% endfor %}
        </main>
        <div class="home-side">
            <div class="side-note">
                <p></p>
            </div>
            <div class="side-links">
                <a href="/about/">About</a><br>
                <a href="/now/">Now</a><br>
                <a href="/contact/">Contact</a>
            </div>
        </div>
    </div>
<footer class="site-footer">
  <div class="footer-left">
    <p>for those who make.</p>
  </div>

  <div class="footer-right">
    <p>© {{ site.time | date: "%Y" }} Reuben Mergard</p>
  </div>
</footer>